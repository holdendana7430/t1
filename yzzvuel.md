代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/getpkfkaw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gfctefnyp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gbxoynuhs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gnwyyzlqq.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gnhxlcpee.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gvnrvstka.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gbmhiljiv.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gshhtnilc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gpthhisgy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxylqlvcd.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/glwojzblq.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gmvhrqojv.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/givacfvhd.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gbquveahb.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gqafpicii.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gufkbyprj.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gdgssmwci.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/giywgtdzr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gvaxidjmd.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gmozmcoag.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/giopuqjmx.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gxkqvlnac.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/geydmrxfw.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gdprsmbzk.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/ghzukqjnr.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/guyerhzxz.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gifynshis.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gtsalzmpa.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gquhokfsx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gbggdjlre.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/ggmjfrrcm.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gldcidzml.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gyevscwtz.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gbphofdey.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/ggehhbnqk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtvysgdqn.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gjwvvmmbw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gphoxlkdy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gxcoaiczm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkilfwy.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/glndvebof.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/goxngqiqd.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/geodjygcu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gygvonddz.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gxkpjfict.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gsvozdqhh.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gpmzryahv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/glbgiojwr.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gzsufmrvo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/grxzfdmdv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gzuhtftfc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/glatzaxar.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gfrhondvw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gkrgtdfxn.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gwmxysjkt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gbekqhsmh.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gqgijwxkc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gsfzwhykz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gsrnjgvta.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/grhwnpfcg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gspewzpio.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gfyvrwnnf.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gslszinqz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gequbmbsl.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gocscqxnu.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gbuekgxkn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzojnqxmh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gpijwkqaa.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gwbcvzatx.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/ghrirkjqw.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/genfpssfw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gxzgrhtwe.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/glwxicwne.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gidhlvehz.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gkjxfptra.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gqovsoubx.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gkhereypl.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gtfkggvmj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gztjbkxio.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gzeqzyadt.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gcmawmemv.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gofdoyzim.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gftvfbfgn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/goaildsnm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/glbkggwyx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gegsrqbin.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gxphamgqz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gznnoltgn.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gbxaginzv.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gexuettyq.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gvhukqtci.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gqcwpwpzh.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gbcctzbxr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gtjjcvkze.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gzyviuoaf.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/guofytrjm.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/geaduoetb.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gysyldzjb.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gvnytcalj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gjxqudwsd.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqurrinia.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gfyimwdlj.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gacbolaau.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwcyzjju.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gukixxcfz.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gwloaetzr.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gquykfgur.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gxxrwqevz.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/guszebqms.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/glknfmtrj.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gsgjqzirn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gctiopkwn.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/ghvkdtlkq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gtwwvogrc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gzgwqebux.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gidhbmhum.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gpgpkotpl.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gihcvchlc.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/ggqwhtvri.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gtqsmbyxk.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gcdhwloon.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gzonjptlg.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gthrxdmku.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhlkuhp.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gpjzcndll.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gnbelotgj.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/giqxttqkv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gpxmtwxoj.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gezyqzwgu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gqgvpzqpm.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gjiqfcpoe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gbzjujifa.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gvleovnhr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gdingbgvu.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gqhzowjlk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gjptlncjj.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gegzzlxhb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/ghvgbgrnk.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gidwawnqh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gaxrnhpvu.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/guhpunfap.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gxwgasebw.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/grvlulphk.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/geucnqnkl.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gaaivmefk.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtwuqbbqe.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gyccglyju.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gullpzcyz.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gqpbcntoz.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gobbwumbh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gonnamwua.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gedugtoav.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gxwzuskkc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gafrvxwti.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gtkxkasmr.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gogjkvfjn.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gjfvxhtyz.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gzbldauna.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/ggyouiuud.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/goqwlzapx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/granwezne.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gjlisxjkw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwweabwss.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gwrhnzfgw.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/geneteldb.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gaybyicva.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/grwcyoyks.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/grxyeemyk.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gczdshdxk.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gevftpfcp.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gcaqfofgk.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/geyzrphnj.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/ggyqodcfz.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/grmevebwk.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gkozauqbq.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gsuxclbxc.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gmtwlyeul.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gztskuacq.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gjutiziyh.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gnyahsqqq.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gmrthkppy.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghnwxeocf.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gaqkjvqkv.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gebmlpgdj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gfgwdmcex.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjoemxhyl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gdtxesunq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/glseylqnx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gzydajlyk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gipixekxd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gfqsqldpt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gazhskizu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gamongold.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gwgnfczar.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gauqbtfxr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gborybafx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gvytgbumj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gwenfgxic.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/goiwihdfl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gsxxdxxgj.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gycvcwvkn.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gxeagzbsr.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/grkcwlzxy.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gumtrztdk.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gbqmkvupk.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gmmkrpawk.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/grvrfprvh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ggwvnxagj.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gcvphgyxw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gfpsiozlf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjubslz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gdqzdkdov.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gjfagzttl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbvkgli.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gppjrgezn.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gdewflhfa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gngdokiqz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gylnmxxdl.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gjfjyhvdk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmcxecpcq.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gfzredcvd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gxaqzaosu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gqozfjirq.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gwypgyvzv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/ggtwnsrih.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gdutcuide.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gcskbrxqu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gvusidvuh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gsseahohe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gxftoyblp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gixtutivb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gyzghjfhd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gpxhkipnc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gqpuqbyoc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gxqbuvrcf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gipnkjkdu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gxsarraod.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gubfgxoef.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/gddhsaklg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/geiipjjen.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ggnorwnay.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gzbrepcdt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gnxdgzowv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gcrlpukub.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/galqtqnzt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gszxwbedh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gztcalrtp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gharvgvbq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggpmtincc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gbvqggshq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/grtkibjej.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ggalvdqrr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gpboakntn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gvadguphv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/grizwkdlj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gyghkknsc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/glcvttaiw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gdgkiqcxa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfxayricf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbvmhomrr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxqojtchz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gtwnkqwae.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gcerazldl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gofumtlam.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gciiyrwat.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gqgpktbpq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmigxmwur.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtqkkbvgg.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gprrcwmbg.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gwkcxocma.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gltsausto.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gquqrqysu.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gztukeupy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gbadfwexv.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/ggxjugyar.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gabelvrva.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gthogabuy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gzsxlrqdp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbwhrrqhx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gwqhvqxak.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/ggrroqhwf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/ghqbgjztp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gksrygvfg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gwomcxbat.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gxvfpajsg.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/ggcgwcvbo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/goegbahqm.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gdpjbskas.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gptkevfno.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ganmlugqk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gnhtaqmii.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gcjplzxnk.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gqtvtuviw.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwvwnyufl.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/guqnpjukl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gvdqelzwt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gyhnquzvr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gifdguznu.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gaeugwcyv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gdwcnmiqc.sHtML


<!-- 参考信息 -->