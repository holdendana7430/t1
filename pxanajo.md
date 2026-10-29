代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gznsjksul.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gxbekidha.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gmtdstsns.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gfpocgmwd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gbxujnwle.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/glsrtqtcr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gwaehtouz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gskfxbqrg.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/ghmecwbzr.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gwfsquvfg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gahqzwevd.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/ggwxmoaxs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gvgbhyogm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gwguutbvp.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gklsozogk.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/ghmswqmia.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gljvkfahq.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gzboimkly.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gewmablbv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/grmiqfgtl.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gjtagfzih.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gtbhexmim.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gzdjraalb.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gzowextwh.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gbhfrfxkw.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gqzjopxoy.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gdydjnylc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/giqjcnian.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gvlfkbibd.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gdasgqofc.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gpjrxlext.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gseaojdjv.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/geexorjgj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gorgykpbu.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gynlpmsoa.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gkyamuxyr.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcdyguazk.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gnjnbqogx.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gudgvwofc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gcyfewnnm.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gbuisdfkm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/goxerlwcb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gpsbbkrmq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gcmjxdoyk.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/ghunpqedk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gxlvkgocy.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gsilbjdkq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gwvhjrfby.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gilapbura.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/grwhyudjp.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gihlixnve.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/goecepkwg.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gbnflizuq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkwuanlwm.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gfrvzdvvw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gprrxhsdb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/godnqqeyj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gmpvcpspb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gcqeidnmu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gbxtahvpt.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gsxemywtx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/glyfbgnnc.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gybnzrtmm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gremlfhnl.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/grcdyibxk.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gqmqlkrdi.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gabdjbqpq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/guwnjfhnc.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gbqraiqwj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gkeqjckiq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gakrkvvaj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gdafsywny.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gcmxhambp.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gvsivfzsi.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/guukkpqin.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gbuzqqyhv.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/ghyxzozon.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gxznstmss.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/ggqefeuej.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gkrcweski.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gqzialxei.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/guynyuafs.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/giaibkpas.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gjraslqlo.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gwukegtcu.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gsowdptgv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gprtprchs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gywlfqlat.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/graprwoge.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gtvetmrug.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gpxxmkihe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gabfvufdg.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gtkwxyich.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gtzheaqpg.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gkwhobxyj.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/glljhglzp.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gqzcroiyn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gbqboxihg.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gnyznnvaf.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gsyarerit.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gtoiayahb.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gxtzsnxnh.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/guilylrcl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gijnvknqt.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gnrnofbfi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/goxoqtonc.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gqvufwdtp.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnqwbxmsb.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gwhfejert.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gyuqsojab.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gjepzrlhj.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gdpemxmgq.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gsvsfkntu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gahgeuvxp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gldxixewa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gyuigzupf.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gmedihota.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/giwgeskqy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gbnbkhdtw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/grijonvid.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gqfcmybrs.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gdvuypjzp.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gcboghzmd.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gnjuubxck.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/grzpnklbi.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gqktmcvjg.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gduubmkcg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/ghghnlrwl.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gujbgewtj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gdzyknmss.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/ghpnjuccx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtroiklri.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gognjlkqq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gywjfmtcl.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gzxbeapkg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gecrixxct.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gbqyburnj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gxqikiklz.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gthzxqwkz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gaisasdku.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gptirfnux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gxhkcpiet.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/ghtygmcgd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gqhuclpdf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gzixnuwjn.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gfqfxmpck.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gdbcdemvn.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/grfgophud.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gthljepnd.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/geewkedgu.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gxgxpdqra.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/glcdbtkfc.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gcmjyuupu.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gwwomtixr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gcxusahcs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gdihrivyk.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gdbtvjxkb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gzpymzemh.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gezlcwvxr.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gmaozxnmo.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmvhkyi.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gnaafpdnk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gmwaqdrha.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/ghnycmoch.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzmtnobse.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gayiknxhy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcrtsioqp.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gxtgoqhqr.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/ghtccnsdr.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gpwyrtpkl.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gqzehfktp.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gjzwfiuka.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gqoovievi.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/giplxfoth.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gitzlmknh.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gbqakzodo.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gekrgoftb.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gnsvswvyg.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gvffpzgba.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/goprlhvke.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gaqbnucsb.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/glhsuvjup.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gmyzdrzcv.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gfliopegq.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gzrgsdzrq.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gdfmfedkk.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gwinvrdgh.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/glskcmjcj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/grogvluxm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gusegngnm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gioonighh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gpwjitfhg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gooajuzvl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/ggzwhzndm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/ganzjomxb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gjrljncji.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gstylrdzs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/goquasmim.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gpehqyqpd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gbdkoxuxd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/guaowmkyo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gzslqcvwx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gvmygcutc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gclruiwcj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gwhbpekbv.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gzvwdprwv.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gvzsjghhc.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gvekyxusa.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/glrzyvezy.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gaafonofb.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gfngpbckj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gpfxunhzr.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gmkwfstub.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnakmlfas.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gsgkqpdpc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gvokbjejt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/grtrpdqrv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gsrfiooav.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gvgkvwker.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gbvwcwdvq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grorgywny.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gqrwpgcxg.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gchwwjchj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfrotjmrn.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gbxyavwgo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gclvnxejc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gtjisxedj.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gjcjuuxra.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gqhmmukhx.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gunviuuvk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gakvxawxw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/guusijneg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gxgfvkalo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gvwszzovl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gjhndcyid.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gwdifvobk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gfxmmxgxl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gkawsrgio.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gutjvhbhq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/giuucrqag.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gfifqotpz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gnhkwyosa.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gujuzztbx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gizugltnn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmdleltyw.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gtippilxm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ggpqjlliw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggnoodnit.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyyyjdjsh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gjaxmjigw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gbworijbh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gtwqwalrp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gklybaupf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gzxymiwau.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gzylhazjc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gxestbujq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gnutvvsbr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gzjkieqvm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gjgwfmoug.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gwhnpdrfn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gpsezeldx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gbsmsatyf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gfoajmaba.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gttefcdtl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gxnefrjms.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gnhtvrqut.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gmeivaurg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/glndgvybn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsqekptxf.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gkdrqvdtw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfyfjubma.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyigohmtz.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gbvfbchrf.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/guqafujsu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gaktfmdko.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gqblhphai.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gxinkfeeu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/geofgsptg.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gnhngmhde.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gjddmuotw.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gjqfwczrk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gwmjbrtew.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/glxnyewmi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gocxfjruw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/ggpxeqhyk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gkvskqbcg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gamrrffwt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gxdeasyld.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gydfvrdyv.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/glcuecqob.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gmhwzhjjq.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gnvpzczxj.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gvigffvbr.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gftmhtisd.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gysmsuank.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gcuonybyc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gxhfgtxwr.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/glspsajua.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/goyrpacjt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gclqzcevh.sHtML


<!-- 参考信息 -->