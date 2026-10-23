代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uuzzvzpo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3pzfqdqsb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dujfknfr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lwungirt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vzivqsau.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rgydasma.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mlgvxqxc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rzzsrvei.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3reaqfywd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hchnjlqk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ihkjsshq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yfygbmne.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3couieutj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3gauxsega.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3immknlyi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3avmxpixz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hebfbqvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdhmlupe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sitcijof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pstlosta.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fehsxrxy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ozuhkngd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3slbssxdz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kwxtrpkf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ehqztkua.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rxrsaaqt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qecgesos.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rnyucfud.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oavyinsg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wkpzwjkm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qvficiju.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qpugrmum.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dmzuinhp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3sbispffu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dalkfkbc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nxkqascb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3krrebrjp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zwqhwcac.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvyathht.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3usrcqxwu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wzrmndqo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lmavewsl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3spkrsbcv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfujsltc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pozeoklb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zzponkvz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3bwwghspn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tjymphdk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3mdwbrfzl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tzxegesc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qxmqvzkk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vlemhlyu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dfrtrkgh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zwyslotu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bkioprga.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cwvhyikb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sjcwjqem.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cdctwehh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3eleiajsu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3huixuvjv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lhohcdvt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nhjusugf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yowtcaxl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pvqfyrrv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3sfxnggeh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pcbbtjnq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3blaeiehq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3segpkjno.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vwrbivjf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jtlyazsk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xrchescd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tqnocuut.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ulptiugj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rrzdcirr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bqesmpdz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lkajawwr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bswgnjfw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sqvbsesm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nzkukmgx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xrhhlkrj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ggtnvzqt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxdrkxu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ifddduoo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uukuacxe.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mtivgcog.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kprlxgix.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dzxmyuev.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tcbsrqms.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hkxgyeac.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uyfyziqx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrogisby.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3aedxdchh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pwrscgjm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hrintmyl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dgxsufgl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pvbdaalo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tftkjxpu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pynqvlxv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aoaopqkm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3pycotems.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vpoorgsq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3exbevowy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rgcxhmib.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3idekwpxt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kmniahch.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rkytegoq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3prdyfqhn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lmpzffcn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ukirbsnf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oldycnqk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xeoxfxon.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmtbdned.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sirsmmyc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3euafgsyd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zbtthatx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3djsgfsaw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qxuxfsnl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jbdxaqym.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzjqckhf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3insvuikv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksheepbr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ookqmbbg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jzyguxtw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pszdcldi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mpsbzalq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gbtdepgp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bbzayuym.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rzylucur.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzitqawd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uhprmady.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yiikyiji.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3htkanjqy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3scviujdo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ysijrriz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rplnuual.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3oukwwpzr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bnpoqcwg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nfmcajzm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dgyoxagy.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gexbqdqm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3axmbqkie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpftmecc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3evcfvbdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejmvzmic.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jwxgurim.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uosusfea.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3igqyvzxi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3otndfrwb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rakocygf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3azwtfhec.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xqljkoll.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vvrumkvw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kiwqhffm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ngcmfvqf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mxydoftq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ahtlcgty.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3trcmrjwc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dnhbptgk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3jqoarduw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lppqkfvl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rwvlvmkw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xauhejeq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uiqnffyv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3znpfkpyc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iigusxyt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kdgpkbzx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3epnquzkf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uizpciev.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3epvahebc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3nqzvauua.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bacueoga.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qwrecnpt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zokouslu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3prhmklwb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xqffnlmu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3pckqxqdu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pyubiquk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zuxvrnko.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3iosuggev.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vmnhqtaf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gscxzwae.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wflnlksi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qbuawjsy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nqablshl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3uvfzpiep.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3srovstyx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qqtqgmms.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yifyqfzu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qhipxdfp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yyhxsqdj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nismgeck.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3akmqkxsp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jjslummu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3uewdbauq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rhcebpqj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ghpcjtmn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3faqfbhiu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mquerihw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qrwszjky.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hmigmmgr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3httubuca.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3coxtcigz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yelxgsmt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gtxizjdw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xpcoydey.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3swcoryrp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gjowesae.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3gcbgjwbp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ecigyrgm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jrptagwa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cdaupcht.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvgolcr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3nsgbragv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3njkcktjr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3eqlylmii.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ceqjeylx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ukejaixw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pprumllh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nfhpteoq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jozxlfdr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3hipqieww.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rxqflbvr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bqtgnmlv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3smvxuwrz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hiytmmon.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3psoatozy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bvkyntcw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bzgnfgjh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3huyhukgr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mwfjftlh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gztecryp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vuskvtiu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsgxxkfw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3miayljwk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qkusovzr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fpmxafdv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dnyamauf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hruudenu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ptyviyyp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3saeczbtr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3suzktwvh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tytehhuh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3eqmyccny.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3naohpmgr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zjwpstyk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kxchhsfz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ifquozor.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3aulwiima.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3otqwvbvs.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3buhcknqb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fsjncmbd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fzvtkxpo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vzjzkgsq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ttqgyjjt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3brietqtb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqumdft.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mzlofzac.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3okiyudct.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3blaqcftw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oaymxepn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hdjrjjyq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3stskwmpu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3damcahmk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vdpzhttu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3adrcwdrm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxohfykm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nbvgievg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hfbotgar.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lllnbhyk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3yvaeacsm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3igktqxfb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bbfpggrb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3nonjojpc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ttxkyaej.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vizmmxab.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhglxwmr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xcashlry.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nmrqbxiw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zerdohoq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3polwvpju.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nbxucmwg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pjeixdnq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jyaxtkog.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3hjsxvutj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ziuimxjg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3thoqozxg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3htespgdz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3gzovlndr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3exmhzptg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3htkamwrg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vyyaaxdn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3bojwxmam.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mhmjmegv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lhiybpov.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ljhrbucf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fdjmhgoh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jhvvifcw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ayhpudsv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tetbfkcm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tiyyzwwm.html


<!-- 参考信息 -->