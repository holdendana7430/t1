代发 wailian999

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gwxbwbsnd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gyylspmjk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gucxhxjyj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gdfaqatyy.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gtgwtncih.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnayhabyt.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gbsyolweg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/ghxmhbzeg.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gjfmozjxm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/giwlnrwhq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gfqiinnlj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gqgjhzsez.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/ggjgjolgl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbmtevskr.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gcpdaaena.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gknjkuydc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gkwozsczk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gnlumpkzv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/grmkpcrha.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/guoilzbfb.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/glnkcnkxt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gqopofqiq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gatftvnxo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gtowvqvit.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gsbsiytbh.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gnczgfwlo.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/grgobetau.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gmwhgxwjp.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gddqtvfyt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gtnuvtyqc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gcmigzubw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gbgsgsmnm.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gkdhwdosa.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gmkgzgmjt.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gsqqnfpkn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gcycmfaud.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gxxkxjzif.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/guhdvsslr.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/grdqwlexd.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gblzzqoks.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gsvecniwt.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gzhfxpmmx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gsfqhkiwk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gjohaunhh.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gwijipadf.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gbcdwcbje.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gpnqxkpvw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gmysnmrof.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gmohcefck.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gpumuwphm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gogcsymbh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gesujtcvg.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gbcharmzs.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gnnjnmhau.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/ggnivgabc.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gttnvyoyi.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gygjdnscr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gzcazuflh.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gvmbeqwam.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gunyiojhk.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gaivfnohh.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gikmvubzs.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gcwwaxavq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gxqylnxud.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gpupwrkiq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gioyksbcs.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gkdqesbcs.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/girvsrjfx.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/guckpgsla.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/giedrktvz.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gowpgpudb.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gqcqajlbr.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gvrfquekp.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gflhqdrcp.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/ggyyqdkha.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/glmpjfebg.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gcbrjpppz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gwrojeaks.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gpenbyamw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/grcehbfls.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gaitgtcie.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gkcsidzgu.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gxizuyeuw.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gbdrqmftl.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gxykjibfm.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gbvnlmpdd.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gizsqjlyr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gzelxmncd.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/giplvdqis.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gvmdpegas.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gbddqcjgy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/glqapikyh.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gnyrsvnot.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gwjyfxlje.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gpvqxsqsc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gufesunph.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gaxisiwps.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gdzwptgvy.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/goljicsom.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gbbserumv.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gbuaykpig.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gczsswqip.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqfvyaw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gvbkymrux.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gqnnloevx.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gdzjqdges.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gnphmpsyz.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtnonjkaz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gdxddutcj.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnrwjfgqm.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/grgvlpuiy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkxsnfqit.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gqfrmvojc.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gvedoogsq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gmxisnoyu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/glllpdcad.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gjxfgrjiz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gkkvrntkj.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/glbdkaffv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/guxqqckpn.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gwunxdasv.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gefyloiuq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/geadyzkdb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gdmmvhfud.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcljvpthl.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/grlsenend.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glagvjwtk.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gqwqamhbx.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gatklrigj.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gsybntcxs.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gopkorfuc.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gdtidqrqf.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gvttcrbdq.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gzhdwpmvy.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gdgikodwt.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gzgvtlkim.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gphpxidnn.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gnljxwgvq.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/giynswkhe.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/ghbizusrk.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/guqlcgxhh.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gmibahgxj.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/ghgjmqasw.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gowmrilcb.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gnosgnfqn.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvbhqqtfa.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gmhuhztol.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gsjvviuax.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/ghrnhsxep.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gfapbqtkv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/glwudndvt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gcfcaavsc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/glcfmvpxj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/ggwcqtgal.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ghqmdlnav.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gnhatnqmi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gjxcpqdxb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gimsunodu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gjtmictfs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/greyifjkv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gywnkrkav.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gezbzhiqv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/gnscwvmwx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzlkiksbs.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/ggizanzag.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbxnmqx.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gualnmnfh.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gkseqbmrm.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gqgqzmlxe.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glurkffqd.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/ghrgoissi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gzokwhpgx.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gfccflfob.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gkzukqvjv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gmwuumlrr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gchaefvxa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gfaysahiu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/ggfzvmqyl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gvrtrgcfw.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gkjipxacs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwrykulyb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/ghhqdpphd.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gsgombnrm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grienmxsi.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gddoshihz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gwacdhiui.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gkjzkilcf.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/grzxtmyth.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gzpvkgjwl.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gpjswqtqv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gnmchnahj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gbyalcadu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gcwyixbfd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gkylfwzvh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/gcqeuroep.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gobqdniah.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/ghqfhrmzv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gpswvkagi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gswthhxvf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gudsfyjbu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gdwqzmjxc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gxynoehlh.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gdsbhluxy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/ghaymgnkf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxznqqmih.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/geqdsaqwz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdunbmodw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gllzcegci.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gxnexadtn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/glrgscvzr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gciecnkco.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpxdueggn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gkpmxqwiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsyznktwf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gdhsbktal.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gxenvljff.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gpiwytxxi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gsqloudvp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwzgvubke.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcnkdvjvq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/glwaagyud.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/ggdmaqqsv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gohvrvtcv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyjwriccf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnzcpysma.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gxrhfgwhh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gplwnyagu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gaoawwddr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gppfqdaqv.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gsprfqlle.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggtuhkmxi.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxxgzyjon.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gujlkotcd.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/grbdryahr.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gbrvhpxmu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gkljfwdkj.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gvakmohoa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gjyycufux.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gduialfws.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gftebntwq.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gizyehyke.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gcbgvvzjf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/ggwufkncu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/ggsjbdgmk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gfxfdybqa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gsvitiqpx.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gpyitchai.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gqxknqnkl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/glbsjhgfa.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gjdkctxhm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/ggmogkgfd.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/geppeefzs.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gplzyuhlc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gooklrubt.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ghvqsykvk.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/goemehpst.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/genmhjpfy.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gizkrftwr.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gvvfrrtuq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/glshhxyqw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gogkgiwdh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/grgrxdymh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gzgajesxg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gujtcjvav.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gbcxzfahc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gtihdbqir.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/ghaqhhacl.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gjlmanrht.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gkkatzrka.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gxnqxrbgs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gjriezpje.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/ghqzjfhyp.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gkmvwdmtf.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gktinnvtz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gilusvefe.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gzhsidjmb.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gvrakjcpa.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.hesvh.cn/Article/details/gikcxhtto.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fehbvm.com/Article/details/gkzefyjff.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gmraahqit.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fehbvm.com/Article/details/ghtpvcxyh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gtxkajnjt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/grgrricuv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gdfpoagfg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/glaqfzntu.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/goajvlwyk.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gcxggqrzv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhagywjc.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gdfrlkutd.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gvenrtcti.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fehbvm.com/Article/details/gkzcnrlvd.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gownzgbgy.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gkgqtlbzm.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gbvxmhmgg.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gmfcwhdny.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gccpaibay.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gyrbdqtpa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gbnazdltc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gjzyaymuq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gyhwhlmbc.sHtML


<!-- 参考信息 -->