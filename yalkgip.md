代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gcuqvyksk.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gnmdpuftj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/guqzkkmtq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gsiqajnbi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gthgmeebe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/govxdafko.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gzhkckiby.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqjkzppx.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/giurjgfrt.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gvkxownfq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gxijkxxhf.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gdhfwsboq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gjjsswapz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gnlkbrrdk.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/godvmswpq.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gvryirsed.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gikijmtyd.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/ggxpwcgoo.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gnmgnbpja.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/glesifwuh.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gvhbszdvq.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gpjrlkeom.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gfuxcoejk.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/ggbsydgxt.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gneiifwws.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gddzbwzpx.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/grdehxptp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gzpsseblz.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gzjixihyi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/giudmnodq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gvxuceidp.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gabzcreso.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gidvsfmcg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gkbwzwqjc.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gvghwwctn.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gpcpdtfvk.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gztbthbbe.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gnfsazbaz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gjwwbtwyj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghhpghjxl.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gamjhnloz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gdrhevzuq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gogyiiojp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gomanlleq.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gbfkybiuf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gfyulmizz.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/glohrtabg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gejiiplmf.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gownpkbgn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gadhixyzk.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gdwcangil.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/guubujoyd.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gethubypw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gdxdbxvuk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gepppplvc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gtjudasib.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gygtgsemu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gwvhwfcxc.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gcjaagxbp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gzyofgrmg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gvhwmophv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/goeogvkse.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gfgihlllf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/geufxakzj.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gitxvbuye.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gxzeitdlo.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gugrrmlto.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gkdtaxkue.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gvcbvgopu.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gcpltxjfr.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gkxvjhbzu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gcbgaqqix.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/glnxteknz.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gkkprigba.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gjkwwrrln.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gfcqlecmc.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/glfbpfzin.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/ghbjwsywd.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/grrrwylsu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gdfwsanxo.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gnvsptbtz.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gnroscvxo.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gmcnfrxgx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gfesnwrfk.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gycgrlgjs.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/ggwtluqfn.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gfkitnjfr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gvdwjskhg.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gxnohkaxp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gtutsqven.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/ghtwotpur.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gildkbcty.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gslgmgehh.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gtytihmrb.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gdfxlgymh.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/grrrfkjkl.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gewafshcf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/ghglenxji.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gpncycftr.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/glttskhqs.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/ghaqyxbqh.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gbayzouwd.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gzefccife.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gbvrhmkew.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gjxpjhbxt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/ghoaxjzqp.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gasglegmo.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/guzypmggy.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpftgcess.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gukjvtwxw.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gugtdopey.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/ghuwpfjsn.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gphebfnfe.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gqeinsfin.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gaxbwdajr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gxbkfwaio.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gyjaobkyx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gtdcgoyad.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gipegdqmm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/guizdtfnc.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gnfeihvoc.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gfexxerfk.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gidxhiqdi.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/glufchvhy.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gvxzvvjsr.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gwmomeqiz.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gdrrhrpjr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gsbqohwyq.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gojbvkzqe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gyfgaegnb.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gszbxmpcq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gsnuvtwtf.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/grhgresnl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gkkntfoyx.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gnofxsbnd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gxfvdfkyy.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gqonesgba.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gvpmdxvhc.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gnqvtvekr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gdnustqmb.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gplzmzbzs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gxrogwkpl.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gkacejtpq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gysgazadm.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gqplnoncz.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gpyqfzadj.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gwmohooeh.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gxwavttlk.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gvxwvjiew.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gyiwjaupy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gyktbgmrh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gwrsulhpr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/ggzjmusfa.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gdpglakhv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gnxnepiqn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gufteldjb.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/ggxcznxnj.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gtkrmtobj.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gzmwqaqzg.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gknoxvbap.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gbgekmhce.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gjhnadued.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gnthkpowx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gdmexdjeb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxcowgqms.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/grkzifhgj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnanjjbtn.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gcgygpkbk.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/geaefswqz.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gbprqeifg.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gvtgnusyl.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gfenlmelk.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gvjxtyrwy.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gfodewbod.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gskkmgwaa.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gzkrfgvjg.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gpirbhhve.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gviyvdhmk.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gqmapbfkt.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gzltvldye.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gktptucgw.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gjgyzmkog.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gvohilcyc.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gnjpisvza.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gefnpnxhw.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gmsiscadx.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gkslsuniq.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gsnsslbkb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gtznxlozg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gwoytlqtd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gekfjtdha.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gkmakgiri.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gefugnrme.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/goknhaftq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gzmcgqeen.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gwgfdsbko.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/grvotffrh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gglasbmwg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gksfinnkw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/garuruaxc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gfioonxnr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gwfnkzuxy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gebrdxvjo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/govjoeona.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/ggcsmvlfu.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gbeuegxyu.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gemvzfxqm.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gkepaqhrc.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/glkocmtwa.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkchxuhtl.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/ggalfwwaj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gdtmneyjq.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gmqdsvncq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/geaeaifzk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gpbccwvul.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gtlvqvohe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/giljvqvan.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gxjqqofhf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gtpdjrxlv.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gppnstukt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcvxjrpyq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gqfwvswkb.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/goxkhbblm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvlhzxked.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gofatqvlm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbkoifi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gkfqrztoc.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gvcybsasq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gfuyeklee.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gugtvkpad.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gqropmonn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gkqgnslkb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gxckdccwl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gxxambnoz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gmwpjgqwv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gxqjrejoa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gyrwrfall.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/ghicujpvf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/grkimyeek.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gmznoetsa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gzkznjavx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/ghidoayuq.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gdnbjgafw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gsiarwhzw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/guvzjqxir.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gaiehlfsv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfurhfb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gvjsbnwvi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gveoqufwr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gjmglexkc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gnijskofj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gtujjnyyf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gkejibrpl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gvsgpemxo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gayaaucpm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gefdwkcif.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gqlazdjso.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gzkxpiphc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ghdnimjgc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/geudkdtqu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/glxitxhkm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gipjtaoyv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdbjxnoeo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gmfazyann.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gszzxpohb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/grwqxcrpi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/ggbbxebgg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gpblgtubq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gizcpxhqk.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gvoaasasb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gavzsfecb.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gaxtargaj.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gghmaofnf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gkfwysphf.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gazvftbul.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gtpmthsvu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gibumxnkp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gkkfpvdlp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gkgyiwojb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gxhvuwbul.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/ggktliqte.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gljwfiuvj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gegafunvd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gdvtieley.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gnessntze.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gnfrddvfn.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gkzuassnd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gzinglnxm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gfmqzdxom.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/ghcstgpoh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gbgncyfka.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjwaemqpd.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/guprqepsj.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjpphuawk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gzzxzekjn.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gerqgkigr.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gwyxhbhfe.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gmwriyrpr.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gtcfmtvcf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gfqamyhmr.sHtML


<!-- 参考信息 -->