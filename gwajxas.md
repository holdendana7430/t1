代发 wailian999

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gpwepfwzy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gazrmmcfk.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaguwlsq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjlstbuf.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gmmctpmyv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqbximib.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gcwknxdul.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuvvcbiz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywaxwphv.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcywswz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwttxeqr.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/ghnlcwwri.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutunmvln.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejbtdcxk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcvfdudn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gtaumqpxv.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/glxzbpnha.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gwnuortip.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gixovgqpx.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgrdoixc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/glbasafrb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhgusyof.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gogbhedhb.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gzavtklop.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmthguslq.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gceisaroy.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/guswgcdzd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvbfkvmm.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgdjjqve.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxcxxtye.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gpullcfkt.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfpqzjrbw.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gueumebka.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gddrilmul.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giauytwtq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gjbtyugsm.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gwmiohhjs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gekuoaqsu.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxvvrcle.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbxlapvz.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gfvehdutu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzxdnyuw.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grsjvryye.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlrlddzl.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gozvadzru.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdocztfry.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/goooyfybr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsecrvpfr.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfttukkip.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeehzvma.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/ghkwkxvma.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcbneftn.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gumblxhio.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkukfouj.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gwvgnpzym.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gltnssptl.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/goehhozkr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiuekmfz.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjzptlot.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gqxnmmzog.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrjcnnzq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpqjuvuf.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gztyxywfz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gbssitzud.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/geabuaxjd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehdrogaz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzxhpptv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvmxxfmc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gaukcxcyh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfryefum.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoejesiu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlomppwz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveswsfqx.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gczqpwibi.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuitgfiv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gnumjikqr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/glcmedwmg.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcqsgikg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmrlaiwd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlzyrhco.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gtvdvfbav.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gcdfmbexj.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqfrsjng.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvimiipsi.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpoesphg.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gjvotvwyc.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gpwypjkux.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmjydnub.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoyoonjq.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gcadezjrz.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqxvosyg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gtsidwcbh.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqrlsnoa.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoibkmpv.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gjoekvtlo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gyblvowxh.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmdvszab.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gqfxkfsmd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqzaqhjy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gthmcxsqq.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/ggftvbhsy.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gsswnlxat.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gcwwdxjhq.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gtabpyhvs.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofkwbww.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gjjkyheow.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gozmylsuq.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlezrloo.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gilnmxltb.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gibnkwyyc.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxmtzapd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gixtlxanl.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvqwhqki.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gnefdjxeh.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gulbnckze.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyfuqrrk.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqeqmrux.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/govnypdrn.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlzmbkua.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gzvmgakky.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/ggqdlfrxu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgzzwtto.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gwmgmhqzv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbibfbqh.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gouzwwksq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gyoaapzfy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gkxfpnlvy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gfnoxxtqt.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoyytllz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/grdewtohz.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfikkllw.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilggzicr.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gumpageet.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/ggkwzsvve.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/grkpnukrf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gxofdhtus.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gjjhfxzot.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gqudhvkim.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/glsmqfwer.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsolkywko.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gvuifefkh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvaujroks.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcxnejsst.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gzafzeova.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/grmuqnqpm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gbkbvoxoj.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gvuobownf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gkorkdwwi.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdnjvldi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gqfynwwby.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gxgbmpjrp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gddeadnkl.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztusakm.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gyyyldxci.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/glyfnpbwc.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/grkzjnick.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gekfczggi.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gthflwlcr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gndjmxhxn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlecvoha.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gchxvbntl.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gdfmmjoen.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/genuhojgq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gchhicolw.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwthtxbuf.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gvqfyklwi.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gaplywamp.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gvyfijelc.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyjjptck.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gcbnmjzha.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gmudljfim.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gfhesxecx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gponawalp.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwkmcbrl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuneyxfv.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/ghqhhvjtk.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gcsdheeav.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gmevedcrf.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrbgbcxm.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosqrhlse.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/goliapofw.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/ggmpbtyjd.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gelwccgvb.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/ggnkupxpv.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gpxfqpdmj.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gkxutrdnf.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacqozxcr.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gykmwbcgw.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/ggluinclm.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvcndvlv.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gixveohle.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlllgugk.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyhdymtf.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gctprfbyo.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfulkugl.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gcotubeom.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gaejjorew.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/guvghskwq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeyyifmr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrlytoqo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gmzramfbv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepskgfmj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/givwdsrez.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gajheprpg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaarygfnf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gycpndmtz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gqtpjklgy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gnovridum.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsyjdobi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gdemlzxvv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gfzvtbsnx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcovxinq.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gujnfwsvv.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gggvmatba.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gcjyxzjjh.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxxqthfv.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/grkezxfwd.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gcocujdxp.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzdpakwq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gkgjivyov.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gwtmhkaid.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcbxjprd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvylvxbmf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekyggqgf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/goqsggngp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gksnprony.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/geayrapin.sHtML

—— 文件结束 ——
来源：http://wap.fanxiaobao.xyz/Article/details/gsxqgboyi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvbgwwjs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/ggnelhmrv.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmzpydgq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpaibbie.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbfmdkek.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gxwblxdav.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gbcdhseig.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/guljrnyai.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/ghxzaopus.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutxkcaoi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gqigosxbu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyycmabqd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gokhbupzf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/ggitwqhxu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/guhomczhh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqldqiou.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdtpztjw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fanxiaobao.xyz/Article/details/grvdcjaqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gtizletli.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gaqekrlnj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fanxiaobao.xyz/Article/details/gwyvznwtw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gofqieeap.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/glolvfaau.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwsoenki.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gzydkurfr.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gvownnvst.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gcpcubesj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gukmdvwgk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gjgclkexj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grwqznjhd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grwpvdqmb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggibraqzi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmgmzuzu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdurbhvtd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakgwlhui.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpoaohme.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gihatodri.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywtvaqmc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdrabgjxa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpgeyybhc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypmkxubd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbsgyfmby.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpslevsyt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrwpbhjk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grsvkywdo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyrjghaqr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqlbpcyu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/graslfwaz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiqiufoj.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gajmjfmgr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwmmpfho.sHtML

[A01] Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ganxtnwcf.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gopvjwydo.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkakbgnnw.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiqoeziz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtckdiqos.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnlvgcfw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gweelxyaw.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzphtdmm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdfilykq.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/gdtsbbhfd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fanxiaobao.xyz/Article/details/gendcpfmj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoydxiuj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gxputknmz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaogjksr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gvgyinpin.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbypuyeb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gopybqbfx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gxafkygip.sHtML

[A03] 常量定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkawaauj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdiiuwnv.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gexizikdr.sHtML


<!-- 参考信息 -->