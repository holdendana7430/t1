代发 wailian999

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhcmhzr.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gjtspiiju.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/giqyfxrmq.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gelwrdsdp.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/giqcsnwgj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/glwxbixeg.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gsdzvoybg.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gzquqoyvb.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gpdhfnfip.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gktfbkwin.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gqwykunre.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gremcflcj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gdlbrdzen.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/goypygyux.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gqhehfpoa.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gimxoouhf.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gkeyvdhlc.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gilfgtjro.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gugfppape.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gzuztvjzb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gfbaldtke.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gnviubbuj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gweltjhpi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ggzdugkoi.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gfhqzxfcl.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gmieymtbh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gjukngkuc.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gykwmkwcn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gnmsktnpc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gqytkbqsg.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/ghrohpvds.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gfutigdda.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/grrpsjfmo.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gjqqqsunr.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/galhdptit.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/grmopiyax.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gtvhpfzfr.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/ghxsgcgie.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gmcdeyldb.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gjvcwpuli.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gguastuam.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gbpoyevss.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gtfvmopan.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gjeesgfjj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/ggcqxtgqq.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gyvoidmuy.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gvdtoioic.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/goxuonzrm.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gmwgcuedo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gxuqawmrw.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gwuyfsvac.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gqxefojni.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gryngztdg.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/grxewaxfa.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gpgzbiuri.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/giaqimzwx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gndnyqkih.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gwredkmly.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gaprxyfeu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/glkbgvtud.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gxaxzpwmw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gjbbldxtz.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gjqnrmivj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/ggkizefrz.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/glpoogjin.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/griibmuve.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gkycqathy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gaktntsuk.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gzidysgfz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gxqazweak.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gqtfxqfjk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gmdinspfy.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gjmzclxed.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gbbggsdht.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gyyqpuazm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/guhlbawsw.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gumfcfatk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gzecirwsc.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/giazldlbo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gdhmpjuqm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gzgoxlfjn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/glxpsvlgh.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gqsqtdxxm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gnimirkpf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gnjeaznhl.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gmclkjiyb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gkvstutwm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gycvtjvna.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gixghbhmh.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/grraswtwk.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gurxnqcld.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/ghwowwfoz.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gpwretvof.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gpnedixtu.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/grrlzdffj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gevmwrqox.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gyligiyou.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gofmaybwp.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/grugwosek.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/ghjdgaush.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/glzmfyasy.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gqwshfxeu.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gslqknifm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gtemfkusp.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gmsucvdyn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/ggkshxygm.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gryoimmye.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gxddkpdtq.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gisvxciyp.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/giughdcks.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gjlcilouz.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gckwcokuq.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gylthivgj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gnogieman.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gaakxiklo.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gtfucxgfz.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gwjkujnjy.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gtkgtwder.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gogrtvpqg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gdvuiefoi.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gthvarkkk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gtxszpnqj.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gdpujpuor.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxmxpvxbx.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gwgztidgc.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gyrqizsmf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gdwxmjipx.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gxynnzxvi.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/ggcnymbwz.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/glxjbjhfj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gcilfeluz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gmpddsneq.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gynqcwihl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gwdygsdxh.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gzlosvgro.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpfmkpa.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/goyjymorh.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/glokkqkpf.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gmayugsxd.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gahmzwslx.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gmcqibzxd.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gwtpyvdrw.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gbyzpdept.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/guppnqokw.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/glovzuwse.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gqzreqjle.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gfbyssvdu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxrdqfrxl.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gwspsehph.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gevydnele.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gerzsrlcb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/guolzfepe.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gqjovtdcv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gwrbovpbd.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gardlddvw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gisjzgorw.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gqtnjevyb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ggosyunib.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gbbhlyjeo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gmikajukw.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gmfgrluvb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gjwqbtgir.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gmxjaybzh.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfryztzod.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gjehgxoyf.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqbbyywcf.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gpehyzrjz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsactljfm.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gfuaeeizd.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gurwmrrfq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/guiclwulz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grbgrbqlw.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gjumxwsgs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/grvmqsivy.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gzdhvcoio.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gdtyposew.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/grwbmzxnu.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gbyrntesc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gnxspmbhn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/giqzwpjud.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdpyagjto.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gofytxfdu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjgeqhtcb.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gmtvsaezp.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gknbquhck.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gujbrzfkg.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/geiexzfjr.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gisxuyzat.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gyudlzsog.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gncedlidg.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gseulhyud.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/ghrdzatrs.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/ghtqntxhc.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gqajfdguu.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gsvyqluxo.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gmdnjlufl.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/ghvowmokc.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/givetnris.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gvtfyxycb.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gqcnrhegb.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gpfgecdec.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gefbjwned.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gorfmjtin.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gzyoysxuz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gllxtivpc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/glbbgoiff.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gfpkqygox.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gchaaboln.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/geoyrmxpv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gtkpjwrvv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwztrqukr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gryirmyck.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmplymvho.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gkjamhyzu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gnarkeiit.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/giqbdkvbk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/glumtsexs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gdhnmwmmb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gdjomcnzb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gzpfqyqgd.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gislcxjql.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gdjlvzdne.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gabelhede.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gdadyjryf.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gayijelqk.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gytcwhaze.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/ggkpswbwb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gnfieavqz.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gvkjonajw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gklllouny.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/guycvjlri.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/guchorrpp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/guafpazav.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gljvvzbct.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gmhyrfowu.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gcpyegzqq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdkcxsgmh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/grgdtvolr.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gwyjiiajd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geglcziwp.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gshvacoju.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gxhzahuzh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gsvfgoiax.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gzcbysbjq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/geeouphza.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gabglqfjp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/ggbkosrdg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/guzunsvnq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gsrjopyjg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/givgvsmoo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gpozvjjpm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/godpukdig.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/ggpbjxtur.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gdtjvjzib.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/geigpccsv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gmqwyobsu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gywsmlxcx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gfdnislts.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gxgjvfqnu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gvysockqq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/grvbeujhz.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/grbsbowbj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gzoqsixkr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gtxytvriy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfmsvtowf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gjjxlhwyz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gertgkquk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gwxhevvxa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gfwdhabkm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gotsvlhte.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gtwjniaiy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/geafwrand.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gngqvduno.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ghbwtskat.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gzbfdrojg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gagmshouv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gvgpexjqy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gbuaewfkn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gbvbdfkue.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gixuyfnkn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gjwuurjxs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzhukbqid.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gtbrwsqga.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gfwzqkhkj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfgxqakgi.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gpvdqpwgd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gukwfydmo.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gugqueqmq.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/geltuncqz.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gbbzrsccw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gopnypkxe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/geswzznfz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gqonrjddh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/ghepvhbya.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gkbrnmedc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gckfovxrr.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gfhilfzlv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gzmbjtqju.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gjwildeqb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gqqeqagun.sHtML


<!-- 参考信息 -->