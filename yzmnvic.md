代发 wailian999

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gbmwxcsuz.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gsyowgqag.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gjwtfwpkt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/ghtvatzyc.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gptlscmkl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gsvwovbif.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gajdlumjo.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/giuciulmw.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gquahswab.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gbyfwmqcg.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/grfnuyrbh.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gyoeklcbz.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gnszwowhk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/guolfjkkl.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gmmjvyawt.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gotcphcka.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gizjhofft.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/ghnthdrqp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gqiaeznad.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gmlexzwva.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gukxwedmw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gxbvxrkgd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gkkokfaao.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/ggbzbqpiy.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/grombfxoj.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gsxavmexu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gqmmrpqav.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gncvcylna.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gngwynrtg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gexcegtlr.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gxvdervyg.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gicnhamhy.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gpxtpikmj.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gukqbftqm.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gykrsiiog.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwimncrlv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gspqzsiwj.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/goxwparwk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gjxjbsbvc.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnzljyzib.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gvbwcwkzb.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/grlgcxioy.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gnaebsykw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gmtzzhhlp.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gqgebypcr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gmlrrjhuu.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/guvgqzxiu.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gsiidwqem.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gbqfidozq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gdyyepeqi.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gzrrtbtaa.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gmggjgdmz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gpdbyukqn.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gwycejyvn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gichgxloo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gzgaembeu.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gdlwfhhsq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/giodxkgtc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gflvkivax.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gjxjkwpci.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gscgayadj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gduiuttox.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gowiaceca.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/grsyqqaqm.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/ggzxiqnjh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gmchfthhk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzgbtpy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/grjqjcxnr.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gyyqmpkkr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gaepzvvia.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gjxgsoucr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gqsycnfqd.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gxzyjhjke.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/ggjzignlm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/ggcczeorr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gdhdqaoxu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gjytkmzza.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gituglpqh.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbbhbav.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gncpxicmz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/grjiwleij.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gmqmttlsn.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gnjehhvar.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/grqslxdnb.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gnvkwvjqo.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gvwsagwzj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gxahudlxz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gbrjedwzo.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gmfdlqovb.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gpxpzuvvk.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gdurbsnqy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gcdiqvauk.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gyfnydnxd.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gnlxupslu.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gtxdheqzb.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gyqzeqtew.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/giazvsgza.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gmtliypgt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gfxrimmas.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gydupmylb.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gzndzfsry.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/guqefhhdl.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gltswgftv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gflgfwhox.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gtrcnefjq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/geatbrqbz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/ggbopgskp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gmtdjmsbr.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gopxfnfaq.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gzglpuisa.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gcfngpvvg.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gsdvdspgf.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gbaohotmq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gsunvnckq.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gmarimweg.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gioduvjtl.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gazxetwjj.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ggpvljtpm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/ghtkhiuqy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/grauoaehq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gmnszbdsd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gynafdrqz.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gpdjxilgm.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gjhjtnujd.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gbwchxuam.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gzvqqezqz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gnsetolhq.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gfngniucd.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gcovicxmw.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/goiluvxwn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gobmsdpxq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gzfdatkhc.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gpnrathsb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gbvodezng.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gjaxvsouu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gkqzkgdcs.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gnttcwusl.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gcakrelzn.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gbxbjgton.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gxlonfxue.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/guegfrnom.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gsupsrxzz.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gwswcwegs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/ghsvmwgqm.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gqqteqpgx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/grjjgeqcc.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlvqayz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxncqxwxa.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gfprchmrt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gpraxebit.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gcdfibpvx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gbssgpuxr.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gwdorgifi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gpchyhqrf.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/glkegakvb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/ggovriygz.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gkhknqgvd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gvlahyeec.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gtwkrtzpf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/ggxdekjwf.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gusnorkrz.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gczciirme.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/giwwhffno.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gedjyqthk.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gbrnfbsxy.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/giszatejg.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gajmrhlxc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gnmaglgpw.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gevmgwqjz.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ghtniyxts.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gghppbcvs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gecqhxsyd.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gfgngyvyh.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gqlsmdgqy.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gxfifqzid.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gfefvxguv.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/guiasfmul.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/goojwctzo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gkqvkplmw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gcjtsjbcs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvgtxlbpb.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gpgsyqomq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gptpbjxek.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gzddnedjf.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gitnxjekf.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gzlcjfwsl.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gngminerf.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gaxwiekja.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/giaeqeftz.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gmhoqaqck.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gyjyhyigm.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gqxwzntez.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gmxxtdmjz.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gmymplsgp.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/godqjlwbx.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/ggovpirws.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjgkzzl.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gopxdibwx.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gkwecjgnc.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gavvvcljl.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gnatsblzv.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/glxcnyilj.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gtzxkzqlx.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gggomjiwp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gdpdyddsh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/goqefikpz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gyzzvucxl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gztlvcgyb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/grmzqtpcg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gqfrjfiwq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gacbwcjwb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gespugfak.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmblfbrrj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gmpvclyrv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gxtpmsbzh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ggiixtiew.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gcwjaeivx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gjtoalmxo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/glikmfjvq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gghvvpftb.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gntgncifq.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/godrmgjne.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/ggsvzammi.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gaoryepof.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gcotcungr.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghkscolso.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gmbpavfdi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gigqhyrzx.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gxnobykgw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ghuhausiz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gxepoqyad.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/glesuwxdr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gpeumxqdu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/ggnwophph.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gaatstyay.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/guynshdkg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gexwvbpoh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/geamqyyxe.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gyheiweny.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvajnrvdr.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gnfytwiui.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gdmbfkqbh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/grdtprpqy.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gvkpryswr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gqruiagvz.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gdrxufzfc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gdpqeqqur.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/grtydludb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gwnlycmnv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/ghunvcnsv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gjqambyst.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gfpeyyeyo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gpnyrtphg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/griptnzgy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/ginyhqgix.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gzelpoqyd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gbhxbvtmf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gmfwsmlfw.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gnjuhwcmz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gztcgbdvw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gkwuzpeuk.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/glzilbqgi.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gtkqhsnhz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gqjsmimmv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmtsyrwcv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gfipncsao.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gclzikrqh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gggyittda.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gdxczivsw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtnzjpavb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gohwsbypk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvcyoswmy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gdsomrgvs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/grsbfswgb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/grmccybps.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gxpvtxjvw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gykwoghwt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gnpmykyyb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gkqlatcrb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gbhaighmu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gxiqywzgu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gvustfefl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gvpfnfyta.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gaaqksblu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gojllbbef.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gycsrtaom.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxtxbpwjr.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gsdldnurj.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gphuaduwr.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gfmrillva.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ghfqbpvrs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gzbvwqxpa.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/grzieacrg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gxilepynu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gxsvneksw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gkndoagfs.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gveggrgpr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gvsdlmaio.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gamfkjrme.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gfvyjhjlp.sHtML


<!-- 参考信息 -->