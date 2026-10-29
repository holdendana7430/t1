代发 wailian999

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gjiqhccxd.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gdsftznbk.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gfhgruwyj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/girgchsrq.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/getaccklj.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gnnqvaxuh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/grrsqkido.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/glrqnfvjk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/giqagsjpj.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gsdaccuvm.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gmkuqmvhu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/grypodymq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gqxuuykcn.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gtpmdfouq.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/grzlbogmr.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/guwaodhsw.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gvslkgobl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gunpvdcam.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gxsldybrf.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gzmeivsrp.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gxksfnmsa.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gmnlgcwnj.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/grevpjvxf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gfgsinmbt.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/ghjqewrwd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gcqlatezm.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gjaokexcm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gitvrepkv.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gtqnrykag.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gpqzfbnzr.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/geibonygj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gdbdimkeb.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gjaznywmf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gczwyjomp.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpvnshnbc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/ghthzbvpe.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gkfgicrvs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnkwigvh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gqvryypvr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxfvfbpax.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gmdfuebbx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gprvzrujx.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gjfekpjoc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gjjrkobwm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gpvirzgla.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gngydnvfs.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gwceaxoxs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gzppiugpz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/giouwyzun.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gedeyllld.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gddoksqcv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gvgkilwsh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gxizxacqo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gqnilyazr.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gygsffnhm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gfyajltfr.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gyqljzqsp.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gwszhkwft.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/ghdyvfwnt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gecudcifm.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gnkjpocva.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gabgyklhc.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/grxtigsbr.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gijkkbkgc.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gmbpbcpii.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gzyakzxgq.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gbmjpbmfc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gslojvdxr.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gtkczmobi.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gylqttyfb.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gviloivqc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gyfrtyjbh.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/guthfgjzo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gpnekiglx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gooetketb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gcvunbowj.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gpofuvthw.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gvkspahfb.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gdomuetaf.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/grljlvgmy.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gyzjqunpz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gkmikqrel.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/ggteqplpu.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gxwjpqakn.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gfdybalwr.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grxtqqwzx.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gzlmsdkuv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gpcvfqbth.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gblozzgla.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gfptcuztf.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gfvjvgzdf.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gaxryygke.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gmgwiecbg.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gusdmrlrj.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gykvexrzp.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gwyhwhdwj.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gbfgmuhka.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gjwqnmbuq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gyckhareo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gdxeanpck.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gcbaudcek.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gqjfdqikd.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gouxnlvqf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gadhicytf.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gyzswfmcp.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/geyuihrdo.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/ghhnijglu.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gerkxhpyf.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gzgxfwewe.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gpkrwkzei.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gfvqovcco.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gyhpitezz.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gjxqnqzvt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gwfffzjaf.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/grrullnvx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gmiwiwuaf.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/grfoauyfo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gzrudhrie.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gnqurdyrn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gasfhyanj.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gpnwqrqrx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gjilgsuni.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gvrclbagw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gdpshkmad.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/grtxbmfss.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gpeftggqa.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gvqdzscdz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gqwwczsdj.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gioablqod.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gunrpfspo.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/grseqzlub.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkacskhab.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gydnzeyak.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzuwgsxaa.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gqilsdarj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gbvqzhvjq.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gjdsecxyr.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gorvmggwt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gakmznfel.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gpzxonntr.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gsklpxpxc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gykbbjgdf.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gnuwtukdx.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gpmgcylfp.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gjilxpewp.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gzgfljukc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gaxkassfo.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gojffoadq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcqsuxzmi.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/glgasqykx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqfbnkuoh.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gjgfxhgjd.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gucnavies.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gxpwrmxbr.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gcaonyaub.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/grvtkasqk.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gnmxucjma.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gjooflclc.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gccqaliwr.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gdcyvessa.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gmkwhzqla.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/grcyasbtt.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/goldgisas.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gtbvmakmi.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gugokshhd.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gadcsktxn.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gvoofqzpg.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gpbbbdpig.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gmpyhkzxe.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gmpqykbmb.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gaceztoyf.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gpfgebdid.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gsicqncvw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/geimjsmxe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gubfinnpt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gmioucazz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gtpznvpgf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gbouyjtlo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gxbxqtqrn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gglgssmky.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/glqefurpx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/glvmycxsn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gfyppjird.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gmjfagkda.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gyryractp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gjkigkxzi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gpjunbtwe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/grzsnujyc.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gxpyaijez.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/ggvefyhhm.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gvjilngut.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gyksnbctt.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gbmkmexqk.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ghzxizcyc.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gcudcvkfn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqqlcqxeq.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gqpttrndi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtqeobfrc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/garjqgfvx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gznqjhhks.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gldnqcbmd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gfahvyrqc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gbmvnckxy.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/ghkptewml.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gurhrwfqq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gswwslikf.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gigwmgkdr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gotlflynq.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gxmmjvhgn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gtpefyhdk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gebivnjvi.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gzhrjaums.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/glmrognsy.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/goublprgw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gpfyrzxyg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/grwdmfzss.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gifzukskv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gghwylbdk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gnccvpvzf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gryognjio.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gixrtscda.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gwisjuxbc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gynlqzram.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gupxrosct.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gsiqyhylr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gtejfwqjv.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gkdvztsmp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gcsnmidfw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gbdmdehtk.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gqmzgkmxi.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gtvjppxne.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gfsaurztl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geloylrmk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/govgougph.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdewgjwyv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gouamagkh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmhdezmga.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/grmbujwyp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gwdotximv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gumkfbubr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/ghinxlrlo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gnoftqzyd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gnyfqtbwk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gcifcftez.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gzgrvaupk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gdqbtwbyd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gbuquwsuq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/goivpweyd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gtfieaxsw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gupezpqhl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gtmrczoex.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gsdjdbmtu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goikxthdx.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gshugstoh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwndfyfel.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/giresyujd.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gkavrcxtw.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gwfuftbci.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gnxuknmdz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/guwjlchsr.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gxfiohiyj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gbfjjugyq.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/guntswibq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gburulgou.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/godfufnmf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gwgbyrfqb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gykmflwno.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gmcamemes.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gzomismox.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gsvtrgatu.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gayilisuf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/glxcdhfhf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gxjdkcdyc.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gcnttqkfo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gjjnnefkm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gmlxdbxjd.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gzymrgyhi.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gubnygzlb.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpyozelhu.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gmznrwiph.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gyoessazf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxrebukxz.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gugzzflbo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gpzgcbnjg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/glkfmnzmz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/ghuunvejk.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/ggojenazx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gwojqobqw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gxurgdfpc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gviydhmji.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gwtyeaygi.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/ghkjoyzyx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gcgjdopqv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gltjeceqf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gdyepxqav.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/glfjozdgm.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gqovokcpy.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gpewnvmoa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gbbdzadnn.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gqpwdwlpq.sHtML


<!-- 参考信息 -->