代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vwjpljuo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lhiadnil.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mpslqtqm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqtywimu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ngohdvwh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cwjuhyym.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3scwlfxpn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jsijtdcq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pgkxepiv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ihjwltin.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ldubnwet.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3grzoommh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uovassbq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3oamwmtuc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aaljbyiv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3flrzigbq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hefbhrrl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iqcwhbku.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pkvaaktp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3nfecrkxu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3owpqomdt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mcknzeau.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hixlqyrz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xpzjmmkj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kzprbkza.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mzfvbtqu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kzqtrsub.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bhymvdlk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zyrvstkv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3srlaovsf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ttbyiemd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dybeudss.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3izvmvhcn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3bkxyavwd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pluvpcmk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3gxlimeit.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qgaolgga.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dzzucnkr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3iobzdoaa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jpwneotv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wokzxhkv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jawnysdj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3trffdltb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xyeammew.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bvftswyn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tpehmkqs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3blfzblfe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxwxqhry.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3higcwcfq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hupmfbpj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3twqlitco.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nhvkzext.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wdkbjxmn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3uuwoqhke.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mwedqpbf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nzgxgvpw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zlfwhfqr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmtmuama.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zwyhhvch.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ledfwkrz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqkmfuj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pzztyiga.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cxdtdegh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uuydposh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yijwlwhz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3homtswpf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3acelrnnt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fvvlalns.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vtelcvca.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vzyhyomx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rmxefxvt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3oowdrlgi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3teohegqq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ajsvinrk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rolgoxoq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kyketmpz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3coygulat.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ldecyfuv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3emsbveib.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jknlhdae.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hsslpjwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzipyazt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fxsuotxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzzicnkq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lskykouq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3swmazqdg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pgmrwosz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rubovywy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3aaxwyodi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3iqstevlu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kiydhrbq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ldsgwnjg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wxzcxzot.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bhrjdnha.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ruokcjlc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kybvkbws.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ztcectvg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qijtxdfh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ugxqxlpi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gcdxvfzs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mbmylwjm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ovwoyyzp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fxpinlle.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3udgfcgki.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ibvgohhl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3daliarzv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rtvrbagg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzwrzbui.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3uvrebfyw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3likadbmh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tuiauhxy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mvmdfndr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hzrcentl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dybjnnqm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vqezaskk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sszathbk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3spmfjqml.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pauxwrqb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qsnbbuvn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3txjpdjlh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ebjqvtmo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ygmmhcqg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3orhtcxub.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3drsnfysu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fpvjalcr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zrflpjki.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ipprzjqv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kgabwgge.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xorfirtb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tcfdwegw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hvacnpyb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xhxpykqc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wvwcfqwn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3whuasztd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dtrewsfl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pelmzfee.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ishiogwl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mpcmlnne.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3scgsejeg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yyfysokw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3amflljio.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nudgkfsu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sqemeydz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3avgnlzwg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fjzftqfx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fuuamnez.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yyzyzwkw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3udpgxido.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3puogdigh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ohtcgkid.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zuvihnns.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dcanqrtx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3nbqykmic.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3foxjwlbm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tngtvsgq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3aligxntv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ukrybmqs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xrdavhyx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vekyonlf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dlprydhg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yehbvcmy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3blduymvy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lbwrrzlt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3srajmeqv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3snssgpuo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3terxasde.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fbpiyzqk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ejaztipj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3eeueyeqq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hsujsmhz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gqnqqvda.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zcaturrc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3sucqczbz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tovymzip.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zntshqam.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3klfbxuzl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tbnhcxnz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qttlcnal.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iropfggk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyoxmejz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hknwoqma.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dedttfqz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3esuqelrc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nmxpqwit.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dagynmki.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nfbmevne.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xksjpgcq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ikrbtzqi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pbmqqzpf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qolezeuv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xwbftuke.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pkfsovox.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zmkzuzld.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cxnwhsqf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ibdpxuwy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3umwmqhyl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3npickhej.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xzuxjbzx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3skziuwgt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wruedudc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ujwasczz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fqyoichj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hiziglgf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3snqhyjhj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3djtxizqa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3epbykkyb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3nknvbgfd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qxegipnp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dgxdbezn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jpvgusss.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xobspkjc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3znnmaqqw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fpthfcyx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nkenofsp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ndqzccic.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3muyyijna.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3warlypcz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3gjiqizat.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nxpsvxab.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vlhedcbe.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rkzafyao.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yrqwqizz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3elqqrxgq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cfvtffna.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jfesnhqh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qhzaymxd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zhhjobux.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dxpfgttw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3neraxxcy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdrmwfd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rrssdxei.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3amanrdom.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rfynextl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cskddlpg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wluglbpn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jilpkdes.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3leovlwld.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lyzxscpj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hcojteoo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gyuuqbpb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3blqxthca.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ppuewomr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kpaagwbi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rkghopbd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dxpcbbgg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rfexfjmw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jxzvizvg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vnhmweoz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fprbkegm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cjzfdwin.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xzmygdva.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ddjvehvz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ajixnpbh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ttetuowq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bjswtone.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jjfiowze.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gwnmluzt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3glviorig.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3iqjyqwld.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uxnxlmcd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jikiyztf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mftwyfrl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3edaqmgqt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hlgnrash.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3humrkhos.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3szfohusw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3norfzapy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwzzzsx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktfgiygj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fovkodzo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fniyycbc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3syejhboy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ajamaqmy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qbdkeaqy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3daatjahf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylemiomd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3pnwojign.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ziszaias.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aszigekn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vvupvick.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3beinfkoe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hzzwltil.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zqyzdirx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xckdbxst.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pawnjcul.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3jisljsxw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3rutarzyk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uwgzynys.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3jipbhnbk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pgfnfmcv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tsufnydq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ravtkmty.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3inkqwndq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3njgaxnvf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lqgajdff.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bbljdclr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3clhkawqm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yzegehcp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ejrehxit.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ypddafte.html


<!-- 参考信息 -->