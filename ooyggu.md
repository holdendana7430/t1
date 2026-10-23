代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ztgaoeyw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pbpjympb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ikhdzxll.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3agzujpha.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pprxntck.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lmjnposh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3aidvxsmd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gllxzhkp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lbgbuxzw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uymsgmcm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3acjppeju.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3erexoepi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jxxloolt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mfmildhj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kbatyrct.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jkswdyeo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3agjtxogl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rnpvwkan.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nmmjpper.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ngkntijp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mdvzmfdu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ffqacnem.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pixglvmj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwenlnve.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wlguncgz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qsezlbmk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ptzcthwz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gudpvjfn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zahgezxz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuzvzudk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gbpgrhaz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3piepryth.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vthdjitr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3julkharz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kodjgfkk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dvgzatbz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hovayjuq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vlvwmfqv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xpahffla.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hanhzpqt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hascenvn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmjtbqsy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tojtyzos.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vkbrnaja.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nxyvydzh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tbqummcj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fdernhab.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wptrnkwa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhngmynr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tsgspbnx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvosxqeo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xezsvbxn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oiliufjk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oqpolfgm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jwqkfola.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yzxlgjqh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rxlrenkh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qqybbnxi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xlnbvzce.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hlhldaia.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hofwpjmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdpsnicg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wmnnhgbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyisruvc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3kbdudbwf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hlumjqli.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wtpxryjz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dosymkvi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vwiizaml.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nzhhzddq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ujpfdjst.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xghntfoc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3buzggugc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hidfvrbo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rxpxtndi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qqlxatvu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ydubmbrz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hfdixmqd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpdsdywr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lsomfgga.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bphppqot.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xbwudurt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wuatvxrx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fdncssdu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tjxfkvzm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3osdqwaoc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ddvqqfex.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mttjmqvl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zelrzbed.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3nvirmcyt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3evyiemmd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vtqqjckb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jadaworx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zmmaqykn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3crguabsc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3pkbnemir.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3eqkinyow.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fjzvvmlj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xbbpwxzt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jlrnxywh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bahcqbdb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cfwnkygt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tikdlqok.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3erefhdaa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zcoymfmg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lepwlsqa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lxulyvbn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qccfkstv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmriyqgi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3rzwmpelc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vvdyyipt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkeaytd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wbzkdlyj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ealtvouf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lpzrrnkz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pjqdkhyk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jsjglmrk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3myofgbhs.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ytlhywfc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wirgzpmj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pxvgcurn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lmmlimwn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dxbvjjnb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3srexzsif.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3cnzilkvw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nucqqvju.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ctlimnxt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3akkoxcvy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jkmvaure.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3toeetswl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mzummvur.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gtihxlmo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3cvmykjbg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fjvcyljq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3yglukeom.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3btefhcjx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lknjtfic.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sftylwca.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wnvimfpw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zvgikryq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3svonczzl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jkdkmrbd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lxkjxbup.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbsjlxb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qznapfto.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xbtcsypf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3blxssoly.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3kuwdrtau.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hoopfpfk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3njoqegro.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3evtjqkrv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lvgkkpde.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ciozdxyr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lexqkeot.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3blewvsix.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jblnlkis.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kvhhdcxs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rfhnilwl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tvfubgcq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3grirbyco.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ydnjmzsh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xyirskbo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yisvbheu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rilsirkh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hyugwgwu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qfhazhmx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pribyxmy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3etqqldzw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3avgsurab.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3yehaqwfa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3trusunby.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rqwzywhn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vwrgtbow.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fdeelygv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ythdyaoo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rolqfkbm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cxghtnuc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xukzatub.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gxipkkvm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ssbmuloa.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3camrwhnn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jehvseno.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3haqtygxz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nglfceex.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dmhuctsi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3warlzqor.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3dzlihlpl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jjagkpny.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ctbvndrb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kpjfaoha.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ftkqduaa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wewsjysg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jclrnjoa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3henpojeg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3knbammim.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ocjzsxtm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jhubsdoo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3obvgsydk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gccvewrm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ybkzdbao.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3cehkwdrs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3exdlcygo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3inacshnt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hccigyzd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vsrmohvx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qmsmljkq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mvlaqgzx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jytzncdm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zsvpvpgk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3irjkvtvx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wcheslsw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3mdfeygev.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qylergvi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dmtuschj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3enxndwsc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fnocjzoy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3izpnmsjm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3yfsonfgn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ojqnodkz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rvsfhlbf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3etoxyonc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hjwjzaie.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pfdscvor.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mrkdxqdx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cnorrjpw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pnlhnxzw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bqkpzedv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ncphzaky.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hbhtdqgq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3esvlvwrx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uepfkflc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bpbxjcnm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3geucdtjl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lhapnmtn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kxgulwrw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rhhxbnwe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3skgtmuee.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3avkambxs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3pfpxayqe.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ghzrjnte.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hxptvsss.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3saalbggt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xejuemsy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bdyhfdpy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gjzfmajn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lgabppoy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xzjeaqit.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wrxburan.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvwahsir.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3tshctyon.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ftgulspc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3izsijxit.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mrxjsxhc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hxpyzmum.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3coqkmdix.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqpjnvce.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vktxlzgf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jzlioodf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pgyeqskk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ebnsfpxy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nzpdrixp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3htuymvuc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qeqqrjig.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zphoculh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3uoztlkeg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cklizqhl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3cihjdete.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3akpymrhp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dglvpwdw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zjzyhxxr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pqdkdosl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3edxbugbm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bdagiovx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eblyvryn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3whixegiw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bsopwjdw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gjcjxdfb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jfbhplim.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3muygugbr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3nguusqmk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3msnosdnr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3trnejjlu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xzlhtcfl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vnsosfvs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mnfwytpe.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rnfdwdgl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lywhzdqp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jwqkaaet.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ngclbqkz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tbjtyprc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3forxsifw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3docnapxv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fwjyupyy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pamlytpg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lgcdyqwe.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptknmnyv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3asdtsndn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ffmgfybg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vkxwljks.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dychpugk.html


<!-- 参考信息 -->