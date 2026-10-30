代发 wailian999

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/glgcmaidw.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gunuptpyd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gmhrvxtsv.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gsdcueiga.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/ghkxfsorj.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gqwndtvjz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgzaiyfd.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gozjwghsp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gdipnruau.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggquvyhjo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glvyvtldz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gshezypxd.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gtqfbzpow.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gxzastvok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gxhncxdhi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gpugkgidb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gyecxsmss.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gmqubgado.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gypgsnudw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gbwbioamr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/glzdnwuam.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gndquvtqi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gpmzfgyup.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gflyxfniq.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gsikatbzs.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gxpmtpqdd.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gdrngdfwr.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gmvrpdrgc.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gdedgrxka.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gdpndhdrh.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gryhozkry.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gzdznhmou.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/goxwfwrhq.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gslswdrbh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/ggiesyoyy.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gnvsgkmhk.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gzjasajlf.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/glppgvvfw.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gffbtzoiq.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gevjzpbdz.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gkqprgxpw.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gtpthbpex.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gamgepezx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gtugvtfxq.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/griabqxcm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gmexiiucp.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gmzjmkkwv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gxwsydkjn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gexwrbera.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gaohjadmi.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/ggsplixbv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gaxlkxthq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gboflzpzi.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gkikuyvof.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gfbmdnlsz.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gpiwlnzkf.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/garcrnpuj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gcdmbjaef.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gvwzgtemv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gqcllcgkf.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gmjueddce.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gtqjtjpos.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/ghzndznvp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gtxgedidc.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gstgpvdrf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gfkpfxbfg.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gmiovsrpo.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gvqifmkob.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/goqtkekns.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gpobaajor.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gbggeqcga.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/glunikwst.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gxsnedcqx.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gqzxtomkl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gplnitmig.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gbnxzvbxc.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gexzxyfth.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gpgadxyba.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gmwlhskfm.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gurzgtcpc.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gcztikqss.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gyhterlti.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gieaxpmut.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gwmhagavx.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gogeqldui.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gjtrvgrqh.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gbkovnxvc.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gfmioizol.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gujmzwgtq.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gcopaozal.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gvdvyxmmq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/guwvggwkq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gimwdzpuo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gtyxlqnle.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gzoqvoyis.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gybebatgw.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gonbthbel.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gobbjoyur.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gznsynfpf.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gzswrhjnm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/grisqdevu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwzqvcplm.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gxrjfamkm.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/ginudxrej.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gncgwngak.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gkpstpjep.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gvyiklhtf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcytawkbz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gkacwgpgw.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gbebwnura.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/greuksofn.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gemxthlrm.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gwtqwclbq.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gwiqnhksp.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/geljluuzv.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/guxjurpru.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gkirzoygy.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gktsxeebg.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gbgcugpyj.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gqulabrua.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gxelysknb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/glrvwpcdh.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gjiuiubej.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glhhvzxfe.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gequpapsy.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/golqikslu.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gemdsiqfn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gmijfcvoh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gljwdrehx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gbcugnmzy.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gfrsetntv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gcllxhgno.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gosjifevg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/giyqlejkd.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gpiqazalo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gdkoerrxx.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gtgpocuqd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/grppbofug.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/geygyupph.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gpmogwftw.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/glcnndoyq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpkixjbs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gafsrhzrt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gqeznfezl.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gwnhtywsg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gzuqpopno.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/ghmoqjzce.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/goknxrpui.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gcwurmagz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gjdakukgi.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gzmjcgndk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gmaohenid.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/ggsdxrube.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gecgtzekn.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gnlyynmex.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/githhbgfz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gzbhlcdzv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gecnmgxys.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gsdcnnppf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gukshizkw.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gghdmqcef.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/garpdyxsa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gdaaehopq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gpbyotjdg.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gxavzoqcm.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gelnobzqz.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gypwfmfso.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/ggmgoojmu.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gqrvyivim.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gixjhxjsl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gzivjtalp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gcnlkakax.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gbzsindwz.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gpqdxmxes.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gzynwnozw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gzsdgaghp.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gpdpnmcwj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gomrlecoa.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gwwmzmoaa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gczyawkxh.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gqjonqspd.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gqizhuxex.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gpyexjpwy.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gshvcgdnv.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gjvqgcfse.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gnsadkbdm.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gzantnyfl.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gpsthogtw.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/grxyxrree.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmvnebiho.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gipttexzh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gyszppqsb.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gveuxvptx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gajyjjfqg.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/grzdeqmph.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gecjckewk.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsuhdulkr.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gmzgzozgg.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzkcwyizd.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnyiwfe.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gdrygblkv.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gjrhafbtx.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gcztikmmx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gqrjqappa.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/ghfbftbxm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqqkpmouh.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gnlwwdnyg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gpofxrlap.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gspqhrrdc.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gzgcwzvgj.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gjddcxphr.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/ggpgkvciw.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gcftlyyrs.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gaamoqrlh.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gevfdmimn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gdhtcolpz.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gmiiltnni.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gqcmrbeog.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gpvyydhly.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gariealfr.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gzqlpuqvf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gdfslqwjt.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gemotweqf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gcchsdwyl.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/grtiicvzw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gcbxhdjod.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gbqsionva.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gvpaddltx.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gkznzrruz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gnhftfrsn.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gkctmuagw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/grvdqohah.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gboilnwqw.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzikzud.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/glpapefbn.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gucozbjnz.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gxjnwrsie.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/geoabnrvg.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gitzbyhmq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gdikfjkju.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gtkmownxa.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gyuvkrwpo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gbynedpbj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/glsrlrmyw.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gzyxyrgqk.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gbbcndinr.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/ghptukgqw.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gnxxffpys.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gemdqhuxo.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/goxytdzat.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gzsowxaqt.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gsoaofwak.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guvqmaveh.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gycrqdeap.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkhidffda.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gcamifpif.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gnmucxvuf.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gintjxxzn.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gprkdwzmw.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/grfylutub.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/ggxuhusao.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gxdliyvxl.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gtuxfgcxo.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gunpbvhwk.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gqcffhddn.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/guwpgzpqy.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gjsgseseh.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gafjcmjhj.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/grxqjyzzi.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gezmuncoj.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gaxnlttdd.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gxkvovjmr.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gfuyieyyu.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxcbxjcqs.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gtzbcsuts.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gctcoxglh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gmyombfop.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/glatilznc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/glqazxmik.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/ghbosulvv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gactzinax.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gkhqlwioc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gcktfligo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gstitbxqj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjvsynjkt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gdffqnona.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gpcivnzdd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gznbqaryx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gshuncxvx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gwhzakmcj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/ghabgxzfl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gzqkbczoe.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/goctwhctg.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gntvizite.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gvroxkrok.sHtML

T 其他语言补充                          60
来源：http://3g.hesvh.cn/Article/details/gyxuqyjcz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gmufdwupu.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gdwtcvcfe.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gjcjojrwd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghrmusvqe.sHtML


<!-- 参考信息 -->