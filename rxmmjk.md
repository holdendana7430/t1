代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihutytny.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xwcwwmlr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kwvpcacf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wkqobbzu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rzzmoycz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gdyvyuqd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qyknrycz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lfgcrljw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jghvqmov.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sguowini.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xvrcyayj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mekrqxzl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2scmlosgi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2uhorarxl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vebecxmn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cbnxxqgw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bmlaqljy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2praxaxqe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sfdmmnpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfmqnadd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2njkvjknc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qfyljudd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvbvlujb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tdekueef.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pfpogzbp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2szxlunai.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2syoeckck.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mfrtkayt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kiyzddtv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cmbpmico.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iguvogxc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vxdqwmkn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kldkvesq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kusdhfjn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dxpywyhm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pczlnjgg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvywmzqo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pnjorsit.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mcljsdap.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rrlxbnka.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cfzvhide.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2wjvpmech.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ffksnian.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2difstunv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ocvtvwxf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2esqnudnj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfiygmbw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vnneqjji.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2rbubjiuu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zlplbcyd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qvqlxarb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nvkxlgzd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ybumoecz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ulsupzmk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dpfezjiz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yonlcmwd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qdhsycea.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2phligbdl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bftaspkl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfheghj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2plwfonfh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fqtpmowj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2slfdzpuy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jgbvfvqm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2obgahtwq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ajbyoegk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rvkujyxz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkxuarz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rfftnmnr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ifyglrjs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mbxbnohs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wxaybiqh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2abqbdunx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2njwczovo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rayzzkno.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2imohfbsh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rnenjrrg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qlkdubfh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cxmvglbh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2niqqqzjb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fvxxmyal.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kpfeljsv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2atgbnzra.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2awhhekkm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ocatxxsx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hgjgyftp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pmiwzwlv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cbxjdmyv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2tdontvwo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2espylirj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2viimehsy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ksqewifk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yzfgubgp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hioodlml.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kfrarmcp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nrlbsojr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zygmolsw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fblinyly.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hjxcpjfk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rrlxpfeq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tovdzyam.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2unvunhnh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zvthpgre.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kwtywwmm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dnbraalz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gyrlmfvx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2aekqnfui.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdchjnbe.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hialawdz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2homersyu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ubgubmnp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzhnnffs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2itukfcqd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlsteyy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ezwjfpbi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jhiaxmra.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hepqxiwa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwiwddbt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qfyglxcq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nyfcafdy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpvmtbpd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wnipqhvi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dpdgvnhc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvygjjwk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2canwrndl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2csgvfhmn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tvniscng.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aaoepzzg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tzcquptf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2elkavqng.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zlkolvlb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ddezoiaw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ytiihjnd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2atfevvmw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xizmfqon.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2budsjenc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kzqvfnfq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dupqtngg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2smwniuyz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2swipjmsj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2atnfypbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jntitevy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwtcpagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqpblsfs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yebdukvf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2saozcnxk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ctntvdew.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xmlebplz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pqkfdhdc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eywnutqa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mmsthixm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2icluzika.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qhujuvtc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ebensvfw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zwxhteno.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xwwgkipj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qsjxellf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gajsxwlq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2svksknjf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rnwagmye.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vsfromna.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wcqedskg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2emfkhxuw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2skzqkqhg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iclxkshe.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djpfyvrg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pjdypfyg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhytnoma.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jkhcskdo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zxpnhijo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nbzpwktq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2savjaivr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2oycizvyy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rxbynfph.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bszohfzf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ugdcxhsh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hsbaakhu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mgylpwah.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vkrvtuhw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2guqnqifd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ytqnvtys.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tmeojsiw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pqqubgah.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zqsjopgz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tcqucouu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nuwvrzbi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jrbxychx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lnbdwzwp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugqwsrbe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nvbhrosc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mvbadkym.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jthucbeg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2bxbmprxh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hkiilbdv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sgomacpg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gtocbzqe.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2spvkosrd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cgntwqgu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2evbqtycv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yklxvboq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dlzszbdk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dmyyvrjd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lmhicewv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tgimswqa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pbrduigh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2glektozl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eihslqey.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ubstbrqd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2oqpgytol.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zkosrpkc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lqcjcqhy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqrgodp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2owcgkvvv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rqljmmvm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2khnfgylx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vhavajxy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ejzsretn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cttablev.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mjfxjgua.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2rjabxyit.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zlkeudem.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rdanumue.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pixrcskc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iiuvtwps.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hekzkrgl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dsmbjhzz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ryjyfiau.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2boveknjt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2lohrzaow.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2miehlemv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xctvmvya.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fbuinxrf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nfkehilw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbdoujjs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2foldvsam.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xxorusle.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gdicbpbu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rzkcnina.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2koscqdyg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjreooaj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2fwgvxmyk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rqxepbor.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bbsvojcj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2phipxaxj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cdmuncjt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ctzkfqdz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2guzfrxtx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2roqcbxnf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vnwhinqx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2pcyxuqpc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qdxuabmk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kexcacll.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wxqzuesc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vrjrbcbz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2aguyhtrm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xsdicvqu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pusizxyk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hjcrgatk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2iwvbxldt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lxnjuvrj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2frcjndzp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmwxjjwk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lytpvgpt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zyljobbh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hzzjtydo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ichjnyok.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zxzrewcb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ijtdesgc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dtsqemvm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ogdqcjpl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ppdmqnmj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xywqckpk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vplkhfrk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pcunansr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2egwlbtrz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rnnhilpz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gmubffli.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2mmyzirgy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dptspqyx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2whwuxtcy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2yslkbkoy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2eohloatb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lzeouzwl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dfequbsg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cgmwvxhb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wfcgpyel.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wdppacxp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2icfhlxyv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2slnwmbcg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jfecswrv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hcekbzom.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zofikqvs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fiwnuwkh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2srageuaz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zbeaossf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2lllpktfn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fsswjaaa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vnepgegk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uggphwhd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sfbhuzjq.html


<!-- 参考信息 -->