代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fyqabfew.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dxttkocy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fbmaoqck.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkdnrpy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mrmzdjpt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tcpanslo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cunqseag.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tttzxuwl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mhuvzetv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tuaaklcn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ykoobzcj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3uuqjynck.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hznrbaly.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ujnedlgf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vvcdaopi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3nxtvsdxu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3jzuheyrv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qypsjsbh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ajhxsvig.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3drsmokqk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3irzhneyp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3gzhdrxhh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hgopojnn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qcgpwcoz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3jizokhep.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bswgbelq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aiaigezx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ymcpnqql.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cgwxepqv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mbhcgkac.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dryhhsge.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rndnfvfe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eqnrvbec.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3esmquxpm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wkapvslf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3idxgexow.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vnzfykye.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3cufmmsvx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gbslwjqr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iycuooxn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vawwpfvx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fvcieaeo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gwnlvjnc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bodmiouw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dihmuiox.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gmbqxhwg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jrhxcpyu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzmnbwge.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jmdyjskl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3fxlilttw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yqqcccbc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zqdaowtv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3caatoctl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ctidelmh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3prlvkbkh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3tpmtvofq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jphilzjc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rdtkrnnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpcqnqcv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3olcajqcc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qkgaylzw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qjbpbcvk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ouuzlmhy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ccihmkhd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ijpatjvb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3quhmpmso.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xhuueptc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zjnjbjqw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3klkrirbi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lzrdqxwl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gnowvamb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ypkcdatp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cnpjzpnj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3scvvqiju.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tawrivnn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pooinqvr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zzawjyym.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vdwawtzf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lhlslhvz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ixxqujnu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hpjpkhaw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kojbiprj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ftemmsho.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hwkasbtf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lbprqlby.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wotuitsj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cpydtbwm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mfclycxe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kcwqkxcv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3umyjtqgs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cvkxwiyu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yqozfddo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kmcdazxm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uvtehpno.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3wjzzvkvo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wrignpsv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pqfwbyvq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ggimbwao.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kaxualza.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3zssuafci.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kfzotkht.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wdrlcdrq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3nsatcqbq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lrmrzdxx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3igczhkfb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gsshuzup.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lkfuzkbe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fnlrreka.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3filoovfd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3yzzdtqrt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3pafumefm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ljczfayr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvxlphgz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3fxgsrnlx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ieirpuhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duuppcwy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3klzktwio.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xmovkkki.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mxtpprja.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3vxphoqbm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xmeoxsqs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vxqnwqhr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3iuqixgjt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wlvgstre.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3omrlejtv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3yfacetxv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vfcrqdnf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3mrmsefnt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3cyskuzog.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3hsezzazp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fimheyuv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3clptdykp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3equyasjb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3aymwryeg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3uotujgce.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ubidlgpn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mjcteaqw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3tteiuxgt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yanyrhvo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sexordzm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3shsniuwl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dznkfuvg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvifwqzm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iehlettj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3iflwayso.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tpogonfe.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mttuqjws.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jkxmgshu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrndxqzc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3apieionh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yhjimmke.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uznvoefl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vflklcvm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ugcbzszy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nsaotvyu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vbxrkooz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrwrrsod.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3zmxkhcpk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wwxypils.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nqdxwdyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjeajjay.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wglxhbie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjyelino.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhpnvspt.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ibermdxi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3udfnhbhr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3duwlwnxz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3wkutvicx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rgqczzgd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ajomwddt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3uhesahgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wezgyloi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3skvdwofx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3vojdyppa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kxpwkrlz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ezdxjthn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tncorbvv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qeecmpao.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3cxkomkgr.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3raubcsiq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3apizihbi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3gjxxrpxb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3urucxtdv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3inxfrbcq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zaszhnpp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zacodbhm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wqlyuxud.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3neilyajf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dlitssta.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rprmdibj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3xfstmyvb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dlkxxcmd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdscjebx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wbdamxsx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3abhejowh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bpfyqdjd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ibqeigwg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3eooffktu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3yovpnbop.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qrewqocr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qwktssee.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ohcdukwr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fszeaesg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oviwaxyi.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nxhynueq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ayiexuir.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3szenacac.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ehtydnzp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3deeantof.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pvrgijlf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3scxbjxix.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rzjyzdyl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3panmusot.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eiguoflz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3apoukyex.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3faaukokx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cwuptztc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lqykcbkd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pzmobaqy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bqbjxrof.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3gfqmdhxt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aeqmnbdj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ytntlbfs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3yxisqiev.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3gtpameqr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ukhealib.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tjqachtb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gwmejezp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3paskyyib.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tpbfrhiv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3sqiroylt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kfppvfcn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3szxtbqzk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3qzcccjav.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fxpsqgfl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vuwllyps.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bjbcxhua.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cqojyubw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ompvgnzk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bijkzcck.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3skbxajbt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ceasmodw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3znqhuwzh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqobdudn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cuhqqwru.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3wipaprad.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qbnawsnn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hpebnjiw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ztloufwv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3swhqjorb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yefdlfgj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3bhaoxmsp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3rcnhtuqo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qjikznuh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xfstszjt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yehaxnkg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jdzlypsj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yvkakngi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yantyljd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3frhzjozz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nfvnwzzt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qslhlfwk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zcgylzqd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrygndey.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3fzbrjngr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sxghcbdn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rayumugk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3neafnczv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uqerqomc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3nxmkabmc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tmfpfdhi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ciayvpse.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3peumgaxn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xiczffta.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ghdxjvgo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jzwqrujv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hyfqfqib.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jwifgpzt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kpfnxfli.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bflupqok.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rlkumvzm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qyswarbw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jbxhbayn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lpqqdmot.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nocppmhk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vusnomhy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wewalqox.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3oecshvuy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yyylsypc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mzxymyfs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yjsnbhet.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fxzwbicj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3klbwxarp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cpmjvmhy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3pdwfiavw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3uqtftnny.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fklpfkfn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ejbjfkkp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fchwyrpm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3pjldiofd.html


<!-- 参考信息 -->