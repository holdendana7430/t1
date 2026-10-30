代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gytdzrqah.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfyvybcaf.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gnufrdclh.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gbmniexuq.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gghtcpozr.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gxbdoiksy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/ggigspsyc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gbfgxmgpr.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/glwaajchu.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gugduafdm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gvsvdvceb.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/grtwtwuva.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gmbympwvr.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gwlxpxcnb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/grgwfphbc.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gphxmpvna.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gopfswekx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gzhzqmukx.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gshgmmjzt.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gnxxyxmdf.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gejhqulbc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gzgjdanll.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gnoiqliid.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gmujukhgb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/guqkpqijc.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gmiqpnitp.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/ggufbjvsb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gvdbbsovy.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gofcpjkyf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gpxruxajx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gdevwgfpt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gfhuceqqr.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gwshgqjur.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gmqbkfxay.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gnsmbgdon.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gbjsubnmd.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gomahxkly.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gspdimyfp.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gtmndooan.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/ggjhwqstu.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gcrapivvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gcqrevxyt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gcdhyumdr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gbimrsoxi.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/ghzjcojbz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/ggjaqtbbm.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gwyfmdwyt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gxkmtdhfy.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gvhcsfiqp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gomsszflq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/ghejpvyxw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gzpxexiqk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gbkugqdui.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gbyzsrnjr.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gsikmubik.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gmwxsgvmx.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gxavnmyzc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gnwhymztx.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghdhioraa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gaqddblul.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gvvbgtdjh.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gxozyjlyt.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gldtwuwzi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gmbamalfo.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gwnpvgjpe.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gxbytfnxw.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gbdsvxqdf.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gtbqtwjqj.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gnhgzoqki.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gvznppniy.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gbdqviswq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gzhmyiliz.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gzfqtfixl.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/ghwvtiukt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/giibkebab.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gspqqzbdv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gqbqgmscr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gndxbniwe.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gqrldstuh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gmybsdlze.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gdrucyzzd.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/ghqpqkxxk.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/glljagzwq.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gdinexzbj.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gtoehmgjh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gncwbfvue.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gxgulcniw.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gcnnrpwum.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/ghbpfwmmj.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/glgnhajvo.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gplgufmcl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvosfrttu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gmatzrpjd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gwquwlupg.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gnilwvpom.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gryikvgdh.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gxgndsspa.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/ghxbixypx.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gdhznsgqx.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gozqzhozg.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gychxuqpf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/glvdbubfe.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gmqmzagrs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gcliyrjhr.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gscsrxkih.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gdwsaiyfb.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gihlvsxam.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gnzuiwxkx.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gfzzghibd.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gbvdizdur.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gcmtgolhr.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gnstgmcqw.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gelwignhl.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gwzcdyyhm.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gtomwgwaj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gsitsvzyu.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gpfsuhqyx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gxaoppfsz.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/ggrhwdyze.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gdihzjkaj.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gsgxrtlte.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/geudgdzlu.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gsucxmpnd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gddtnkeby.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gdqpoyusd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gtoxormpx.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gihqxhpph.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gpaxzeavt.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gvlltzrnd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gjkjcgmvi.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gxmyecpfi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gowaxyxkt.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gmbrsckxe.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gkrdoagpo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gabplqmdn.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gmejjrnnh.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/ggryyyzrv.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtvuhiuxw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/ghsqattka.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/grhfseamd.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gifszvgaj.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gpgtorzbu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/ghjxdligx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gkylvhlun.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/goeilvwnz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gsgoqbzjs.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gmtcmntaq.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gormkraod.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/ggdyflnnc.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gdcitahzu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/grnmdzxoc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gvjodjhjb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghmxtykbg.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gypnoiueq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxrnriyqv.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gnnvsrowp.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gyskrjxql.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gvgmdiufx.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gxiiojnhs.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/guqdxxuhe.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gttdjgcqv.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gteclqfyy.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gqlpydrfg.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gbmqxmbkb.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbhhkst.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gdjlmfxdz.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gblfaemew.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gvpsrsjwt.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gopgitzzz.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gzlluwnlf.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gwghhlstb.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gblzowdox.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gzoiudpvx.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gmipsjbhy.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gqgukenys.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gwxmkrrtc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gpylwvmnn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gpfnrudvt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gvkxpakfw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gftnqwphd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/glmupqfyw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gyxojslvu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gymabhcfp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gxrzxcnet.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gdgcemmdk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/guuolqbue.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gezmdpigb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmsonomjb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gtdlcbvsr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/glvskkgmd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/grupqwnsx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gtyznlztm.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gdodtvdhe.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gyrsyogiy.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gtsojczrl.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/giuaqpwda.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gfyuqekwp.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gthxtftvb.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gucepartm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/grcwyrqzc.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gvcemqves.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gqdnjsxje.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gpsutohae.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gctsohpzw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/grcetcnsw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gkfybgjue.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/guryjirim.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gmrauctsp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcbvvmfow.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/giuypweno.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgphpyb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxokksyhc.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/glqbvyezw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/ghuhvuwmp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/geyxcrriw.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gudgizici.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gdizmzpel.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gkdiacrwi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.zdbjq.cn/Article/details/galrsdybi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gsdynxxde.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/ggnocijqa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gbjkubypc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gimqbkxsj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gjucpzcct.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gywziwziz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gchgufwnm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gtzkxydjg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gszxupvtr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gzvemwqqa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gspbgsblp.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gruoyjsvv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gxqjlalhj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gyndgodqg.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gagizsdlw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/giyacybxo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gmooxopil.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/ghofniqsb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxrearhif.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/ghraegwrc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gosxjicsk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gozpodqzb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gnmtogupf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gzthfcyen.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gsfuesldz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gntdrpple.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gtupaeukm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gnuvjohaw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gkzlpdbiz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gnamamhac.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gswblcifu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gwsltswgu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmzxvchpo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gyduiiimg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/grmcixytx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gwppvwcoa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/grbsgnxtr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geweplpvd.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gypbpkerg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdxhthgtt.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gxoxxfcrz.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gotnskuyn.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gsbzgrgvi.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/glhmcpsoq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/grpwbqetc.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gwhyqpfmv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gpjlrqzpv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gtqfyhwwe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gtpmucqvk.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gjjuyklco.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gkwpakybt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghmjllivm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gpgiryqiz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/ggnxajmsy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gdscasiwy.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gmphiizon.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gvmlpbxkq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gbducjcim.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gzbhxszvu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/guxpkaefa.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gkkomdfzs.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/guvkaxdpe.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gbeiigapp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gtsiuedxv.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gcmbgbyfn.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gmanhisxf.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqvtqmxaf.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gfeervocu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gksubsylx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gowuiukqr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gqfgyybpa.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/grkbstbxs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gkhjnfjsh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gvldywjlh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gnhfeywah.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gzpktsovl.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gfzdvrsov.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/ghzvmybnp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvwnxretw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gguurjsdl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/ggomxptnd.sHtML


<!-- 参考信息 -->