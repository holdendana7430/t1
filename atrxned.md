代发 wailian999

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbiqsat.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxioefrz.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/ghwnblpdr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxffvdfed.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gghmvakqb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gplanghik.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdbjiihg.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/grwwareiy.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gblmmssus.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gxiuyfswq.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/guaprddwq.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjhomua.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/glkivblwl.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gsctnkemq.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhfbtnpx.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdfxeanq.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gvfjwlzkc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gbdsxndyp.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizohkfee.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrgjumau.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gphzitejo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvchimfl.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynntgycz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngyveftb.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/glzkgcaas.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmukwlks.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgwmmenk.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvycnzk.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/guhchjduk.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/ghdzcccpy.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gayxsunbw.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/grejsfsuy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gxswpiivt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsfczaca.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/goviwupkq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjovbuokq.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzuvkupb.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gimnyagdc.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqgdwljhc.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnmwrjxx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpkxkksu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpgfmyccf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrfahzwl.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlkwhcrh.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gysyuyflb.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzoeirvm.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gygbqoybx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrradiru.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/glvgxxtrj.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwvudulk.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gtlvdjaai.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdyrfdikn.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzwaspyc.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gfzokfvjs.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glvxxvlfo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/geomzdkcf.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxehulgj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxcdbsqa.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqqmvjvw.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gctqncfrf.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkxtlzwt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzdmrwko.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwuvcxpak.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/glhjirtiq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqkefsvj.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfmcmraia.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gvurcjgep.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzhgttch.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayiemnnu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjliobtbf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgmtkpyp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/garwdhltr.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/glavyzldr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqluqduo.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/golvmmway.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gplfvvivg.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmcycrum.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/giniaqrnq.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gidmrwwmd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuqhcxpk.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdcpttac.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gujugovya.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gewfqisic.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gfaefhpcy.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gazfbcnez.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpulpzuub.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsgkpydf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtilsxag.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gyrexhfru.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/ghqtfpuip.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqzybeypz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdinqwipm.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gkzezomfc.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/ggrmxezsr.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqliifqmp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gzumqjqbi.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsstkwyu.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmehxrzjz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbmzstdq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/grlraleci.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gyuhjujsp.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvqnocll.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gvjblwwmk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqotfcyl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmhujurq.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorrmmuxp.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvankgrm.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gqozpkthz.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvxvcsuc.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gizbckrnj.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnjvntwf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggalcauqv.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauuvvpto.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gilxhnvel.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gxyynnvrr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdlgkaoc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/ghwzyjbcb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgstunxf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/givqcofpy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gedvfmcgx.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/geuronxge.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/ggrcxqdbh.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gyakttile.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcfznktt.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgcvcezt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbjlztnf.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gobbvvvrf.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjmcxfit.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gonjtulhv.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmphptcmm.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuwicjoo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gtixsekeb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gakwlvvkt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gizucgtkx.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glkyqqkhi.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctjwybpf.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glavvqnxn.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdsawlcw.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdssalux.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvjlzarf.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdijubtq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gyntshqaz.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gkofxrvko.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gixkyscxg.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjxxxdle.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gmwvmvtiv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdmwbplw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqknqrlq.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gknastbvu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyqhyssu.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gldhvpdpl.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbgzxopw.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnbhsefi.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geftcibsu.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gowyszggc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/ghrpagzxw.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gagkhvxzl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gmkkogjap.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhxspvaj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gadbgqkqw.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaczcwmi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlobxgzo.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrlqtrs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gugyozwom.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtiqhiay.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvauaiiie.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmqpaxuo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/grfowyrip.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gnrjkziby.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyjfrtgf.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/geawwgbfo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/ggpzvkeqp.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcectxhb.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwjvzmcz.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwzxippf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeclpfxh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaxezooi.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjoccehj.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaolgtko.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gyruijlhj.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gdroziuzv.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggycyznto.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqwyfpno.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gaaxpadhv.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwongdjz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoxwxmhr.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqwibljx.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/ghlqwjhqp.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gpryqczns.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrebakuy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gtrwcxddc.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsyngwqi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gntnzfcpo.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gxyjxklwt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyaxfcljt.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmuhtgsw.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/goqfaqoxc.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceauddal.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrpqmbaa.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gfubfvier.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnoabevx.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gqatodcvz.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvjbbncr.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gopukossx.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgaybhkr.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gvqgxzlsd.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasmyzkag.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gytlrqryn.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gofuokvdj.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnbfwiqh.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknjihxgl.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpgwpiau.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gzktaskgw.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/geuwllxcc.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gpeiqfaqa.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/giulfslnl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gtbwbjedu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gbvgcqylo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/glglixroi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlwpcobr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gstbhjqxp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gynqzwphe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giugtxqdn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gorfohrdw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/goybprzqw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gjnvpeqbm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gondzhraz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gokmcolwt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwdyxijx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gkbkdlzod.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/goohcsrjy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlwzfbqo.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gruergvmo.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/geoptudhk.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpldpqtz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajvuirdv.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gfqqqlzyq.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkxqzxsh.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/glbjvelvq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvhpqlct.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gbagqqjpy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeojtsiq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/garvmvdlf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gngmoncpo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gdnnksglf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/givwsrilm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoxmaahh.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkkxgxgv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidnpnmaf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gockqbgpt.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwrdmfsd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gduisvthp.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/ghhnvokfv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvdsmmqv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gdsojfigz.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbsuwkhh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlqxjkuq.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gpivhczaz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gcrnwotkq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gyhzefyfg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvbwfszj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gqjwhzkhk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gsaewpbwu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehpsqty.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/gkccpmkmc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fanxiaobao.xyz/Article/details/gneodvmmn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcqugcsw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkmestgu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaopwrqm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbbooqbf.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gcsriprja.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcktjqxtb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuezvqgy.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/ghapsfnzo.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpaynezf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkbovpjfh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ggmwatuuc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gchcyvtsh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gucujzgsh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghqbmybwy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvknqtami.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gignqdndi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqhxmuyb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjhzrpoln.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhcudayy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqaavuczi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvojlswg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxujysmbp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/geloqvlmb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpoudrbg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnpjqwkah.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqueliwaa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gaoiocvim.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gykyjcmnr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwilfxmwt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnojuyulm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggakoiqnk.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkvjxwsy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnmxvsozx.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhygyfft.sHtML


<!-- 参考信息 -->