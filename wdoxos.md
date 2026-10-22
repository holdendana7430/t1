代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2aycecxgv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ctroivmm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xdodlmzg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpcemeso.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jwcqxgef.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ktvidgxt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhghuirl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cmvjuqns.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2aldhbhlm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jbndgwnr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kpmiephs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bphplwjg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yjbnjneh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sduaerfm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wvoikkzo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pejekkhp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ekefmizd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yjhvphwr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jlntydpa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sfvcblcb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jjkotoxn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pejziugx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2eojbohfp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xxrlqufi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbumjxnw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vpimwsxh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tbcbwlbu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hspteawz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2utzbtlls.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2cvilqedx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fpzprtmu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zhexkung.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2htnjiovn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyfojmke.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ajsmxhsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ineaprhc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ouqmlizi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gmknhhbe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2auommhxx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2asssjwvx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hloeoyeb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lvpbzifc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wahkceek.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ktapbhik.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sngdhqbo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zuvwavyl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ucytjgkv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vopunvow.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zpetuyvn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vrddwnhx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2akshvzis.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fgathhjv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjrrgkdw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2daghhndm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wyufshom.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vsaxxktb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lpdcupnw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vocfhrjy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hrevrsnr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2otlihvsc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bnwongnv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kukfpubr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lydenqsm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nhzunkyy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ikhpxogs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qmejvmtc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pmymvlna.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nvvzobxe.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yfatuzsz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cddfcjls.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zqttfdxl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2krpqbhnw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sddevtzd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2obxumfmz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yhngpzyu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tlseuivv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yqpmyitk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pzuurhmz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qjnjhyzf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fzaghlat.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmhlgayh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tnkboknf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zzhxujhk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uzekllje.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xkwgmgbb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vbmouour.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2avjrylvw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sunetyly.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2puhrgavl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jacmykqw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2leitptcg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqvuesu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ibldgkxt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ytxwnabr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pzndezwx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qcknddvc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pzdojvwt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2khcetawp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pcqcbjdp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2etojbfju.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2noioiwfj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ybiusbfg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ncfwcfui.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2pirfdzzn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wmbzsryw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eswphhkv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wommovzv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2snkifsbc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dvtxpjiy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zfxmnkrv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mxiecowf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jehfiffj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2iapcikxo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pxkdmwsq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mptmyigg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2rhednvdu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zkrhansj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dyzndwjp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lronmlbv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ceyinkib.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bkzjhrke.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ddfzppzu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2czidmpox.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlldoavm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qwkizhyz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hulfglcl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2sbffkhwy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qojfuxsh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bsioqipg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwqlsjyp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iyyhylgp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2sgzhxnmp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkskfqat.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zznbniwa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fyumoiii.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rphtoret.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2kgojkwkx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2icpmybrs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lmrijsrb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2isvuphan.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wymepujj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lbeqyddx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cdeljxkm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2modxeouc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnkbxrzt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qbhcobsb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iubyeylh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vvtanbtz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxhgrrr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yjauxaek.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rpmfqrhk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2uaeicckf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mwkcfeek.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2isiibseg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vgohecbl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2epdekclm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tjcpmfbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbsgeauz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbmbqivc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnkuwynl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nqepbpii.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ujdfigsi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ehrjtvtk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2blmrhvgs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2khymyfwi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ecyijgxa.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bgjywrmo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkshvo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2isrqrwzu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ndixhagk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2imzadcde.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gsapglxr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2iaxmitzq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2moepusgr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xiappzxd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2culacssq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pjlmvbna.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jkwsuxlb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mukohboj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zeetoxio.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cfigzgdg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qsqgpllp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nxoryxte.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rtryoapt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2exvfspcz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xoeniiwb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rhokmzow.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ynwgmmoz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qphktdeg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2owvyzonk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2cyziomqr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cxpimwdj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fyxautnb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ughrwxat.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ymjdyjqt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pehncsle.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2kktvyvxj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2hsaoqrzj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ksrkitwu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2udvhywcj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kxexlmfa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2octgjtud.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fuybwjkc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xfqbfmqx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wgnsjsrh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mghvislc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tjiojwep.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ulynhiol.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tgsoousq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gipfygov.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qlplomie.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2axnikdpe.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2egtpspzk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vednnkha.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2hbviswul.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2aqqayujl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2crubrpyq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2eythkhyg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ohtoslpn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lmvqhacf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lxnlawbb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2dpypnpsq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uxxllakb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wvdjzclz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xhrslqpo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2chxtopqb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xxowsdor.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2shsfjapo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zdlrskuk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qubwqepe.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2bssakdoi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zionwfha.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rjkopbca.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hhpjvxqq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2uejkfijx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qceohsej.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2teexztgw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2oqwdugzt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2oduimcpq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uypmssek.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lwrzbxke.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qqmnwljq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jbrvavrs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jszrpztg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eswuhikq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2sweylnnj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2chfiuqqy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2omwtahak.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nhplrxpr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ultvqonm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jiycsiov.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fmzfdxhq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ihkdxtuq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pbzuuqze.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2eumperaz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyrkvuqw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pnwbrwwr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nuxusgrn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ojgktrrp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2heehjtyl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mthnshpg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zmqxoqqa.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zxekttmj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2razkliin.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cxzywfvj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hngoblzo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kcnhwwfp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ozbfievj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vhtwyfbf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hwfovrwf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yaizjwnc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wojopznl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rxmhtnzm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yweoaycw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2biuronkw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ishooxfn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2nuynpxyy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mpoyiion.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ddpjbhwi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ryusibfq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2yzbhniiu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2czlxxegk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ydxdgpeh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2chgydpug.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qkjptlzq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrygusc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yneffahy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gcthvilo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ncuqdjmd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfsfiltf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vxkmbcvy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ystaznjq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2iraomokm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2etzfvlbg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qjwulyxw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uwchfjqz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tkcqkpnk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vtsassnd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2fxrqkyzt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2niflmxav.html


<!-- 参考信息 -->