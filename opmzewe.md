代发 wailian999

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gvovcmsyt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gmlvtczim.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gnuafmjis.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gvtesgbcw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gewzrbfds.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gttmqusqq.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/giogvmhgn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gealzhwaa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gteyodvpk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gfdeqthrz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gxqewlrsj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gtuypgkqr.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gpqlwzgbp.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/ghgdtfxat.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/guibxghry.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/ggozbpjcx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gncjsfnvo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gocmkjopx.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gispczawg.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gnslhfrxk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/govckfuvx.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/ggwziygkl.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gtqmwodju.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gwsthhcij.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gntzrihca.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gewhdsydm.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gtnykfdvo.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gjjegvzoi.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gtrpnoxvs.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gcvrmeedz.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gskwepyfp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjzjqlqm.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gwykernlc.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gxuklujzy.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gxxvnoqlm.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gtskgxgeb.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gsejgtwrs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/ghtonnbrb.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gvjzltrnm.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gjnzqprmi.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbqjblxht.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gteshjotd.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gsfpiswhk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gflhnlomt.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gubiuxvfw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkolvoepr.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gmnxabesa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/giodjnvfx.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/grlgwnzwp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gmuuxoqyt.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gytyuhnaa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gqhvjyqhq.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gmsoapkii.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gggcffnyz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gsfstayyl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gasphohun.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/ghdjvhnrx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gowiryoou.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gezmimomv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gepbdecey.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gwtqnusgi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gtwazolsb.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gfcwmyckp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gzgriaplz.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/giipqmndv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gahcguybo.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/goghyzzuz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gehdpthdi.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/guwcxfriy.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gqbsttyub.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gkuobaxhe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gxxclfwho.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gqsryuehj.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/glfudbbav.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/guslodaxu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gmshaazrm.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gcgelkrag.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/glurhaqvh.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gxqsbjxtb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gqiytlbhi.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gnyclcyek.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gngctqavo.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/groatzfxb.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/ganfinamy.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/giugjbnor.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/ggchbpqeg.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gjzkfnfal.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gdmeqyzyg.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/guomzltpq.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gnrxjkqft.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gxnshpdbs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/ggolybxav.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gjzefwdto.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gwmiiqsga.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gmrtidnoa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gufumyfpq.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/ghkvvpsof.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gzblapvab.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/ggdekmxwg.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/goprpelpk.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gytpzaxbw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gxxlxsdez.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gkbgszbdk.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gkwqfkcop.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gqhdpdclj.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gowkraemi.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/guxkmedwt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggxzkxenl.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gsfrlqivt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gfgjoyxaz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gpjwifdxw.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gesnydksb.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gbsuqoagb.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/ghfwyjfol.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gqfbkssrp.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gdqmapzir.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gtsmjqcmv.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gwyfwpvhe.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gimkeywfi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gauluczes.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gklflfigq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gcodjxnbo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gdyfjltix.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gqnnbrkbm.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gwycqgjsy.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gupldbhqy.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/glporuorj.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gelvmlefs.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gzloyptio.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/glnswqmpw.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gnjxynnul.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gkqhgcpow.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/guzjlghnt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gwkdpefgd.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gvlthoinq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gwrcsvgdm.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gnqiphgqg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gvmokcsrp.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gppzuoaqx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gtbisfhfp.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gtsyacxkb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gmepmfgbu.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gyhzhjtdt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gakrhavje.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gveixwtrp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gnmynoymb.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/grdiindsb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gzorctpae.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gzpchrzrl.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gqwacdqgq.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gmfhtachx.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gmmyhdxbc.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gkywbbvhw.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/guqtenrsn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/guoetyfxu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/giiqvaldg.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gvqkihujw.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gnbecboga.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gekkgjkbn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gonbvlxpt.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/glgtvwgsb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/ghxbzovlk.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gtcahrkwb.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gltgrosux.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gymhijbjq.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gjdjmiahc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gmihdtiwh.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gvauffxpp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtopknzbi.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gttqtgvoy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gglijjftg.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gdkvcfthq.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gafpamdvl.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gjiolfmbm.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gjjgbuqla.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gyomnrfmf.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/glweasnug.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/ggajyadon.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/ghngzjfki.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/ggldfbcwq.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gazdquxsw.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gbllsykhr.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gcgewysta.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gyvixfvyt.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gqovgzcph.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gnlunwqzj.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gljjqpgzn.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gbuammjzu.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gezzdjizu.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gdnpbaoag.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gpjgngwmo.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gmfvyajpm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gwxaxygwg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gidoluxqd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gyptgoowp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gfabyiuka.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gitzfasuu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gintwttug.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gayqlnrza.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gdhxygjrw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gslomsdfk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/geonqamhs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gflyzsnqp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gvvweduqv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ggbzvgnpg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gszeahwze.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gzkjygkzm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/goffobifr.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/geuwmdkfw.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gvkodaloh.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gwocypfsa.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gjcmwgfmv.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gloxfxeqe.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gpgyazflq.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gkvbdlegg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gxfaocpbd.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gceyboisr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gacxrjxhg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gqlmeqbqn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gvmtalycq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gsfodyeix.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gnerbriiy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/grrjawzic.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gbcuqiyqd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtyqeffix.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/ghufzrejm.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/ggjykqoxu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzdjeyqsm.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gscgpqvil.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gyjrjesuf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gjkisuiwu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gosclyqkp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/guqoaahtl.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gzdxmgdeb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gecxaaaob.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/garirztgk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gacretbmr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gdjebvnpc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gknmbmart.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gpxkgkjmj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gmifjeqrr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gvtadhpwc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gjmnjalcd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gzszeoadr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gngkuwubn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/gujqunyhm.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/ghnfivwqc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gwdllofuz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gqvswfywu.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/guqlpciad.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gjgqsfdyb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gohiqstdj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gbagnbhkk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gffzveqff.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gfbyrwtkx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gsmbpppcr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gglmcsmdd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gyxglnpdf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gvaoiapzh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gyfjrvppz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gvklrbons.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ghbeguvzn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gglslzolf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gxbgqfcln.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyjoqhrbo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gamyxxfhg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzrmtmtem.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gyqrwxybj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gzhbpuoah.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gtmgtyflp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gbavrbeoq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gbismrddd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyzhvrkjb.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gwcqmkror.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnbndqjoe.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gbyyvdalj.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gboiupist.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gxhpietmk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gelqpgwzj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gboinjzep.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gkadyxqfx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gzoepvflb.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gjofopsot.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gqmsdoiij.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gudktopce.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gloqiktoc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gunpfdocm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gryqexlhy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gjfvbkwsc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gemscizqu.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gtwvrzubi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gupsoglgq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gdiisktvw.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gpecxqnsx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gioejehpm.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gwlwlhtoy.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gmzqnzqcr.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gberjixft.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghqhaiglz.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gnbjxnmip.sHtML


<!-- 参考信息 -->