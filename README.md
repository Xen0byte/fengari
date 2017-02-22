# fengari
🐺 φεγγάρι - A Lua VM written in JS ES6 targeting the browser

## So far

- [x] Parse bytecode
- [x] Opcodes
- [ ] Basic types representation:
    - [x] nil
    - [x] boolean
    - [x] table
    - [x] function
    - [ ] string (8-bit clean)
    - [ ] number (32-bit ?)
        - [ ] integer
        - [ ] float
    - [ ] userdata
    - [ ] thread
- [ ] Tag Methods
    - [x] ...
    - [ ] `__tostring`
    - [ ] `__pairs`
- [ ] C API
    - [x] lua_version
    - [x] lua_atpanic
    - [x] lua_newstate
    - [x] lua_pushnil
    - [x] lua_gettop
    - [x] lua_type
    - [x] lua_typename
    - [x] lua_pushboolean
    - [x] lua_pushinteger
    - [x] lua_pushnumber
    - [x] lua_pushlstring
    - [x] lua_pushstring
    - [x] lua_pushvalue
    - [x] lua_tointeger
    - [x] lua_tointegerx
    - [x] lua_tolstring
    - [x] lua_tonumber
    - [x] lua_tonumberx
    - [x] lua_toboolean
    - [x] lua_pushjsclosure (lua_pushcclosure)
    - [x] lua_pushjsfunction (lua_pushcfunction)
    - [x] lua_pop
    - [x] lua_load
    - [x] lua_call
    - [x] lua_callk
    - [x] lua_pcall
    - [x] lua_setglobal
    - [x] lua_upvalueindex
    - [x] lua_createtable
    - [x] lua_newtable
    - [x] lua_gettable
    - [x] lua_settable
    - [x] lua_absindex
    - [x] lua_checkstack
    - [x] lua_getfield
    - [x] lua_getglobal
    - [x] lua_getmetatable
    - [x] lua_setmetatable
    - [x] lua_pushglobaltable
    - [x] lua_pushliteral
    - [x] lua_rawget
    - [x] lua_rawgeti
    - [x] lua_rawset
    - [x] lua_setfield
    - [x] lua_settop
    - [x] lua_tostring
    - [x] lua_rawequal
    - [x] lua_error
    - [x] lua_concat
    - [x] lua_isstring
    - [x] lua_istable
    - [x] lua_remove
    - [x] lua_rotate
    - [x] lua_insert
    - [ ] lua_arith
    - [ ] lua_close
    - [ ] lua_compare
    - [ ] lua_copy
    - [ ] lua_dump
    - [x] lua_gc (unvailable)
    - [x] lua_getallocf (unvailable)
    - [x] lua_getextraspace (unvailable)
    - [ ] lua_gethook
    - [ ] lua_gethookcount
    - [ ] lua_gethookmask
    - [ ] lua_geti
    - [ ] lua_getinfo
    - [ ] lua_getlocal
    - [ ] lua_getstack
    - [ ] lua_getupvalue
    - [ ] lua_getuservalue
    - [ ] lua_isboolean
    - [ ] lua_iscfunction
    - [ ] lua_isfunction
    - [ ] lua_isinteger
    - [ ] lua_islightuserdata
    - [ ] lua_isnil
    - [ ] lua_isnone
    - [ ] lua_isnoneornil
    - [ ] lua_isnumber
    - [ ] lua_isthread
    - [ ] lua_isuserdata
    - [ ] lua_isyieldable
    - [ ] lua_len
    - [ ] lua_newthread
    - [ ] lua_newuserdata
    - [ ] lua_next
    - [ ] lua_numbertointeger
    - [ ] lua_pcallk
    - [ ] lua_pushfstring
    - [ ] lua_pushlightuserdata
    - [ ] lua_pushthread
    - [ ] lua_pushvfstring
    - [ ] lua_rawgetp
    - [ ] lua_rawlen
    - [ ] lua_rawseti
    - [ ] lua_rawsetp
    - [ ] lua_register
    - [ ] lua_replace
    - [ ] lua_resume
    - [ ] lua_setallocf
    - [ ] lua_sethook
    - [ ] lua_seti
    - [ ] lua_setlocal
    - [ ] lua_setupvalue
    - [ ] lua_setuservalue
    - [ ] lua_status
    - [ ] lua_stringtonumber
    - [ ] lua_tocfunction
    - [ ] lua_topointer
    - [ ] lua_tothread
    - [ ] lua_touserdata
    - [ ] lua_upvalueid
    - [ ] lua_upvaluejoin
    - [ ] lua_xmove
    - [ ] lua_yield
    - [ ] lua_yieldk
- [ ] Auxiliary library
    - [x] luaL_newstate
    - [x] luaL_typename
    - [x] luaL_checkany
    - [x] luaL_checktype
    - [x] luaL_callmeta
    - [x] luaL_getmetafield
    - [x] luaL_setfuncs
    - [x] luaL_checkstack
    - [x] luaL_tolstring
    - [x] luaL_openlibs
    - [x] luaL_getsubtable
    - [x] luaL_requiref
    - [x] luaL_checkinteger
    - [x] luaL_checklstring
    - [x] luaL_opt
    - [x] luaL_optinteger
    - [x] luaL_optlstring
    - [x] luaL_where
    - [ ] luaL_addchar
    - [ ] luaL_addlstring
    - [ ] luaL_addsize
    - [ ] luaL_addstring
    - [ ] luaL_addvalue
    - [ ] luaL_argcheck
    - [ ] luaL_argerror
    - [ ] luaL_buffinit
    - [ ] luaL_buffinitsize
    - [ ] luaL_checknumber
    - [ ] luaL_checkoption
    - [ ] luaL_checkstring
    - [ ] luaL_checkudata
    - [ ] luaL_checkversion
    - [ ] luaL_dofile
    - [ ] luaL_dostring
    - [ ] luaL_error
    - [ ] luaL_execresult
    - [ ] luaL_fileresult
    - [ ] luaL_getmetatable
    - [ ] luaL_gsub
    - [ ] luaL_len
    - [ ] luaL_loadbuffer
    - [ ] luaL_loadbufferx
    - [ ] luaL_loadfile
    - [ ] luaL_loadfilex
    - [ ] luaL_loadstring
    - [ ] luaL_newlib
    - [ ] luaL_newlibtable
    - [ ] luaL_newmetatable
    - [ ] luaL_optnumber
    - [ ] luaL_optstring
    - [ ] luaL_prepbuffer
    - [ ] luaL_prepbuffsize
    - [ ] luaL_pushresult
    - [ ] luaL_pushresultsize
    - [ ] luaL_ref
    - [ ] luaL_setmetatable
    - [ ] luaL_testudata
    - [ ] luaL_traceback
    - [ ] luaL_unref
- [ ] Standard library
    - [ ] Base lib
        - [x] tostring
        - [x] print
        - [x] getmetatable
        - [x] setmetatable
        - [x] rawequal
        - [x] rawset
        - [x] rawget
        - [x] type
        - [x] error
        - [x] pcall
        - [x] xpcall
        - [x] collectgarbage (unavailable)
        - [ ] assert
        - [ ] dofile
        - [ ] ipairs
        - [ ] loadfile
        - [ ] load
        - [ ] next
        - [ ] pairs
        - [ ] rawlen
        - [ ] select
        - [ ] tonumber
    - [ ] ...
- [ ] Debug (errors)
- [ ] DOM API binding
- [ ] Parse Lua
- [ ] Generate bytecode

## References

- [Source code for Lua 5.3](lua.org/source/5.3/)
- [Lua 5.2 Bytecode and Virtual Machine](http://files.catwell.info/misc/mirror/lua-5.2-bytecode-vm-dirk-laurie/lua52vm.html)
- [Lua 5.3 Bytecode Reference](http://the-ravi-programming-language.readthedocs.io/en/latest/lua_bytecode_reference.html)
- [A No-Frills Introduction to Lua 5.1 VM Instructions](http://luaforge.net/docman/83/98/ANoFrillsIntroToLua51VMInstructions.pdf)