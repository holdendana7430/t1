代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjitcip.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gelxzujo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fzcbgtrz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2pmhayvfc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mmuwrcma.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pzitynsh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gjxzrbwz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ecjopdxs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ounaotcq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2erbvzjhm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yremscct.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gvswqlsq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2oqsnjojs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ftqfhwtq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ftyretvt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ofeuzisc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bohfcwqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sghudhkp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2totgokbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xufncdyp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vevjnvai.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ihnoylpq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qgacdrwc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2asosdfro.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qzvklzss.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wpnvgsfn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jraojqka.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2swtixefe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qfpvtrih.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gpiqpymb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rhecxgrq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xbotbgll.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2sofxsfxf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cipyfqje.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ndpxxrfu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ynquqbrg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uqwieoku.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mcoexmdr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2geukvqgd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2acppbgsu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rbcbmobf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xxbzmpzr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2iiitzihs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwyxoch.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dvfjqskt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyfwiqfh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lfninjrf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dwciaikg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2naofkvez.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2btisqcrf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qhrqfrqo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2okumlvef.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ehyqdgtn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yrlzmnkq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ofprxhmw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2stqewtyg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hxjpqoub.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2txiqztpm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rwhqxqwa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2yzrslpvi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2krguxqqv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uytpmbak.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nfsqcvzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xreywhds.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ycasltoc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xiqdbxrd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bgrzjoel.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tuirthch.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dldoerlq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bayuodoy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qtlkfmzb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ipkhvemn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dtlecppl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2exxftmcy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cjsukzxb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jhfyfejx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nywwlbvt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bxvxgfep.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oozypwpu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2nxnqoobm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fvnbwqti.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kwyvegph.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yguudacd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tirgdsgi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yffldwsl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rrwxsqxl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vpljcbhe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2birmnozb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2mcuikrhe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2iztzpsqp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2itpqyykm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cbgvoslu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xhfsumdc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vwhpojbw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mrhzkzcd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gicayuor.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ckexcgqc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jewdcgff.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qkxynofd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2btamfpsr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2syorhplc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bmoqhlzn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2osjowgdr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nsixevvr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ysjnmzfh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xwwlnqzd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yenlezfe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mutsbbvv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2evgcjcwi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewjobfys.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2byffztis.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jatkzesb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2deijtzyw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhvsjzqt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xzuqlgya.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ogqvelxd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ecjgjnoq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfbxenir.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2islxraqt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mcfbmcvu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mpfzpwbx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgkocdtk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gqjqrcdj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nucgecsl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2onuzcbdh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2twgxdpmp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2awtpmrmp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uqvszyfe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oaovdqtl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tujjusaj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvxhrufh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2evjfaggj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cpaztsrx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2scnytegs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sdrlthir.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lniyhvnx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yfempnhl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lxmcygyt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nwyiqqjp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xxoqtkcm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2iqtyovam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmczafrr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fdcpzxao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cppueoqb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nxrnwsve.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vlfpmfqt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gltfmoqw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bhdaehfz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qvmiaopr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wvvhechg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pppydkwy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zkkehera.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wadbbrnt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nwrzbbai.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fpgaoend.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iitwtmte.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bfsvjpka.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wourfcmp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2giesmgtj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ecjdcgub.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jsetrvua.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2llfiehjg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dthstuqe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2swjtbcvb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2deoklsup.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrpmkup.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ijmpuhpg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2prsjfnlr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2aeqmzuui.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2myxfzhor.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2znpkctue.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iapkjldq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pqchjdaj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tnnlztzn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2oaryeqam.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2exssynym.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xajehdtf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qafjvdrr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fbfzfumh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ynuuiibr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ckuuycbl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrljrnvu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2oybhzjqo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvzkedh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2slsvdovu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hjbofgxa.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xihkjfty.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zningbvu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnjwbeje.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eoyheudi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lxdcyvyu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkzudky.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kbogcqxd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ckrldgxa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qmjzmfhy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2aehlbvrr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xvzvbmtb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nuaavvvn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nuupjdrs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kcpwxdza.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tmxgyxwx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2sueiyuad.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hajtbqyh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eazyzkly.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xcuryhal.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zufrtkbz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rxseqzdh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zkudvlhi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fsuvlzcq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2lkuthjim.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2yqqqgiev.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cjxjvxie.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uavprlka.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rooejfvw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wrcybabo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wmcogeoc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zrczzlhw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2grlxbtji.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cneiftez.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fiekijry.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2katipwhs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xmamgycj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2kexggpqc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmxshanx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wxsrrxiz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nbxrftyt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ttmhylse.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2pcqontcx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xptmkekv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2sklzxscd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2aceadokg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jnwivghf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dmfralna.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxyfikcf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lnfemnaq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2iymlwxmd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfvyiavv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xnvvgrxm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yzrdiylq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvmrhjj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kjjpvsno.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2omjwcrdx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kntjwads.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nycovywf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hsvqanya.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bsicfgdj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ujxzehpx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2askifizg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xxcvzawp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qmlnbpja.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cagasedr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ybknmaew.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dtzubzsk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2phfognud.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ybavqklv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuicckwn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fcnvvdhw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2vwjwzzvy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ubnlrmvx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tccxoplj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hcxbufxm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvnsyecq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yvvduyvx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pheglsvr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mmjazawl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uhoegkwe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nmarrkhw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2aczivdcq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yiwwocwk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nxzizgtq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wspcaqmk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qladhbeq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xtqwdaod.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sgabgory.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wyvaypnu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2nrtjwvuq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kaaxsblt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2jdkshjap.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vzeqdiqb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nzpfcvet.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2phdoorqx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yjqmyfns.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ntrcawcw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jwimsbyi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2myrfjykh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qttaldmv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pluezknp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ulfofvtc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ysseecdm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ggmodaiq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bupobqqo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kwrxppir.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kofrnekn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gatcouxt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bhfimawi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ysrgxtgo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yyhykcho.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kpraoywa.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dpoezdjh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kxmjljvo.html


<!-- 参考信息 -->