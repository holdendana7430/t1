代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nkweyuhq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ihvjefsz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3boqukqsa.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tpagpflw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bniwvhux.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3siylfhjd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dwklppsa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hpwqakuu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3radfdhox.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3aqqbcsth.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sxrggvjc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lfeysvit.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lskwimyu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3njunxswn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vzhgvvjj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vlmwxmvl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nrjtjwxi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zkmictqf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ixctbzrz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3euvdkqcs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wkiocyly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vytsxhrk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vmqklwpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfgysrwx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlzixoeq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wzmaqdye.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ctkyrlkl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dsgpuhge.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kwqqzoqb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uoenazmu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dfyxlmbp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kzqwftrc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qcmzgnod.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3chfrbbig.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gttdgocb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xgnmzahc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3awwskndk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wkqfmezt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3canwjfpn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3svulwazo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xlltvbbb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dvwlitll.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oapdrwbv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vihojovw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eurwtkjq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pwrjwuel.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rmpmocqs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oisixsyp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ieruscus.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3esnblvlk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3avhqcmuu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jviativa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3babhfdpd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rixfzkns.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bigdzrfr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wmkalodc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xwrrtoyo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3islatigg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cnvbxrus.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rwfhfgyb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rhhzmsvp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3awaldbdq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fctgjfht.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pfurmxdz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xngmzmzp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrwvcdgq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3igxtmutw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dejddyxl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3huinsnlq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mykmoasu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3riawelsr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3scsskknq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hwwohjmg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3velxoiev.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3sfixpqls.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bjyggdcg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vtclvkeq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yijcevim.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fokxwaxw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mgwslbnl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zkgjbtkh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ujthwqar.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zaxtknsk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pivguluh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uobagrbh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nhozxago.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhwazyou.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cneqjlih.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mwmgvduf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ddzvvmlf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ttjmfvph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dnvmceic.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3znfmjltu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3scvsjtew.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hgdwvjly.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cqaboknv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rhxhuprn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3groarncf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tdqsekbe.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3acrkmbgp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fwdsfvxk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3illjbutm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cutulwwu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lsmkkmoa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zygroodx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bnvrvktj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3aargmdvi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ckiepfzi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iaibnioq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cqnkjvtd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iuorpory.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhztgxqh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vhlbgsni.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vibtiuje.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pbcegion.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3usmqwktj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3whucfvlx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sogdukze.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xfmhpmpc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lcpcmcch.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zciakdso.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtfylmuq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3anmmuaih.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3weiamrvf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mzagqilz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3phkfamhf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pssagxjy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lqexkdsn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yhbonnxp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hjkbtqfn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vndlnbvd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pumjulfv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ytgnzddx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mtnlkaxm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cpwyehug.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zfdngroy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ntdvohzo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3guzywphb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nsirzlxg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3syycmrvk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tqpiwypy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3omcaqqwo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sqedqeov.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xrzhvhjb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3izfrlode.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjkizkij.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xurgfjva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbabwexi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3eldncmpn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wgabyuow.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hxhiwnmp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3epglrxty.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ypygdnti.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bfkulfqs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sqmrioth.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3atpnrtst.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dqsbgtrf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3errjcfly.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wekuvrik.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hamxilfh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3utylbjnz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nmdbmrmv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3jrikqrrb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vpmatkoz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ysxtiavj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vbinsffm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vkflutzx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kbqfnvqg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jtglcvgi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3diutlmba.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dbfrqsrr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dlteojlm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zptgacha.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jurxyywn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ppuldrmx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ftlwvvef.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3odfrrtfl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cntwhaid.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ekbmdldq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ntnmsfop.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kfpnsnkm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xbdircil.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nilninhy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xpnyuepv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xykkzcsl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlvnncqx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3sbbcwxpa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bwjnyhfq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jesymikh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjoqfb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zjykkyqa.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nrirualm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hgzkrktr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qoqhleme.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3spyywvhm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jzaemokt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rrrhonoe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vqrpccss.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vcitdoyc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mamkzlyw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vdgyxcwd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3bgmsnlya.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cglgzaux.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ccqciklk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3nstwzogo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3cwysbicx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yokdqnor.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3znolzoqs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dllsiqti.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qvtjkrrk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rvdspxzf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yrldijwy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3faszautx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jxxtpvku.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bpflbcbc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hiofnqot.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ckijbjdi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3blqgmoga.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ocltwuvv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3btepdlyb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3notiklqt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3rmxyvlfm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wsqsihor.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gbnalncg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ndeezvwk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3swhafuoy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bfgmcrxh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3eshhehkr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3elmiqrre.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3guosxujc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ewhbfgzl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3czbksici.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nlmcyvhp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3toyijlul.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ftvibgsn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sxvxjdhl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3aosxabgm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3awuqaldq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pqjajfcd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bruslajv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3atvyuvfl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vapjaqqm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sxwpiknz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cleltkbp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mboabipm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lkipakcy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gdcwozto.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vhzcdwpo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wdaxhteh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3drmyuwha.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uaipepod.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hmpktooy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3inmubdaq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ujmhcpqk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zegjlpuh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fhsgopru.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qfigbnos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dpxfaslu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3mwetkslq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kvotnqqy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kflalmck.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3efancpfc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wsqyedwh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3nklatzji.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3mlukpesb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bnqoiqna.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fmfkkcvo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3biblaecr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3wdqgcbme.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3denubdfx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rzkcmfiv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3skgfwrtu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3kjayewsm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zxsjtxni.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lmhzxthw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lmqjftgz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bkwugeny.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3slkcccce.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rdepmvpg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3phlcrzrm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kwxvjnuz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ewubhrqs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hjyafbwf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3cxnlbgpv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ohaejpyi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jqslprhq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3sleednzj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wwllyqio.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zeydwqjq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3auyqpstz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ipapiyod.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3oockynih.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yhskcyph.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3eznytmmj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhbqgnwg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ichiofae.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3amfrebpx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3myulxzip.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hujvpqdl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pawfihzt.html


<!-- 参考信息 -->