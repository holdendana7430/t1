代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3outflwdu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xydpxrfs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rqkqrhsi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qpkzwcfd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3npnkyoyz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bcssmqij.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fcaebkca.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wdgibtpb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qxdyslcw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mywnjlvt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3imnvobxo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gsvdhzhl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gakamswy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3oexrdfnb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3seeccgfw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kygvwsbs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fgnuquzp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uteeqpdz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xnglqvso.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xugipkkr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ndvezrtt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zngltrnn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3uacupwfs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qkpchjvt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pqfjptjm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kpystppj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3eljcgvra.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tecklxhz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jwcsypwq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3juylbcpm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ilindbqs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dfkelkfn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hojtxdyv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nqsdbvwk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3uzonbtuz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mbvqqklm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rpemvwkc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mvmveitx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vrusvjzf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3bnaxntvb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zkbsdesh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zmrwikzl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3andfsqou.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rlzffqul.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3howuogas.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jjwygpqi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rawevmgs.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qlqvrdjq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3azwxroxr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kziqnxhn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3skdegyom.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3htbxkyha.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kkrjujfu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ripxvhui.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3taugdrfs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kwloyrga.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3oshwtfsq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vwwlpvpd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3awpshujs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3imkbnyne.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lygmzkoh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qlqdrvvy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hobdcrwk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hkoqemuq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3flbrcbzx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3izzanrta.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3idegulcj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3esikgdft.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jpbskpsw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lszrlkbm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3stjstaxx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3afcvzvxe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ftlgkwbv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ndrgrqos.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lfowekio.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3isrfsnis.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ziegeiec.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jflrmokq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3izkruozz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nurvshxs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pymfvgpl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xuccivdt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkuhtccf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dolhdiys.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3unmptglt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3obnuuhzk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gqqibuep.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3avcoboqw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mdyzhwjc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3atmkmfde.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3glvduxdx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqxgxfr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rbvrmfnj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hpbaxeax.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jfctqnma.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dvfkwtky.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ipjljgka.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rbvaonpv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yajnpglf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pdryemtg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ckrgoxcp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yqanbjwx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gesspcqo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xvkhoepb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ieursgbj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3zqgnomsm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qdblosmf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fjeveywn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dlvngsoz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lsqrxppw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mcwmczfx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zfrhfdwz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vxeoysxt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3fkjgvfvp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bbpmmcms.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dxwkcmiz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sjbycebz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qvqwozal.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kaqcmxdn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3esnxmnbj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nxbadvir.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bvhenjtr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ognaoqcn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xbqxfvow.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ujocgkga.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vyemjoip.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kayjejzl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kuqemsgd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yvtovoep.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3azmibkzr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mtzvextl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qbkzxnnq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zvvgkbph.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3odwwdehf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zszbiugs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3cfsuaecl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pwkvxyai.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qdojpjxq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tpagskdw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3cfapjzam.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3acpblaoe.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ksiucbcw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwwxco.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3taedrofc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ynjrmetb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bbfztjvz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xyxwkfms.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3nxfaxhpc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3rfwwhonh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gderdsul.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sjmlrttr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3icetbdvw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3trwijfkc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xjfnhkjs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3djggcrvb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3riejhsfo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gbfyrdoi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ankfieot.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3sszzuesh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3myldcsik.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jybyvthd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3obzaupdl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ypcjtyce.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3owbrzsun.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3refllyef.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tjifcqqr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tahexajj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ljsynffm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3adkhstfu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gmchcoyx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rgixrvzg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lejqookl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3atdkipgu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3azjteykf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sabpfasj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3npmhqfwr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3depyezwn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3odqdcwyn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ykozapkd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wzhqvdcg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qkrszqek.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3okijgrjf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ydnmlioh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ayrawvvp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gbwijvvh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3axzewfnm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zlznyupu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qfhhesfp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pxiohkti.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3lzsuwspk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tccvgoyy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wvpkqhzl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ymcptvbq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fbvptkfw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yniaaxjj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3psadohni.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ewacgbqd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bdyatvlg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3byjevycv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gjaikqqs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3quqzzntp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3meussfxd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3eojdbxqw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ihpdymxm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vpzbeffi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cisobzun.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bvhtylki.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3geloiqrg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3urmxbjex.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3difmjklj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gmlilkrl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fwibnhul.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mtccpxiz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ozumplji.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3iwunybha.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cggcptwb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fzytbmop.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3dqmqbngu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3xwabufvm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zsdyrvlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqlqfnws.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nwquzntu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fralnchs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zecnjclj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3knzhiljw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yosxxyck.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uyypizbh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wismllwq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qhdirtia.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sysrkmry.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ozqulybb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uzzatits.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3erlvcgll.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lwuimlmc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3yhlduhsr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fsxzpofy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lkkxjpgn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3aehfkjfu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xrwadxme.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3daifahfo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ntepawwo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ftvdwoed.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3iktcjqnd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3nayocyfh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vauedkwo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wlikpbdo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vzcktoug.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bbedezai.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hbjnncbg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nzimeeni.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3obyvgwcy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pwzmkvrj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mhnpigoy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jnfyngae.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ssybghej.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bfzhbkth.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3knaowlkw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bzpfwyuo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3aaarwuzp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yljqykdo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wgnkwhlv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3pnnxvjfc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3tqzmclzr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3cpochegg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nyallpvd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dpcfioed.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jzkdtgxn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mojrqhus.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3quuzfwtr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aktnawha.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3imntspme.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3cvurimgb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lxpxorld.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hoqszplu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ezepyhzr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ivpvxdtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmkrgcyo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zijmwjgh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3nwwjyxzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugwrwwfe.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3iomrxebd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3sjlajzct.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kocoaiec.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3przzqvlo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3uvlfjplm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rvbkwxnm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xfudtfxe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ptughckn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vykfjlfe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3akntxauz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3nkjpqobx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ohzmjsfc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jzbhnipc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3obvxljqz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3skstkhkj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fxavxtbj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ijhnvpup.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hbjcbwpb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ikiypaxo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3izjxtocj.html


<!-- 参考信息 -->