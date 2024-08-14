LOGIN COMPO ->
```jsx
<>
    <div className='w-full min-h-screen max-h-full flex justify-center items-center bg-neutral-900'>
        <div className='w-[35%] h-[80%] flex flex-col justify-around gap-6'>
            <div className='w-full'>
                <h2 className='text-[1.5rem] poppins text-center capitalize'>login to Artiverse</h2>
                <p className='text-[0.8rem] poppins text-center text-neutral-300'>create and share your articles on our
                    platform</p>
            </div>
            <p className=' text-red-400 text-right text-[0.7rem]'></p>
            <div>
                <form>
                    <input placeholder='email' type="email" autoComplete='false' spellCheck="false"
                        className='w-full rounded-md mt-4 h-10 px-2 text-[0.9rem] bg-black/50 outline-1 outline-neutral-400/50 outline' />

                    <input placeholder='password' autoComplete='false' type="text" spellCheck="false"
                        className='w-full mt-4  rounded-md h-10 px-2 text-[0.9rem] bg-black/50 outline-1 outline-neutral-400/50 outline' />

                    <button
                        className='w-full mt-8 rounded-md h-8 px-2 text-[1rem] font-medium  bg-[#a7fb1f] text-black outline-1 outline-neutral-400/50 outline'
                        type="submit">login</button>
                </form>
            </div>
            <div className='flex flex-col items-center gap-8'>
                <p className=''>or authorized with</p>
                <div className='w-full flex justify-around'>
                    <button
                        className=' w-[40%] bg-[#ffffff] text-black py-1 rounded-md capitalize font-semibold '>google</button>
                    <button
                        className=' w-[40%] bg-[#cb88ff] text-black py-1 rounded-md capitalize font-semibold '>github</button>
                </div>
            </div>
            <div>
                <p className=' capitalize text-[0.8rem]'>don&#039;t have an account?
                    <Link className=' text-lime-200 font-medium' to={"/sign-up"}>sign up</Link>
                </p>
                <button className=' capitalize text-[0.8rem]'>forget password</button>
            </div>
        </div>
    </div>

    <Card>
        <div className="w-full h-full ">
            <form className="flex w-full h-full  flex-col items-center justify-center gap-6">
                <div className="flex items-center flex-col w-[50%]">
                    <p className=" capitalize text-[0.9rem]">get email to change password</p>
                    <input placeholder="your email" type="email"
                        className="px-2  border-2 border-[#a7fb1f] py-1 bg-neutral-900 rounded-md text-[0.9rem] outline-none w-full" />
                </div>
                <button type="submit"
                    className="px-2 py-1  text-[0.8rem] rounded-md font-medium capitalize text-black bg-[#a7fb1f]">change
                    password</button>
            </form>
        </div>
    </Card>
</>
```

SIGNUP COMPO ->
```jsx

<div className='w-full min-h-screen max-h-full flex justify-center items-center bg-neutral-900'>
    <div className='w-[35%] h-[80%] flex flex-col justify-around gap-6'>
      <div className='w-full'>
        <h2 className='text-[1.5rem] poppins text-center capitalize'>sign up to Artiverse</h2>
        <p className='text-[0.8rem] poppins text-center text-neutral-300'>create and share your articles on our platform</p>
      </div>
      <p className=' text-red-100 text-right text-[0.7rem]'></p>
      <div>
        <form>
          <input placeholder='email' type="email" spellCheck="false" className='w-full rounded-md mt-4 h-10 px-2 text-[0.9rem] bg-black/50 outline-1 outline-neutral-400/50 outline' />

          <input placeholder='password' type="text" spellCheck="false" className='w-full mt-4  rounded-md h-10 px-2 text-[0.9rem] bg-black/50 outline-1 outline-neutral-400/50 outline' />

          <input placeholder='name' type="text" spellCheck="false" className='w-full mt-4  rounded-md h-10 px-2 text-[0.9rem] bg-black/50 outline-1 outline-neutral-400/50 outline' />


          <button className='w-full mt-8 rounded-md h-8 px-2 text-[1rem] font-medium  bg-[#a7fb1f] text-black outline-1 outline-neutral-400/50 outline' type="submit">sign up</button>
        </form>
      </div>
      <div className='flex flex-col items-center gap-8'>
        <p className=''>or authorized with</p>
        <div className='w-full flex justify-around'>
          <button className=' w-[40%] bg-[#ffffff] text-black py-1 rounded-md capitalize font-semibold '>google</button>
          <button className=' w-[40%] bg-[#cb88ff] text-black py-1 rounded-md capitalize font-semibold '>github</button>
        </div>
      </div>
      <div>
        <p className=' capitalize text-[0.8rem]'>alrady have an account? <Link className=' text-lime-200 font-medium' to={"/login"}>login</Link></p>
      </div>
    </div>
  </div> 
```
