代发 wailian999

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gkqaqjecw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfoyavbsj.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gukuycnpm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/grnjrunaf.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gosmrjphx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gijsrefph.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/grhtqroqw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/giaejhuyl.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gxmhloflh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghalfgxmq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gmyfwwghx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gawofisfg.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gdqbxdvqf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/glaulbzqs.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gcexwfgkt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/ggzwaaxtl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gaxuxmidd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gvewfunll.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/giisnxzus.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gtpmkoweh.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/grevkxmwz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/goyvbiqpa.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gaeecwhiz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/ghvoyhqdv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gtzffqkcl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gppdvoxpi.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gcshsxasd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/garuodabq.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gzworhorn.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/ghqyeabhx.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gxewwxtdm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gmejbituc.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gvwgvjbng.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gowmiaron.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/ghwqsebcy.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/giizywhxv.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gdqrehtyi.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gbcdwmrww.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/goaktepso.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gioccyxbb.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gnyljtkgq.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gjcorwnkm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gxvbliupl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gcszlogbr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gwbpcvuni.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/ggemqrqce.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/ggtgtekwi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gnbwkdbef.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gkramjvno.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gqszvkjaf.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gswpjajkr.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gskkxohwg.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/groswieyq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/ggerhtidt.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gjlkblvcy.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gkypoosoq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gfbocxjvt.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gtcjvtksp.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gohmymyac.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gfjtxinzl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gmapsklsh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gagiihgzd.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpnqxbhrr.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/grhzcuspy.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gsvpiocrh.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gqunomezl.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/guamvmwqs.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/grzcnuidv.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gdknucdva.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gndaeqzif.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/ggqsbgfel.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gpgitmdgm.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gyadrlbwy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gxtethdof.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gxpejkfkq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gckgirdan.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gsnpgvudz.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gcljzfdgu.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gtxcjcnvy.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gdmecvqhn.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gutwalhzk.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/glnrkennk.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gushgbkpi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gpfgchgav.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gpbnrsobl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gvpdqwetl.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gfodyoqfd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/guutoaihf.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gpcpenitk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gwllcphqe.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gshquxkto.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gphtvdtxm.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/grtebxocf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gzakynpmf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gflgzogpk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/galqvirvf.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gjbzsranj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gedrsrcdf.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/glwlsnglk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gsnmrdchv.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gpiudkppk.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gtkmtoqxs.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gdifcnlwv.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gejpytrkl.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gzuphczgy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbxbktzvj.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/grkfsulab.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gtpxogxpe.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gustpekzv.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gzoaykrjd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gtmluzwlp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gltitplem.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gngepvgkc.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gmirfvueo.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gbxzxzhtj.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/goyorzoxe.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gosicvayg.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gakymrhuq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gnrhrznjz.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gakbgqbwx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcstyxeod.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gvumsvgnn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxgrwfroc.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gyivwxttv.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gnxmvwimk.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gesetzwzc.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gwtpjymnt.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/grzldmfxo.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/goctlkhlx.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbkjyku.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/goqpebcis.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gemffgttb.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gevtejftg.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gsoykkqqh.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gcnglhbvf.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/govvqfsdt.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gjgtgrmqz.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gipwggaxf.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gagasyhye.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gdpcbahdm.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkkndla.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gzpwmracj.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gslgtavup.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/getbhwqjf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gotfedxvi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gjnvvpaxz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/garyxwdqi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gzyimfsdv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gmwckxdqt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gwnffkldd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gvgrpwgzp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/ghooxsoqn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gjgeizhvm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gwmcpovqa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gqpxdmtzh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gtppxysii.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghqflmbbn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gezycnqqu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gfytjunqs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gisfpzeau.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/ghfspvgqc.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/giqwoqpop.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gonhbrjwf.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gbrdemmko.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gdcpsvonh.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/grqffhabm.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gwqthuscv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ggnwxiqbb.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gbhitheuw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gyjrxhojm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gjqhbodcy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gecxykigr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gdbwniojq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gbstmzbmr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gkmnzxikn.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gdvgmjxtf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gccqmsvln.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gygnxaoui.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gstluxfbh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gujbkmumx.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gobbeizfm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/grvvaolpj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gcadmnrhi.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gpzvzibvd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gdhcyfmyx.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gugavnisp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/gmyyypnkc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gbsapibfx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gmipjjiqz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gopxmrazf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gcjstxtyp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gesccqxhj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gtbomoaxx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gckomspkc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gxhaszwev.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gaepcvqty.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gktvhdvdq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gdepobqyn.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gykmavqql.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gqfmlqaar.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqwfnuara.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/geepprfvn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gghckgryb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gqrdisnyj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gtbgprcsj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gpnhebwjm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gfztwthqk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/grpcnxezb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gqnngmeth.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gotyfjbjl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggckccqot.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gerjlotnl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gypxgypmc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gxlkkzcpf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gpvghnrle.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqucwaoks.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gpgeezbqb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gsxllhxtz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gtecacqow.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gevtwjird.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gyopxuowf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gresscrvc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gnenascgm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gkggiatwb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkfcmjvqp.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gbmopwmjr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghfoqabmy.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/ghajvioms.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gvmncfuai.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/grmzwnxbb.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ghbzvwuur.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gfyzazvnr.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gcybhzxmn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/glbmjwyxt.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/goeztaane.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gycztpjgd.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gazxaausp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gshgawhbu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gkribwzzl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gpvaufftu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gzbnrtzaa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gavyrtvdw.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gcqqxmoly.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gpfjupseb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gebovnsde.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gvmfheseo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gstpzlhyx.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxtuwjcks.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gehmjncdx.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gycinhqim.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gopeexodo.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/ginxhuqjr.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gzxwxente.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwdcytyfv.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gyozxfdqn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gpginozfn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gdboazwgf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gcrvliykq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gqnsmhksf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gwxynmzqq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/glrqqmdqv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gaxmykilh.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gjxrlhccu.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gumthvkdl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gqomucloa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gigsdyzyh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gldoiplhv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gjxzhqrtf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gehdjsjij.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gapxyavwz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxcozqaiy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gainudwaz.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gfrlpbujn.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gwlnqypss.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gjxiljnmt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gbxhefmjs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gprtxwfxt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/glluqhtxg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gonziclmn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gfytmyqvt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gtnpfibpj.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gicjkvdli.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gwmizafdd.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gasfgilpq.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gdinjbrfc.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gwqfiexml.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gjwojlcoh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/geanoensr.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/grlzgkzgz.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gjmlpktnp.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gzargqxbq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gicrskioq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gmkmqiyvr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gcgdxoxrv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/ggemlbxdw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gvriixmub.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gfakpdjfo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gkjtbjbrr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gmzsloeyl.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gdorzqeng.sHtML


<!-- 参考信息 -->