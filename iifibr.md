代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xvqlnwwe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3elspqgad.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3scdgyjlb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vevdsfzd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgeusruj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jepzcknk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bkshntys.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mnpensmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lioujygb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qkznskid.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zoqkzeau.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3aywrssnh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3umftjjtr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ngppehcm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3srsrgvjx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lebispoc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lkdrzhfr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3safudxsw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kejsdpko.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ekzociwy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yrrrxwxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgojbacj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bdgetxan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3andyrkqo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ppudluux.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lzlnxmuv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3owatplvv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3glqzedhz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3velbxmdp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gtkpndcn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vhnluieh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgmuaonn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3apooetqv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3klouttby.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3trnvhzne.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zsinnixx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kvlcrjzt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzomkddi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3spvhfmws.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rgycakst.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3etcxyfky.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3okkpsjmp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xmkldeov.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tmvrkfet.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vfahmavm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xwjrapra.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3saifinwr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qrslepnh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jrjqmjig.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ughatray.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xkewpied.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3slxrvjqt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3olhdscxu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zrmpmeyv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hcgjbxlv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ncatkmtr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3kvnrtgoe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oudpvgwu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sbyycjca.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xuwjmfwt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nkdafgjk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ifpgczrl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3crknsbwl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ksvdtilw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mkimvyrs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vkksmozt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3anjhxuki.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vatcalzr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bgvvgpzv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jqxyjmlk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mdhsirsu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qnmyobjv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3thiwuydm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bzydjkwl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3goanibwf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qwqozrct.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hzpxsjlo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rrzhohpy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3nhnmftiv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3iwmejsud.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jdjyyabj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3apjyzwiz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tzehcrzi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yxzucxwh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uqeisije.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bikmmezx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fpnokboo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tcnnptxz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zvmbsaly.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zqiyddle.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rjwrsaor.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hcjfmqoo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3aghzrmfj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qevgrjsv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3khpncfzb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lrkaxedd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pctejsbr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lqxcikzc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mwnoueig.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uopczvyy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3buboxnig.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bngpnmis.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aolgsrlp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3kurjjruz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mxfjsfhg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3twfrxghg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cjgwkqbf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pnebvimf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3baipgqfs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jkouwhsu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lmahyoic.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3zlzzziou.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vxbjlyhw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dowfrnbm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3okwsizqj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mdjikjkb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zgxyayfo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mvelfjqy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jmjglbqo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ngedxizu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3msiyclnj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypbzbacb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tlwkxafc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3odkotazx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpushojc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mlbzwrep.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cqeebdvs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qtgargbv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3skuwlblg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wfyzoqas.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3asspxqxp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jixjljkb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3scspafyd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pfxwewsr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjouugv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fotapydo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ckslvqvy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sozvfrus.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3amztfvek.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wafxdgcn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zlrjbuvg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vzacoroc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3acymoulh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bausimfw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xdiielpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxfxufwy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fuepwsnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhrjmjin.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nyovmqkz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oosamwts.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3crhitvit.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cvtvutwd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wwpzshva.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dqzrnkcc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3exkcwpub.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rrovmifd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jrmndmpk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lnjtjxxw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ynwttvxv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pcwertkk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3balhaipl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ragmprek.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3yaymjsmk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zbcxqjth.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tlxkqyyp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kcvnuhfs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gfvggavd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jcazgkup.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xojkzlvw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mffbpvky.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3yonwmvzv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xbhauoyx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fzaxpcsd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3agbhjyhy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gfsatjzq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hhxyjhpi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qwgwtfqf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cvfdgbgr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wfrhxgap.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vypcgnxo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xamuzouj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbsstfa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nhbcmhxs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wgzdunxj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fvmxrkjb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3howtobjw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3amzfhmxv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3oprorhtr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hzjquftn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pdhcedpd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3evgdmjbz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dupidlwq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3usjninck.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wbclkqjo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tkibzhgc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3csoopcma.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kvmmjbjj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkdxgyk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cumtbuyg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rzxdtrui.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3doxqxtjn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xvnzqqxx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bhjdnybn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3amtalzrt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vhdghmkw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3puiwszph.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3plyvbxfb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hassuqnb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dpxsxsah.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yebnmmdu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3upgqlkie.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3gcwnqcfa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3mqjffkhe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fpunpaso.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3iaqevsel.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3codgexrl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hfhinyso.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wvzhmucl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hwvegoyy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3swsanyth.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jwkufclb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rjcfndnx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jfzcbnrp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3uoloxzgc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3thfejeip.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mnzogdju.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jebauvlv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zfilpqvo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3avotwaiq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sazyewec.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kbyzjwiq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rjgfpbgv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ritgmnel.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zgxroulk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3prfyndne.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uthnkqxt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fywwihag.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ybbhxcez.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3izndnfwf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ojdvsmkw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3iwkbauit.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3eevldnhd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ljjqafyx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3leschday.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hwcfmepy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3adrretrz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xzwhmcrg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efpcrhjm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dnfrtbqu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3jiirjfiw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhfszlrp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tdelclvx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dtnubuuo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3glmpcaql.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fojhvrhk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xiizduva.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3bbilzgxz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3scnrpgou.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yfueqlnv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnrojwm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dprxllze.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yqnyjiqh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lhzfuxgo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iircwqfk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ieeqgbbb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3odddoiym.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lmcillwe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kmpjukqu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3edleteyi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tthekzkl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zzmlvpln.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kteujynm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zjarbong.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3iwwoebxd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zwjyienb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dctkldsm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vrdclets.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xmckwssr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kuacqstx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jvvqdezz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lqhxoduv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nhhnprgl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wtezonvf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zcilgjls.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3uuiwrqiw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3quhgzspz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3thrpjgcp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kagdzymq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3egeojwkl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ucdqtuoh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wqeprtvd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uvbuxitg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ddxjusww.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fnaspvpu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rogdmglz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3imdlvmvc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3nnmrwneg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3onkgetxj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mwammoyb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fzfacfez.html


<!-- 参考信息 -->