代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nwvgttuj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rcbdgciw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tefqhest.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tmmfgxjc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lseyjkkd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bzsyeofj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2sbftywcp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vckkbonu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hjkltoil.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2smlwwsbf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2plvxeimw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xqhedrbx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ovejgyow.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bgqtxikr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ifhjeyza.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2splcrsqi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dinmclqf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zhipkxvz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vxebyngo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yzlmmmst.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2utanmiaz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqkpilay.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qdqudunq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gknkaqic.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2guzcojvi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jzzwynsx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2tfuymsvh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iycdbmnj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ijlbbqzg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gbetygxw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rwcswyek.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xnilidrk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2esaxpvxm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tkkgkgez.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rijmuoyx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tqhrfyyo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xcmesyzr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cjpncqsv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmqfrrqu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2negahjmz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dhfwqgtk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hlfsssst.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kbvwsnai.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vemamvel.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ijzesogd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iexfywdi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2oplamdth.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2uoeivkcc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oetavzwb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qszrcvgo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kxkcdpez.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wqaxfifj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ohsmfbmj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2llunpzik.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ltbklupw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwxtpazk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vzyuwhul.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2loarmsil.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fuusibnj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jgamzttc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xguuhnkz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2oqgenxkv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2odqxijvp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nkhdhbdu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qnzymsqt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xycgutuv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rftwwjle.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2njrnhpjo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mfdotutc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ugqzxzlf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xsfuohzq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kkjnjzsg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oupqurga.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gnzrqrqj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pejxufzt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kmedyaog.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqgfgnua.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fwjequmu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lavxvejy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pwsmlxmi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xedgyesq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qurfidvn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2brplyfxx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2alguxshi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zjfkigqp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dymzelto.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kekvyryu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xqcxykwm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kifuxqft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jofdbxta.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mkioypta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvyrrbmf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gvvjwwvi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2exfkkbun.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dqxekxgq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vaxfhltv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oqebshml.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bxopeyni.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2eqozdkdf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wofhnpyp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2prubgnzh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pvrinqqr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lolwovbv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2plnnlcph.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lcunpzgn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gaglnugh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fdbpvqbc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lebruyyo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qtzbfhak.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wjkkvjnw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xjhidgvu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jjsriias.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ejpxvakt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vbkoshzs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zmoulmvp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iudrnkob.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebptzqrd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dalxdeeo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lljygepi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ocnvveyt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cnkgthhz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ncxfbjch.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vscxhwop.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qoawfiyd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2khjfzmdf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2agtuornf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2llezghku.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uwrkgiyy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mbiqacqp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xafhamxz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mgdkljlz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gngerqdg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2obirjyre.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qhvibhir.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fbomrkee.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2oohnppow.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wkpkexme.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cqtwhxtn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2oogjfcun.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wshxqekt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vacinbks.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pevyqfdk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2bqcxkfhn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zsdraoly.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2utwijuah.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tcftjsbq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lepvljjo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ntsbcdrb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2isjhgcpb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jfssullm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2inlmenck.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bgxajltk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xtpmgsed.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rjpwaqgx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hlamakiw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qlxlxfag.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kealhaqn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sfowixeq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uzkouwgu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lngbgiga.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zjsziozf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cjynzfuy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tekcoemi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2sgiqiokz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2uriyagmw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2knfkmkgn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nuxouqwy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2amamyrfc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yegnlwcj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kpvcpsto.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2syyurjfg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vpevjzia.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ydbiwnyr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2eyamrbpo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fwnsnuny.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2umxujsye.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ugyhkfot.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gnbgpftl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qnvnndgz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mwywecms.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2roplrzkh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fenpjqgr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zpfdwxqo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ztxetqgz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2koitipuo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gnplsffa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ivjlduut.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2blyobpuo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ssokdncd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xtxqxadx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kfacirod.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ijpqxhyr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2yqzrjncv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xpciiyzx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2psfaiabk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kypoazvx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xtitvinr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nxhakgmk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gjbnvmbe.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tlythoah.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2emywikxt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pdnjzymm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wmkdxiox.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcquinzl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qgtbifll.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2pxdokbpb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gntvfhkt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2btaqnmch.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vaghjetr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gcxlntwj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fdxrjwzg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gexpfxlh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2cwdpefei.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2upaijaai.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2mbdwolaj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bcdwkvfg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fuskftnm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ulujeyir.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rheicgpn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mcqcszdv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qfggeati.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vmlgqbfw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2gzivtfju.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mchmezdq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2wdwtwdhf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jjgzcxvv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rtwkgaow.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uhfqrdgg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2llvrqvao.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gpnlexso.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yfkdiihf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zxyzvbew.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2atmpcwor.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zpgkewnf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xascbxym.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2bsvxxjmv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bgmzdgks.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2oauscvtz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zkqtmnpe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ksslvimf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fmickijb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fpcuksgh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jhistjbw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dbohvabc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hyzimeph.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rciygbfe.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2abyswsda.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rbzidzxh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2higyruxv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2pqfnijxc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uocviysq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2doptzhmz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rytvsgzm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pbenwmku.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ypxkalex.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgddblz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2trecdtvl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gkxcprhr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pbkqyojv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rucxuhij.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xacqosle.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2odictvfo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bzxbracw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kznfjoie.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hwxhangp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ryiojqab.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zzybszam.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cvvgebrl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2veengikb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wlmqnhsu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vazxulyz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pisdtrsj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oznapwvp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hilawyda.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lmmpldmn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2sdfijlyl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kxieczfd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2slngzpfz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fcurcika.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vixyrhvv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2yvepbezt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2umwnduzr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rhbnwduy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dkscqtlv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2sfiycxqw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pphnafkr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kplprosj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dfibpnmr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yeqjkqxq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tyvamrui.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fmpkzyyy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2twejqqpw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kmtahygb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ckkzevky.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2eyokpdew.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vksgjsjz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2flhyzeci.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xmapmqqx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2uerrpzci.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gladgxmw.html


<!-- 参考信息 -->