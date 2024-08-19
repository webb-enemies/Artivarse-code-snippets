# part-7

## Navbar.jsx
``` JavaScript
<div className='poppins relative bg-black py-2 flex h-16 items-center justify-between px-3 text-neutral-50'>
    {/* logo compo */}
    <div className='w-[30%]'>
        {/* search compo */}
    </div>
    <div className='flex w-fit justify-end items-center'>
        <div className=' w-full flex items-center justify-end gap-2'></div>
    </div>

    <div className=" z-[999] absolute top-[4rem] p-4 flex-col items-center right-2 w-[20%] h-[20rem] bg-neutral-950 outline outline-1 outline-neutral-400/70 rounded-md ">
        <p className=' font-medium'>{userdata.email}</p>
        <div className='w-full h-full py-2'>
            <Link to={"/profile"}>
            <p className=' w-full p-2 text-[0.8rem] capitalize rounded-md font-medium text-neutral-400 hover:bg-neutral-600/50 hover:text-neutral-200'>account settings</p>
            </Link>
            <Link to={"/Subscriptions"}>
            <p className=' w-full p-2 text-[0.8rem] capitalize rounded-md font-medium text-neutral-400 hover:bg-neutral-600/50 hover:text-neutral-200'>Subscriptions</p>
            </Link>
            {/*createor links*/}
        </div>
    </div>

</div>
```

## Profileheader.jsx
``` JavaScript
<div className="w-full  bg-neutral-800/50">
    <div className='w-full h-full flex items-center'>
      <h1 className=' text-[2.5rem] ml-20 capitalize poppins'>profile</h1>
    </div>
</div>
```

## Profilesidebar.jsx
``` JavaScript
<div className= "h-full w-full  overflow-y-scroll scrollbar ">
    <div className='flex flex-col gap-4 mt-10 mx-2'>
        {/*list links*/}
    </div>
</div>
```

Mainprofile.jsx
``` JavaScript
<>
{/*profile header*/}
<div className='flex w-full justify-between'>
    <div className='w-[20%] h-[100vh] sticky top-0'>
        {/*profile sidebar*/}
    </div>
    <div className='w-[75%]'>
        {/*outlet*/}
    </div>
</div>
</>
```

Profile.jsx
``` JavaScript
<div className="py-10">
    <div className="w-[80%]">
      <div className="flex justify-between  items-center">
        <h2 className="select-none text-[1.9rem] capitalize poppins"><span className=" font-medium text-[#a7fb1f]">account</span> overview</h2>
        <button className="px-2 py-1 text-[0.7rem] rounded-md font-medium capitalize bg-red-600">logout</button>
      </div>

      <div className="mt-16 flex items-canter gap-6">
        <img className="w-[3rem] rounded-lg self-center" />
        <div>
          <h3 className="text-[2rem] font-medium">{/*username*/}</h3>
          <p className="text-[0.7rem] uppercase font-semibold">user id: {/*user id*/}</p>
        </div>
      </div>

      <div className="mt-10">
        <div className="flex justify-between w-[60%] poppins mt-5">
          <p className="text-[#a7fb1f] capitalize font-medium select-none">name:</p>
          <p>{/*username*/}</p>
        </div>

        <div className="flex justify-between w-[60%] poppins mt-5 relative">
          <p className="text-[#a7fb1f] capitalize font-medium select-none">email:</p>
          <div className="flex items-center gap-1 group">
            <p>{userdata.email}</p>
            <span className={`text-[1rem]  cursor-default`}>{/*emailVerification icon*/}</span>
            <span className=" absolute font-semibold hidden group-hover:block bottom-5 right-[-4rem] outline outline-1  bg-black px-2 py-1 rounded-sm text-[0.7rem]">{/*emailVerification text*/}</span>
          </div>
        </div>

        <div className="flex justify-between w-[60%] poppins mt-5">
          <p className="text-[#a7fb1f] capitalize font-medium select-none">joined:</p>
          <p>{/*account creation date*/}</p>
        </div>
      </div>

      <div className=" w-full flex flex-col items-start mt-[5rem] gap-4" >
        <button className="px-2 select-none py-1 text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f] ">change email</button>

         <button className="px-2 select-none py-1 text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">Verify email</button>

        <button className="px-2 py-1 select-none text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">change password</button>

        <button className="px-2 select-none py-1 text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">change name</button>
      </div>

    </div>
  </div>
```

## Prifile card compo
### change email
``` JavaScript
  <div className="w-full h-full ">
    <form className="flex w-full h-full  flex-col items-center justify-center gap-6">
      <input placeholder="newemail" type="text" spellCheck="false" className="px-2 border-2 border-[#a7fb1f] py-1 bg-neutral-800 rounded-md text-[0.9rem] outline-none w-[80%]" />
      <input placeholder="password" type="text" spellCheck="false" className="px-2 border-2 border-[#a7fb1f] py-1 rounded-md bg-neutral-900 text-[0.9rem] outline-none w-[80%]" />
      <button type="submit" className="px-2 py-1 w-[50%] text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">submit</button>
    </form>
  </div>
```

### change name
``` JavaScript
  <div className="w-full h-full">
    <form className="flex w-full h-full flex-col items-center justify-center gap-6">
      <input placeholder="your name" type="text"  spellCheck="false" className="px-2 border-2 border-[#a7fb1f] py-1 bg-neutral-900 rounded-md text-[0.9rem] outline-none w-[80%]" />
      <button type="submit" className="px-2 py-1 w-[50%] text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">submit</button>
    </form>
  </div>
```


### change password
``` JavaScript
  <div className="w-full h-full">
    <form className="flex w-full h-full  flex-col items-center justify-center gap-6">
      <div className="flex items-center flex-col">
        <p className=" capitalize text-[0.9rem]">get email to change password</p>
        <p className=" font-medium text-[0.7rem]">{/*user email*/}</p>
      </div>
      <button type="submit" className="px-2 py-1 w-[50%] text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">get email</button>
    </form>
  </div>
```

## Conformpassword.jsx
``` JavaScript
  <div className="w-full h-full ">
  <form className="flex w-full h-full  flex-col items-center justify-center gap-6">
    <div>
    <input placeholder="your newpassword" type="text" spellCheck="false"  className=" px-2 py-1 bg-neutral-900 rounded-md text-[0.9rem] outline-none w-[80%]" />
    <input placeholder="repeat password" type="text"  spellCheck="false" className="px-2 py-1 bg-neutral-900 rounded-md text-[0.9rem] outline-none w-[80%]" />
    </div>
  <button type="submit" className="px-2 py-1 w-[50%] text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">get email</button>
  </form>
</div>
```


enjoy everyone
