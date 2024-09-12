## part-8 important code snippets

---
- [CREATECREATOR.JSX](#createcreatorjsx)
- [CREATEARTICAL.JSX](#createarticaljsx)
- [CREATROARTICALS.jsx](#creatroarticalsjsx)
- [EDITARTICALLIST.JSX](#editarticallistjsx)
- [CREATOROVERVIEW.JSX](#creatoroverviewjsx)
- [CREATORSETTINGS.JSX](#creatorsettingsjsx)
- [NAVBARFORCREATOR.JSX](#navbarforcreatorjsx)
---


# CREATECREATOR.JSX
```javascript
{/* ADD SCREEN LOADER */}
<div className=' w-[70%] mx-auto py-10'>
        <h2 className="select-none text-[1.5rem] my-6 capitalize poppins"><span className=" font-medium text-[#a7fb1f]">create</span> channal</h2>
        <input type="file" id='coverinput' accept='.png, .jpg' className='hidden' />
        <input type="file" id='uploadlogo' accept='.png, .jpg' className='hidden' />
        <div className='  h-[13rem] relative '>
            <label htmlFor="coverinput" className=' cursor-pointer bg-black rounded-full absolute bottom-2 right-2'><span className="p-2 material-symbols-outlined">filter_hdr</span></label>
            {/* DISPLAY COVER */}
            <div className='w-[9rem] h-[9rem] relative group rounded-full left-8 top-[-50%]'>
                <div className='w-full h-full absolute hidden rounded-full bg-black/50 justify-center items-center group-hover:flex'>
                    <label htmlFor="uploadlogo" className=' cursor-pointer bg-black rounded-full '><span className="p-2 material-symbols-outlined">filter_hdr</span></label>
                </div>
                <img className='p-1 bg-white w-full h-full object-cover rounded-full' />
            </div>
        </div>

        <div className='w-[70%] mx-auto mt-[5rem]'>
            <div>

                <div className='flex flex-col gap-5 pb-10'>

                    <fieldset className={`w-full border-2  p-2 rounded-md flex flex-col border-[#a7fb1f] `}>
                        <legend className='mx-5 px-2 capitalize text-neutral-200 text-[0.9rem]'>name: <span className='animate-pulse'>
                            {/* DISPLAY ERROR */}
                        </span></legend>
                        <textarea className=' text-[0.9rem] w-full bg-transparent  scrollbar resize-none border-none outline-none' maxLength={50} spellCheck="false"
                        ></textarea>
                        <p className=' self-end text-[0.6rem] text-neutral-200'>
                            {/* FIELD LENGTH */}
                        </p>
                    </fieldset>

                    <fieldset className={`w-full border-2  p-2 rounded-md flex flex-col border-[#a7fb1f] `}>
                        <legend className='mx-5 px-2 capitalize text-neutral-200 text-[0.9rem]'>channal description: <span className='animate-pulse'>
                            {/* DISPLAY ERROR */}
                        </span></legend>
                        <textarea className=' text-[0.9rem] w-full bg-transparent h-[20rem] scrollbar resize-none border-none outline-none' maxLength={2000} spellCheck="false"
                        ></textarea>
                        <p className=' self-end text-[0.6rem] text-neutral-200'>
                            {/* FIELD LENGTH */}
                        </p>
                    </fieldset>

                </div>
            </div>
            <p className=' capitalize font-medium border-none outline outline-1 outline-neutral-300/50  animate-bounce w-fit text-[0.9rem] bg-neutral-800/50 p-2 rounded-md'>
                {/* ERROR MESSAGE */}
            </p>
            <button className='px-6 py-1 bg-[#a7fb1f] capitalize text-[1.1rem] text-black font-medium rounded-md'>create channel</button>
        </div>
</div>

```

# CREATEARTICAL.JSX 
```javascript

<div className='w-[60%] mx-auto py-10 poppins'>
    <h1 className=' capitalize text-[2.3rem]'>artical details</h1>
    <form className=" my-10 flex flex-col gap-10 items-start">

        <fieldset className={`w-full border-2 p-2 rounded-md flex flex-col border-[#a7fb1f] `}>
            <legend className='mx-5 px-2 capitalize text-neutral-200 text-[0.9rem]'>title:
                {/* DISPLAY ERROR */}
            </legend>
            <textarea className=' text-[0.9rem] w-full bg-transparent  scrollbar resize-none border-none outline-none'
                maxLength={100} spellCheck="false"></textarea>
            <p className=' self-end text-[0.6rem] text-neutral-200'>
                {/* FIELD LENGTH */}
            </p>
        </fieldset>

        <fieldset className={`w-full border-2 p-2 rounded-md flex flex-col border-[#a7fb1f] `}>
            <legend className='mx-5 px-2 capitalize text-neutral-200 text-[0.9rem]'>short decription:
                {/* DISPLAY ERROR */}
            </legend>
            <textarea
                className=' text-[0.9rem] h-[5rem] w-full bg-transparent  scrollbar resize-none border-none outline-none'
                maxLength={200} spellCheck="false"></textarea>
            <p className=' self-end text-[0.6rem] text-neutral-200'>
                {/* FIELD LENGTH */}
            </p>
        </fieldset>

        <div>
            <p className=' capitalize py-1 font-medium text-[0.9rem]'>Thumbnail/Cover</p>
            <p className=' capitalize py-1 text-neutral-400 text-[0.7rem] w-[90%]'>Choose or upload an image that
                represents your ARTICAL content. An eye-catching thumbnail can attract and engage viewers effectively.
            </p>
            <input type="file" id="cover" className='hidden' accept='.jpg, .png' />
            <div className="w-[16rem] h-[9rem] bg-neutral-950 overflow-hidden rounded-sm">
                <label htmlFor='cover' className='cursor-pointer'>
                    {/* DISPLAY COVER IMG */}
                </label>
            </div>
        </div>

        <fieldset className={`w-full border-2 p-2 rounded-md flex flex-col border-[#a7fb1f] `}>
            <legend className='mx-5 px-2 capitalize text-neutral-200 text-[0.9rem]'>main content:
                {/* DISPLAY ERROR */}
            </legend>
            <textarea
                placeholder='The Beginning: The Big Bang The prevailing scientific theory about the origin of the universe is the Big Bang theory. According to this model, approximately 13.8 billion years ago, the universe began from an incredibly hot, dense state. This singularity exploded, leading to a rapid expansion that continues to this day. In the first few seconds after the Big Bang, the universe was a hot soup of particles, but as it expanded, it cooled, allowing quarks and electrons to form. These particles eventually combined to form protons and neutrons, leading to the creation of simple atoms like hydrogen and helium....'
                className=' text-[0.9rem] h-[30rem] w-full bg-transparent  scrollbar resize-none border-none outline-none'
                maxLength={50000} spellCheck="false"></textarea>
            <p className=' self-end text-[0.6rem] text-neutral-200'>
                {/* FIELD LENGTH */}
            </p>
        </fieldset>

        <div>
            <div className='py-4'>
                <p className=' capitalize  font-medium text-[0.9rem]'>Category</p>
                <p className=' capitalize py-1 text-neutral-400 text-[0.7rem] w-[90%]'>Assign your article to a relevant
                    category to help viewers find it more easily.</p>
            </div>
            <div className='flex gap-2 items-center w-full flex-wrap'>
                {/* MAP CATEGORY LIST */}
            </div>
        </div>

        <div>
            <div className='py-4'>
                <p className=' capitalize  font-medium text-[0.9rem]'>tags</p>
                <p className=' capitalize py-1 text-neutral-400 text-[0.7rem] w-[90%]'>Tags are descriptive keywords
                    that you can add to your article to help readers find your content. <sub>min: 2 tags</sub></p>
            </div>
            <p className='text-[0.6rem]'></p>
            <div className='flex items-center gap-3 mt-2'>
                <textarea type="text" maxLength={50}
                    className=' w-[50%]  rounded-md  scrollbar min-h-7 resize-none p-2 text-[0.9rem] bg-black/50 outline-1 outline-neutral-400/50 outline'></textarea>
                <button type="button"
                    className='px-3 py-1 rounded-md lowercase bg-[#a7fb1f] text-black  font-semibold text-[0.8rem] '>add</button>
            </div>
            <div className='flex gap-2 items-center w-full flex-wrap py-4 '>
                {/* MAP TAGS */}
            </div>
        </div>
        <p
            className=' capitalize font-medium border-none outline outline-1 outline-neutral-300/50  animate-bounce w-fit text-[0.9rem] bg-neutral-800/50 p-2 rounded-md'>
            {/* DISPLAY ERROR MESSAGE */}
        </p>

        <button type="submit"
            className='px-3 w-full py-1 rounded-md lowercase bg-[#a7fb1f] text-black  font-semibold text-[0.8rem] '>UPLOAD/UPDATE</button>
    </form>
</div>

```

# CREATROARTICALS.jsx
```JavaScript
<div className='w-full min-h-screen max-h-full py-10 poppins'>
    <div className='w-[85%] min-h-[50vh] mx-auto relative  rounded-md '>
        <div className='bg-black sticky top-10 w-full py-3 px-4 rounded-md '>
            <div className='flex justify-between py-2 select-none'>
                <h2 className=' capitalize font-medium  text-[1.5rem]'>manage your articals</h2>
                <Link className='px-3 py-2 bg-green-500 text-[0.8rem] font-semibold uppercase rounded'>
                create new
                </Link>
            </div>

            <div className=' flex capitalize text-neutral-400 px-5 font-medium text-[0.9rem] gap-2'>
                <p className='w-[50%]'>articals</p>
                <p className='w-[15%]'>created</p>
                <p className='w-[15%]'>last updated</p>
                <p className='w-[10%]'>views</p>
                <p className='w-[10%]'>likes</p>
            </div>
        </div>

        <div>
            {/* LIST EDIT ARTICAL LISTS */}
        </div>

    </div>
</div>
```


# EDITARTICALLIST.JSX
``` JavaScript
{/* DELETE ARTICAL CARD */}
<div className='flex flex-col items-center justify-around w-full h-[70%]'>
    <h3 className=' text-center py-5 poppins'>Are you sure you want to delete the article?</h3>
    <p className='text-[1rem] w-[80%] text-center text-neutral-300 font-semibold'>
        {/* BLOG TITLE */}
    </p>
    <div className='flex items-start gap-3'>
        <button className={`px-3 py-2 bg-red-500 text-black font-semibold rounded-lg`}>Yes, delete the Article.</button>
        <button className={`px-3 py-2 bg-green-500 text-white font-semibold rounded-lg`}>No, keep the Article</button>
    </div>
</div>


{/* MAIN COMPO */}
<div className='py-3 flex gap-2 bg-black px-5 hover:bg-neutral-900'>
    <div className=' flex gap-2 w-[50%] items-center h-[5rem]'>
        <div className='  w-[9rem] h-[5rem] overflow-hidden'>
            {/* IMG WITH LINK */}
        </div>
        <div className='w-full group h-full'>
            <p className='text-[0.8rem] font-semibold'>TITLE</p>
            <div className='group-hover:hidden'>
                <p className='text-[0.7rem] text-neutral-300'>DESCRIPTION</p>
            </div>
            <div className=' hidden gap-2 group-hover:flex h-full items-center justify-start'>
                <button className="material-symbols-outlined text-[1rem]">edit</button>
                <button className="material-symbols-outlined text-[1rem] ">delete</button>
            </div>
        </div>
    </div>

    <div className='text-[0.8rem] w-[15%]'>
        <p>CREATED AT</p>
    </div>

    <div className='text-[0.8rem] w-[15%]'>
        <p>UPDATEED AT</p>
    </div>

    <div className='text-[0.8rem] w-[10%]'>
        <p>VIEWS</p>
    </div>

    <div className='text-[0.8rem] w-[10%]'>
        <p>LIKES</p>
    </div>
</div>

```


# CREATOROVERVIEW.JSX

```JavaScript
{/* EDIT CAHNNAL */}
<div className='flex flex-col gap-5 w-[80%] mx-auto p-4 h-full justify-around'>
    <div className='border-2 border-[#a7fb1f] rounded-sm  p-2'>
        <div className='flex items-center'>
            <p className=' text-neutral-400 text-[0.8rem]'>channel name</p>
            <span className="text-neutral-400 text-[0.9rem] material-symbols-outlined">stop</span>
        </div>
        <div className='flex flex-col'>
            <input type="text" maxLength={50} className='w-full bg-transparent border-none outline-none' />
            <p className='text-[0.7rem] self-end'>NAME</p>
        </div>
    </div>

    <div className='border-2 border-[#a7fb1f] rounded-sm   p-2'>
        <div className='flex items-center'>
            <p className=' text-neutral-400 text-[0.8rem]'>channel description</p>
            <span className="text-neutral-400 text-[0.9rem] material-symbols-outlined">stop</span>
        </div>
        <div className='flex flex-col'>
            <textarea spellCheck="false"
                className='w-full h-[10rem] scrollbar resize-none bg-transparent border-none outline-none' id="des"
                maxLength={2000}></textarea>
            <p className='text-[0.7rem] self-end'>DESCRIPTION</p>
        </div>
    </div>
    <button
        className='px-3 py-1 bg-[#a7fb1f] text-black capitalize font-semibold text-[0.8rem] rounded-sm'>update</button>
</div>


{/* MAIN COMPO */}
<div>
    <input type="file" accept='.png, .jpg' id="coverlable" className='hidden' />
    <input type="file" accept='.png, .jpg' id="logolable" className='hidden' />
    <div className='w-full h-[13rem] bg-neutral-900 rounded-2xl relative overflow-hidden'>
        <label htmlFor="coverlable" className=' absolute bottom-2 right-2 cursor-pointer bg-black rounded-2xl '><span
                className={`p-2 material-symbols-outlined`}>
                {/* ICONS */}
            </span></label>
        <img className=' object-cover w-full h-[13rem]' />
    </div>
    <div className=' p-4 flex gap-10  w-full items-center '>
        <div className=' w-[9rem] relative group rounded-full '>
            <div
                className='w-full h-full absolute hidden rounded-full bg-black/50 justify-center items-center group-hover:flex'>
                <label htmlFor="logolable" className=' absolute cursor-pointer bg-black rounded-2xl '><span
                        className={`p-2 material-symbols-outlined `}>
                        {/* ICONS */}
                    </span></label>
            </div>
            <img className='p-1 bg-white w-full object-cover rounded-full ' />
        </div>
        <div className=' w-[100%] gap-1 overflow-hidden flex flex-col justify-between'>
            <h1 className='poppins font-semibold text-[3rem]'>CHANNAL NAME</h1>
            <div className='flex gap-3 text-[0.8rem] text-neutral-300 select-none'>
                <p>1M+ flowlles</p>
                <p>1k articals</p>
            </div>
            <div className=' w-[90%] overflow-hidden'>
                <p className=' text-nowrap'>CHANNAL DESCRIPTION</p>
            </div>
            <button
                className='px-3 py-1 bg-[#a7fb1f] text-black capitalize font-semibold text-[0.8rem] rounded-sm w-fit'>edit
                info <span className='material-symbols-outlined text-[0.9rem]'>edit</span></button>
        </div>
    </div>
</div>
```


# CREATORSETTINGS.JSX

```JavaScript
<div className='flex flex-col items-center justify-around w-full h-[70%]'>
    <h3 className=' text-center py-5 poppins'>Are you sure you want to delete the creator account?</h3>
    <div className='flex items-start gap-3'>
        <button className={`px-3 py-2 bg-red-500 text-black font-semibold rounded-lg `}>Yes, delete the
            account.</button>

        <button className={`px-3 py-2 bg-green-500 text-white font-semibold rounded-lg `}>No, keep the account</button>
    </div>
</div>

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
                <p className=' capitalize font-semibold text-[0.7rem] text-neutral-400'>Deleting your Artivarse channel
                    won't close your Artivarse Account</p>
            </div>
            <button
                className='px-3 rounded-md  py-1 inter text-[0.9rem] capitalize font-semibold border-neutral-400'>delete</button>
        </div>
    </div>
</div>

```

# NAVBARFORCREATOR.JSX

```JavaScript
    <div className=' z-[10] sticky top-0'>
        <div className=' flex w-full justify-start items-center py-2 px-8 gap-2 bg-black border-t-[1px] '>
            {/* MAP LINKS */}
        </div>
    </div>
```

