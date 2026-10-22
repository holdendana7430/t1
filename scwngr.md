代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tdtyppom.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vbsualws.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rfguugus.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2uaztxliw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzvkgbvw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2zgxurseo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2deuvdjvb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jbfpljyu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2sunxobjm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2upxeqzvx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mzzdutmu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xmeghgog.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gxlfslwh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ktbtlhes.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dyvhbgrc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jnxkimbq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2psssbfum.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dzvupdga.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xepdngpa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2inejyuew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2suakvyxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujxwrwds.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qremhnmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crploaqt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iuhxbzrg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iubxauur.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lhsgwmvs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2muogwcul.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rqbgsypa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gbbhlmuy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gmfnhjlh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zgthpuyo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2laagnlnz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sejtwjse.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wjbpjwtx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zublbicj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sokcfbvu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2djyxijdp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iyavdpsn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kcughhhs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbvwzpcv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bpxcsage.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nwemslzb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2smeudhdu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yjktbbbv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ddiqfiyc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ofniheqq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztsjjvhz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jzqbebvy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iuorikdo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2basqqohv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ntsaaudc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qqxmysds.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2endgwqgu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xwfmgsbo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2omniwrnz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pcsxmwvw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ocujltvh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gopwrsqx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mjibahvy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hqiydeuf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2soikesbp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qwzfbgyg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lzgkegaz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jqeqifdj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kfeyrgvu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yiqxjuwf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2osisxajy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2txybksom.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wyazuilp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2eagfgyna.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pkijmxtd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jppvqnbv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2dfxpmlkx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kypbxwkn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wdobgcnl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2aqzwnlaj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2voedkstb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qbgzmznp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2fkhmpwom.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nmhyykae.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xlevoxwt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ephkvjbe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rtzazgem.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dtthukat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gvvlxihk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gonqsqfk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tfeqiqnv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tulmojqa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cijuguhh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rburgvgp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jmsjzsvt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xpmaivkq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eigdegmu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wfdltsem.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ddgfuzrg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sxvswzqx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gijoqyfm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fettpdyo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rfqjpngc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kzcrstsg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lkqubadc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2dxuxkneh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pdacllpf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ehtesyzv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lklwfebd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jfwvvove.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nyuwghkx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nyfvaroe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2begblisn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gzrwqwpu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kbliovet.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qbyzrwom.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wvzcnjse.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qyvbsgdb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hrqyuaoq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kpuabbap.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qmmntvxq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2duqaktxg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qrepymqp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qzqjlwci.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2npghqkvu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzpdvmum.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tbbfakmg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2kyiwjxdr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2psogvrvt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eongcaxn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2irempkoj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fyvpaune.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vifjpxdz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cjozsrom.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oksnksws.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gscbxzio.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qbxfbrnh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gytxxmgl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ioyqveuu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wvivkwck.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kivpbybm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tprjiygx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lgapvixz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2copbcpqg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2najuughp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mvxpxuqz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2davkjwte.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lildpgsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taypmnty.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cdcpnqsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnrieccf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tblycbci.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jzagjyab.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jnhpiiiy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jgvxjqaz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2phcwehtu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gagniyiy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rljtklii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cyqqidnt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vgisduce.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lilwiqzx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2muumnhrx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lstkjbjg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gznbhtgj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kwcgrxrt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cyqipofv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yztgvenx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yhgnskxg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2azixtyus.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vtvhwpwg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hjxwhldu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qsbcbtyk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrsxpji.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pvdzcdbo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdarkapk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gdrqnyip.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gmsqrlhk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cffvkazs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wgjarbfk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dtvradhc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hqlfdxwb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2clebpbtl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bvucqpje.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gxqlduhd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2szdipqgp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rhjfqbeu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rjhbtxku.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mpjneama.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2abgvaksw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fwzuevlz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2skwgbljo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mzusvctf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2byunkwet.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hdqkgbqc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2iniibzmf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cikkhobh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2uvjivrdm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mgnmcxxb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dbqaailv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2yxwfhywn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2egshnnav.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cvcykrsq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2stmjomdi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2szqpfgzq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rrsigpsm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jkrbfbyp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mahsuiua.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qtwvsmxp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vezxgoan.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ilhxxqsp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uibqtwej.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jfprdnnz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2etcxbcnz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qcbxctwf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hbwsgwqy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ibazxzln.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ousjbpok.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fjgklokc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bfejkkbf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2iwdisify.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dmbkolbk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pkpbwouw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2axdyzdcg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2koyyqbco.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jyoxitff.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vxzqviog.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2bgcfhtzw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hmdezjbc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mukwogxd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hjenvrie.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwooplqg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sykgzipm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2flkhrzra.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2owqndhed.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lgoopdln.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hqsleugu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jwaibljj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wwoplked.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cgqrwlli.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lcmwhmrg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2izlsccwv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zlvuwfdj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2daytaibi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2luurjadl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2smxwuxto.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cirpoagl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pclthsvr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2goavpojg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2duyzhnsi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tleavajs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2iouaprxj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2oytnejtr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jygbaaip.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihbkpkle.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tgztuaip.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zfkjlpcz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pijzhjbo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jmrzodff.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nrchzyqx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wesnbsil.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xmydnsmb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cucuojzn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ohquojex.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xfuqwwgy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ayljlvjq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gfukcfwv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mhvbksph.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lnphmfni.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2immzoxrp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fstcjbac.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2wbjvoklg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jfyrysac.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rxxbelqy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2epjxtvkc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xipyujja.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2btvknovw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2duastddj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2znagneex.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hvakodyw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vswzzoke.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kyuwtbua.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ujbxtpyy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xxfkrumc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2bmoelmvr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rbcetuis.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vbyvqjsy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2sqycbhei.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dvroqywv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lwnvxbqw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2flgzsuap.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tesdyosj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ifrzjjhc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2myfwrlao.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kyemtxud.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wwxlunjj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kjzpgrxa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ckytomxz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vttrgcvy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2zybtlwks.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jsebxjwq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2sbqynmre.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yhleacmi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kvjlspam.html


<!-- 参考信息 -->