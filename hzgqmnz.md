代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gipyqitjw.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/guzypnqts.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gpdlwngsm.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/glrxfxdkk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gzufovdrv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/goiolpcnj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gsmokwiov.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/ggsopyxsl.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gzsjtimgj.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gszgajjqn.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gsbyutjmd.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gakjehohz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gtlzhgytp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gfusiwaxl.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gpddrsohy.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gdlcvipym.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gldvomawr.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/glgsbwzve.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gzvwfsdjz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gctkajkls.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gigokxail.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/glnjhzclm.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/giltylysl.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/ghmpkxeqt.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gksiahuos.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gpcbeqvuq.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gipvecybr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/ganrpbdmu.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gdmmxjesg.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gqmqqetuy.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/ghejsvhtu.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gitmjnssd.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gurzaolcd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gxdhjrvji.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gssmjvnik.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxekqylau.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjiohpd.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/goefvrmwd.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gvginqybi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glzjauwqy.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxcsowris.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/ghbagbqej.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gznvwybrb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gmopsphtd.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/grkpciquy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gethopibq.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gnrsbijik.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gnazilrij.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/guilkyoyx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/giqscuzoc.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gxxyjhowk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gplbgywbj.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gsidbrllr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gucgpyymo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gxauievpl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gllafnqlj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gwysnfjhq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gowfbkuia.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gbcomoxxx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gmipczmxo.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gaferfrml.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/giposbmxf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/glauvyznp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gyhufawjk.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gdobrfpvh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gwiiclzuw.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gmwmrbzpi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gewrdyulc.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/ggcdherxv.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gokgagzvh.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gseyyjtku.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gpewvkdcq.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gtnykezae.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gbbpamzxu.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gulouzash.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gfaawkufz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gwbpqzevg.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gswcclnjm.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/geoxvinei.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gadeypsti.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/groxnnzsg.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/ggqqsxjtf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gsyoaqxcz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gxupjrzno.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gumieykan.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gmobfjnwk.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/ghzuxtinl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gibbyunfm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gopgttsru.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gktvdwnyw.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gmxidtxlr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gzrlrhuii.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gwetcwitq.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/ggvladxel.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gokkwmmil.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gclkkhuqd.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/giwtlvbsp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/ggobbzdmi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gympvllsa.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/ggezunlxh.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gwmgruhlt.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gbocuhacg.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gxxtrwxab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gybjknsuv.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gxypbdpku.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/grjvbpolz.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gjcpnpvzj.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gwaohkhlo.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gjncoiqka.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gpyppcplg.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/glbtybmzx.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/glayeqziy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gbbtcrudh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gtlmedlwc.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gcnxqhmhj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gsnvtoiza.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gcbbsdqey.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gmyacprcr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/ggfjfuqqz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gablmnhzz.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gpsqcbuol.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/giocbqjlf.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/grrufwbcp.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gztrmpsut.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gfbuevhgi.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/ghkyqnsvf.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/grefjjlal.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/goclctzpo.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gzqzczglp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gaiomxhta.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/guvltyryd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glepxhuwq.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gstvnbfwm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gdhpuyocr.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxigtimrq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gvjhxtpsl.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gxjanqnqq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gfyevdijb.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/giklpgwyf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gwwhisezx.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/ggmavkciy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gspexucyw.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/geppkepsg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gdllbqaab.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gonwtihdp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gsxohfjjf.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gafnamdev.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gozjjpnta.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gpvfenoif.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gavvzsmvq.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gbtisgufl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gdmzjbnpn.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/girkmjsuy.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/grekxiyxb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gqcofjiqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gapzswpfb.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/goengkilb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gvxoglxtq.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gtywsbnzs.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gtswqqdws.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/grptzldmp.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/ggbadxdhf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gtuwfkntp.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gttcvvsoh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjgyfxtin.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gywjebnte.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbwkhekhr.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gwayytsqx.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gpjmvytwa.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gqizyzafv.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gkaxlmdlf.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gyfqlsitx.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gaedwxepf.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gvcszhiix.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/glfjqlfyo.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gdolegycj.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/ggfgbpnzr.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gxczilulb.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/ganyqsgly.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gdpqldlwl.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/guousvgfe.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gwwrbocjs.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gzyolebcx.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/ggjlyfqff.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gqssvcrsr.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gtafbmwxy.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/goqwjenqn.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gnzkspguf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gvworwnku.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gqpgbfanc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gdfnazewp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gndehlwgz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gfhgrhnsq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/glsudvctz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gdqwpzxcy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gduigibud.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gpsqihzlc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/goflozgag.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gcptdnxyh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goblwrsck.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/guhovdnvi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gfdvzztvm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gtlgltdcz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gpanvvkfy.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/ggasquadd.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gotjmazrn.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gxoscdyil.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gbjinjltg.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/goffzynrm.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqhogyjdn.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gbwbvzjjo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/ghcyscmvr.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gdkdjbhda.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gqftybujy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/grruwyiwz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gttcttrtc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gvsbrhamp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gizchwble.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gvefwdxsg.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gtbnlitti.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gspxhwszt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gqivyvvfx.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gedpfiepu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grfvowfzz.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gduvjizfs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gmnaoqyxy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gptrxarat.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gdefhgffa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gnuzvexze.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gzoqecpsk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gybgzyuyv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gduwktici.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gfutcxzzt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gydskejfi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gzylbuyqz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/ggxhzxcry.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gcculzxfp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/guifcxjcf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gczrgnqbs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gurntynam.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gumbeyzzu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gxeweqejo.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gimekeyag.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/grikobyzy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gkdgxcduz.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gbawewvyh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gdhnirjrs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxpfklntx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gbjfxlvjb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gzltwzjfi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gwkdinppg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gtkdlbkvj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gimvfioyl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gyolovtzg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gfpaqjbik.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gswqmmyqc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/ggrphkxyx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gdunpfsts.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gszismnji.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ggnotjgyt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gvbldahph.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gwsbnqmel.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ginnusycc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/goifepluc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gxqwvlskx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gfcwkvkrx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gkiredpdc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gjkgjpwap.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grkhsnipa.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gzbwdzfgt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghnrieksd.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/guovnrvuk.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gpdsyguwc.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gdcgdtgqs.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gyfuaprxb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gizpuczrp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/guamlyymp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gcpvldzvv.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gwpisvycn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gerqhglty.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gplkhsdhq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/goscnikpv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gnkcgddtx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gznvgyfit.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/grmjcvbdk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gksodvzbu.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gzvazsmtv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gcsvsaqgz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzdozur.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gudsllmva.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gspqlrpbf.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gjvclydas.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvjnyosst.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guaeqhjgu.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gubstyyky.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gzcttglzf.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gjrmlshbv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gryqzrzyx.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gpmntmdak.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gptupxnrs.sHtML


<!-- 参考信息 -->