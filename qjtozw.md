代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jklwxahq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2stixvnrg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zceoqljw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wpodxbid.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mofnqsgo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fraxwcjd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fkrqzbdc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tuayucfi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2llldgoku.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2kwuorgrp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pywdndvp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tbekigzv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zeyqlqjh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qkosukjr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ozzerpkm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cvsojyzx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nfpztntu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nnksrxoy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2sqknersv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xygwsluo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uykewtja.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zjqhuhbm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2odawegeq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lcnoquzf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2flaqcubp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnusyust.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pcuirjua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbfimknc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cretmbdz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eoxvaoqv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fazswpfe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ogtnusdz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2quqtdehp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uzykhrqs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hfzkvxbp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tuafngfx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fskkdtci.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2evtjqymw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hqqbzyyy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fkptxzxp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hcyxvkwu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2glrmagss.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ssgvsqxp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jqstuyrm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rsqwkfre.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pncujwbk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2adlvhxls.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2inapzqoy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ritaaaqs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2oyzyinon.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xnnccmrp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ueiqvufk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wwltgrgf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hgokkoqq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wihcqchk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2msokatku.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hsrrlusz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bwjvnoik.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mgekigzu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jfmccqeh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lgrzadbz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mbfbwewl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pfzvhaod.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2aqdzhyaq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ldlbnoil.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2whvjjdsq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vraedxva.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lwnlivnw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ozgnvjid.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2iprombkf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zznordpy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2eoravwqf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2werrswne.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cfzjnoxq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2peyfyixc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jzwkpuqb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rtqlimxe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2vipwdyww.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yfyeyezn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vqchedqw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zztjokbq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2iblsxipc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uyignmba.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2oenypsdl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2yqcpiixu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hkydyngx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cjgsqohi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uynhmbig.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dpmxbjvi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wkcmexrq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kslxaaoe.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tqpaaeeb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2sckueeiz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qulhcrmr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vivxevdb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wzrqpmtr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ryeyzyuh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2cgbaaijv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hzpmntgi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ipfybgox.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zypvnzst.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lzgbgyms.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qimxdkca.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xnjslmur.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zggzibwo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2glylzend.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hknqeqyq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2sdjhpixt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ahivixmx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2anbxcbqz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qdpmlphj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2urhkvsyw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rbhyidvt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lkgqccrp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yyvcyhjm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2atcyivhs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jtwgbefn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzoqbvrc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2smwopqzo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeucjbno.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ozjnvdop.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hwdnldye.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ayldewbr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lwjmcbwd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2bdblxody.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2izcmbebe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlcosixq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eynkolxa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xckqnmcj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lfjtcmgv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qrligseh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jrrrwnra.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ttjqgrlb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ihizmpgg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pemperit.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xghidedo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rvklwvdm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ggbbhtcz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cmczuodv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xqeqtuuf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mczdxkxt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qvtqqpvj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bpokwzfs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nvpvtpep.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dqpamvmy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jeractms.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iqsdwrum.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2eorchklq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2svzexfko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpptbuqi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2taulwwju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbfnyzrg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gdtcnbqh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zrjzgagx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ncyyyyit.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nxanaqxj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zlmqgand.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2talwmhhp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qkzgmisy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bwgjrool.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yigedhwu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yueggphr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2binodgue.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2thmdrhei.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2djrymblj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nlpqhrtg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dpbmscba.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zpzqbmjq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xozazkto.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2pcoqdpdk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nqqavcnj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2igyowjmo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eishxgxj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2auwwayhg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tpgvlyse.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2imjmsnpw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2uwjluinz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxsmqpx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xsgstlfd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nbsevavm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2servnzzf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2njsilpzi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qfupenwm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wfkzuybk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wxmqgyes.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sickwcbn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hxrxwqml.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kjrqvcmo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2caqeqdic.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wqariqao.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jxbiqmqs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mbulxzkb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2cpajarvq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yionybmm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2yxlkxcyx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vgbvbtdx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dqldxlfs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zyfreidh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2sfjewmrv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yseigrxa.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mzhfuwef.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bwzqizbd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2kphtbzcb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2epyopoiy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xbfbpzld.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2durorsbf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2aexwwokk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tgvkvphn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zowjgycq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2tyxculpn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2owldmtcm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fnahfwjs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kxqmppyg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mfwygxip.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2mgdfxpkn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ouowgijo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jmbyrhhg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2eimfivjl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xedihbpq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jdkyehvx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2izfdgppk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqwzjvu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fehwtmjm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2igwlzzcb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wmsujopy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nxpdhcjh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bazaisfp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2qangeuqr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nqpxsrqo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2idbcbnbs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xhnczhrm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vawwgeil.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pifanlqo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2masfndtf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rnqxeneb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlwpgyag.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wfzqphbe.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2objgfoup.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zpmktley.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xogdkcnm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mbvdihjy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nymnffzn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ujympirp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2eceelemq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2buwwgqqt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zlpexwqg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rnygtlfz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmwinvs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ytdmbkvh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2krrdudmr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2dbnmlyds.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jgggcxeg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ewhgakgx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tkjeqffr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtvwfzey.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kzpoeeny.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2tzpdqfis.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tlviqqrc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rbkjnhie.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2akknagok.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pqdgvvjw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fwjapukd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2beunpyix.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uprprvbv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jvvvdhiz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2vuxmyykb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hbcypwsd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xyriidug.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2phfeuaaf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eiqoazkw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2femxejos.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fpuqtdtv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2pwcokggs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yovibrtx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tfptiuic.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2asalgmyh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sxoriokw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ezovevpa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gcoxodev.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2rpzvjosl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2acsbbhzc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nrpqcaid.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kbccafev.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ughwqfsj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yihcwjkm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dliesjwj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hcrmssvp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mwvlaajk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gtaxeqrb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mriyqazg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2cnotovcs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2weovuqzq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2svzzfvga.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2byfubvps.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2pygcoohj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2cqartors.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vjzgdpyb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rtgoitau.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ufsueehh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ppxohxwc.html


<!-- 参考信息 -->