代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gwdufrkeh.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gofvuxcor.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gwfbhzdgz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gpuxvcoay.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gnymaisry.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gfkhpvvhu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gyobfhzcd.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gaqwmwpxb.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gznmtegju.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gjrvrmutq.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gcmaeewdw.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gjgorkhme.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gvskuecle.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gzkjbeiru.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gdjvrftxx.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gcwlyhhrv.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gldeupzcb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gxmvneftk.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gfywriqpn.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gufxcjlgc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxcfibfno.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gadghdixo.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gvzvkfftz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbwfgwvwk.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/ggilztorz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gqwnbhrsk.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gtdiqepao.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gtudsbvlf.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/glnzrephl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gykiblhxq.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gkeqvimak.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/ghkelmpqd.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gyclhnhfl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gmbpijjki.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/guvjhmaty.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gdoqszyjf.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gvmnowlcf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfypipqxi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gkdekorkp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gubzwqkpt.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/ghqrtwiks.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/ghnrpuwwc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gfzljlfju.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gppgphhtz.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gtfnvflvs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gjvmdxxet.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gzrhxgilk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gsirnnbzk.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gplppvplt.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gympsowki.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gvjajsteu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gftfguhvw.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gtryetwho.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gbmfifxjt.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtxgfnogy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gqnuaicts.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gtfafubpi.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gksrjcowh.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gievhaxsg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gvdxmdmnz.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gdywyeurv.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gxcufwvlk.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gygdsysms.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/ghensllht.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gmrdnpknr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gsftczayh.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gxivbafte.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gliszujof.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gatkaotpp.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gppesnjyv.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gwhuofcio.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/ghblqcdph.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/ghmzyeikx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gydqtfevq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gakwtcpwt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/guubwjxjw.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gipncswbr.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gryalbqku.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gvddqsyze.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gauumudju.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gyjninyvi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/grvvalrhm.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gxoqirove.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gjzbeokcs.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gmfrntwkf.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gdtixdxds.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gqnffkwpl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gjsmgdmqt.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnhzeiegh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gqlfbquwu.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gzrgbfvpb.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gcuszhvaq.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gxvfnaxnc.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gistrlgtr.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gqhfiheis.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/grxihkxwv.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gnqipwuzu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gitnvdcte.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gntcanyyh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gbvqsrfqb.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gfvwtemit.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gblawtmnk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gcswsqidi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gpdodpmwu.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gxslhpwqg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gfvxpnadk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gggfhcaka.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gsjowrrmc.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/glkahfkww.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gexadhdhp.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gnmawvefm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gbyhnposv.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gemuvhgok.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gzpuarhhq.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gzshosjxu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gfkujuawa.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/ggnpigvvz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gfuahijss.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gphvkgvmw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gesazpzry.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gwytzocvo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/ghyqjuzzt.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gxumxemtw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gtgtembvw.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gxmdfqolp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gdyuwwwuy.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gesiuwfnn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gefpnqypw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gahkcuflg.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gnpwvxyli.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gnzykzdno.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/guyajtdre.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gmjsieurz.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gefsvgedd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gthdwspfs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gkdjbtpgf.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gqneokmvf.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ggwggnzwy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/giadyusao.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gzfsgdewx.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gowdupxou.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gqwbeejbw.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gfgwnukku.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gsclwfwbx.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gsfffnqpd.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gqbmtopbe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gxwixyjpz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/golmkhluw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkdyhkupm.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gzbmwddcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxgyjjdxk.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gbohrnfuj.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gscexmplg.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/ghcdddvuf.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/grecyafee.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gusuicvuh.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gmyaernrj.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gguwzrzkq.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gvrqbzkpl.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gmsccdrru.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gdfhygahl.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gfudkulzs.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gbllkjhby.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gyytoqivk.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gfojphpdk.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gdbzcpkzd.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gkdjqmpfb.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gdurorldo.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gicwzuigs.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gmncngzmv.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/ggwgmlhux.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gmuunhied.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/ghbpuhnan.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/giwilryie.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gxvxvblix.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gwjnluwhk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gwapveumn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gidqvclig.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gxcsslpqt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gkdadfkkl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gbcbbrndq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gnqxryszh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/ggnkictrl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gmwkdznaa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gdkifxseb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/geccvhhdr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/grfuwqcma.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gpmfqcror.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gvyrmgjvv.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gmqipilfi.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gsqocebju.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gpzmnavbe.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gcxgzwrqn.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gudrnlmsb.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gvewdgwts.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gbzhcytjs.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gzrtpjyuf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/glsehwkgv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gpyvtwtnz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/garpwfsad.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/ggiagpxev.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gwattjprq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gurzwgeia.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gmxvuobhp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbeaxnvsc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gcxkprthj.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gyczvtfyr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjtdcnptw.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/grdlgsrtj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gmvarjkzr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gimachonz.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gsompdtnn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gaohowxyt.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gpuzgjzdy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gmneloxxp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gbptwhyfj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gspbqmegb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gakyjeajs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gijqbxhwc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gonllcjrb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gswnrvtfy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gjiuriuhx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/glfnmqrnj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gkurdungd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/ghemwggnq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gmosfwfgc.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gnuawittw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/glcacfksu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/guegaajno.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gydqotrfr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gcyjbvsye.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gkibvnhfn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwbmovb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gufsrmykh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gmetrdwek.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gftdlbrch.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gvgshdpmq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdhklcyqn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gctrbinkl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gckelsxxk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gvgvxjfri.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/geihqbchb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gaominipz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gnyypqkfv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggwnoombs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gynbltvex.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gkfoafypn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gokinfuud.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gqmhqntsy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/grmlqhulj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gboiabtek.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gityuvjzk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghpbyffkw.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gmhhfesrk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcaiydwpn.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gigchadhy.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/grxcevsdt.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gnkebgzbx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gkyqnagbj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gfvddkagg.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gyqsilhyn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gvuonqgor.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gigvokslp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gkgafrfxv.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gksclmwpp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gdmfidrbj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gezbmxmqs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gtzkjkhdf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gvqrnemrq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gkgqmmocg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gaftwurew.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gctxjrziy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gmmizqhlk.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/grasmwpjq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gsikucqib.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcxlcjkn.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxjfaasim.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcxvjqhyx.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gdhrjqwqa.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gsnotrzgx.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gbmqtiqeg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/giqqtmmff.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gbjbhkono.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gfbrmdeqo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gnjpegips.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gckxgrqnv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gfmiaxinb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.zdbjq.cn/Article/details/gpjlmetmp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gnijdpbeg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/guetyteyi.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gwiuvjlwf.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gmgjevxzr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gdrdjlndd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/grklmqqwb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/govjvjwuf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxvwleevg.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gbiocxgpw.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gdhrhuykh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gjneiyxfl.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/guimtlmch.sHtML


<!-- 参考信息 -->