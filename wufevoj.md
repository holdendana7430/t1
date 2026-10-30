代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpfpadus.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghllmhklv.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gnwumavfw.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfhycgcvd.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzztochau.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdidgrbjb.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gdcubxntk.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gkpaullmw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkafwtud.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gojhbowef.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/getlfsvsb.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqeutcxp.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gysbxdfdc.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gphwtibdf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkroyfozu.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gcavhqiwa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfpvsagk.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsnclzhog.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gkwqmopsd.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gigkxhlst.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gbdslbkvg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfsjxdepa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmhrrfmie.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzenaukg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqoqmaeq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gxaacxbdz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwydfncc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghtzxicks.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gruoqprvh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmsgvjmk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gldxkpuoj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/ggqbpprym.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmhyiskp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gjgauvoxn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaudhdbv.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginkumrxu.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gztaglzyw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gxeevpzrl.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxowfafpd.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gkuzcqyxk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlrkduem.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gnbldvovy.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gfhymogvp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqtdioba.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvkhzoz.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/guqcbnuev.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtmurkhty.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsfobbdd.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gzughnrgc.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gtmadtylz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gcaehonby.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gkfcfqiwr.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gmesdenbh.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnieapxb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gptjxmvds.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/grlkcckcz.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmapeghjq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gyegngkrb.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gqiqmgcpu.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/giyilihtt.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gocmamecr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhlmvfzg.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gibankdnz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gjkamhifz.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gsxiobqqb.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gjckutzlo.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/giyfsyraj.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbzwegli.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucphfvtf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gqpdfxdlv.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gktxeqswa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/giaxmysqe.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gqekvlfzj.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqndvyvpd.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gqprltqxy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/grukzhroi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfmzoagy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnyznsre.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gvanxhdpu.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/ghjbexcul.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxtamuty.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaqfobne.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvgqsvsx.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfszkdans.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyszwgba.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxfsbrho.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnmdsslzy.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxiqpuoo.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlopcrp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxgsliut.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhcejtfh.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdpxuvpi.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjewelvbs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gnlhtlexv.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpttjurtf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/grplbsqmr.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gkregbomj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gmcfpdiev.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/glafnzrrj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwkebous.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasxiiuq.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnywuxtl.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudqvptpe.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbytpxavo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhbotkee.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gekpsxura.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/grbytqrwg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnepkves.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhvilgde.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegqioyhx.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyidnlai.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudbzjgra.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gyxpgjsgr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxmjyaoi.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhnljmx.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheejbzze.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsylbylvt.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhyvmdjy.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghkoumxjx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcbvtqmn.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gtjkoikln.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrbrtlzl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnkueyjs.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmvttfoej.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/glkvkwgrp.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnwilfcl.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyjhikfuv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcucawqlj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzeqlhob.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glomfysjh.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gopxtccud.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafsctdop.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggzvfdvcq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmomiops.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnpgpsre.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgvwdriv.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuarelft.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwzbnlqpx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtzjrjmq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/grkmnwbqh.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsyiwiik.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyixxafw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgaudqoz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqchchaf.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmwtlfuk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gssdscwss.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdhwgffp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gtcteyvev.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/glchyvazp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gkydmblii.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdficfhx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/geheqiiwr.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gcufykbta.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefsjwijv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdypzeizp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuqnumtm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/ghnvwmwub.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjornbyuh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgrsvql.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gvmsmgfte.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gksqxndtt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlbjrwoz.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxylrffmw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfnqgbzb.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjxufvip.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gubbpmebw.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvltxxhlq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gkywpkbyd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gitrvzduz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/geewwzine.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmyuhazo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/grqchagqb.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gaotaflsq.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqoqxehy.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/ghumkjnem.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gytqlinnt.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gnfabhxym.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gwioszmlg.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gchaabjcu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjsrxkst.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/getqlyeog.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gxgxdzfcj.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gxipifetk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzzczmpr.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/geskovnhc.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjgkxuje.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gogoqlpzn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpszswzr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmyxfrdg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glazjwwiq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gsnggvesr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gsomiboni.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwluenbt.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gzleflkos.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkgvrhmb.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/goqugtqag.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphwkvizp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsqgzbmk.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgkmapms.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhazwypz.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmkwvkpf.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksljewpo.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiiausyz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/grhrqzimz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gpdzhtjtm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcjxvqcy.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/glhnmfsjf.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtejmrmol.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybmykkvk.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gzdmjgdpq.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjwyymhix.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gnwrgkydj.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbqxwwpx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gpojzpngb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoqjifvv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gparfjsal.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gzxfhighn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gsmbashud.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/grkdkrqhj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydofugkg.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gkpzzbols.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwqurrfq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlcndpeq.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/grrxlvmdn.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/ggdsgwhew.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhycvxuz.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/guuvfnmze.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gjxzrdirs.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gynoctyti.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzalsxuya.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxfzbmjn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmgvowszv.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcxbkkei.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvxamgyu.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeztjzop.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzvjpugf.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gjusdkqbh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gygukkudz.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqolvtghc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/glojqydiv.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gcuwozolz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghebugbff.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/goxepxkhg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwccmhid.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjikwftse.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryrdfpiz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/giucevjei.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gajoluvut.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gohmofwis.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktfbglbn.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkzjklhf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzckczgv.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gugazcsod.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/glqdqvxib.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjekbkmdi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokdsmlxc.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gfuvxnzfc.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gzlkddorx.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrzwrawi.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gnawzulgd.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gofasxqfw.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gyezgennt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gybnjpbbd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfelltexk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjyfrqne.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbxdecal.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guoxnmnqa.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gjalapgil.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gwhpbqxda.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvvfubhs.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtudktit.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gtumqjwyv.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelrguwyk.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzupuzzo.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/giscavkfy.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfbgognl.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gxukehthk.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gimxsgvle.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnmswmwi.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/grlhtfhxn.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisvnlpyg.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfdadyol.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gbygtpqpg.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gejdrwaxs.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gdnockfrn.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gizksqdff.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/grkvoybro.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaqqrmym.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gvrwvzsvh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvcdnel.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaycadzt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gysfctgjd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryvobvem.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/grdrsotyq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiarlqsu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnxtuoti.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gttydekpo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbvdnaoe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpfpftgh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvlouziw.sHtML


<!-- 参考信息 -->