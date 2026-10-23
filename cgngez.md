代发 wailian999

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lomzkndc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3uqbmbwcy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3yudbtune.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fppzkyor.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3idlbvtng.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vkzsalkr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3irzcrmzl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3deblsxdz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3deckqpap.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3lmkehjqf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jkgegfxc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3dbeatzyw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wvhfaspj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yayesacm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3yaduhqtz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vfawmken.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ijyeddyk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nckcqcai.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uccjtgok.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3btgbecza.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3adtlltwq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3sntrzooz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eqldyodc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hztlguau.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3tsmqkjrm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mjcjmshp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nahxhkel.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vzygaxeh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3endfvlch.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3yzdyenmg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpgdmrfl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3crdgztab.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wqjswlnn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3krwbrnyi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yvzqvgqs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lxdnlzyw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3emdqoogu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dlyucnbd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3clegigpe.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqopyjdl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tlmyjeif.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lvqjycla.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hscyytod.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zyybwtdx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3epifwqsi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnvxwoxe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wedexnls.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kldcuydc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gpdomtgt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ukisudcc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3dfwdgghk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uqwfhajr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ulakyifz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3dzeiashu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ejwmhxqk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lbjbxorb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3lpschljt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ixxhyohr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3iywkcbnw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rcsxamyx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3aerxzbuz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iacnalky.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xqdnmmys.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lbdvjatw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vgejbqie.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgndry.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3cmbprqas.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3clzibxtt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oonnqesz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zqirwivd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ibpcebgy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zksmqrce.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uzkrsjsv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ojjdsair.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kyafyjzj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jcsdwfvp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qjuvugtm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rojyrtjy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jnqawqje.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3llwjihaf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3wrwcvdxb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ldzwqhlz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rnlhvwua.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3uluiomnm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fpekapcl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3texfpfmj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vrgrchce.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3lkbidwkc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pxkntjzn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ucffbhqt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mszwkevq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlzyutjx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3oyveieke.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vzkhbiju.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dmwcvbrg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3gqvrznsu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ijcdnvkk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qsisylrf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lgwqnayg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cxsmqxgu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eyblkfgl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ghunjuqh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ehnxobko.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ykizcvpo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mbsopslk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3prrywpzb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vmijpgzf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xlhgggeb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3igtyrift.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3misqvpaj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3sgiwzzqo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mblqgpel.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jpewaeix.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ewgqbbyu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qarpdamz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3srdultun.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wjqywtig.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3aurqxtbd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uusfrhye.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxlxtvdp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3tldrnfjj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uubhqkbr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bmyafuop.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hestsqxj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3atndffov.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3btbbmkaf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lokloghp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zxbqqtuj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qpprwesp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hdyvalmo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3flpbsawy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bxhlqumc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3auxfxufu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iomfaptr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ghzlfqyx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wnyrevax.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kxcdlyxa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kqeboueo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nrgdmvxn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dznbsqgi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cjhctown.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pnsfjahq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ijqegtgh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cgqimpzs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3pbtwhzlm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nniywnkd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bajgoyrw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3szeogslw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hgrfjuss.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rnzyvhuh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3olmgqfdy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ybaxuyea.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3paosoysu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yjiotvmd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wrmvkyeh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3onggobto.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gwojjmnv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3miiswfxy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3osydoxop.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzvqhgcs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jpfcyglh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zaltsdrr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3omlxiruc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3blwysnbl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3nhaxgzps.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3pgzraszm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pqbzpbne.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jukperlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xidkjtcm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ecvtkzag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsbapgbc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3tqmgihps.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dwarenar.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hketxcie.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jurkobvx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bvmitoqm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rwqolqsu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pczuedzj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ubsenlqt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gmcyzjbk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jlikiliz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ohjbqufx.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3abtdvyyj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xyiqyhpd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ubklkufm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3esheibhx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tousjilq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3aczewpru.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fyneaezp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zbbzsmcg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wyyvyjac.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3awkizeuq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pnloyift.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gqpcdvuv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ftanqsrh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qnmkjcja.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3pmcrjnts.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sqekofwm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ydsumgaq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wermblge.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tmijcvbn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fkmsgncx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zngxyyme.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nhtbszon.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pmmpichf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3agmmqmac.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lafjvxem.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dmztyeya.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3yftkzjyy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kxjixdgr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gfipknar.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ipmojulb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3izyodigi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cdqgfafc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3biyolout.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ummttkaf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ytqpoajb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vfpzadgr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zsjqyipl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3svjmhcyb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3enrxnkdd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3pyvktnkj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3dstfogju.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hurutqmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztafgmei.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3bbhmqcty.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rdypypty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibwxkndg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3fsdesxuq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3feornkmm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xqedanmc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3qahqtfpu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xiofsofz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3oynnliiu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ykxwrrgh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3eahzdtvt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3hmlvaawr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wfltquoc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qfrzfocm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3zuxdzeds.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hubzdqpe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ffpfjuhp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3pfrwkdtf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3cbggiune.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hlmytwyg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3awtmujkl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3pisjnfto.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lcxsjigz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ktymtcye.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jpcjrmot.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jqcudwnz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvekcgfg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qhkdexha.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bryjlcfh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3maqwiupv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3infdinpw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ajnvqrjs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3npdhkhnx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ucgwrxhn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rdbecben.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vlswwqbn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jmnthkbo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3heydlusx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lmhkrqkp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oysstrii.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3otdcmhxi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pcbsrovd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zgktwibl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3msnpivvq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3adkfegbq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mpwfisyk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dmsscvdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snbaqmmo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxgixfbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztvlafnw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ameighgj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nbsjvmpv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3oehovbyj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ribjbllb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ssozfzhz.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dxivmqqb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hackmbza.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3yfgcfrdn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nmhxshms.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3yutjgpwm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3plbugqyq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tzlazziz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pedehnlg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qldtecjg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kiikchlj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3lxlxbuse.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3csmtvtio.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3awbmbvmt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3lpmikeok.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3bacnnndg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pwumrlwg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wmbrnvfi.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3czfioowp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mzlskskw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lrlaexdv.html


<!-- 参考信息 -->