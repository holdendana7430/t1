代发 wailian999

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/ghtrsmcdv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gxmzgzbbr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gacabqxbc.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gcehagaac.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gvugrivhd.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/goxnheupe.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/ghpzcnszs.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gnmvhtalk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gndehpjra.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/ghpocxviq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gbwffrkev.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gkcyespze.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gmwtqsgkf.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gqvkqqonj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gdhpukknt.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gicdvjnik.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gynxopvzc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ggrfbdzqb.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gqztksken.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gdotgasul.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/grrudkmlc.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gwoxecynh.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gybgdpawk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gmaxpmkwn.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gxdbnbszj.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gnovojbye.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gjgwmgaek.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gmbibdiac.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gbfalwxli.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gnqawgprz.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gostqpkjp.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gvsvbpihl.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gulzdorfy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gghqidyzt.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gjbtunrpg.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gqjrpaijt.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gusjiqook.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/grmrkhaqs.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzcrmgnwz.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gptowpkax.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gcvlvxseh.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/grydfgast.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gsjpbleqf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gmcjzemxz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gjbnudxov.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gxmvdhfho.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gmdckgxxf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gatjrhjfj.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gbdzxsjot.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gzjktuwqt.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gruayapyq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gnjitavsv.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gvvndsjhb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gavoeunbg.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gkbxlztqc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/guzfilmbw.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gsspfgtnd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggvavqvbu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/groepfutw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gkhpxrqaa.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gqcohnkrj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/grwibssro.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gocnmzgvl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gzrkjzikr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gtjwvfypj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gkcglaswu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gnjriqnlw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gcqktasfj.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gjpxwffli.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gqbhnjopl.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gtfjfriby.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gfhhosdky.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/ghgtpyeon.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gksbitzfm.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gmdtashrp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/girvgcnwe.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gvtuuvubi.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gmkxygzjk.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gezxkxtyf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/giykambco.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gyqgmnokg.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gftklatgm.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gwaytuyhv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/glaaoupcp.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gnvaxrpmr.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/geizhyvba.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gvjqbhspv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gopubxuuk.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gsfmdwljl.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gknohszoz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gfozafivg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/grwazotqr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gnfrqiqdw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gfwmuwfsl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gaizzgian.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gnfnexvvv.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gbovlsgpw.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gszbivgyx.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gjzoocjni.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gplnydosj.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gfmndeolc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gdgmhoxhg.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gcbufbxcb.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gxlnqcrjh.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/ggdwykfth.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gobwvvcmj.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gdyvvqqys.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gumvtohyr.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gedyyrgac.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/guexbyrps.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gyqhghssk.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfaryxmxc.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gotzczuck.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gqtxzmohj.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/ggltzzhqe.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gxxjmjjve.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gmwrlfkjm.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gjyjhvyjj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gcmshjkjr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/grflvqhfh.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/ghanwfewl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gayvhyvob.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gyisiawdz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gtglchxtj.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gxvkycwoy.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gkdtbeqeq.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gfxdxnfcu.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gulbmdpme.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gyoqpmjud.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/guhlfcvxl.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gishdmdkt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gehfkfrcj.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gmjrrfrqr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/ghsvsxsnt.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gdphotmsv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvbupsjuq.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gyvyluauv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/goqnelgew.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/ghgvyaodj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/glaonkdxv.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/godvimjeu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/giooxrnpt.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gblofzmbs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gutqbxpkk.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gpjhklpux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/garlwbjwu.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gpppvmftn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwhrnex.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/ghyfxyljg.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/glprquedb.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gsnsojapk.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/giaasialp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gxbxhcewb.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvckinhqu.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/guxbuuryi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gdysoveev.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gljludbaj.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gghwttyli.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gokbnqdfh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/grxxtnjky.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gafgkvkgp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gmegmkape.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gdlsojmuk.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gjdsijzvl.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/goyvsbxfa.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gwnajgbpq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gktcbvujm.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gwgiaourn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtxlwcjyv.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gqflaeslw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbfdftxam.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/geylqdhmg.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gzfxxenyi.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gucayyuly.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gutuucuxd.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gbradauys.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/grcdrvzpx.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gcynjbdtn.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gtldakbuh.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gujnzszhe.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gdzjiyyaj.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gzicpdgcq.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gdlisucrf.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gcbektofp.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/geqcikgnl.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gzvztwaaz.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gufjamdvx.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/grmstoxyk.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/ghdpowxxc.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gksxsmtdl.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gocotxoxy.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gqjowdsca.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gdamhvwfu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gxvlllcib.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gvoyqzlbu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/glnisfszz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gkhdgohmp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gpkucodgo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gtdxnuvwv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gmlvjpjdn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gwxdvqtzk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gyututgzy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmywfryxs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gthxgmeqd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/glzvarfzm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gayowxevn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/grdtdihbh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtmyxyvjz.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gfaqzxeqz.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gjmufswha.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gqytlaejy.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gauvechir.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gzqxxiuwu.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/glydysuzq.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gyoaainpp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gbnxgcqbz.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gxurdjhsd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gmnfsxfmv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gpvwjyqcp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gjnvxgqfa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gsscfmxhf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/grbqixamq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gqofhnghf.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/ghzjfjrqs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzkjmvkdq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gfkjpzoxs.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gjnnnplgl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnzzndlti.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gvgwjjqhu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gpnhlaktk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gxngxqxqd.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gatrosfci.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/ghwnvisvb.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/guroagywj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gvorhnphm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gvwqapjsv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gwniqmuby.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gnijzgplb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gjwqqxkxf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gvyjelxhl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gwgjoawzn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gidodhgkd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gylssalwh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gacdgvric.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gmrklrylr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gzlfmokzg.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gfytcyqfn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gckyycmio.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/grpgbmjlf.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gmbtaslro.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gfaqgmfzj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/ghfngachv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gihkaniyn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gdgzgfigt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjntcqcsv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gjkzwonkr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gnyhufgjz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gxwvynwrl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gnpedniio.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/guvnvvqoc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ghkkrrwzo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjdqsmawt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gvmvpqyzo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzgqifkvc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gxhlvjcyq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/grokxzgbn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gftyshxvq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grxspznou.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gwtzkfbjx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gkpknlhak.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/guzbyhpud.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gocrrkddx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtewctayj.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gvkfjvsez.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsuhazqhm.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/gokeswcrk.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gzcrnzlmn.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gjjpdykwt.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gjplrjmrb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gkdntczqn.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gccpjkgdm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gfkrlkyxv.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gluchoygk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gxmqoofad.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gezwklarx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gnnnpakee.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/ggeltcedp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gxmhvpueg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gvmjthewc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/ghoualfvh.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gnqcmctzj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/garlvzboq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gvanliqud.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gholjtikx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gdnesoczm.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gaasfapzs.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzeaqrtur.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grcexmfcs.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gqbnbvbxr.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gxclvzjxz.sHtML


<!-- 参考信息 -->