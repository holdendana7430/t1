代发 wailian999

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3uxbgqjof.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3umvlbdnb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3inxboefp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mpemwrdy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3odsmxmht.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mhccyciz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vnptakwz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vajfnvil.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qizfcrvm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmmsdws.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ulpwbnpk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tktdfkkf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3onweihoy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vicceoxw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eecxcsvv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dvtikxxk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cydobzkq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3reqdehsq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gdgscvtr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vbjrepms.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ixilyoeg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uojguzio.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bdxmgxkv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3utvxhyry.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sbwuussz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cpynorja.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bpgfzcyp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mnhikqqp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sajfsurk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yqwhtlcq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qhpmrdpg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3iieobbpo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3habfyfcg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bumrcmvk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3emmekkyj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uncxemrt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mqxuziut.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3tpfvgrre.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wwujmpez.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3plyjrnwd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dketrjfe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uywpqczv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ckhvisaw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kjwedlgg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jlvaanqw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3iitmuwkr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rvxcrqna.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gzjzvgls.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bgppusau.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hnjlyykm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yehirjss.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zzmltvwu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ktdyzvmd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qwbcmicq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3udvueuqa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fwugcciz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lrvgcfmy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mdtffxrt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vdjewayc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdfmjtxy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rsemmfap.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3kkznvokb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3izhjnozp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mbzrkdvo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3heewwyrx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pykuhkkt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3szsmuknm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xjrnrvqt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jgfkpern.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tokqpmtb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fregxyfw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dygpvvgh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mczlptzp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3koddjnmh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vvkkwyry.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajbgbekv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rgtyrslz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oqohhvgl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qnqrkvbi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jwsdqywt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3clgjbtav.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3frystxaa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ynchpook.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fctqnjrr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pfifxpwm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3klznepiw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3meerbxqy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xyllmlnn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3buoiknge.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3issbeuvy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgmjilz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mlukarhl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3aspylpxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svwbvifo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pwgbevsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnsnfiou.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3olzzrbmw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gjqqqezu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ovynzlue.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tevcpxzh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wswpyawl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dgoakynb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ktjysfnr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nftgqxjo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pqlesffq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lykstyvh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3efpqauda.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lubifsme.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pzwziihm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3erwijumz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gnpzxzpi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xqxobroi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vizjdbif.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ywwlpuwf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3oooiymnt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fjcsmwbi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dsthxxav.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mwrxljgp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xvclhdcj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3iirdwjxc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qkslwifa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cmjbigqq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lckoqbjs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bhmxxtqw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qcozhaem.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qyflrnyu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fpkkkgpg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3sciklszu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wjfbmupm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uiapmrkz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lsdkthof.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ylhsrtwb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3klfnkqnl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3drlgmnhw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rzrvtjdw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrwygat.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xthcuqta.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vqggopbs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hxhwwesc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ziqoscaw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3juwgzbhy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pxobbeql.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3xutawcpf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3umdhjukp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3yyadfhfx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wlzjztth.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ojhmndjm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjyfkdp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vaivoyit.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dhacomtv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ickxpxlp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3scibigpc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kjumfqyn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3avjidbdz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hbyzovue.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uqodjwsl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rttermjq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zanxaaqn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ilabczzv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yvytahbt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lzajdvcp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mzyiwqee.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3accagrqg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pwuepmhv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zvquajro.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xmotaxfl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zyxnunak.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fbjpdklt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rjjxvsfx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cilgbafc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3oreqtilk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dbrkpbag.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gzszwyjt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3symbgkej.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tgcdksbg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zelqnmot.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vbfjhggs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3yrqkyqwu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ujqatcvm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mhcekdxv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3shoeamxq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3noxvnsym.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bahjhiqz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3rpmitzrg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3egeoupvo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpnvrjne.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jvbazvge.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3uenrbmow.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdcmkblo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kradhedd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3taetkapl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyndvkbs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fwahslxy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qbhbuztw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jodwemzx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lylgqtxy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3abjziqqn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bhdlunxe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wuwbjgol.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ywnoauob.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kpxrczao.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mdjoxiaa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3pvdtretv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wotkvkve.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ytwllyvu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zzvaxptv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tovjuydx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3poswnjxa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vrpfmmhk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynbaoqvd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xwqddenk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3omyhtxum.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qtwqfsha.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3peybtizc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3enzoubyj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bcpkgxtr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mwwewqji.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkhqlwpo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wnccpbsq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3eljiorpd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lntshvqf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rngqasre.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uiaixjjm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ncwzcmqy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3bwvjblpv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jmqtbffz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tefgroso.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qsdbqurp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cvoqhsqq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yhcqofyo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wesxwnmk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jmzjxwhw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3epecspza.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qpteorxh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3inhvmpey.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cqxamalv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qgfchuzm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3cfuekssk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ycrruaxd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ljnknsbh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jszimsdb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rclbktfc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ygkblnwb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3rjstoqzu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ismcjuky.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hjfujgjt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yxbhsntk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zixgyydo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fnnfqkrb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3aaxptfeq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tjamhjzn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3efoygmnk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gvlcegme.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fsoenxzu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lazfwifs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jdcgkkgr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3nucilonz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3emxzuniu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xnemkdke.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fnifqdnz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vkfehacs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lhsirqhr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jogfcmgw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3gibqbyoe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xdgoswoc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3digkxvvl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lrvdnzhy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kelkzsdn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qcurdefc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lglxwyzo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rvhhufmr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hclzousv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mlxyihdo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3otrmnzyo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wuolzetq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3flrrdixp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nknyftwk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zcsynsho.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jydwfhhs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vgnmbzpx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3blayjclu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jowtqyik.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hondlehl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nmcvzord.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jhqvdcnj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ezceoixw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3krhpqjte.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dmcpvonj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3irospnai.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kryhvixb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fkbupfyg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wizqiczk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xgfpulzr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bkaplfun.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dhdmjyda.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3eyhnzmiv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fcfmjvps.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3kiccsdzs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tayredaj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gfrokoto.html


<!-- 参考信息 -->