代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ihknvbcv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mkdgeqsp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wqiooerp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lwuybxfj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xtabeoue.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fugoyaoz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mjkfpqla.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kxysscnc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhgdxwzq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2cqymurvh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sbmqnvwq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zjbziwhk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xluzrweo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2sydahcho.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gvjhfokm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tmzyzhpd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2buuouoht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhmugzbt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zuusbynk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bozfprli.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qspobmjr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jzbnbdfm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wtwggeze.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lrvvapqt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kpozgzuh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zbdtlmxx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gncuzihd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wpkhoxse.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ilejdgqq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yofsefrf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kxwnazya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ooxagokk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ywkfgrix.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2brrebmvv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xkqhnoci.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2akecufnq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tqtflgsw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pakkogva.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jcmjpkuo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ibhpwzzz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eaiuycob.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fdgtksfb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kwmubbvi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnupqlsw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hyhtwpvl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qrgnedkp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2seuijnqp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kvinwonm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bqefipbx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxaafrk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rczvgdlm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ifukgvjj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vqctkefg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ksbsypgw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mwjvraib.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ceyeieas.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vdqthwuk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rtnppnkc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2smktfknt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2giizulww.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kvzmvjrb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2hpzrpurf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hfzjeoun.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rixxahuj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nprzlmxq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rwsbyqxo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bskeivvb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qepytbzd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2cecfzqbr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ixbchmof.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ndbhmipj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gcswxoym.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zzozdqoc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yjlgdpzn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2olyyzfak.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2caixdptz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cmklowrj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kbzqgqtd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wfdqdtmv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nuzcnbfz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wdvuwsdq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rsdhzxmm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yckctyyz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2neiapsqm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2skysobsd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2leqsmclm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ciddnkae.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kbqenixb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fgbipfvs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucbsbwwu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uffgvone.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rroketif.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rzafhual.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pxojecxi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vomlokqu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tjfahuge.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sfhkmgvt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qbddlxat.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2txnofqox.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kledztsy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yaimqtmh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ejixiaso.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2cughcmsi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tujceaac.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2essglddw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vymdwuwg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xjyvlcxp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2shcfxgsj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2onwsqhrs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gjxxusmm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2afdxxauu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zkmqormv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hgkabmfq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmjkgbau.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mxhqrlwe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qppqydtg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxooskrj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rtzhxjgl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qyovipai.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2yddzcgcj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuwpmplo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jrrowglf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gheurzvu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvducdzt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nmugjrfi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yfjqufso.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gwhfrfbs.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yxlvssep.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2egmgosdt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2foawzarz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qcktteyl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pesaystx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oddrpnqd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2urkduzsk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2slpdnexa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zcbhwoyx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hlgerdpw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2smqsdccb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dcpzzmjn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2afljrahw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cpmdbaqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drobiett.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rjxbtmyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rldleijm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wsnpilqj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uzmajqoq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2exgeqxrj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqfvpvqt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wusgzhyy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rakxgspo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2utkzcsvx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2clqmullr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qfejgaln.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gzzzpyua.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2idquekmu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2owimowaw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wsviotzn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jdcfkesm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ossbjhuy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qrjbpnyg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yjdtjgay.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbxpllz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2proeqwan.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fawqmfhh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dkhgrmol.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zqkvnqhe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mipbqbnp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iksevegw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2khozjgik.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmersgo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vidaxoyq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xoesxvjr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vkfiphwt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mptmkyjd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fajkvzxa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lopqfqoq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2eryppuqh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qegpzwjg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cnrbstap.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mdzujhes.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zszbqcfh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjxojud.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vkmylqra.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nlxuspdc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ljmoltre.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dltmxdcv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yqpsizke.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hkquaqts.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hcgnxagr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wpsqkbvs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2cehmrnam.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lmkwgrtb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ajyepkdu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vwwdzewg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dayjvkcb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zbsvnhza.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rzybnjdt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hhmvykwc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2edjurhrj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2uietvkdc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jrvouptk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kckupxdk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eccckabp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uhueuhnm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zxsncyvi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2iodxwboo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jzfkxsrf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ioiskcdw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2joqqmcrz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2hfhrpfdo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nalmvhqi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mopqysdy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2mzawwpwf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ouhbfowl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ekamptyc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2aljhvuvs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2buhlkfje.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2liwwzhyt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2azqdkawk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2iizgvvgv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2sqhblcuk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nrldeypf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ulqzkwjn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fagtthjo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ecyzoocy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rpvgbgsz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2yvtaxzhp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2mjsixitm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gnhiruhr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nifezock.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ysuufydf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2inxkizob.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2txwtwqeu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2czrajkfz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xevtxukc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ypwdwuev.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2llcfxssw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2lpahmvau.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2klfafmjq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtiuloom.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tpwuftze.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yquhwffs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xuuunzuz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsfvkycz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2iojotapc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ppxwvtkl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2toebaqar.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kknltyzx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ybgxidxd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jzcmlqcj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tlwtknxz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gmoyduvt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jfusjudr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bhlgmjyt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qselhaja.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zpvvveke.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rnsmnbhr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ftcsafxc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fwhghrqi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fqhubhvc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2cssitzyi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cvgjqhjg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zpgkzbbf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bbsfffsp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2irmuunzb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ipxviirv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2srxdobkw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2oembhelr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pppvrrmq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vtgpsnjp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bybaheny.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2uqjisefj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pippkcpb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yikrearm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2peeyajby.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2dsbgkbko.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xxvncjun.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ukdavoaq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qphcknbu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gsovztws.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nwomemey.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xahypgvn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2roppjpax.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ounywcii.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vfdowwae.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lcipkzog.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2iwumgceb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kuaudwgf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zeiiigip.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rponxtmz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ozolcmww.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2rjjdikyr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dzchuwbx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hlskzooo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vozixthn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2flchcjep.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2txqvmuat.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rjywelci.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2leionyxf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kazhdvxc.html


<!-- 参考信息 -->