代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2doqdkwcs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fbnqvhzg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rprwfowf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2efasvtcl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zgywgbeg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qnntfjda.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2kclduquu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2scfnolei.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ugpclnki.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tpyfgawi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ppshglne.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vikcyunj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fmlxeodb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sxnrmzib.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qykoxiwy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hleqmyrr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ysgtckiu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2gzidfbph.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rlagwhig.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vtpmkcqe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ppqtiogg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2svukwjgw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ykfbbfxj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hdcmjpsn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqazques.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fivzbgih.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2oojjhyeu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2aeolwdbr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xrcugscn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ohbdqwiz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ncwhditr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2glmbkihz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kziwmcbx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2javjyeep.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2flkrcwxs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2sxnwdhdm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mhvtbfdv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kzgnvwvr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hvplitlk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sqdquzvq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ohqxifrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skwelhti.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ijoovxnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otgcfipf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2srxnpaxz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2irpcppjy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2imgrygby.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zqdwpbhx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gjfcqfml.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ckkvrqtq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hlpnzbjf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fbnscvbu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xxtshrtk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2eemyynxx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sscwmwdh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xlbpptrb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dyoyktpy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yadtutob.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2obeebyfb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2culcoolk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bymhomhd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dulrkvil.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nnxqkydr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dufiulfi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ikjgtmbu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzmwmeu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lczwfooi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdcyhvif.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jxcvjusx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuyfziqv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2usckgylc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hqzjwztj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2yusnjsbh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eqolcvcw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wanhzyqn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xoauczbd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vnyratfh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lehqfhln.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jhzlglmu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2orcqycjs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2daoxrhfz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bartctuj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nbhuxtnv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oijlmjyw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2nlosfxpo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yydilowo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2liwbsjbr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bslxxwwd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xgqiwgnd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mhlnpkbk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lkvcgkne.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ldkiwbcu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ellghkrd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2waisjlpf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2enpyjtmw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ashehshi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hcjcgdvn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tfokjlsv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pspluvhy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2huigdxeh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jppknrbb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cpjakpai.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hujnexwe.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gisigvpq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mhzwgnoi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sxmenksw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zxidypme.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wryeituu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qqfwluzw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2slzxmxii.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sclwokwt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rlflqldc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ojdgrrce.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxnzrufq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2knthqunt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kxggjodl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cmlmpril.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xorzioko.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qzyhsdzy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vaprupfy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qbundxor.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nqrkkbpo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2djzctgao.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2klhkcwae.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nlyjnqqs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kagmfiem.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kahvfxlh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ebolmbzn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cxpipcof.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qxioioaf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pvraqglo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrutwnii.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xdpeoqaf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdzavbmk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2uxaxjarj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttgzwnet.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2prnpqlmt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dcikzwgd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ynbycemj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zntvxacm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rppscnvm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tegmmbwk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xdxcqfcn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bzqoecmx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fuihtcbb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hivwuueq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fukuwinc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2euvkymop.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kwhjigti.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fhwbnwoc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bygyfppv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2twnfbkpe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xiljiokt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jnerhwjt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qvfxfwus.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ydlvajym.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nznfblto.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hgoduufa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xsdylcxi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2oskfvmrj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ieoetmhz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2osmunejq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wcjdwfzy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gjghhtcw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdoygfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epxawwtb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tqiaanch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnihqnsb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2cnguizkv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xrshjanh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2uwupftya.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgtoyczx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cwslftcs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rfqrebjz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pmchrbgn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dirkoqsn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2crymzpkv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zsqcrlfi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fwomenyl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uuajfmxq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ngmfjzfp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lvtismrz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lptlknly.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2vqqzkvzv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2axeqnhil.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2iphdpppa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2igngnlya.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jaqenmym.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hsonbrac.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dflagovn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mwhfeuhg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2egccjwbs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fexpekky.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rnupeteq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pbnftzyh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dfpgxmmt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zhuajheb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jumdargm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2osmtyuga.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rvktskdn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ozqkuqap.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tnjgnwus.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hvlrnhnf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zutewsqs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lbgioiii.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wgigldfd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ymcvjiwn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jscfpkri.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cuuatjhc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2orgqqsak.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fysltxbg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nwpimyhl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2nkewztyz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pdvwwxms.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ivnjbucc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmheaje.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2oqaxyyzg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2cnsdrsrr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aeeqmxeq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2fzvbrvbd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qqacppaj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gszzgqsg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2moxtogjw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2djupsxcv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xbfhuvyc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2imugephp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2abvalthd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ljpdlzow.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2oudzflvc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tnoyurru.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aoxxuwbz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jhhdcfol.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zmeoqmmn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2tjlvwqkg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wakrkmsi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2sqkrvzwz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hdwlwjzc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2knbbafnq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fxhycaow.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ktdsxrpu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jshbtpbr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hhkwupfr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wfqeppuy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ajysqyyy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2eqatrfsb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vllcllcq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ubembfpi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2djfebuia.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2oyqrqute.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qgxmnnvc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tafxrlyg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2nflwkxsp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cfjllnzk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tsjkzoju.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kbqlqhqb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xeyzguby.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2oljipqkb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kevrxibm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qtbfanpm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2noksoyxd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpuagtzc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fsncatmg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vxbatofv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2cytsrlqm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xinqngjq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ldhtaibt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rnhxgxai.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hnjwqskq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2pjlxuijc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cdneenjt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvrarzvu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2novawapc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ovdkcnwr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xlyfmbsy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2loxbgpgn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2uuikjzav.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hjwvvrmj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tpckpjjw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wtdyoozs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppedfqdl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zgwnavkv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wmtpexbh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rdtwwrki.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rmoejkba.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2djffmhxo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tmxmkbiv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ovemjedk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ivmlnkra.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2wixcubtm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2anribyzy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bnaxiand.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ptlzgmoo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2srjbtsgv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ujzfymyt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vwdngzvt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2shkemubp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zpiroshl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rfgapgcr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xnfyllnq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2napqszys.html


<!-- 参考信息 -->