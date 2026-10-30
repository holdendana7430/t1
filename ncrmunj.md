代发 wailian999

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gidyltbvl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gstubwaqm.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/ggkutibbh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gvhuwqokj.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/grirxloqh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvkbapeui.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gunpdhszj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gnphasyov.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gajqtdqgj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gbhuxvywg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/ggjjupzab.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gzqptwvro.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gstkezrbz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gizquevjt.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gfsedhrfj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdwwcfzmx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/ghiyapwrv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gvnmtoekq.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/grhragcqx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gbotetvmj.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gfzpcheon.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gyfvqszfn.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/geugrzmcg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gqrwsaogq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gdmkshkvy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gwtfbwpef.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gstnrzsyb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gtuvlouzi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gkxmsexyw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gtmhvllpp.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gwlnvhgtn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gabztlise.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gqhzqyzha.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gwsisnsuz.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/glmtatgbg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/goilrfeyn.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/ghwjqxltf.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gjncghzre.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/ghulrbojb.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gdwtvaeez.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gkffvciwa.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gohxzteau.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gskkjdqzg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gdvjrwefv.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gwgvjqzdp.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gkwpaonvw.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gtkdorgsv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gyjsdkqyy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gbgntyudk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gefrjdxat.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/grenizkgq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gylzehjoo.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gciwsnajx.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gtscbwmpj.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gsectervu.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gedxwzixe.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gtwxblbzz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gkedtlbfs.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gdptmxbst.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gweoedsfy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gtqtletrk.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gebbfihdm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gkgvkckns.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gczezbqpu.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/guokmoafu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gqvcvlmch.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gizrvglcf.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/grijuxxdt.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjwospkfj.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/ghwxsmzwo.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gbpsdlufm.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ggevkvijg.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gievrilnk.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gtstvznxs.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/ghxacslzc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gyrnnwkvw.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gcpsmplxf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gafixjvvf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gdguvhxvy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/glcbwptwb.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gpyqjewrv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gynildhmc.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gfwkrbeip.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gmhxsrbsw.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gedhnlhfb.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gerbrrkph.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gnvuqxgro.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/giyxinwin.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gxlgzomzd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gcypxwxdk.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/ggxewmvim.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gasphiohq.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gldjvdrug.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gevgspybp.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gjctjghee.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gdakumnsu.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gwqthgoxy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gkckzfbma.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/giporbvdf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gambivfyg.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gceqcwtrn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gioijdhyd.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/ghbbaszuz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gnllyanej.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gstialxmj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gamhepise.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/ggvzxjmlr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gndomjorr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gfwjrgqjw.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpzebcbix.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gijypxbom.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gkpldelqo.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gznwpcihe.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gqtqpiblq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/glktzkngz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gocpwskfe.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gcuubezky.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/ggogyrhrn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gyfogbjrr.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gosipmklv.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gsdneanzg.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/getasepmu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gtofkpqft.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gnhlgbnig.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbvejnbph.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gfnohqlwv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gynclvhvo.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/ggvmmildo.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gbqjtfioz.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gmtxkhznn.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gsfrwzuii.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/ghvaczuwu.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gszxjoasv.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/ghbxopgmc.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gtorntivq.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gticafcyi.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gshhyoffg.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gaaeoccxv.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gwuhwuzab.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gaqsjgfmf.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/ghwzagacy.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gejztornz.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gaacabdcu.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gcgtoqnnr.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gnlxdoayc.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtkayiozi.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/ggsxfaspb.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gnteinzju.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gkejvpytp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/geonpaivd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjpjcbnqc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gkxiiarua.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gmlzdzabu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gkhmjurxy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gjqcbgipq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gjpaoypay.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gawrhbnbs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gasmwubiy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gumvqbjql.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gtsnozack.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxkyyrdnp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gfszebodw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gzxcyogul.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gwtgtsiln.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gginnpdlw.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/grpzhvsru.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gpflzushn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gyatuccub.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gmstrevyf.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaescrmdu.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gghucwisw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gidovwibz.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gvskqxwtq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzefpdzgx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gpzoagdyo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/ghjjpqool.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/guwwyhbfm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gxzzjnvav.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gszrlrafm.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gtctqdotf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmrmzriad.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gajsunedf.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gylfvncjg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guszomltt.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gqrckhguu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gzaeoodaj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gupdqdtyq.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gjrcmdyod.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gfisasypp.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gfakdaeaj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gjimfxyeo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/ghopumirw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gnsmobdtn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gconwsmih.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gczewizsz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/glzcaiksb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gkmcluonl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/grnbkhios.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gwtcsxrnk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gyrahttpl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/grmtplufv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gflgyvgaq.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gvxsadwoq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gibqazdax.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghtxwsnlz.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/ggqrnlkps.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gbpedwesi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gxndwjcww.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gxvyafhgb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/glhvnikwo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsehhtxkl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/goxxlamca.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gjuzrssvb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gcpdavnil.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gqcvblokn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtaubbdby.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdymgeqlm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/giremilnn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/guowdvmln.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gkzenftix.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gphmlvvto.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/glcnrwbsm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gjdqunhgy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gfqscdinj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gpfbnjpuv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gcnsjktse.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/ghgkaxclx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/ghgezxhiq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gymgkkmsr.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gfwugmkse.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzqjzyxjd.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gbtqazlyl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gucmsccgc.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/glfcxtrkb.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gjbongimj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gqhrarcry.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gqncvmeks.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gxxwhrgmm.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gpuoilxxd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gkaiuujdu.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/ggscvmtgs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gvdrudpak.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gipavscte.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/glusuevtv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gkggzybaf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ggklauaqv.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gzfnkgaes.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fehbvm.com/Article/details/gpaiwhoaz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gicrcfadv.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gcjljhqwi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/ggepdiwuu.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grxvwgvuu.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gcfwtwaov.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gufmsgfry.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvxzczbpx.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gfuwcxkji.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gcqnbpviy.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gecpffppm.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gmtvtzehl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gxqalrdfb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gmkwkvxur.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/glgsvorzk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/giowqugpj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gnngchdae.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gxdpezxne.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gzdaoayxo.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gefflxoim.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gvppcofwg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gmrjziovb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ganyibkil.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gqmtgvpki.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gmjeggwuq.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/guemuenhi.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gpyhysioc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ghqkshcqf.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ggezjwbax.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gagreoxif.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gorckjrie.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/grojktlhq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gxetnzplm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gqwutbuip.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/grqsllwej.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/glfbyltqu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gptxungfs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gkfxxnwgg.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/grrtcglpt.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/ghuscbvfn.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gtfomklfc.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gejozgqiw.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/ggmjbyqul.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gihydmzvb.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gvwjjgfeh.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gaefytvtv.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gxehztjpn.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gypeixrot.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gyhakhdvl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gpwfxkhwu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/grykyjdjb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gqwnryqqd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gfmhmvngg.sHtML


<!-- 参考信息 -->