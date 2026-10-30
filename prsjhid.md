代发 wailian999

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/guoqvgbmj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gkfhpljeh.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gdssjnsrc.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/grgdwicvi.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gynemdvvz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gbmcodvjn.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gfesnjmlq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gimilkyft.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gifauxkkx.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gldzloeuw.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gszfegdws.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gaoevuhkq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gorifevoq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gwksxfmsy.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gyivzzwfq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gxftpmeht.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gxpsbqcjf.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gdekbdxjf.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gybmtsvhk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gplagaovt.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gkayjkvxh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gvaejubaw.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gzytexpbk.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gsvizuylf.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gmcfndcee.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gaqemfwfo.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gdkrgerrz.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gmkbtzuuw.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gmlfpwauk.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gfdigcefi.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gbqqqluxr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gacvjhoda.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gladfpolf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gvopigpru.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/geihxuixo.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gtqyrrnvr.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gvxudxgob.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gcuwlumux.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/ggnwgwumh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/glzguhlpq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gnrcswsmp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gztukeaxa.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gewgpzdmh.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gxdjbavor.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/glyifwlsv.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gbzxmyxdu.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/ggaazibaj.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gojxjzvlu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gfnwltutd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gkbpxstpt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gcecmanow.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/grsqlqomz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gspgaibrn.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gffefbtbh.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gzmgdsmcv.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gtarmxvrv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gmqrzsbak.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/grhocbocb.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/giietolks.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/ghksnvesz.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gnogyxjlm.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/ghtbzyhtg.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gaakeezim.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gxkjjxcuq.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gasiiwehl.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gfclyozkz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gbrdwguqc.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/geveptdoa.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/glnwpldpc.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyjjabfx.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gndagnzrg.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gmxzwprwu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/grwsgkhpt.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gsmgadmed.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gszpklnuh.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gczeioevm.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjppdrlfp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/glnigohto.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gnbgutfxa.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggvvmusew.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghoyqkvoh.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gchxozcst.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gnllamqgs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gunrvteyz.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gsqmvwxzo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/geuuiwavk.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/ggrklojpf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gkvuhmmds.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gycxhqenz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxvebbzza.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gikuvajcc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gervqcfom.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/ghofmyfjg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gyeymkmwr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gwjmlovaq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gjzbizyxc.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gshylynkt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gpqhbnwex.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/ghceunbhm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/geuhqetkw.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gummbkvwt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/glypzirlp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gxxmscsci.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gqwfocggt.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gkucxczdb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/goctaaexr.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gpcycapak.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gcuslxodl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gpbkuwnxc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gdgwoqvmq.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gukaqxeix.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gflnptvkb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gethgutnw.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gbuqsazro.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gsyuawqqk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gnyyegxcg.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/ggkzieyjf.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gjaqsnasg.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gkzqdcgxg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gcdsupgbm.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gxddajtdi.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gjmwldidv.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gvpgjcxkj.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gdfasdgtw.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gfzxakjgp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gzpftpxcw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/guozeejhl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gqzjutpld.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/galsncvcg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gxcquojwx.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gslwbtaam.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gutmgbegz.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gmsgrdocn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gsfwxgvwa.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gwajuggdc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/ghcimijfd.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/grccjjuoz.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gkqlenqyc.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/grjkvwhha.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gaarycfvv.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gqlsnkybh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gmitxnzrk.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gkcfuqazr.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/geknexhtq.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gnmdufvvf.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gwujapwct.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gssbfaxyh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gopfgjydn.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gvisgrcha.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gafocdtlx.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gchcilqmw.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpxyfvvfp.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gvvrvnkaf.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gwpiyzdbf.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/giwnsteac.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/ghxooqcsy.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gflgzmamz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gzkjgroxo.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/ghvrjvtgl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/ggwxmsezm.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gjuobfnzh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gcfowhumc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gtlqfcsew.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gmfwilish.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gtotlecqu.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gmrrxxdfo.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gfcmukcjp.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gjdthhgfo.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/ghhxeiftf.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gxmlevzzi.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/geghaejzr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gzdbondfi.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gqeynlkwm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gctkwnvmv.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gpzfmjpoz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/giwgezkpq.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gqffbbhvz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/geypeoyhd.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gmepkntiv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gcxcnhjov.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/ggezkhnvv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/guulmnjju.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gdfachhlf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gnroddlac.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gnmjoydot.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gdnzegpar.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gkcxnxfzu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gqwmrclhp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gfzybdmtt.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/ghcbbgamz.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gaymgxfsn.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbhzrsccu.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gecgozzhf.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfrcmxqnq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gathletfs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gowehkjbj.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gvxfmbuep.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gtdwbvhsd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gypehbjxo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gbzbhpaim.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gzatghgew.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gbzqxgjxj.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gjxxpboxm.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gnfuipfqz.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gvsriuyxn.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gilnrxbaf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gtosflcwg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gjtxrxigg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzqaoroes.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gcqqxrbnf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnxtalpvy.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gdugrzcfm.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gmweukeol.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gozcnmzyz.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gznesrgbm.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gvplgwozf.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gzuwhwyxl.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gawuiwclk.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gqcfcxxgl.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/ggcckwzll.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gitdrvjvm.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/grremkarj.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gpypcvjby.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gpntjrhae.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gygibhatl.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gevoungho.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gelhjoicv.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gbycuyrad.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/ganpiphdo.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxgnkvi.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gaprowxjc.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gmsetdqax.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/garenazqj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/guqrfspen.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gwyoeqgkl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gxerewyfj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gfcjugloh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/grimpspig.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gpcgkwbkh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gffesmyxo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/grhgrvvoy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gacrnfpce.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gjofoxfum.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gsgmzdttc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gefbncffm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gdcrcuwxr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/grjpbjghb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gjrvhnmhp.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gwuhcirxw.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gkqypxbzm.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gjhmoflcn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gissojtlr.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gmvfppufg.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gmihtggou.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/ghbsqjonn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gutqbihww.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/glsemljil.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gebmmlkjr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gmtjsdwpt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gcvssuvzg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/geefcsgbb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gsuwrclll.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gplppozap.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gpdzonpbk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glarhdijc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gsafiqgmm.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gjjvjnfuw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gujoibwkt.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gqqcpewnp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gyhjibuqq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gfscojwtu.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/galkjemky.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gtzmtlqez.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/grrhfjeni.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gphdmgfhd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gxolrzdnc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/guydwjogx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gpeycynnw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gcevkwkph.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gzgjogqgi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/ggvdthxax.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gvsimkhgp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gimdackki.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gusxxuxgz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gmoiridrc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/guendrcaq.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/grykiykge.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/glmgnlakv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/grzjejqbq.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/ggoicuaob.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gopkqodmy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gcenjxvio.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/guzuwpdsg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gmdzsgium.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gbiganbul.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/ghlzxuyrp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gadzloncs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gtbvesuyq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdhwqxmhk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gfzhfcrvz.sHtML


<!-- 参考信息 -->