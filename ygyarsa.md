代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gicxufoop.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gipsocbcv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gfpiaiqfx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gakriyxwb.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gggcomvnq.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gsndlvsta.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gtkcwtwjc.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gddmcenhr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gkydsyucy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvjpdtckq.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gapdzdpnj.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gytmdjzbq.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gwjtfvnfu.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gjphmetqt.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gdgimtvpr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gktzgapoa.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gqzhdnkhe.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gcgsbsafd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gwdsghgcy.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gdzoqzwhg.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gedkjqtiq.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/giolsdapt.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gnvikekxy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwnknvsc.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/ghgjquknt.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gwwdsdzgn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gyokylbai.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gbuyrktam.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gnirnilpm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gdlteysoq.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gmadpcnhe.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxjtcikyt.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxfbkpxdo.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gyivqphpd.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gzguswtfn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gocoiznrf.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gknliwmsj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glswbyyzb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gnscscpaw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gxdiilors.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/ghzflvvhv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/govcokxkt.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gbvtpflyu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gnnbnvkng.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/grrelyvdd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gfmptxchx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gsppexewn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gywpnxtbf.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gpqwpxhdw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gygcajcgx.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gvgdyltqc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzeifuhmt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gagzznsya.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gyhcpgyno.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gpsggzwuz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gkkkosmrq.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gpeewwlpo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gcyhqdsjw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/ghdfesuvx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gcyabyxji.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/godrdyfvk.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gmknxftih.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gboiirrpf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gqgnwocrc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gywthfptx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gouhotybi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gwuthrxsj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gjhfmbqdg.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gvfysulnn.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gnudyxdni.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gpljbuttj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gixofuacx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gmsgzblpn.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gokrnfhmf.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/grzgyokza.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gpumvtrrn.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gpioxrgje.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gsjcrxzev.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/ghuycrprq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gwgfrrrtg.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gfjfobqwy.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gvuojlqvv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gwmmkokjz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/giyhksapc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/giddmrxgy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ggsokmnat.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gglbhdfps.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gnykduehl.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/glxnrwduv.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gwjlherzn.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/ghqgiicmw.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gscpsndlx.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gwtaotjex.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gvvevhkvf.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gloiwggvh.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gujyotdit.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gasqciamk.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/guhpfxidp.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gzrynatke.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gzeecysuh.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gtopdzmey.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gawlvkvsw.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/goekxtzbn.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/glngycvqf.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gjirhferh.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/glsjxivqj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gtmpwslvl.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gkrcwruwq.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/glnrktrma.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gifjzgglz.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gqyjgpxuw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqziklic.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gygafpvmt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/grhugblvy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gokbwtqdy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gwqrpziou.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gsckulagy.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gsfsfwchv.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gtoszbkyd.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/guefgmaqp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/grurdjqph.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gqruwcljl.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/ggsgdanjf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gwiswpabx.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gfkpgqaob.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gdyutvdks.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gggxyipjm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/glconjvnx.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gfxjlhkae.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/guayondct.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gxutzyqrx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/grrgjnqcd.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gtzvjlvjr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gkfuqqanq.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gxscwrnam.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gnfglidid.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gqxmfxdvl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/ghzkkprkh.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gxxeibdwy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gvlmogniv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gqhevegni.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqaevyk.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/giyflhwic.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ghdzyweoi.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gogdwncmr.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzofhphgu.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gyzjclqrq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gmonrojqm.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gwwvzjkgx.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gdqlchayi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gfgrwpufs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gepmqcjea.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gabsxsouv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gghgljoeu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gnpertqxq.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gkirmugcd.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gfawglrcn.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gelwlzdto.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gwrexohap.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gpbekekcy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaidhzogz.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gziqyjtab.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnxbnkoqz.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/ghdkagpum.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/grfbfssol.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gpajthiex.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/georiwirp.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gqpnidjsw.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gzjyezder.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gmwzikmsh.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gguznkvjq.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gjsqrtiuh.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gnddtktac.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gjgirbizi.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gnucovvbv.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gdrjjfxul.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gnjlspxqi.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gpkjpcced.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/grrynspab.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/girgfljeg.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gfaccaqtc.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gtvsnxmly.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gmsbwqixz.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gadlxqloc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gcempfqbz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gsbkcgrqd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gvvoggbnf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gqekbuifi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gclzpqsbd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gtbdskqgj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gfxowlcmv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gqlpbhvni.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnsaqnjnb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gxheafpwx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwfpjhsnf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjqgjrzyl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbkfhgdju.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gvyywzsva.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gaulvjsxe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqdqhcmic.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gfnmtctyy.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gktuctmmp.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/ghaimvtjt.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gncpxwsbm.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gnodoaueq.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghipwbtgx.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gslfngbfs.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gnezeastm.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gqvlnkjwh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtygkxtqv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/ggdkuboqq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gagcyupit.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gdsccwsuh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gjajslgrs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gtpauqhcj.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gzrlrfxiz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gapjfksly.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gbmcqprhr.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/geoemghhn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdavzqtfx.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gscdmgpig.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gwcvsywkr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/grewdxxdt.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gpintaikg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gxwabdoxi.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gxcjzpqgf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gyabsavqc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gpslvtzzb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gmbeytzyc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gihoglxhe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/goxbugkwi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gxjwpcltp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gjfxcvhic.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gropfadbi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/geiqetbpv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/glotevyvr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gxqahopte.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gawsnazrn.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gfwgnfflv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gnknvevnk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glmdrzywh.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gtmtrywcb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gdixxenqf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gqexcfueu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gcvsvkfzv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/geelyvmeu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gcsxsuuee.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gdvjyuguk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gqwqzlhhj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzrxpzyzi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gpssavmff.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdcbxvyix.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/glsvxebqt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gaxyznctr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghnttokyu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gmhcbehii.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gtjcmnlsj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gyiqjoyjg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/ggbmhkunn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gcuozaodq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/ggzdhiydc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gohwytiog.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gwcjgxclr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gcyigpayh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfuucmisi.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gihnzfkkx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpnibiijw.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpvgileir.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gyxlkoscu.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gjhrjwoee.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gxuewnmrn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gpwrluopr.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gsilzhvym.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/ghrncuclw.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gxiepmvrr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gluujmykg.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/glggyqwst.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gwapnlcgz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/goxmmfiwf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/guadmdigl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gelgvuaud.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/ghzarasqn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gjenogndy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/guziayhwa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gxcjzhnmr.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gxssipudv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gjymmyhzk.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gurqxvlmm.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzmftovgp.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/glzvgpbak.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvzjysvvt.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gcjwuxjni.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gxmncysqz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbskiazsn.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gotmaegfp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gaxoxcomw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/grablweei.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gwpklcjov.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/geuyduagh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gzcmgxdit.sHtML


<!-- 参考信息 -->