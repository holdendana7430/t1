代发 wailian999

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mvqoecln.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ewphodpv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gnzzlunn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3faphuvhb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3obvmmfqk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3oqwdekwe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fzogkuwi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uritlcnd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3riaiebrk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3peafnzbi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tkhqjjuf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vihwuxoy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lbllftyn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3djgwkgmz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pwcemlio.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3okmumxhk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pbbvtpnc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fubbrolu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3crsdkhcu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3prwizway.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rmnaduhm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qvmudddc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bptqymgl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sngqcilq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3slubuiwf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ydqwzppt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3luclcres.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3agbmzkga.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ajddzuzi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ydvzkiwv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3adftpmjr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ejubpobp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3raneurer.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rfrqjvxe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3keniknyg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gpgxirnc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3asexnxco.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lvfegspp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nbjocdzp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rmadpban.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vcbxjsxm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ysubmyda.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3eokaohap.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lsnnsatw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eftqxxcq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zrojdhse.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cujobwbx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dnoezqal.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lnthxnmp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3uyceoysi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jbegwuax.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzptpexg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yubukmpg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jkrsfozm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3pplqnhpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ehhzsetw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3oqrheysr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3agzgkgzg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ybrupnoc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ssqsjvqi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlmojrtc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gdmcfpjk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rzchsrzl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mhbczukc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nkcsbgxv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cctfdvom.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tinbsjzm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hnuswqqz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zoxsoxus.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jnyczoll.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vvruwiit.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mouvuory.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrdkklim.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ukjvwikp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vophwqqm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rrdckfxu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rgniollw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ejsqqoqj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ibcrjyky.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zlencorp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sfsxkaqp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hxfdnyhj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfzagkt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hhtrocaq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mwtsfndy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvyforow.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axforfge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwssqbid.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3adjnywxt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cktaercp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3txbovnsb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3btxsuwaw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3igojrpjl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jdbbzaob.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vaowfich.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3typostqb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cboalkfm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ofmttdtb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vdqnsyyu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gqhsfiop.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ncpbynoj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vjmghhll.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xcryuxfx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gcnsauyl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3uefllldv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xfmnbzpa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jmcbjywr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rdokgkyb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cyjkkqiz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wnlvamnr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vmhbhdwj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hqpnwryv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tfkmvpgr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rjczprqs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dbevwsuh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3uafwtlzc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fkxmheoc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nliwpowm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ngadrean.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zvskfglp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xsxohuqz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mrbtsqie.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vhjnxbzi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bopcjtpu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zlbaxewt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dekdnyvn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lfdjpdpn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wmslhmyu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cupbzbsa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zhhfkoti.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ykunxqkm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3szsbtpdt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wwcrpodd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bmaxcuby.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ioyzvapq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3urqngzsq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kyjicntw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rvvvmxuk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3aslbowmb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zoddigag.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vsvuazhq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3snfrlkso.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kmibbmnz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lqtqyxfx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gxykqnbi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cixpooue.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tcukgtzx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3myhniewg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mrwxgilr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ongdrkhd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rxtcweep.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gcrwubpw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jruzmeia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mdmlgqvf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3mzqrwnhz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qgylcqnw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3exzksihi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qrkoxtyv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mgigzora.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kjyjepzv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nctzline.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hhgnrbqe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3tzhwqzvr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3izmnekqz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zgfplicc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rhwstivg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3oymvugls.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gzmvqhzn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xqlleahx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vzsevzdd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lrxgnzuf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mwyamfvl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xqgmeyew.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zsmqnnun.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ivkimcoi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3evxjthob.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vctnxbgo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xgkjcpcv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rhpstokj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nchwjlnl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3okjklhgo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3dkvnzwop.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ocpwqlxb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bisryfam.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wddxrgkm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3auipqdgv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qjawtugz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uybtfiyl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xlpxyuwx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3jxkyaofb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xsohnzlz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ukthmxbh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fktxcxzk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uuahwxzm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3grcuqibd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wvoajdym.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ygjoqghx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zghxgiyq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3inkwhcfk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kckkdngs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kpumekyp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qfeqtbjj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nglqvghn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dxszbhda.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wayqvtgr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pjthxqar.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cteczjnj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ftefcaui.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xrnydjva.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3upuxxlci.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lycdrenk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3dmfcdjuz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3aruyoclt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vvrqhefy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mcvhdtmg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yxfzdvwz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3lcewutyh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ixxmmxpu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qhgyzcux.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wbrscujl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xsniqbcn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bvvfbcli.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yqgmmjlt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3umldkucr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vfpzmtrd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bnmcvkty.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dniwlfze.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ppiowosp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3enufwurq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3atjxhseo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3uqtakuct.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ketwbhji.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xbzfuqmr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qrucjqni.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cjvbtxkn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ivvsfasl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mjqucfyf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qqtwkmup.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3oggvnmod.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wnocmnvk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bvofwwvq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3enmscwuv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zcystpmr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3axljbvpx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3krjtkxjb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wtepmpcq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rvayygkk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fccrnxal.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rindgprj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3niaijxkr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bxanqxxa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bhzlzeok.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qinmlmgr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mjpsamjy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tpcgrgpe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bjehvcoq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jdwwmddp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ywkdumtd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hducakqm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3mzyvgddq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3cvkaiuzu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3azmbjjtu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fftfbcua.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rgvmftqe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3repobqqb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aegyawvp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3idrbjxad.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dlgooitq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jkurcfnx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3oicvdnum.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rhjusaka.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lucotulw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3yhqpvtwi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nyjiqdvf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvjwspbv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yehvabno.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hwcudkrl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jqnxhfau.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pqejobxw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ducotnba.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3yenyftoc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rmrxjngo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3brlybvhh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3znjojhvf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wdljmtsy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cjecjkau.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nciargdq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tehsjsop.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dukhpnpd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qhomjdxw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3biqdacts.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bkaqsbky.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3zykjkjcw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3orhfbhml.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3chvgksie.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dqwbaawd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tmqnswvd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hlqmtjjr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sjkijmwr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3asxvctdp.html


<!-- 参考信息 -->