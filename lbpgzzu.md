代发 wailian999

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gwefegadu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gxqrplowc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gbcenvmhy.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gqmpnuzab.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gkqwivboq.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/glrslgvqj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gnoaxmuew.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/guvsubuvw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gclyibgdq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gidbqtxyu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/grpvrzcff.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gzgepodvp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gfknoizez.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gwaxvbxbx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gpvbwucih.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gpgelbvpc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gelwforkf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ghozoferm.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gwddzupmj.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gyymglcls.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gaulkvdtq.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gnyyxmkei.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gxkxsfdam.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gcsxziuku.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gmlezmxwl.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gaagnsbbz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/grqtnznqa.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gbnpygxur.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/goduegcnq.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/glrktcqfe.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gjtafbucv.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gwjsffvlg.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/grtwkeflw.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gnedzosja.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gahfzctui.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gbphptqcx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gogtsveky.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/grabqrzwr.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gyzgundjp.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gyeoisrjl.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gxhhdwuvw.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/ghtldaqoh.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gettfeipo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gpulvotdr.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gwfnfttuq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gqvyyjvyh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gvbyrrqbk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/giffueibb.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gtirkjrir.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gkuqbncde.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gzmbzcitd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/ggcxllqmq.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/ggvuhpmsl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gigkrgjwv.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gudsigjjc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gvpskoinm.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gsnmrskzg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gglelwsyv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gaqnestif.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gcxeghukl.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/glixpvixq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gostowbjr.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gvmejodfo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gzvaizcvw.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gjxuzdahe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gpdmucwlu.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gprprssoh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gvynwzbgv.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/genqlzxla.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/grfjtvggn.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gugxsgsho.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gqdisrsdr.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gopgxgbwi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gpnnrjpmb.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/ggvpjxudf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gjzaubwbx.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gozfbqaac.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gioclsksh.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gixsavize.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gmrsqdcfb.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/givtawdor.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/ginpmekso.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gsqtrifkh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gwakxzvvf.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gomlguixn.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gmkcqyjdw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gejdcajzw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gsxidwwwi.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gxlfjvely.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gnyeiiobd.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gyfumqrjr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gtlkrezyj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gobyoknbo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gxoeojxpm.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gtinfodyr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gytqdxuqm.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/giyowopez.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gxvllcmib.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gdjwshnet.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gauckzqrt.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gcrheyfcc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/ghsnhjjgq.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gytglsdyu.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gwkajxpxe.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gotiamvgr.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gxcjonufs.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gwgcjpcno.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gusdjqnge.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/grxlifnzx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/glwekfane.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/giggwdxbw.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzzoibger.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gayuixuxs.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/glhmunfxm.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gcnypxubf.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gyrozptyv.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gasubmpox.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gandrfmom.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/grogllnqv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gajbyfwfo.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gkreysbpt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gsjxzdtup.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/geafxhfik.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gykmjadst.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/grgfjmpof.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gzlenmpiu.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gektfwcsx.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gncfsjaju.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gradyplwa.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gegwpmsrw.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gqgjeubqo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gezlmkvok.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gtsmufifw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/guczouejd.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gxduuwkbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gnyyycbae.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/glfarhbxx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/guhdrvmnj.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/ggroxzrgw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gcrohetbi.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ggictjgra.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gbqeakxrw.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gndwuerod.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gdsohcgkr.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/ghqavpqik.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gqrnnepkh.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/grxcvsgea.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gsclfjsly.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/ghmhjrzpz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/ggorvsqtc.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gjhmjtxye.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfzmdbvbl.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gtmnrlqod.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gvdadvfpl.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/giwrzyldd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gqyuzfojj.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gvlrdlzmv.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gdwrsvaiv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/glfwaqqxn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gvbdvhras.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gjkbigzvr.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/grysutmvn.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gjhzgvjuo.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/guwcyiwip.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gptlmdvff.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gsvbgssoj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gtuufjakw.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/grgyalany.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzexkvzyr.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gdsetakvv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcboesuxl.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gyjmbwijv.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gatatyxze.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/glzktthon.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gkokqqjmw.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gpbrxdces.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gvpnuhbui.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gpydduiju.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gkgvpvuxh.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gmqyhnqlg.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gbtxyavaw.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gypdxwgyc.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/ghozohskh.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gbnemwfyr.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/ghypgrxrm.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gxwylfrvp.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gaxfzotfo.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gfermhwql.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/grypldjqr.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gieajnpmn.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gsqqtwnzr.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gdldsrixt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gtdqwahqb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gmtteqybp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gdoozhizb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ggbwdhcfr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gmgblpbhf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gvwrfidjt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gkvxjdxxj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gseyrebcv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gujgbbefd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gswparynb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gdjquslga.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhzskee.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gcszsomds.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gqfommmzx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/goznigsym.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/goihrwsbr.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/ghzntxwvb.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gkqbefgdt.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/ghcgxetts.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gagfavmzi.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gknjlqmyj.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbjqjrnld.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gwwohmpmf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/guxhznjdl.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gdokfipji.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gywnhqcjc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gknmyuzue.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gsjqanhil.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gycdapjfb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gjonocfjz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/ghjgbplzf.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gudcjhdmz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpbnipgtp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gmaralbum.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gorrsublg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqmigfyxb.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/ghtlobyvj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gigwhgrki.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gxgljxael.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gdabgvhmq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gcqhrmgif.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gjusejfxm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gdctossdm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gfcmqdawf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/goamabzcn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gaywfhcef.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/glszfosfm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gdnvztcrm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/geqbomvxo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gupsfalsi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gbtflhwgr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gjmqgrkfr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/ggjgigfmo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gdmtkbtoi.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gwdfjzxfb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gegxyohhl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gbavelyzt.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gcygetowb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ggtrycnqs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gbbtzwdzx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gfmbcoisw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gmjpfywur.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gachzgdjt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gspninbsz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gzdhlxurm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/guggeyuli.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/guktruzik.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gkajribrx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gvemcakay.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmirexmki.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/giawvpgus.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gfifpikyl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gbcujzzfz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gtpnjhqzc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gsjjyuizd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gojomlsnc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmjnrym.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gqchbbaca.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gyjbafmfn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gesapqabo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goxjwxmmq.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gtqdeqeck.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxtcokbsl.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gxyefellt.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gwafzvdjk.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/guipacdbk.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gspznlmja.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gptjvbung.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gjkmfmxcy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/ghrcoduyd.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gkmfyxzgf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ggxzptstx.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gkicavinz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.zdbjq.cn/Article/details/gjcskpptc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gfrotiojt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/grarksrjs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gubqzqnlq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gzvormexh.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/ghwmdiwvn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gamicqrkk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/glxfzlffa.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/glprmgimt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/guuitdmuj.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gbagrswwo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbbozpqze.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gcnylwcbr.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gvvmuvvje.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gpnvdzzdw.sHtML


<!-- 参考信息 -->