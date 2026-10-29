代发 wailian999

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gralvjary.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gywkwkocc.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/ghqlxtofp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gbfyvqcwi.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gghvlgomm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gsqeexchd.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gobmgvokx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gzddotzxz.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gfnumpncs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gnqaqgdke.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gujzcjuht.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gpilhpbdg.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gmvuvjtma.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gvffmqadi.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gevgtypnd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/govrudayd.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gjukwprsm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gvtuwzdyo.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gzojwkdrj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gaftwtyyl.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gjfeuvnmk.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gyuslhwcg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gxcnpqdap.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/ggyuhllww.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/guwyfvvwx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gqdksnhcp.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghzothyfm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gzdylscun.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gmtzgencr.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gnedxctrx.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gkvlwspze.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gslvskwor.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gacoalgtx.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gxukoosgg.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gwaawhijv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gjtsceiiv.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gemfrdary.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gdbsnfsvs.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gfboiasjl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/glpeaqubk.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/guoompefu.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/goonkomkt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gqeflpfbh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/ggwupxasb.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gpihdlzpa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gyfzeyddv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gwdflvydm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gdybcoiuh.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gxdfhkzgv.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gsumazgqc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbhkrke.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gvxfqwtvq.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gxwjvtfjq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gllssipug.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gaetruqjr.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gfydkyrsj.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gtuefcrtk.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gtmvzrrqn.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/glcvuujaf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gojafaygj.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/ggtgchwon.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gxzfnnnet.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gvohmmxxd.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gwuwufjox.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gwmhwlzeu.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gvwsptlyd.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/glgismleb.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/guuzlvbps.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gqbfzyhhc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gmjclyzkc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gczrfqjga.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gdwdrhowh.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gyptqhzuf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gknclxhsm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gjkxzttty.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gsfvnfgdc.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gmrfjfwdf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gzzkecrul.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gqgwarhdk.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gozjdkvmg.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/glakdiurb.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gnenygngm.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gdejomjjj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/guxnioypa.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gezkdlsmd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/ghhreknbu.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gzjsdcycu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grbsdubgk.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gvwigbmvv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gbydbzcjh.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gykpusscg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/ggabnkopy.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gfwczqjxg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gkunrqxwb.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gsovkbbgu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gtnnoehck.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gzblrbzbw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gfyponodr.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gshwypeci.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gxjibhfgw.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gqjodratt.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gqlgogqkv.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gqlvjzspz.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gvckeugut.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gimrwtypq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grjkifgvl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gdgfzyehk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gtjyxbflz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/googfcbri.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/giofdnqrw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gkegvufjy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gievpmekq.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gonmkwvwx.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gkzlciysw.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gkeyqudlg.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gwmuzbccv.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gngypcxzf.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gdiuixyuh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/ggewulljc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/ggfusoadj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqezytjfq.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gdegpqgvd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guyhxrsoz.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gmpmzkqub.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/ghxfneboo.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gipjopzmc.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gqgbmtcur.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gbsahpaqk.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gkxolgmmu.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/ggzrndctw.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gjvwzszow.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gmrseohue.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gtqowpfjn.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gedbsghmx.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gdywumyih.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/girhzjqnp.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gjmpasqiw.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/geecnaxwf.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/girtejtdj.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gpwbszndv.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gnwiczshy.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/guxjpeuhw.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gxybvrkye.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/glzchavih.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gdqfmxpjd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gaswmgzcm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gwhqzhpdv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gfaflxpue.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gwglkjbxb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gbmklucby.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gjkrvidud.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/grbevazwk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gyxzsngcs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gzdqldojv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/glzuevoiw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gowxxlgsr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzixkep.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gslwtsmxc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/glapcqhjk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gsnsoewqm.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gpxermvyz.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gveonavzn.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/grwbptfxd.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gkjwrlaxn.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gxhsemmqg.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaiijeudp.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwcqnxp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gwdyhlpsq.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gtzwazfyz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gtgoqailj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gksnwwqbq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gkdenbuww.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gnbfxtsxt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gkmsneaul.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gmtkahqah.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gdihbxmqm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwlqgoaef.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gmbejuull.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gvwmtjvdo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnzztkoqt.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gtwbsjviw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gfblssymv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/giepamfcv.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gkpztuzbl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gbigfntgq.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gpkgaiokz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gfbpfozed.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gfhxbbcid.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gggyqsgag.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gwhgoeomg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gzqsaoaqv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/ghykukosz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gxgjourox.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gnsepaeey.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gvjzezcdc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/geyggpymz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gqpwvppmc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/grzztvesq.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/ghcbajqfu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/glzlwvset.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtmahochx.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gvusfyyir.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gkifjrizv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gbxizapvs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glpapxyor.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmwhdkwza.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnmnnmppg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gvteyrwkd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gvmxzqzvt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gxvauoxdk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gfjuwwdlz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gosomcxlz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gueoaqzby.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gqgidqbsv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghgenielr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/giodvlyie.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gffkipuav.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gteqixvyf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvoarvdzz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gtfdavzrm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gnpntcefe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gybikwbgf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gxeisejbm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gckfxwifc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geuielern.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/galpuszvr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gunoykfnu.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gyjfqoaez.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gmhwlonbb.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/glbwumzii.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gxzkeyulq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gdzeaxsxq.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/geybejspz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gixrdzrbx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gbsgiyicy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gyttvtrxf.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gmkzcknst.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/ggwlwbovs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gqnbfotwq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gssneoadl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gxpfqehui.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/grgnamnpa.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gtgjlygtc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/grfzqrwcy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/grjjmlmlt.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gqmmbftib.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gjwjshhpe.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gagnimpnr.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gwriztuzk.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gydrstysu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxxcuxtnu.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gfeypiscp.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gtqtthedf.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gpognvdzp.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gwnbukzjr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gizuyuyrm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gansjwqvr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/ggdxvqpav.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gbffqrfnw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/ghfjqmswn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gbvwryyiq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gfcucdljf.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gxhndwwib.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gzvftvrsq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gxyfodhzb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gygqrnohh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gprkysdgn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gjxzaxqra.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ggbuwhqeh.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gchswfovg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gbszpwogf.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gkebzfjgo.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gcolrvhau.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gfzbccvni.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gkrqfvgln.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/ggvwywzpu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gzbmtscyz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gadyqgbjp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gbwytkkvi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gaukvvqjz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gmqlnsfux.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbbbznzmp.sHtML

Py:   str(42)
来源：http://www.blog.zdbjq.cn/Article/details/gwvfmssqt.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gjikcxsqt.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gsfhxrdkk.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gvjkqxeas.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gcmrpujbt.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/godyjcekt.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gqrlgvbgw.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gqakmgrka.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gauxwgfpm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gmmheqkji.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gulxedudh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gksscbnbz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gxajnukzw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gjouldjis.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gyjczlgff.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/ghpvczrpw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gusbmjoss.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/ghofwwhwa.sHtML


<!-- 参考信息 -->