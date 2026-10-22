代发 wailian999

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2sababkwi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ailikqvi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jvzxcfcv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gcqxktki.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kxfbxhfz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wfkhvqss.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rxtgwjtx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kyzjjwzj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lgxxayqg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2yzjqvjjr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hqtdttqn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bzqiwxkq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pxwdmefl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qwnnsccu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wvujsizx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gxwkisxc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ayffvytp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcvdwkeg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wenfrvpi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fxecnpyy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mkvonfni.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zzujsrzo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gdlfetyd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gaqgvncq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2huxauccd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2yesmjuyg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gcmetkkr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xnqqiosr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kslxbmfs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2eqmtfzgm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2piqijcme.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ozrcfucc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ghpzpeek.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hqjkyeuw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2himmqbxy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2opydkakm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2etgtctgy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2voisnomm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cdmtfawq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgeahwnc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mmqzktzc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jjwwljlu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fyjblkyu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tsecxokl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wfvupnlx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2foyzxuae.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ufujpigb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sbhawrto.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vfgbocxp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jenxirdo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ovnoypew.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sljppkfl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gqxwxmec.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2owuvswiu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hdydcqly.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hgvsuaje.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zgecqkwz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aihkvwxh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2yboflvet.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bhpjjvmn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mccqxiwh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2avsnsazp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2uphiybck.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2olypawlk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nhuexxwf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwphnmho.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2etdsnhxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tlskciod.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zkwtgcwl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wnkppfxw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ayttrgmg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2thpratrg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nhujpxdo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fskrpcen.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2squiwndc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2oxebytta.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2efgiubwg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2buymbcvj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2kcsdgqnp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2srivgzlp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2cafqjbfe.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gqhsdmnl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gaudwhxq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2recrzchs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gmkgyrte.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2sdurcflp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fdhmngtw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2oxylcarb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vzewypfr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2fdhbykdt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2laampaja.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ohbtvoav.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dwolnmhe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fnbzskgt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fmjobrle.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2pvmtumhg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ftlqasko.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vzzfehpm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sqcbklcr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jlydrdys.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2knttjidp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dunmoyep.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2soqccegl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2axermrcc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2pqaubyvg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jyizgipi.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hbbvgcks.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkekmryt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fwmueqqw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pqmnpxvs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2myrgnumy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmapaly.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ivnzcpdr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nspeblua.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bpclvtkz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bzwenfqt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xzltmnlv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lmozjrna.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wxhtuzhz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hvmbutdp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tezrvgnl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yeqseeiq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ertjfxjr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ulhofuqf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2igrweuou.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2rwpcuynj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mfpdqoio.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2kzmlcndz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mcygyfod.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2olwvrubr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tnoprvbb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ofvzuzuo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lvclgjay.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rxapevvf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jawlseob.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2epnvimug.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qinljwyz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ysbscebo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mysfeeiw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2phcrsqas.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ccfdbacu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xkiirvmz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rhptqxcv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2waeuritb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2yccmfpfg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xvjiskdr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mexthqvv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kkxlovdn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2icuszlwv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nfimqgiv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2shxbsmqg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lbtkeajf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jfttiwwy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kllxlqpf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2szoqhdtb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykwwxodl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2awpnevse.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gjkqmxob.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2prgmyyzi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zoikeojr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2irgpbkjg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2oowmgbdo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2itshktrb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2pmrvvvsz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2hhmhhfdr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mohzmytr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2kqmdlmry.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hzhcgzfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuggvyay.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2aiboujth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyzzsdth.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vslkkevc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2seymbwwc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2voyykszl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2laqkkubr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kwkwzlvo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gxzhizkt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hzboptjt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gfivrulh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2aghfpuwe.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vtryrdct.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2orewpdiu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nrcqlkid.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mtwdidri.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2cxcyzrfa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mcegrbsu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fepagmua.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2buavgjjq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2egwovcnm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wcswinut.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lwowihpn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2rnewpfsc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zxnkpybk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fzpynamt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hpgytush.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ewtbqoqc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2hrnnpetu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rzgkxupp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bljaohxs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hqxaxqep.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vmngzaxf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2crltcqme.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cgfdslfy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fkjywfiw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gfedmpvo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zchvzhwc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ztpmywbp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xmyowhrl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ezfzsbho.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zvsawuzi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qwhvlipg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fgiwntaj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2byskrrgo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tcaydphz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qehvrdfu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yllfdimg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2kgkjqfxh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wkzyvmgy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2hclnadxt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2poggafsh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2hmvbyczn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2hwonbdao.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wmaiayus.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pvzqhush.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nritzgzs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2mriabzmi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2mvdvzyda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfjddwch.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dnwmsbwi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hbsmgyev.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kiptzifr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ulwiuvyv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2qserbiyf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2stnnnsoh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qivrxxxs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2spvixrlx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ywoxdeaj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rzqaaqoj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mwltvzkx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mpwcnadp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2cvirullx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2duomwbsq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2nkcbcdgl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qbaqchqt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2garaxrkq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2cannavuf.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2tzdgzfoq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2izagirwj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xtvdgzad.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cijfxloz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2znonogmp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wvawmlha.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkrczrqq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zcqttgsw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2khjiyyox.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qfpjjfti.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gqdzvtbi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2htchbtrm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ylgbeqcx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gehaymfn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dihwqwdg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tsyrozko.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2taaehuez.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kymcddnn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wimnlihl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqoqtxql.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2neahfpwz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zokgytbs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rrdlbaqq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2grhvqtst.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ikyutpuz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2brszvoqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmcyyois.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2sktjnwtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yomqyuhp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cyzizxsa.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2udejdktk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2iofumvfi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2iruzoxsw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2kqbjtfgm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bainrduk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bajbjfwy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dgsrsqqi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2elxjetyc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2irbmfyaq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zzxgqzdx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gzyczaqz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uwqfvxfm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hjsvbode.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2coxkixso.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2arabzyct.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2wsvfcbmw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2noijtevf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hteffbod.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jsrgvfpe.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nkqsnzyi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bomizvma.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dqjfxjbc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xxavfgxe.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xqivqlog.html


<!-- 参考信息 -->