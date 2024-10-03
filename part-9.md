# Article card compo

```JavaScript
<div className=' w-[30%]  select-none group hover:bg-neutral-900/50 my-6 mx-3 '>
  <Link className=' w-fit'>
  <div className='w-full h-[13rem] overflow-hidden relative rounded-md'>
    <img className='w-full h-full object-cover object-center  ' />
    <p
      className=' hidden group-hover:block duration-200 rounded-sm text-[0.7rem] bg-black/90 font-medium px-1 bottom-1 right-1 w-fit absolute text-neutral-300 overflow-hidden  '>
      creation date</p>
  </div>
  </Link>
  <div className=' w-[97%] mx-auto py-2 relative'>
    <div className='flex items-center justify-between min-h-[2.5rem]'>
      <Link className=' w-full'>
      <p className=' text-[0.9rem] font-semibold overflow-hidden inter'>TITLE</p>
      </Link>
      <button className=" text-[1.1rem] material-symbols-outlined">more_vert</button>
      <div className={` absolute bottom-24 right-0 w-[90%] rounded-md h-[10rem] bg-neutral-950 outline outline-1 outline-neutral-400/50 p-3 z-40`}>
        <button
          className='px-2 py-1 rounded-md hover:bg-neutral-800 duration-75 font-medium inter w-full text-left'>share</button>
      </div>
    </div>
    <div className='flex items-center gap-2 overflow-hidden w-[90%]'>
      {logo &&
      <Link className=' overflow-hidden'>
      <img className='w-[2.5rem]  rounded-full  object-cover object-center' />
      </Link>
      }
      <div className=' w-full'>
        {logo && <p className='w-[80%] text-[0.8rem] text-nowrap text-neutral-400 font-medium overflow-hidden '>CREATOR
          NAME</p>}

        {!logo && <p className='w-[99%] text-[0.8rem]  text-neutral-400 font-medium overflow-hidden '>DESCRIPTION</p>}

        <p className=' text-[0.8rem] text-neutral-200 font-medium overflow-hidden  '>VIEWS AND FOLLORS</p>
      </div>
    </div>
  </div>
</div>
```

# Article card Card compo

```JavaScript
<Card>
  <div className='w-[80%] h-[80%] flex mx-auto flex-col justify-around items-center gap-3'>
    <p className=' text-neutral-400 text-[0.9rem] font-medium'>TITLE</p>
    <div className='w-full flex gap-5 items-center'>
      <Link target="_blank">x</Link>
      <Link target="_blank">whatapp</Link>
      <button>copy</button>
    </div>
  </div>
</Card>
```

# ARTICAL.JSX
``` JavaScript
<div className='w-[70%]  my-5 mx-auto  relative flex justify-center select-none'>
  <div className='w-full  h-[55vh] overflow-hidden rounded-md'>
    <img className=' w-full h-full object-cover object-center' />
  </div>
  <div
    className=' absolute top-[35vh]   w-[85%]  backdrop-blur-sm h-full border-b-[1px] border-neutral-100/50  bg-[#020304]/80  p-3 flex flex-col items-center justify-around'>
    <div className='flex flex-col items-center gap-2'>
      <h1 className=' text-[1.5rem] gugi'>TITLE</h1>
      <p className=' text-justify w-[85%] text-[0.9rem] text-neutral-300 poppins'>DESCRIPTION</p>
    </div>

    <div className='w-[95%] flex items-center justify-between'>
      <div className='flex items-center gap-3'>
        <Link>
        <img className=' w-[5rem] h-[5rem] bg-white p-[2.5px] rounded-full object-cover object-center' />
        </Link>
        <div>
          <p className=' font-medium text-[1.1rem]'>CREATOR NAME</p>
          <p className=' text-[0.9rem] font-medium self-start text-neutral-300  '>FOLLORES</p>
        </div>
      </div>
      <div>
        <button className=' px-5 py-1 bg-white text-black rounded-2xl font-medium text-[0.9rem]'>
          subscribed OR subscribe
        </button>
      </div>
    </div>
    <div className='w-[95%] flex gap-4'>
      <p className=' text-[0.7rem] font-medium self-start text-neutral-300  '>VIEWS</p>
      <p className=' text-[0.7rem] font-medium self-start text-neutral-300  '>CREATE DATE</p>
    </div>
  </div>
</div>

<div className='w-[60%] pt-72 pb-20 mx-auto'>
  <pre
    className='roboto text-[1.1rem]  text-neutral-300 tracking-tighter leading-[1.8rem]  whitespace-break-spaces'>CONTENTS</pre>
</div>
```

 # CREATORSETTINGS.JSX

 ``` JavaScript
 <div className='w-[90%] mx-auto min-h-screen max-h-full  p-10'>
    <div className='py-10'>
      <h3 className=' text-[1.2rem] capitalize'>settings</h3>
      <p className='text-[1.8rem]'>Set up Artivarse exactly how you want it</p>
    </div>
    <div className=' flex flex-col gap-10'>
      <div className='flex items-center justify-between w-[50%]'>
        <p className=' capitalize font-semibold text-[1rem]'>user id</p>
        <p className='px-3 rounded-xl  py-2 border-2 border-neutral-400'>USERID</p>
      </div>

      <div className='flex items-center justify-between w-[50%]'>
        <p className=' capitalize font-semibold text-[1rem]'>creator id</p>
        <p className='px-3 rounded-xl  py-2 border-2 border-neutral-400'>CREATOR ID</p>
      </div>

      <div className='flex items-center justify-between w-[50%]'>
        <div>
          <p className=' capitalize font-semibold text-[1rem]'>delete channel</p>
          <p className=' capitalize font-semibold text-[0.7rem] text-neutral-400'>Deleting your Artivarse channel won't
            close your Artivarse Account</p>
        </div>
        <button
          className='px-3 rounded-md  py-1 inter text-[0.9rem] capitalize font-semibold border-neutral-400'>delete</button>
      </div>
    </div>
  </div>
```

## CREATORSETTINGS Card compo
``` JavaScript
  <Card>
    <div className='flex flex-col items-center justify-around w-full h-[70%]'>
      <h3 className=' text-center py-5 poppins'>Are you sure you want to delete the creator account?</h3>
      <div className='flex items-start gap-3'>
        <button className={`px-3 py-2 bg-red-500 text-black font-semibold rounded-lg `}>Yes, delete the
          account.</button>

        <button className={`px-3 py-2 bg-green-500 text-white font-semibold rounded-lg `}>No, keep the account</button>
      </div>
    </div>
  </Card>
```

# Publiccreatorpage.jsx

``` JavaScript
  <div className='w-[70%] mx-auto py-5 flex flex-col gap-5 '>
    <div className='w-full rounded-md h-[13rem] bg-neutral-900 overflow-hidden'>
      <img className='w-full h-full object-cover object-center' />
    </div>

    <div className='w-full flex items-center gap-3 py-4'>
      <img className=' border-[2.5px] border-[#a7e642] w-[9rem] h-[9rem] rounded-full object-cover object-center' />
      <div className='w-full h-full flex flex-col  gap-2'>
        <h1 className='poppins font-semibold text-[2rem] text-neutral-100 w-[90%] overflow-hidden'>CREATOR NAME</h1>
        <div className='flex gap-3 text-[0.8rem] text-neutral-300 select-none'>
          <p>FOLLORS</p>
          <p>ARTICALS COUNT</p>
        </div>
        <p className=' w-[90%] overflow-hidden text-nowrap'>CHANNAL DESCRIPTION</p>
        <button className=' px-5 py-1 w-fit bg-black text-white rounded-2xl font-medium text-[0.9rem]'>
          subscribed
          <span className="text-[0.9rem] material-symbols-outlined">check</span>
        </button>
      </div>
    </div>
  </div>

  <div className='w-[90%] mx-auto my-10 flex gap-3 flex-wrap'>
    {/* LOOP ARTICAL CARDS */}
  </div>
```

enjoy
