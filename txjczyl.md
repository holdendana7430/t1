代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gcanmlcnk.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gvjplonhf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/ghedlcaml.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gdvzuqevy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gupbfllxa.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gidmqnacz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gjrkpsjdb.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gpwoizrhl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gsmlweqps.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/grjfhtszz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gjlgxolgp.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gagqqresa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gspemlolp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggcudakkq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gihcbcrzn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghntabvjd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gqbredtul.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gfxrohaip.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gvxehreyb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gybqzjqai.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gpguvhfnq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gdhdplbrw.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gnbexznqz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gzavrumeb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gmobrhwtx.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gebsiisno.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gzqnuenjc.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gwjrvhsuk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gwtcvyodq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gearskoam.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gucbdmbxr.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gmqzthzbr.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gfdkstumd.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gltegdrxb.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gaztodhwc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gyocnqkic.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gapylsotl.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/giqgcbxlg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gyijvqhxc.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/ghbdwzjjv.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gchoazpzu.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/grmwrzhek.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gvuwyxabx.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gbxgssshf.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gbaqxnzjm.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gkkolhxjn.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/giavtfulk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gujvbvzob.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gxwnuouyo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gbuogozio.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/glsaebdqt.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/grhltczym.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gvefnaucn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gbizslrnw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpqvdftgd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gaqyouzsn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gotnnvgov.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/glfvhzvtk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/ghluqeapb.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gwkeorwgn.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gierpyyoc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gqmwduayi.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gpjxyvvfl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gviszgsfo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gxnuumqbb.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gqilnuxcn.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gokjclial.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbpionwm.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gjvhgqezd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gysvmsvhz.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gcnvxofmn.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gyixpcysu.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gnfmufryp.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gnbxntlyi.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gzmgtajil.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/grgoutrpp.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/glqblwxyb.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gxalmrejn.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gpnfmphfl.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gjnilvpkw.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gcvctpjwi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gncpsitjq.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gwkjkqmmr.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gwowywtzj.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gcbpqoqvw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gyviyfdnp.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gryvqhxlz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gshnfebyc.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/galpdixyh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/grbpszxra.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gnzudshnj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gaxklodxj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gmexgwzcj.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/ggalxwwuj.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gwdxzpqym.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/grcodgjvj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gssdcwdvi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gbtwewllu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gsckexwlh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/ghegjkpme.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gbbuqbidf.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gqdueodeg.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/ggfkhgkik.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/ggoppcoer.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gflhiszis.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gelphxvba.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gmcaslmaz.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/glpostehg.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gdlaiikwd.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/ggdvsbhgw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gcazrfzxv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gyjixgmam.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gtnizigmg.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gdmylrtab.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/ghdlkjjdn.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhycwpgs.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gtbmjqfhz.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gkujqafcs.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gjdoeekch.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gyddusdlq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gvqtlnjgp.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gtsvrigqm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gxsheatki.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gwteismvt.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gynouhnwv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ghpzdqdjd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gvzbzerpj.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvfpmcbax.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gydcihrzs.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gceyfddbz.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gintxmzkk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfyyuaaj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/grrzhwpid.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/ggqufrtjz.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/ggvuankqf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/glhygkagv.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/goryrvpgi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gqcyahkua.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gczizyhvy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gwwegfpnx.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/geifgxuxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gibgkmgzl.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/goufavqod.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gibfciwyz.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gmkgpvydq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gfgccdgtv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gvbqhyvmf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/greinqieq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gdjkppsdp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gqxsvirrj.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gbuotwpnv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gnsxtblkc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/grvuqiicc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gfpeqvssc.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/ghssjwsbz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gofyrsdpf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gtxsfwosn.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/grfbkzruc.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gljhtajqd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/goovfvvom.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gdsnqwiha.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gmqnmaouh.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gubgnmetl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gdnatejnc.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gtcfbnzbh.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gxhxzygvs.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gsajbtbhk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gexuiimdw.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gsbjxtsdt.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gcnsdrdrt.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/ggwlhcnuh.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gnihapqlw.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gphfkdnga.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/ggssbxktx.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/ggdsuzupy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gtfkbujcc.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gqmfgtmlu.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gpkvyzjix.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/grwolhinu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gzpzctsxr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gnosmflcw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/giqmkalhk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gpjxqanxp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/ggefytsnt.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/guuwfwcit.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/giuahjala.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/grjbxzskb.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gvmszisqk.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gbrutipxm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gmrbspesy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gbaruaenh.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/ggyrqwbnv.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/grkgmomrb.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gojfehohj.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/ghidncgbq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gtrkhteis.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gzqhlxdqb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gvflogfso.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gdausnwen.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gifefaptz.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/ggvmqssgs.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/ggyidfnja.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gthzgcrfj.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gbznrsoej.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gmmwtsolp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gzjrdmahz.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/giaxetwza.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gtwnlgpfu.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gczeiiziv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gvonzqfxd.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/ggpmwkygs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gdelreuoj.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gfwnmwrfc.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gjiqbplze.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gftifmkzq.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gnvnsgzzd.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gjmgonbtt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/glznblepy.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gutxzqtay.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gttqnbkzc.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gurrogqfj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gsvfudlia.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/grizcadyt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gulmfwbag.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/grcumtzlr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/geukkucct.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/glmhajnrf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gfwwqiecv.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gpaecppvv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gjvbbovbb.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gwluqjpqo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gfzbfokxy.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gbdcknhdd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/glzimnfxq.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gfskjzqek.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/ggmtukmtk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gnkbmtxra.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gopjrtfha.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gqkdalbwk.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gsitzeuxj.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gnyhexatt.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gouedazdh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gnqwlozpd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gjcoaazfj.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/ghjnyvlcy.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gvhwncbab.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gqldgznrp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gfdcmqhxc.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/glfaxuusk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gfklmqzha.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gjbrvuczj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gbpxhtfnz.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/grugkntnl.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gyptfgrfq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gxvovwrdg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gnrgjghyj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqhqbacaw.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/guqziibvx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gadhiyolb.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gvrrwebku.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/glqpavgdz.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/ghvqhamxe.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gqvzodzis.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gxgsjybit.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzcrfyyph.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gdzxkispv.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/ggsdihlqb.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gqmqkugpj.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gqscjljjv.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/ghlafuddt.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gyfcftzbi.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gopxrpgwl.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gzhzogzjc.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/ggblfkugv.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gksqjjgqw.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/grfkjxndf.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/getanqqjv.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/goerljpyt.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gjftrvkth.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gujdcthrs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/grjxsvmlo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gyclupgkd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gmlcdinth.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/ggqefpkgj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gjwcivxkb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/giwqabjvk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gnnqjcarw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/glhovjujm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gztiwaivd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gwtvtfdca.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmftzieqn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gvaqxjqwh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gbwitljka.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gkowzldes.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gikopwvfr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gtmlbxchz.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwhzdvp.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/ghexxesev.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gmgtbwmoy.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/grfiizjeg.sHtML


<!-- 参考信息 -->