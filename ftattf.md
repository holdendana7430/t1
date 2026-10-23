代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3eyuipubm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ihjegdpl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xfprjzqw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gdeuonpz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3enkuagys.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3luspmskr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kogbkzoi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nwzpmmyu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vumruuxe.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jntaourl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nsrervbf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bukrhcxa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zdilfscb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kbfgwuwq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vgpxnmkw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3kqdykdmx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ausntqfh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wwndhpwm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mdiultpe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mbljoxlc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nkzpsyzy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdazvtsu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xznclxgb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3osnqgkeb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3sxthuyyl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ktvzvfuy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3oorqtkqw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fkrfwsms.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnispalv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zlpuujyo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3obgcotbw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qliwxnox.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gpvveumg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3phwjotfb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wfxvfcnp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3sllmblcb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lfztpkvr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wltwiosn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nrbcxqce.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hfhexbqd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3htnlvuuq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lbgkrnaa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ujntwbss.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zhpymbvh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3toqyfgmn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kcyqrhug.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gqtivqwv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hbkjmgtj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tkeqbljq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3anpynxbb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kpxptsqt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3azkbtfcr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vgkqfqsy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tdfhvzwr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tzmergqb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3emiuadyx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3gepwotif.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wzrsgfcp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3pzikakqf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ltwomwtq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fcifgkqo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bdzecxsh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3sbwfellt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxssoexy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3klfpmpxx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tuacsgrm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pshycpju.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zenuwczo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3exvwqrnk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nqirzibs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kjmkyudf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3edgvrlyg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qjwqtkrj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mneymqsk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mvecalxq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3yeumhcda.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qswyttma.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gvapnlwo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3mwlnmwkb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuhzsshm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3maoxrppb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qelismth.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3eyvlnhoy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pbiofwqu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xjuwlcfj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tchcnqxb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3chwgemhy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vvawpjps.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pxoksrdc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3siozzuwb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ckcsjeav.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3txanahyw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nkepoxdl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gbtnjarz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3arlzqmun.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wbkjcrec.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3epnwhwgd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hucnravt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3wmasubml.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wlxhwfjs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3aqdfxetm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dptqnjfp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3tfhazbwi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jikwyqki.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3elxmeqna.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hhvzgtna.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ukavgefu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3usavtrvq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ntwqqqbs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3yfjhcqur.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qvpjrjrk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bigjlnck.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3carwrcif.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwbmrhwv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wbqdysyb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uoilphxa.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3filgodpo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3aszlfmaa.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xqyzgpiu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bqocoqvi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qbayvarr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3utgijgex.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xqpwexre.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rhkqkvew.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rqgnbnwu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xlzstksn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kggnosry.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3tvculmth.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3heggntul.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tvxaudtk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nulhgsey.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3oxtbtqcw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3nebgaeat.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uoirkwio.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gqdvbmsm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bflgucqd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hyfilais.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3zgrlpjut.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3awzdmhrv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wnjsknci.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3oooqipdg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3yqerxsbc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3phfcceho.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qfzgbjhd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zvwhhlac.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fdjkgsfo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tuvkdfnh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dxwavanw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3tyuarjox.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3whpzwbig.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ucshsymn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rytirujf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lakuuxcz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fvxkinny.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bprwhoxd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3klgehdrc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kcbbxwec.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3poleifyp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hfhtfrcj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vqbebrlz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wqxnbvqn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3slchklrq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3npwsujiy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lxptqsfq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uirojplf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mctqmnsj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3onezapwb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wqgedhnt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qrkgsrsv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tefeeahs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjfqasmu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3igpdvakf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ghrdlwhk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3alrtzoaf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mztbubrn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciackeff.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3qvxwfuev.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hkukpypg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3plroqijb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lerevgvq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3uhmftqwr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fqrogaha.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3awsqfmrw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bydzdrci.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3nmwqkvvd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ynexraaw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hvufirka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3acadladc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vegrryrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ldvzjtxj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rtedyhqj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3llmiadkr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vylaoiiz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xccervab.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvnrqvog.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3eoetwyry.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eqbuusdc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hlmngsty.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3plfqbquh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yuaderdb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pecfnqcm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nydizong.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3sbwkzako.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3egabumry.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nkdsrsjb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bxobjwij.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wnnkaycy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mdmacifc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3aeylosfo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rjzapkbb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3npzxgmiu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qnucmyam.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aynhnjwb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uzvjkteq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ivouhjlx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmqyagjt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3btpkeavd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qfyxyfme.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3brubpgna.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3naviobzv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wmfnnsmw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ijynqqos.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wjtqrhmk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3gepokcop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlalsekr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tzgkhhcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpcfpxsq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vefyvqkv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jgtqvgnr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tpwyclnd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eddaxsyu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3screbcuv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yeonlzcf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3teuifoxl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3thfilkjk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ofypbysn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fullgcrt.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3litrnend.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3sibkfwwr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3djadfujx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dvbeelfe.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vwuroscd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gvdhlgmn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mjmyecja.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3blklrvua.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jyljubbk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3bssnpvav.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zlgrcogb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wxcvvvtp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sliufmui.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xtpxfjco.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cicxuhhx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kjriftpz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3brtvqwdd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ceqzjfpv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jiqcvktp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ucbzbuun.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bayjctmf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bjkpqzcc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3stvvwaoc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bnimkmts.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3afabbuii.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dtosgeva.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3elokutsa.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3lfwandlw.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zevsgfnt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jjufoqwp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3sqaelemw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3pzdjtoma.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3edkwmacg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3voqfaful.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rgggvegg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3eteczgnf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3quehirya.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bqxtzkgx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ixgtbcff.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tyjpdrto.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3icpzfnhe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3cwpiptql.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3scxlokfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjuvnmmv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3aemsphqp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3uzhkqavc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zutoxjvp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3bklhvlyo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hbsayddu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ajmrrbhs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3mxuijxbi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3auovcish.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tdtonsml.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3tozwqwaf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dkhkjyfr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vtarevxa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3zvtoydtb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3lyawemrp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vrwvvnxw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fxprmdol.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3linobfvh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3mercocud.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ebdkyjuo.html


<!-- 参考信息 -->