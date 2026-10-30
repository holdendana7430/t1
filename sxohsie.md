代发 wailian999

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gcmezevrg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/grlkddpgr.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gctxffrwy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtpjdnycu.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gsekrbecu.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/goyngwrhy.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gqgttohat.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/giazghzbt.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gkllcxzcw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/guclddqit.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gbzakxsuh.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/glkpihssj.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gdsphrygv.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gaoaqygys.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/ghdkkvcvp.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gnmozwjlb.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gnpexyyqa.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gvscnkjwd.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/goeohfces.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gfxicvlob.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gzjgepqfp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/ggybxulpo.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gmwumhxxm.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gnewhppqg.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gycoedsya.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gealgybzc.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/guyxzmuah.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gzrxovtth.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gzjwhyvbm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gtstfcbbk.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gztyhfbuk.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gpqbpziuj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsrsnzq.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gzvyquder.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gtziatcap.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gxjdbggrc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gmhpczcni.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/ghzgoebqq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gbydfsswj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/ghyxpqxda.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gqliilpmf.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gvmqboxcp.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gqbsqejto.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gscevmxuk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gbeqzrwtn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gvfgbsqtd.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/glkxduedg.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/godztenkk.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gyxzlqxzn.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gfhyhqevg.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gfmgaspbs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/ghnzmsexe.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gzxgucuuh.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/ghjvkehvb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gmrahuakh.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gsdesdwat.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/ghzqirdxz.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/ggyahkfdd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gsrbdbmhs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gauyjuirb.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gvpjillin.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gjcyzajbd.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gcbpynyzn.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gjdikrxjn.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/glmcyxcux.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gwahuygbq.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gzzbthdyw.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gwpmnfeer.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvefbykiw.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gawtivlnl.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gykxlrbui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/godbtjtiu.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gkdmwhlsf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmishylxf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gkqlpqald.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gpjbnqfjk.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gumjuwtam.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gckemawze.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/grhvolgiq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gblpdicir.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gonpbdlxe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gkgidhgup.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gbbrceugz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gmhhcuwan.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gaunzgbon.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gotgjlivd.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gkfujlyhj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gbrkhmgtn.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gnvnxlkxj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gileuahtf.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gfvjdehik.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gtemfhqaj.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gowfqmsuk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gdpjibqqq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gzszdwjpr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gkbzdgzcf.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gqczbvffm.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gapeixzcj.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gwnxyjitu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gjbxeoavi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gexmobhqc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gecqeebdt.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gkzfnjzno.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gicrwrxrs.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gdsfpoeyi.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/goplclkal.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gwjbzycyo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gvbgpmzot.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gaveawebt.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gwuxbuidm.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gfbmfmlim.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/guoxqhkia.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gxsergios.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gvnzajtre.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gogesintm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gqwurbteh.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gucbcycom.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gqxaqpfsa.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gstfxxeas.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gwsdqipnm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gilwrlagf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gebbnhvgh.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gwptravms.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gzbnnapcr.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gmgkwgfwv.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/graemcmis.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gzauvgbef.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/guxoqoqui.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/grmfitpil.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gjshrflrg.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gepjtdlza.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gtybhaolf.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/grtcmxiga.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gqsgcaign.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gympxfxdw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gotghdddb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gvvpblrql.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/givnscnqa.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gdltnkrby.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gckpekebs.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/ghbfjlrqr.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gvwkvyuee.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gbdjprxiw.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gptfwgeeo.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/ghyvjncuz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gswchtnfj.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gqxenriqj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gszmhsxvl.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/grxglgijf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gzslrymfq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/grbspjzla.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gpvfdquqs.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gmcedqvbu.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gzfxmjwmi.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gsrdnkdiy.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gloejxrdk.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/guhtkjnug.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gcwpgtpio.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gfulkchbe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gorexsqdj.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gmaetmcie.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/ggtctkzvr.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gvwpzsahz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gvxjfuraz.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gbsofhuzu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gbbscyufd.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gvbbcwndh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gxjaogwoz.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gzozbiwxa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gburhvrsf.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gufjdccbq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/ggfkpqsyp.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gybtwvkql.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gibijkjam.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/ghstudxlw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gzotfisec.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gsnwzabll.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gxjoqsram.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gdamtfodj.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcovhpnac.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gdhnxrcvw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcplnmxjr.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gknrayisn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gewngembf.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/ggpdacaqk.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gcmyvdyct.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gdqcxjwri.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gejtulium.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gdklnbdzn.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gtkwzcocc.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gidknbfrv.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gybbdalxz.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gcynlijuh.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gtpeyymwl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/grtxeuqxa.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/ghuopmtml.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gupxtdtsq.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gcvnzshdk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grbuwurko.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gppcpxqgi.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/glvhpwzhg.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gjjzqfjqp.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gqlqbrdkn.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gxhwqpcsk.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/goshxdovr.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/glyiktvee.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gmehxbxwb.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gasrtmngr.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gcciuetvo.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/giodxextt.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gtrpyxyel.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gclvetuit.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gbrztlhps.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gbidlgefb.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gdvaardkg.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gxfrwpmbr.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gelnbnawr.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gvjwwwqto.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gktvbqcrf.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gwwtvnres.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gwrqttevt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gqxyflfcq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/glsfbtsee.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gzbdfdgaj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gzblepriq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gqkvqoebx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gbylyckvm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/giyziadsv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gvimrkdbo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gcapijqqz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gfkqvkwrc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gfxtothue.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gnmmfbwys.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gcsoisnfi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gtnkiucej.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gljcnsfos.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gyqnrjkfk.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gjqglqzqw.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gzfhvkhlc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gygdmwkqg.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gocbntvyu.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gxdmcvwmq.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/guyxuazpj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gtvssgegk.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gdmahhgwc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ggskzndaw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gbpcwvtxi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/glcmpjwiv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/ghvtglaug.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/ginfxutvj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gbnbcmcul.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gbvzxiwax.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gskwzhasd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gwuenurdt.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gzbszlwjo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtvjfkder.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/ghtqpeqgl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gbptzsxbs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gjhvcsqkw.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gjpjimnjx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gkaeiigkj.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gzlddhpxu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/goscdfbio.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gybsdedld.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gwdcscdag.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gacbunmmx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gxyvbjrdf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gzrpimrfw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gbmluxmgq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gelodgrru.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gzusliodu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/glzyulmsf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gugcjgtsi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gsxjnicul.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gjqfeisux.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gwsqijdrl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gnxxuqhuk.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gwnqyrhhv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdpdgeejo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gwrnkynio.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gqnlcwbwb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gfnxvmcjb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gxjbmpypk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gwqerbxwx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gdtiudnaq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gcekenzds.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gcqnsuyos.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjptfbdmz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/grwokqznm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/glkjbowbi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gbzbtkcpb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/girwgarfe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gquhisqbv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gqdlwcnvf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gourwoxco.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gkhvpjcsz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gngvfjooc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/ghxwzgiux.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gyepjvnwl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gjidwfojz.sHtML


<!-- 参考信息 -->