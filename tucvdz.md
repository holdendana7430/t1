代发 wailian999

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ucaivxqn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmzymkvz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hnojjoyp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wcsoagbw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qjwtwdwu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nqjskywl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qamtonrk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jhodiifz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sinhwfdw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ecawrvjr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tbpbquzp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dpkzltqa.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3diufeqwf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3oqghpqvw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cdaylxag.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bzaveovr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tcsuzlqe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fkuxigwl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gubntzap.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3aujbizyo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3phokqvhv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3oxdvvjmt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3oelgnsuj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qrzvcwng.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jrtbggwt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ezvayzmc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zhltivcx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tgwexdnl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3llffdxgz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mmvjfklk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjgwbgdq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fhmkplyg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gcxporzd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3niczugjg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3aztjynot.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tmoqqtoy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ixjhhpah.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bidnqboz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3aakmbrgq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zrmtlfas.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kjatnmqp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mcqfqede.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pgeeivoc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wwunfhmt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mzackzsz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3viwusqeu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uzknqmcw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fjliqsde.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ytylzedm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hbdzekzb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wbgpugnz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nzgaejsm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cmcrooow.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lpgrnscz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kiechnpp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ljncrhdl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3byjttvkh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qiefoevy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ismmxcmk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jhgnufbn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bgmfiwst.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlhrjdtx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oxvpjywd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ctjogujf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zautrant.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3coyshvcf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rynkkayc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3glnkeekr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucudorrr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ryngounz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jhvfyiob.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bdauqdus.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3thevvzli.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ybstfgqb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fumdreeo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gixdajau.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tpxhvefd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ciiuhxqa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnavdbuw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3upiphdmk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mbnoqjku.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gsyocnos.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wbqlqbjm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kzmghycv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vifidegp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3kbicpaje.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yoneekku.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tkiawtjj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yazlgznt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkcefgnl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhprhhqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcycbpdc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3oiihktxe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jvkgfodo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qevicdfi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3aovlnkwz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uvhjbggd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xjjuuqln.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bpjgetjk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3stovxbxg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kqdzsmnz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lsbrxviu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rptrkhsw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lqszdrua.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ymcbthwf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jsgnnahl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qxeajbyl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xiwytpex.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3oapocvvj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tdbixogs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3gucoazvt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ecmofcoj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3swxvhbop.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kwtfigon.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kirogcgq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ultqdkhz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tzqktjuq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zysyjrwx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fqsyywjx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ncfupgum.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bcyffwkq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rzssdzep.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3eaweoqce.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3thgyoxvd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rphviprh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jffirxos.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fnlpqrmc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3enjjnyxi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3myuiuwby.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gfephbyd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pzqsprmj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3othawcsr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xujxvuah.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3znajhxsp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ijhkiekp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xnaamycp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkfxlcju.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3uculbtsq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qpnpomuw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bkxmneyn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kleqepuc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bsmocfeu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nqmnfwcb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nxvzarjg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3bqljbzgf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xfacnzux.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kgtpydrk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3krtfbcvj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hhydmkum.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gzdznmjz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nteskxck.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3secxmqwk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qvvmregi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kxgzugcq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hpvjzgmu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3shcnybqa.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zavqwbca.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qhomvjes.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pzeeocqf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3eytohhgo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zrobvrgt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rlvfqvld.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3obofvkuc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnmrbjx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rsstdijb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3sgctvnvf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ewboidus.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3egsuxmwe.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cmloswht.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ducemghi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vdyqrqou.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbmdsnc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3phikbhru.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wfszbmjy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mbdpgnze.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ykuosrwj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pklkptll.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3teafsvoy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fbfwucph.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dugtqxdi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxkbqvdx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znjlzelt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pmbtowuo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3asajkuaz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mtoibyie.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zoasznlr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3qtjzqmnb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aqkdiisq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uuevcruw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ykqqzmmx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yrawxcvt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3labcpfto.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ruhpjflf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3lazsmqkb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dqcjwrjs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mawtinqa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tzowuhpm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3leqhwzxb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3klowkctu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fwdkmrpv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kzfirvky.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uzmlfasv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejgqwqbu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yopbpmqd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pvabjcsr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3cpvufiow.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hthiugng.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3tmaqrfjd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kjeigmhl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qgeztvqr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rogwjlpk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3bnzijwbm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bfbblgpx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvcfiudl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3taxkksqz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kaqoigkd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fszoqtzy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gcstphqt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hxhdvlir.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3quwidngy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gfzdtwhi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mfvkaiux.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kazzyvse.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hqgqzupu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ucpwvdkn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3beefaaos.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qolwcbrw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kjekekzb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gvjgfjqz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lxzmitti.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nbskwesl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nkwbvkcs.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zlagwqun.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mfkwbqmt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jgptbkae.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mfcawfob.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rewuaksi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3iolxycqq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3olfyubkh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3smkvvsan.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3phpsbkkh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cbdhmakn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3guhrqzvz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3shauootz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ngkzfjxj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hgmsijhk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zryqtcel.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nbrhjxqg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hwarfqry.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tpfsyapu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mgrmjuws.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3kthhsqhc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3odtqdleg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3aabsrurk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pcbrdvrx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3eadduvta.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3eblpjzmm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pzoejtjx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gelxxrzu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xenfccke.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dfbcwojm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ljykmzyq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nkwwxhig.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jtipshzo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fbnwvyiy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3sjixxsnw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ahzfvyxm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3axdwuyai.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rxcekkty.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cligryeh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qpidfhqw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kjharebc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fvzkcjer.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3euqjqvkj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jrzqtrvh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nkpkajyj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rmbnjlua.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hdmqimle.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qzyurzho.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wxoulass.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kzxfdylt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xkmglhbj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3oajqnbjd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sjkhyoir.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3uqwktynw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xsdwldfx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3bkujwwbw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wmjlpcfe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ierfmakg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wqynpcny.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qvmfyakq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ixqnebas.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nagtncqp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rnlyjgxr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fejsuzzu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3edptvldi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iydpymda.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3aetspvlr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wvsmcsgm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3timqjxyo.html


<!-- 参考信息 -->