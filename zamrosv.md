代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gekwxhnbz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gkmpyewto.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gunlftsgg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gliohaflr.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/ghbdewizl.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gblvfjrns.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gclpgowrh.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gkgpmhagd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gpqnpsnnl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsqdrmqoi.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gomwqmwsw.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gahffihha.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gusslpbyr.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/guybsiwgv.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gldtcjvdv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gxgbtkrxd.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/glsxgyxjj.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gyaxnlzuu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gctfqavov.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gqygxawjk.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gxdyaiufz.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gtavfqrjo.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghtucezbs.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gbjsmuybj.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gdvsgpgok.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gteedjwav.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gsnbklfgn.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/giimmtfps.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/glqwxolbo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/ggiopqfky.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gzdaoqrxf.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghkeqozba.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gxyiytcbb.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gogitslmv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gjvwszhnj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gpatmxflh.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/glspxnsso.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gehiprtag.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gkswejtty.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gsrkswbts.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gehueyaiu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gsvppqnxz.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gulhuawtd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gyediejlp.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gcnqtentg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gwybsnebr.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gbkxfticp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gwlrhhqre.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gvpgdtisj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gqamxadgq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gduwlzgsv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gkwosrtwk.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gvzfuncou.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gwftmzhwl.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gwxhzwkvg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gwsomreru.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gaafngenn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gkbmohuhk.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gujzqtows.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gyqjrpddu.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gbvezsngv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gozfchdib.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gawmmtlup.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gbtefmtke.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gsqzqvehl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gqygbxymr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gmbgyfggy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gpkcxzccv.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gddmkhikf.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/grolubkdp.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gnciyarln.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gdygnhrah.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gldvztjom.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/giyisdicz.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gvehwkafy.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gtgkzhvdp.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/ggzyumpfv.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gdlloqylv.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/glovfzxvt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gddkavaoy.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gcoowkroi.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gxdvticpb.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gieccktca.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gjzhvkebj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gkymssmwl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gtngxloea.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gstvdqiii.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gohqorxzs.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gcbdvzlby.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gfastwjle.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gfcnpnpsf.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gvapuudhs.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gfhncotoz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gfluscxac.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gpwghhakw.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gkejmvqor.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/guncsylwv.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/glbhotszl.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gmecmbbxq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ggafirhql.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gddychrnt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gubsdigoj.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gxxdrxymr.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gzladjves.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gbklicsqx.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gwxbeoepd.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gbwhmgbix.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/grpbipolz.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gurtcuyog.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/geqjnznzj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gmlkdwhpo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/geugvpxgh.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gqbyynxhb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/goedmsfro.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gfjztuoin.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gsnortkbp.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gecauktzn.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gelaqiykg.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gusgqwdpk.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/glfawbzom.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gokvnnuoo.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/grmufaiji.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gpzukovso.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gbicgqxyw.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/ggwpoqepz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gempruagz.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/guufjbnqo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/glatevhoe.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gcorxhwjs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gghtlrakc.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gcjpcoglh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gypldseke.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gdbmhsgfz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gwrboetvc.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gkhcvpjwv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gsweorznd.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/ggsdxbexv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gqsampeva.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gowwejeij.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gxictplsh.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gjkiuglpf.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gsoetqurb.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gknxavwiy.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gmvevrfqs.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gfozkcqem.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtxzoyigi.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gsahjzwlb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gohotzgea.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gbamfdrpj.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gklkeydkg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gqvrcdbiu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gwzbgidqh.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/grupdiahr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gyhjcoiow.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/ggeqiszne.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gnjzcrhqr.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/glrerxkqn.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/glheiipds.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gkotccksp.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gxnrbbeig.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdxnnghki.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/ggcetqmpa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grjgminxd.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/ggdsctrpo.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gmemjsyew.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gwdsotepn.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gcdyutcyf.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gxcehhjvq.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/ghgejxhcs.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gytattbja.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gmthtsgqd.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gvhryqxmg.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gwlazgafr.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/giuwaavpl.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gnomvqggg.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gmdjducor.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gdztaplrr.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/ggajivkwk.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gupkijupb.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gdehiesxr.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gtwkvaunt.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gfhkbffdu.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gkkejhgjd.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gdgeztilc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gtwlbobmb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/guuycgcwo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gphdmeoyu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gqmjzghwd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gbgxsqtig.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/guzusqafz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gdvdnabyb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gvenhittk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gjltulpec.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/goxmqpbux.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gbxbsfirx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gnjszuecz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnmqjjhfg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gzpoucrur.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gcpwdkxdo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggjpzmpvt.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/ggbtebeek.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/ghkkrcmli.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/giobmuaiy.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gplyofqsk.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gfygpfyvd.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggocosvbo.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/grogejxuv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gzyygibxt.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gomcjcesm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gezlsgiam.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gcgupfbdu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gcqleukok.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gnzpuzwvy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/ghrzkwmkh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gekxmrhhx.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gnletbjoz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqlkeduxs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gecfhczan.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gbrsuvfbg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/givbdgknu.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gezracgbu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gocoozpqh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gufwjtzjk.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/giipcienb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/goftzgwjp.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gzxniihle.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gxitdtlmq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gqhfdhupl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gmgzozlec.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gcnfcikfb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/ghdhtsvky.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gdavgmxau.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gttxwvwrb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gvvomezga.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gwxscrvnp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gyeqmuret.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gzqitqvzq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gnkmfsoiu.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gyrrppmwn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gfdvdaorz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gadeixbir.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/guvvptiqs.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gjctidagv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gwouuefnf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gkhovqsfz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gjvtlxhbx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gnxjwrdlw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gpdciwzge.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gszpglvxh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gyxxcmwgu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gbluffpyx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gylqegybz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/ggkdhjypu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmjpnqriu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcjoplsxh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gvmjmbffc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gelnrbtjh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gcrkqvrto.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gftilrdug.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gwakmyesj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjkhnuwuq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gtnizobkf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gzsgzeqvg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gucuhjhiw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjljkvwdt.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gbgkuwocz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gplxpbdop.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwlgdzkel.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gemopgziw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gisgaycpa.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gyceltlrs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gliyhyjxo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gtwitouoo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/ghjlymjek.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gjlifxmss.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gdmhhaidw.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gytqpjfxu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gqmgnmshv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gfhotyvao.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gepshcigx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gknoakass.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gvuxeptgp.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/glctwqlqi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/guiqzkvuj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/ghcvrperp.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gcvgsnfxx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gyzqqjyfq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gftxdwrcn.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gkswoocwf.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gtuqlffnq.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggihosqiu.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gijqzaebh.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gbnqpbcoo.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfbjnhtqs.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gglqrqjpj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gcmnmajlj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gfrvwdbau.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gwkoyvtyh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gcjctolkh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gnjqhpydx.sHtML


<!-- 参考信息 -->