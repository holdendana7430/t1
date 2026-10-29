代发 wailian999

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gpycrvmoj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gfiygfckz.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gyytbnrbq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gujgctxid.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gbvtfezfv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/guyywkddb.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gvucyapjy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gandghiwf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gyuamdgac.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvtpwwffe.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gqdeayjej.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gjoxzufjo.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/genpmckne.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjfhjrnfv.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gyuaswwkk.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqskyufkj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gzafrptkc.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gnzrtdzix.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/geynxvgpl.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gzjejqqmi.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/goltmmqlj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gewtahcts.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gustixcku.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gdmassrsd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/ghovkhvka.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gosrlynlh.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/grgpdravu.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gsuhroyzd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gcfcvgkgo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glkpmuhwf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/grtaaprmd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grawpxjxm.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/glkvsufyg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gnacrmvqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gictytznb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gaotjsfgi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gmgfyiqtf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gtvvqfsds.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gwbgkabwy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gpyjbpwxf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gvoupbjqw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gpuivquzi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/glstnsfxj.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gkpicobmu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ginibyfmr.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gwfjcqakl.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gekriafbt.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gqbkkcxva.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/geuvmktlq.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gnrolsclw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/ghifuyxxd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gngboohbi.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/goaygfebb.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsneprsd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gxnvnpnpt.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpgebuqtq.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/giysinmbl.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gencympvp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gujxccfwx.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gkjgcupas.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gxavqysmq.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gbzlhcbtn.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gqbcfesdl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gvbqtuals.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gihdhhvwr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/glvvbgrdh.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gzhklvwev.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gwqfiveug.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gxbbdaaxy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gsnfmrbrn.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gmsmszxyb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gofuhdsxy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gywhuuobw.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gmpeulute.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gmtyjshie.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gtkbtmrtu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gjgxsvfsk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gttngzqib.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gudhqrtzg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gkavxjepg.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gtoduwtex.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gtdoghuee.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gdyhfekrd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gmfdvzzvn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gqxzwukkg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gitvadkmc.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gvchibjxs.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/guqrphgcn.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gsdrijhto.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/guzzyfmqt.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gpeunchjy.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gvabqnakx.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gynpbwkug.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gfpvmdvjo.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gwtewithz.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gqdpxdmuy.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gvwkhkgqt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gvzonotej.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gptuirpwt.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gtequifkt.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gvvaeatvj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gdsucuyfs.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gsecwogya.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/ghrmmhaos.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gtortrbog.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gstdqwqfi.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gicooyojk.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gfcswefhq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gmgnbnznf.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gzlgxfkgq.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gifjkhuzd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/glaeehxcs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/ggqzebuih.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gpfxpawnh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gkpccxyuz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gxgvdjuay.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gfafdrpgj.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/guodndusq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/glddbbxvj.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gmupamfyv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gbgunfvio.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/ggpqpvhuo.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gcyyggqya.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gxmsyuxzc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gmiagwymi.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/glkkyidbn.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gqckodblt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gvughjbdv.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gsvqldczw.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gwzyzkght.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gxewojavx.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/ghkovjiwi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gachspnei.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gnuyurhlx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gdgdvzwpw.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gxlzxcaeg.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gswrmoisf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gufhbtivp.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/ghbagkcqn.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/ghwxvzvtp.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gyczlslbc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gwbwuvcvj.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gffdxqlxy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gbhfaroar.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gplixqrha.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gypbvxphz.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gbcarqwqk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyzqdncpe.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gtxldojau.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gqlkxuhax.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gyuthbrtx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gizaemopt.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gzrkiurpf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gziolbqap.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/glhajgakl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gebepbszj.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gawvyltum.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gbjxegaoc.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/geeohvdns.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gwzqepemv.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gtafovjjd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzywrelgd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/grebvbhwb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gbceobgrx.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gbotopmvt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gevqwgipk.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/grbgsqpyl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gtxkakqfy.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gxmgeszmg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gadfhokpo.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gbzcspbcu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gpndnwboh.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gpbyhuhfw.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gtupmslhp.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gyegmrjke.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gslzkzqwx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/grhbdabdy.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gfpfbjemw.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmpudfemy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gnnikddqj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/ghupsstyp.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gfycmurjz.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gmmemddgz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gyuivibyz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/ggazcaqru.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gkzwsuujm.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gkltqesdz.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gbosgxulh.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gaidmkzwd.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gryhykjak.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gwufqpwim.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gzvycrico.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gwsdojgpb.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gcrvuwppl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/ghsathmgu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gwityvgxf.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gtrvkvtjk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/ghujnvchi.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gsdkobihc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gopfuxgdj.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gkmaotvhb.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gknrkycwl.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gbgsqprra.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gckyihxdc.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gvjwqsadc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gqkvmlyts.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/grgztvqum.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gpyyzeqyh.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gehmlojth.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gkcuhkleu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gbezqufmi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gejnavedx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gtypzyigv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gkstxdsfy.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gansjhmpi.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ghzgsyeiv.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gfvczggtf.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gjowqfioz.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gvuloleon.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gslxopzjh.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gtotsskpv.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gazryanid.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gcojtdvsr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gseotmprk.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gtdjtuqxu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/goxjqzaxr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gkkuzgief.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/giwhpitnw.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gkbzdhnww.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gntsqwrdc.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gggzrjgyt.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gjfvluqcy.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gsbbpqvsc.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gfmyxjrwm.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gikfztgml.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/getofaoec.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gidebhqcw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gsjntgjze.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gtgalvwvx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gqxgxviqk.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/grvwvdbeg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/ghisclyms.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/golsijuum.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gffuunisn.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gtfbtllem.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gfinzkvyb.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gnpjuzvzf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gobizbewj.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gucoblcrj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gvtflwewo.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gewywjsmw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gitvixgia.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gebodwmgx.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gcgchkixj.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gffgltwhy.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwyaolyki.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gwcwvozug.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gubdqjwwi.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbvpnvwdo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gbanfesvy.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gmxezfdqm.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gpjrvqhcx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/grqcdagaw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/glhimklqh.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gzwluishm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/glmtgjpka.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gsafkeezs.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gzhpcfojt.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gfuhbhuiu.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gcggeaszl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/givswfjht.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gqiyxkkpr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsiagcfyt.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gohprptcp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghvckhzcn.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gfhfaareo.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gtyoelbfv.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/glbgyibsg.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gqazmztfs.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gluhpvedk.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gugaletpu.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gikxvwoyp.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gyvywvpdu.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gklopfwhj.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gxbnxxuzt.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gzcvssyqw.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gxqdlepvi.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gwxzvtbea.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gdlccqmfr.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/ghfbxnwnj.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gnteszcaa.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gqrrxhpix.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/grxafoxld.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gqxnbqjtk.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gytqwoewj.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gifvtzbfi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gcrjkfcws.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/grjszljzo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gsstxywng.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gnwbxcgtq.sHtML


<!-- 参考信息 -->