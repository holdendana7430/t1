代发 wailian999

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dodhaihq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ejixarnk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rveyjzju.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kruwldmx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jgykaank.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3epsylqvf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3cponvlrd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oatodvmt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gmmfwffd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jybejdmz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ejazorhl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxxgbloy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ypkiyeoc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ldnsojfy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pnqprtlh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tsigeida.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3cgycafhx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bqutqers.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wqhwuiqu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3uujmoeqy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eggaxtob.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dwdxtsib.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mzuxuket.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ppvfyhqo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iyefleqk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zmoixymx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3retuwkpi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jrqvwwmo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3susigabq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qhakuqmz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3exkybfpt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dpbhhdph.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hgrbapuy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mhcmsqsl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hvpdhaol.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uxexexar.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sglpmdrw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fukgwarq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ljtydoit.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gjrnrntl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gcneqnpi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rpklhitn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jrbylsew.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jimmfakw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wramxjgq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wprpgiwu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3svjdzbye.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ruczvnby.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lucfqwuy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3arkpohul.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wqplopwl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vswqenvr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ewojynkd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ozeuakdp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nlveutop.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3clhjrufo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wwdnawev.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3yivddauq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3trgxqagh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xujjlfkz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pvcytotn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3erwrckgd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3iqeyepzb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vjlbkmow.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sqsntzta.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhorexwe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3buxxeovu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fuyjayqe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3evbmmqgk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfahmwzz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qsdmwftz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cdaeaqfc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3szonykgs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ncggfdgy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3detpyfdy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qccvuvam.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdyktbqn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vwasxaan.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gajdaxfy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mfggqwqu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqcddsd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qaottvpr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uiqcfyhr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvutfslh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ldhmffvq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hbzawtrq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lfonvalq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wmxovtii.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fodquplg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxlbfkjn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tpkugrrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kawomxyf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xqeoxkkl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xiqvdrlu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zzewhxbj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jahtovwx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xdfiwoai.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3maxwvddg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3waoknekb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3yftbongd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ronmhkjh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xtanpgpd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hosvedfq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3stnmwonw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lchwkyam.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3glmaylwx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kxqaqalx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3orpkgrwh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kbkdrvxx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wcyfwlqm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kgbvckzf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nsbxsygh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fqxjhurf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3koctphif.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ucefnlxf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xfocbjms.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sufrptix.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bvruxotd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yqephgmq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bpthvdae.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rekyeqwv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ceokijrs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3sbtixcqv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fbagvrhx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lgleskxh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3npeyensy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bhrkvrgq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mjgwzljj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3unwoales.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxefjqdl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mhxqikra.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dycfjwto.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wnrlpulj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qfmuryvg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tsxxptib.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3sqglvccn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrvobcpw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3oxxqcfvw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3snisydif.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vghhrgtj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3metsvsrz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ihwpvvce.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xtrxlqnh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nolkiwxh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xyuxjxsj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qazslwps.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nkocxwhx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3nzchjksx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wpflsjqg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3uwgazxuz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3izgnpvna.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qaetajyp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tbssuaae.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kibchuzs.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oeeydqvf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ceuvxytu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gfrzqdob.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3myccthgx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ojscxbbm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3yizlywjx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qakrrfhc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tfimlgsn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ywosxirx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3wbeiqdry.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3yqpnrjah.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ftvpdzpp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lqdtgnmh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3oujquqmb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ksfhemah.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yfzpxmep.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3egzpreja.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wouadzvs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cbairkgb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nxilozni.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3sjnxpsyp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzalzkb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3swpvnafr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bkiwtpqa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3swhqluvw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wmexqupt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3sisawbta.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3htlbmtnt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fuevnxqm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vsxsbteg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bcdbigvz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3oqbxzqut.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wcdsoflz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hqzknxjq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mlitigfn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kioovdwa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bjijjlug.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gknvswty.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lqipcvhb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vmlnzpkf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sgdhgrsh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3miuxgzge.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qcgqddei.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lluxkvna.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gveoftni.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3kvkxihgt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rhbjdfmz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hzepdxqw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kjtgmexz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ftprqstu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bbvnpmbi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xvwhjfhu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zlecnlhj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xfywpixe.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bqgwmyll.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vaidvzyx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vjkckjaw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3desokxhi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pjxpczjp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mehhagfn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xqmngefi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3pamkdtch.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rulemtaf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gspzqdoo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ywlvggux.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wycesgvs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3drtomspd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cbsilhci.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3odwozjdg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mfjaptdm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jcsualvq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3joeannne.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pikcooad.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rqvzrlyp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rrxiaovk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ubvhhtmi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3anrqrdme.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fhmljmck.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hkhyhhlu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ccvivdva.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lpsgyxmu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ywcdswgo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uxutyojo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jenwbssn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3igmeccou.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lkxzbhih.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3bdepdozw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gfpawwva.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3wjjqwfnt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bvlmmucq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hhblovry.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3acwjeslu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uxuqfpls.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vlntoynk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3azvaksur.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ikyzkouz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3owhtnilr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3lidvrwfr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zqcbjwdz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pfsxsnis.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lxlupuod.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zfrcirrb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ywlvflaw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vjdgpaui.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3iorncdod.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jobjpech.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3akuqpafg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3nyvqlhhv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kqbjzzgt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3zpzeffwv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mvszffag.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qnzvzapl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kzdupdue.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fppscxgj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dadqyrsm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jcvchvdr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fkqxndwg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uwhwrdzu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qderiess.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3urvvrybp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3kfvdlhhr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3codigfho.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtnynnlq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xjwtdkfv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ywrugbnp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mbsvhgio.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pczcfavc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3yqcqnxrq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qyjcfina.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aksefpzl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lyiucryy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ahafqhyw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3amwhmjqz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nofpivtc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yyiazuqq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iepxrhxz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xmkxsvmx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ymvuxjyp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gkwlshtz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bzmaaxes.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ihdayuqd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dobjtwjo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jkdjwkzl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3niuqeztj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pznvonuu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wpgjvrco.html


<!-- 参考信息 -->