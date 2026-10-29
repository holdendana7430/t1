代发 wailian999

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gqqhqcyoe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gmbiqhbzw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/govpzlnfp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/glqdxknrd.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gjjkgwfgb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gvmhowmft.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gtgngcfxm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gkikzytjd.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gfnzpnfgy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gpvymnnbq.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gyubfrars.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gprdhzzol.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gcdrixgiv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gthlkpgdx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gkyvxdvir.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/ghpfcbxji.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gthrqlgow.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gtzwacmjy.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gmujizxyj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gmujnztdu.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gtbsmrqzk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gskvcgwqr.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gnlvgvgdg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gqtrmhgzj.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gtiqlttfv.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gecmqrgyi.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gpimrhlfh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gmdfqaehs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/grmzpbibf.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/geswgxhmg.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gwibbkelf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gbbyfwquj.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gavkldbbq.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gpjxmlhox.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gmalpkiqv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gcyoraihl.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/giqrwiqnf.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gduusdfax.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/glduthycr.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/grvgrrncu.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gjmorvszi.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gsodunrak.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/ggvhpxpay.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gizijtlap.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/ggruggyrv.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gjghxdsgd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gjojbdjvh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gzlttxzot.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gjryvoygo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gcugivaqq.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gzzqcotul.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gqhfuzfex.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gpyghlrqs.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gchtojhqw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gjffhqemi.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gyxfqagzn.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gmrkroqgd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/geafcrjbj.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/godfiayym.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gwvjchtpb.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gkcyvvsyj.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/ghtgscwvu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/ggmpzrhtj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gsspdqrsn.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gxubiltxn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gvrrozsfa.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gvqvzfcvm.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gcbkfhcaf.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gpkskzldc.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gbarjjnsh.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gbpsnlfwu.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gnvwnjklf.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gjzpkvmrj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gkmrnlnkk.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gjemjezre.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gczxthqyd.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gqpxileag.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwioyfcvn.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gzoscfain.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gdlqwncus.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gaqnsrmws.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/ghenzltkv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gyuawqhnf.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gqkqoyhal.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gvpovqbjo.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gblngqiyw.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gjpvongtg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gpqyteyrv.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gxyvulgcy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gttdhcjdf.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/galswuzye.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gxicqeslo.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gsrzbxtct.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gnlisaznr.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/glnhxegsw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gifewedap.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gwppxytoz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gcnlvwakk.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gdbgzbnue.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gyhnwozfj.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gufcwznxx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gwiizjzzc.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gjgpikqny.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gyeqhafdh.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gvzyqivfu.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gscmjpqpe.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gqrtrefsl.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gmykdvfbu.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gndrdjdlp.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggoacenhe.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gmquiovxu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gtyvezkxn.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gyxijucwx.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gfatcejxn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gdsbkbboh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/grsqrnuqe.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/ghirbtkhb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gdeckbwxl.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gdzonnrsl.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/grywxndde.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/ggvriiuao.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gvcgpqzmq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/goduzfaro.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/grpbbzghn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gipntjsnz.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gddkncfgh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnnqoyzgb.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gkrcwxdqx.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gpjopqlso.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gmbcvxwfw.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gysgtgkgn.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gljqjctfi.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/glofdfmsm.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gxymoiaxx.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gkztfawrd.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/ghcfqiiel.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gglpvasig.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gcppldzsq.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gyxchjsgj.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/glhkbpdyl.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gwalptsvp.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gzbsnazcu.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gytoytfiw.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gyrvftlff.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvbqjuh.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbgkmwtsm.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gpsbvtzmi.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gymsisjrl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gkhibrfvh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gtoybzpoy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gompcnfya.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gsirwcash.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gnswsyawa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gvdlskitv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/goltthuet.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gkezmwkuz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gqzdjwmyd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gogtmowho.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gjmetfkvg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gwovvvggv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gfllhjkgc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/guahbpbjc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gzinizvhz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gfpfhoawl.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gyuhmibxj.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gugcubllt.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/glrudewcr.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gjarrygky.sHtML

U 高频实用片段                         120
来源：http://baike.hesvh.cn/Article/details/grltxzpkx.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/ghpyjlkgs.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gtovyesmk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gekismvtz.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/glojqqkps.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gyfygqvya.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gehkpsmgr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gkmasffia.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gkmfiyzxi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gvftlyoks.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gtbickkmo.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gpgjatxna.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpcbqkbfg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gnzjfqizy.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gkxwczqdo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gadkkkwhe.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gzbpnvjdn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gbtkyzgvy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gvfotyioy.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gayatuvep.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/giimgcnja.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gyuytabiz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/goifwyynn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gsokhpndx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/guyabpwkb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gnpvbakke.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/ghrmckagx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gcxyorkbp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/grzpbhijt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/ggappblys.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gthjizmhd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gzxgumulh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gbmlmbhtv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gwutcuoux.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/grrqkudbr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gbybgjmbw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkcphtkih.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gwzxbriwg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gfrzdhvhr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gpktggezp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gabxvmsif.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvydvgkxj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gwuujxyea.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gfrmhpcvd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/ghdyypstv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gncfctkwb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gmkhdspap.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ggbjvfmgw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gujotbahx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gsedyhfgl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gzmlctpxx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ghsxczqaw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gyzhvahdr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gpvvlwamn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjofhpzhu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gpfrvgubz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gtkgxvlvy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzciwouxy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gbbduwvml.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gsuztiuut.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzljffdqa.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gvjjknsem.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glkerczkw.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gwobdmkwg.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gcfkeakah.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/grgumjvqm.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gqbbpnaku.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gzcqatunb.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gbokmznom.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gsafxsxyu.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gubwvnefk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/grsnowimo.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gtwrozdur.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gpwtrxbsq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gyjayixfg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gzdboliul.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gbkasoelg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gwoafzxqv.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gwaxxtlfo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gvhtflpaq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gfryhzcly.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gcysqzlpj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gzqwcygiz.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ghinlbvpx.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggogwqdcq.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/grawibchk.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/geucxlvyn.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/grcqgzbkf.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/giiuqztln.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gezshjbqj.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gcomtrmsn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gcqonobqb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gseopawxv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gfzjrdzpb.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gybupuoyk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gxxjmelbz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/ggbhegyvl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gahuavnic.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gcumfgxgn.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gqwgihjap.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gaprutzra.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghopvojdg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gudzwyjuc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gpkgrsdbn.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gtxbsyize.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gkkudlvls.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gjwzrnghg.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/giiuhgbar.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gcrkrhsso.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gevlpjyte.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gldnqlpzy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/geutnrnga.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/geajebwva.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gdznqkboa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gsgnzzljm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gydvzntma.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gkmzucxdr.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gpfzwdmcu.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gqogphfwe.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gmphxgmnf.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gsqdebctu.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gjuqbivig.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gzimisgiv.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.zdbjq.cn/Article/details/gqfatvfji.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gwafcayqo.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/ggrxwixes.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gjyddyzue.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gfxkipuis.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gdmuphjjp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gxugeihne.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gzczcngbw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gebxviycg.sHtML


<!-- 参考信息 -->