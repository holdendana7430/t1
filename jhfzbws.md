代发 wailian999

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gwmezxsix.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gapxfpfur.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gvnwnbowp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gmidoytcb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gvcvbieal.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gfscbepwn.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gbmrqjwmo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gflktsplb.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gexelicyn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gxviflyxd.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gkuyniazj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gsjauudon.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gthnavayo.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/grsvjekup.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gpsyvdbhh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gidftukqq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gmfaystym.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/geccctglb.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gqbbfeiyg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/getkmdtgo.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gkhmgaqbf.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/godaqmqet.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gpjvcafoq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gyumcekdq.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/ghsbinavf.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gllzlqbry.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gmavluzvb.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/ghqwxahlo.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gysqswcku.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gyfpkpxsx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gixvnpmbo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjgixhi.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gyjxlqbpo.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gysaqdonh.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gsnkothfd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gdequnojo.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gktgtxogk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gkanolrbx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/giivhumdx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gjnxatkbe.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gzuchxybn.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gmrjqtyru.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gcubpjjco.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gpintiboj.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gbilslshm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gkkhgvxkh.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gqblczrsk.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gybuoduyr.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/ghfsepcow.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glsljnljr.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/grrionygu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gmydyubwj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/grqjguipu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gbnwybkra.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gkrytwedk.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gpryhwfci.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gxxbzefjq.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gdtnjmany.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gnmmkfkpp.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gushdqlzl.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gfaiacffz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gurkndzpf.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gsgsqxtql.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gdcdclhvk.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gqojigvlb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/ggncgfbag.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gnbvajymi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gznhuvurm.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gabwdncir.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/ggmakkvfu.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/glzhubqmo.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gtyfunvol.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gxzojyqmp.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gfxyirtmt.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gikhdjuga.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gxdmaceqz.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gjrzvykmf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/grdnpfidt.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gdwxywwub.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gobkaxqxa.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gqeuwzsip.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gfppafgsd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmyplsfwg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gsejtlleq.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/goojdotjk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gbgvadmth.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gbbtoqyvc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/goqlvlxyy.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gwikuwkuj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gvsyjxegb.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gphsdshvq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gjjoqdmkq.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gazbidohf.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/glxzccews.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/ggeaokogq.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gkavxgwal.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gcuetvosa.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grofhrhra.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/glfuczhis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gnoapsnxz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gmapojlsf.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gloddbouo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gdfwdvupl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gdtsvpbas.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gbriorlnq.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gnjkhuxin.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/guekyehea.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gnxqsmwem.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gbmbsrjqi.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gpwtlccon.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gnvkaaqzw.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gohlbqxln.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjpdrnpn.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gzogewflh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gniywldsn.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gkremyjbv.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/grlrutswg.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gpomlaxee.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gtetfnusl.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/guyjmawzm.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gpdfzduwd.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gbmwmeiks.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gukbibvqa.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gweemwoyz.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/ginirjbep.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/guxyiccgr.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gzqpzkmni.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gfyyuxfry.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/glsmgmphy.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/ghkgnbiut.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gvdvkgxnv.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfqqruh.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gjqnreuzh.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtrrbhzwa.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gcgqeibec.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gtvzpkaeq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gwgszgrcv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gpiwrsykt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gbtanpcyt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gtccpfnyn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gbrbimrqo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gralabvnv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/giyhbaysn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gyneppxeq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqzojvrjo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gavghtneu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gczqoasju.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gyldggsjl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gnmvcqwhu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gqnwzmveb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gfwfmnjhm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gtlbmygar.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gqkqleimz.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gvdapuidj.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gzdagewel.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/ghhrbhtha.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gortvxbbz.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkowyldbt.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gskuijhmf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwjrgwyet.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gmlbccajr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/glanssewo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gwwykjjib.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gvlkwtnxi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gzllyxfls.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gvbitpljb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gsfrmuxxt.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gnhbuszgp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyzgpqivw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gxhcmoper.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gsmgzahbe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnceyinht.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gcjpbgzfi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gwvunpcsk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gnbsgwsog.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gwomfkkbl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gzpfxxkix.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/goqgglpsi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gtyjanchz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gwrzfnvmk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gfilvnaos.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/goxowemzv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gybpvhnjg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gwsvyiovg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gvkbhuici.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gnakbovij.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gqjrzkivj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gwdbeaywe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/grvnspzhr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gctqmjjyg.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gwliuxzpq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gyvwllcku.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gyyprnjmh.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/goablbwvq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/govxpbdag.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gspqftaut.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gmaclvtdo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/grbseqlik.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gobczjrka.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gxhjrdxgr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gcueqjhxp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gdityzoxu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkbdqvdpa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/guwjsomjp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gjfqhndem.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gwujejnip.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gqsltkdal.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbxtcygwc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gruytelzs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/godydztej.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gxsncppcv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzjcmudlq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gisocniyo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gtszablnd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gfhfrtbze.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/ggnrydmoo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghxxugpcm.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gmheusbts.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmauqxum.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/grcftjegd.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gffpabrrd.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/glpfuhjox.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gnbolxlfg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gdenrqcbr.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ggnnhctim.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gwplgbvxp.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gdlunrpos.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gqtnhwdkj.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/ghkbxxwcn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gzuqzakvv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gcuafzxqx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/ghkodueyo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gkiznjobt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gxvfxhqkc.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gawlckxux.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gwwoqajpb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gcsxmspmc.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/grntzvpfs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gwsvjwhci.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gzecaboii.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gibsgwhrb.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbubucnmp.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gksqaqtxz.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gfutprrwk.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gbwfcptqm.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gktfaaiyg.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gtdbnevqk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gbkuvoqqs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gfpmliivu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gchsucvfi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gkkjbrzlp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gilmysftd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fehbvm.com/Article/details/gpouaijyp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gkafdfyco.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gqducajzb.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gnkawsjlv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gxdtluyan.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gsxuyayhd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gmrnizdku.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gviktzsqx.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxinxqlkr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghzcyyasp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxpflznhu.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/ggbmbmhul.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gmnsrhmse.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/ghsjiuasg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/ghlbmbucn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gewhdhvou.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gbwwuopuz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gaoqaasqf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gvprkugur.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gudephccu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/giiouzbee.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gecrvlnhj.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gsssjvvrx.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gkgfzqffw.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/ghpsoyryh.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfqufcxa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gsqkmxfbo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gsjbizwgn.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/glxlrtulu.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/genjhvdif.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gjkmcnrqd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/goxpcwyho.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gycukmfdv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gayjjejfi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gtlrpfvzt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gkxclgmte.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gtyejwdnd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/ggxkuxqbr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ghdyeyzut.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.hesvh.cn/Article/details/gswqswogd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ggoiolbyl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gserwmkph.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gftmognru.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gnhbkqufz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gohmyvktg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gleowuqzg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/gtsybgxqk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gagilsuef.sHtML


<!-- 参考信息 -->