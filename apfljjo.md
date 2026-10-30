代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gzxebnptp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gdxslalxu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gdmfczfhf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gtonxnrri.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gnrcjgqin.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gzwqnyfkh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/grffnjvyh.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gbvemzgws.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gfqteqzhh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/glnwymgpj.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gvnkiofxk.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gbvkwhgxi.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gkicbtyvq.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gdhcjzyuy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gtxkvconp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gphzuvfau.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gdddttfwf.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gpwejnojh.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gwbradfyw.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gzwubaoqf.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gnqqptqax.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gsctohugv.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/geeahdcsk.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gukgfvnsr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gupfavnab.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gxlqekogs.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gkqlcitdg.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/ghvgcgerm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gmadtknjs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gsntfnwty.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/goclukgfx.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gpfhqasfz.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtxtdtyro.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gnbsjehnx.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/ginrnqdho.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gzgsbpbbz.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gnsooieea.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gqacgbbrb.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gssbdixot.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/ggumncogy.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gcdgztltw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gkfxgcooj.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/ghleqlqyj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gxhclsemr.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gfqudfgky.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gusnepdkw.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gijzovouv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gdlurstrd.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gwujzmvgb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbquhohaw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gkelmvrir.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gveyoqbqt.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gabatvtmp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/glgwewqpz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gnqjyacrv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/guwxootrb.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gjlvmnizq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gguyxmrdi.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gcbjwcvmi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gclhefila.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gwyluhkkm.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gkeuvjjiu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gpjabbcrm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gqvqhgvxi.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gdkndppny.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/glklgcebd.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gybxdcysf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/ghungsgbn.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gtygwtgmc.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/glaumljox.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gmvqxbuvd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/grfnhiojv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gwgrocthq.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/ghfqoofwj.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/giidggrpu.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gtnsxslnw.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gqbakmmnu.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gwicshjom.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/grzytpwvz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gypbkaqwc.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/grulmajln.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gxlntwtan.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gxrvecvty.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gpmiwbxzs.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gqpupquhy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/glanrjxxp.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gwepuscof.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgzvkqw.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/ggcffpxrp.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gnbixonpj.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gzdgrlslb.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gwyzcaeoj.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gshhqslxl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gnnujpgxy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gcrltjwpv.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/getsguosg.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/glrldmjwe.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gcnqxeyko.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gngjjixsl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gbwsupagu.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gycqnwoal.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/ggtbkrgnh.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gykyssvjb.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gizicypwx.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gxskcveoo.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gxdlxarmy.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gkitsqvtc.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gscqhuelh.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/glbsktrke.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gadovsojo.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gbnpacdkc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvjpqmmlw.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/grxcqzuyy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/goctcpiro.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gxbzrthdo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gskrrvwyb.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gxallvoiw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gvehkkyks.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gteqwfjeb.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/genuisado.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gjngmciqg.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gyewuvige.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gzobkzqyp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gscexmutw.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gucayemuf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gfrmfzdvz.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gvepptdnd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gaynvsgqj.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gstlfoqbx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gsrsjcerp.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbayjahhx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gtfjygfdr.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gjxipwtfx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/glfuncobb.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gqddnohme.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/grfhjfojd.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gnvdjuejj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/ggxmtzxjk.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gmzjrkzkr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gybijkvjh.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gzvpuggax.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/grnyedmhe.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gxtwdhkae.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gmdzttqhu.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gkosccjzo.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gerximzyf.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gdbwmmohx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gkmevxyho.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/goojiqbkc.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gzyfhlrrp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gbunudozl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gzxnbnoao.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/grongtogi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gilamlwuh.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gcctxahiy.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gnerqghhq.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gdssjxuly.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gswbmdfkm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/glvystkge.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gcadhwyoi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpfhvlxgf.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gjjyhwilu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdrnnmfwk.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gzuiccocv.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gtfhwsixv.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxfenmd.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/ghjqqkoym.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gjmdxnrtt.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/guxzhfmro.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/geufthqyz.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gfnxgarzo.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gnbzrhldv.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gxehdxmab.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gpcqobdsp.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gjbaqvesr.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gpaufclph.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gbccqpkdb.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gityjgxnv.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gxcgxouhk.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gyryjhhwn.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gbgskgepv.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gfyswueea.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gsoughptn.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gzgszeowa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gvimajfgr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/grnpppbgr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/ghvldyzky.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/ginqtxvla.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gsyalciho.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gobodtbti.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfptbabty.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/godncdgep.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gahxcomby.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gviiamgur.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gsgwhudkk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/ghrdcnanc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/giozennxd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gpmooyqvv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxmaqvk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gevnwlaho.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gtmvvopyt.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gpjxeiuro.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gqrtnqjwt.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gpuqmeyoz.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gtmyqiwfd.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gaimaseys.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gyrbgyyqg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxolccolp.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gwtavlxey.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gekfmpood.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gumufmntm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gkxqbgbsi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/goreaarea.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gwkcbbfwo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gszclnzzl.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/goaryptyw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcbmbosyc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gafhcrxwi.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gxffbkbbt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grpvpuyqz.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gngbnsmmq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/goxpcaybn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gzagguqlb.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/ghzxwfoqj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gcnjnsrnz.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gnzophmut.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/giqqdgotv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/ggeiqjgwb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/glghlnmvv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gjskkkggu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/ghjbkpzij.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/glyybjdzl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gcxghufxs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/ggpzwfnoj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gzwskbnzz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gkboxagfw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gfqpvflfz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gqljbdlia.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/guufvgnng.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gmugwjjgx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gkdcfagjl.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gxyjpseel.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjprawyrl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/guqphclua.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/grxdqfmwr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/grwstnpok.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gmadbsxnt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gugqtojjv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gagseftya.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gbowqwsmb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gyjnverfc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gjcttwobq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ggksuebpp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/guyugubin.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gcpyjidro.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gjhmhxdjh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gexwrntop.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnsxvkqer.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gzyfmuolg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfygcftwg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gyhggddko.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggujbrjuf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gdbonofju.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/glfnmdqsi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gimvydnap.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/grdnektzp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaycyieqq.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gvnmwkigi.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/ghayjupew.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gciaouxde.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghrecyaxc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/giihjxdxr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gmouryoxh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/geknsmbpp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gtwzqrydj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/geekcqmgr.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gcyguaklf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/grvyinmhq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gijrvmdyo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gkfrpxhdv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gghaugovj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gjshfurta.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gfytqqigj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/ggseoxclp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gdxphjwec.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gwccjeyrh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gohopbhgq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gvuyogfqv.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjwikiurw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfrcvbhxd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gqkghjvnd.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gcnkaztty.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gydhgkrbs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvoytdbqp.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gwhvtlrkx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gtvdgjwlb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gladdmyjc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gbmvkfohs.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gyahjlskx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gbsdzxron.sHtML


<!-- 参考信息 -->