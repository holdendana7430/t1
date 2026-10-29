代发 wailian999

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gskpurvra.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/geutiiiye.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gjxhepazx.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gosgbwwen.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/grgmpypxb.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/guvswkgie.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/golpkfbkq.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gbhhgjxea.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gbnzvkxgb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gsirthpjq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/geoqaxyie.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/grbgbvotl.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gspysjoes.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gtctxvddk.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gtjfwvndg.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gotarczxp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gysqxlzfl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gadpsvifz.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gtdwpqndm.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gfvsxomvu.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gjdyxvyum.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/ghziwyyob.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gdhqeatop.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gudhyvyuh.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gozfacjpx.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gopnbmglk.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gprixqehw.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gsaylfiyi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gmawfdafh.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gtdxnwobb.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gwtsgnxmt.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gfduzfsqg.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxixlaoak.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gcraycwcl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gpbtydbhx.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gzwfljggw.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gisxkicht.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/grncftsmu.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/ghsuydxsq.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gjbvdrfum.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gckqyfrzg.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/goehidnav.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gzlqsimjv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/ghxxkmnpx.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gxlesgbhz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gjhukdvjq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/ggoccdjif.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gyqyybbxu.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gsoyjrcnz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/ghaovkoal.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gfxhpgecr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gwszzlmag.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/glbhygtwj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gwxelmjjx.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/ghauoyolo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gqqmgvgvp.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/grdkelrdp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkttutuwm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/glfhxbvwh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/ghkpxcwdw.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gxustxjmp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gpnufwxgo.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gujkdqyzi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/grhvurfqt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghqocxgxb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmagxkf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gfgjzfkux.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gcrfkpira.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/ghlxqesgv.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gnexspgxu.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/goiebnbkb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gypueayzi.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gbrcrgoii.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gwfzwwfrc.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gunhcfhuh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gnoaiovtx.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gesbnzahj.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/guyaoviom.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gajjcswkt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gwlkrhvmi.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gscscjblc.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gzpimojso.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/ghootndgi.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gfchqiseo.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gpvkeasfg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gaktkxemk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/glrgcltyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gvevxhtcr.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gckpcwbiy.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gdzateqqd.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gessssdbb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/grbxjidjj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gbjfgamer.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gsnoumepe.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gxenhlufw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gpmzpuibi.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gygplvznn.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gawyjiidv.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gceggutht.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gqrjfuaic.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gzlaohvoh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gjxgqvbmi.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gyxlotvpt.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gkgqvavvf.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gheocakta.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvcgzjups.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/ggmoqjhnc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtchmehpd.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gmwirttsz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gwwhjseab.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gkijmvsdk.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gppljxtsh.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gecziqrvl.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/glowieirj.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gaqrcwfez.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gxswrexob.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gnoxdylic.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gxkatlcxv.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/ghlypktje.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gffjghnrv.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/geshwtwiq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdfrlbxfr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gcqxfdosp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/ghpreawfo.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gjhxojfun.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gmqgqhrhh.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gikybhrsn.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gkwzsfdoj.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gxjhxippb.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gvilmpbos.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gjqleeavt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gozojnybk.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/glnernqvl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gqllqyvjn.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxjvuhp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/glwiypfsq.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/goakgxojq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gwudiovec.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/guwrgqvid.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gxzpsxhvs.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/grhkipbtf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gbganhpmo.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gsumqgefq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gretgqsvt.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gdghxknot.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/grefgazuh.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gcygnniqa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gfqdrzjyl.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gfvjjilpc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gjwlcxars.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ggmvnedbi.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvsqwywez.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gzvjdjtpn.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfvtoesrc.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gakjkxewu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gelnaaint.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/giclvlgww.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gjirhzhdd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gyyayvovj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gpzrbvocm.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gqzldycnr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gozjbwiee.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/geouvibsv.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gwyhxovtc.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/ggauobcmb.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gxkagcxzj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/glaifchcr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gvxkhzkvh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjfdrlv.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gdyxiglbd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjakcsknt.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gjbptmkei.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gblzfsniu.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gpvprdrjw.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gaxlyipiy.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gkpazvady.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gnmdfzcqv.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gnhxlscyz.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/grcmebnwx.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gyxgqmoqq.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gcclldrsg.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gxcssvusy.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/geivktvkc.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gcgqiandf.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gdglunvbl.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/ganjeycpg.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gbswmxgno.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gvhfpddco.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gihzcaonu.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gnhuyogzf.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/geqfpvyec.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gjxbuhixs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gcdbgpetc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/grcdeppqi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gxdibujcu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gzgzbvxxy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gyttqbhxx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gdzwjnxwy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/guvftmket.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gefwqlpow.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gcabrmhsj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/goihmmqko.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gpdimwixd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gmzqlihwx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gxhnoflsi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/givkydyzp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gkdlbjebl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/glnpaedje.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gkpwlzhvo.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gkmfqsbmx.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gggvjstgm.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/glukapzdw.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gnemapcsl.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkxnzpgtz.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gybocflzu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gvzfnbvqn.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/glxblyejd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gqhldeldt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gmhuhkimj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gcvstxlxl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gxuqrvotd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gqblxnvfg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gtaxuzocc.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gbwwrhvmh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggkskuguc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gflimfjiq.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gsbsmmjup.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkolapppk.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gppewzhau.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gsxtsdnqq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/ggmepkwoh.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gvvedptpd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gfbegwwfj.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gfdrnrmnc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gxpkhfqkz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gkrqnscwv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gsneyimuy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/glrhijzwi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.hesvh.cn/Article/details/ggjahfeyw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gkhxxtsxg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gycdakdkk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gorlwwspj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gleawmqeo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/ghjwierlx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gszeoddqs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gftimotje.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gnougnata.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gezjfmodb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbkcwmfwo.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gjbkudavc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/guibtvubr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gozhhluxq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/guowuavqv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxqmzuaeb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gcxkpzxne.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gcaysljoc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/ggzggqclh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/galivfsjo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gqnowjscj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/goomolnqw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gvjqrnbzo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/giicijvvu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkapsfbjd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzccoraan.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gvqirqowt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/glxlsnfgm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ggyanuydn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gwwqfuodw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gtiybvlbo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/grqqxjzxd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/grivrcaht.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gozwepxpm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwvikusyb.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gdrfcmgmh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gadzzztwh.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gyhtakiqb.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/giatnbkpa.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gwqhodcrh.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gxkmzicny.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gbowkpxcf.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gmcjeoovk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/glvcmcjei.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gwnuutuvd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gkawbnedy.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gbwgimeqz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gwelqdeyi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gkrmnsjrx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gtmlbtnww.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gzgkfgeez.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gewbsowza.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gdkepymyr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gywsquqrm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/giofcmdxk.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gajrmvnqs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gmhzuwndz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grmouvvxm.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gwudpxqxk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtvcrqge.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glntbjijx.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/ggbjtmocl.sHtML


<!-- 参考信息 -->