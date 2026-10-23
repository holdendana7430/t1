代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3diyxrsxm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ubahkjba.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fungmbiz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cgmbvosm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xacizvaq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qzwqotuu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dqdrzbqo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vqwnomiz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rnsfcibv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lfcgtlej.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gxedskoc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lejcdpgr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ilemkmeh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mleelunx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yeqdtrns.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sibkafxk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3eysdgkcc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3nhuudtmd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3eelfulbz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3segtxcqt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dbkrglky.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dnmljpxs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lmwegclc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwutskao.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ovikeawo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uuryukiw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xzjnfhci.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ljrogjug.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sjrttxkx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfwwteou.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3axslhmxs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bqflfmne.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qldothba.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jkpwfgls.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uznxhvkq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hteqqequ.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sweprblb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uwflwjkm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3glemmele.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3iaynaspi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxrkdgsu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pwixllkk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gtwshkce.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxxpzcp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kbatfdtt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lfqjknmd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3gkvdcbrl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krmnrxbx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iannssvs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdshuwyg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3latswugf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3drfiehpl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jqnzitqa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dbzopnrr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bbixvfup.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lfbbctyz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sxchcwtd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jullcyqx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3viwfoswi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hickjbfw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ejfhreun.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kgwiwvad.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pdglagxt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bvlsmeio.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bnkaasgu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tiyqydjt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3arwmbchh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3enjfkmqu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ichdiden.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3llrjtqya.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlallaba.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3lifqjtja.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ywafiqbx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ahscddbt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3oeoosdxg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yzooufan.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zxgutizk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gotrxqwx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3akynzeqr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3idihgjpj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kpyslxtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuqprblx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zbsrnrii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhiidxbv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3macuhpvl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zmmhvtro.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3prbujeif.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kkaerhem.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vybtybpc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3riuwjhic.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xblsdwjo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3enpxbyml.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zxlaiunc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3byyoystj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3znbpysxw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jqentefe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3aybnugvt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3esqppkep.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3miobzbxz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3filbdzkf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kkbpovee.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3amnrlere.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rheawqjn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cjvjyync.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pmahxdcl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pigxhtqz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jqirmqul.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldctsfhv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3brwjolhl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kjrqhxbb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bhaighgd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmcopri.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ztuywyyu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hbcsvwfm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ecwoabiv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tsihqgqv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ysrzvjlp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hjibrrtm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3teztpoer.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vnepepcg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ueazywde.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnruzjwz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ikaarfbq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vpswjcwz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hbltkpqf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3efyimgqx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gqybghnw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qzdhhblg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pwsfvoad.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bvzldrqm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ygusdeqc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bwxbsahm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ciizqppx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ewgiswbh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3uauddyvu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qnunemth.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ipjgjvfb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lbltbxji.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3atehlrdh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lthuavur.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3sjobfrfk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gbjgahmj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3avluzqef.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjizwec.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zcolpsqf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wvuonbma.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wllbwhkr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qubfjsbk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3neigilph.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pqzodbvl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tbmzqbji.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ysszfjsd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qwzwouve.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgwmlt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mcgfkjna.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgdhixx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dnhgvsjy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vmxdcvln.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kaekmlqn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yidcvvol.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3glrjnjsk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3soewsiem.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wutvnizm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufnvljhm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lfwfbmfb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3knetxsyb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3koozaxuy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qznlvpvm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ldsdpeam.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gubztqzu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gabmrykh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wpgjlmhq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3thgiykle.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zupzldfh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gvmqfhoi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3nrjbvvkg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vndanuar.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mlgfnruf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dsbehqqz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3enfeggor.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3pdugyqqd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fvnrkxcb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3uipyhcdk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kmwlkzdx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jhbtojgx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nrdreeig.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3izoqdlcb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tnugwzwi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qcatbvab.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jxhixygu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3auvcvnci.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xsizasnt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3imupxydk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bxslxdct.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ydfhikmw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyhjwswg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fzhekdgp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpiatfpf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rjotuxoh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3uadrpzvf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nlwqmtde.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfyslbyw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lnjomjmy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mdhayxbd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3eqmgwwiq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nultmdci.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zujegjzh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wuuivjvu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3iozorizq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mymxfjke.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zvkhtnbw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wvmetxvi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ambvqsfd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wveowfzx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ynryuhoe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mnfkdvmd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lmwqdpye.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hiyikfhd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3crnkrdpq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eedvwnci.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rgxbkyuu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bycrcumm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zbzzdrid.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mlimtwxa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3swxvpvcf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ptlgypib.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3amquiwrq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3idwiqyrg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qzkwpitt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nocxagwp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jtlcafzq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tsffsujh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3psbxtqly.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3trotrmvm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3yyfadtau.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ynhrquha.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3isxwddle.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3venxrtsx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xhtxrqrx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ycyuznjw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bkvtplvx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3euipkpfy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sxrmflbr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3scrlgtrt.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kaegujex.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dfkwaooj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hnlolllq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rmhzdakp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3grqlrxzq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3awjxepbe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hmhybgxd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3egimfohp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3awahonep.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tvftzvfc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3anicjeee.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3aznnzivp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tcogywqi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bkveevrz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sqvbgave.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hgdtrqli.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qyvuygop.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jpcdjtnv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vlchunui.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gepflgsb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lnvvfhyk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3jdwcumtd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qfprubvm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vnwcaeck.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3kinotbtx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3omyojtop.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lrcxzpla.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rnszabub.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mjwknqyn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3awrkskdp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hrxywwaa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qudutvaj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fgpyckqu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ftrwzokd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vcqrsimc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bnjklfnf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3gfmhympp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rkptruay.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3yvepbezo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zkqnedeb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yrpdyjxz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3fyhyqexz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3usoirgnm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xwfwmzhn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fgumuuca.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qqlkcfjl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3dffsplkk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ayeyhomk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3edoacscd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bjiahxrx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kuwambap.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kegvohci.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nqjidvhj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3urycidoq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yewtctjl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3yloclzrn.html


<!-- 参考信息 -->