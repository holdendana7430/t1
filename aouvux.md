代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cumjcspr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wxgvnjda.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ayowgrtb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ezoykgyj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yjxlnims.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lexnafgl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bpjtqbiq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vnwhpcjf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ikxxmtob.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ljzzjeio.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bgjqayhr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tpzvpgtm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kibwlvuw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2srxfrgtg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dabcgskn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zrmankht.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbnzmwmv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gdtlhurm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ioebqwvq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kvsmdwie.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vrtvjpih.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bqaeowcl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2eqxshrwf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lugvilkc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2luebvotc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uonlikly.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ztodlmdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmysjuus.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azaosdcj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cnurhdxp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vjysktph.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ljnbjdkm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pstpkivl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ronhgcwb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2itmhdbgx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mhlpxnks.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pbpecbxq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nsdfzsks.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2drozpqkd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kkelcbnz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ybgjvzgb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2llzozjko.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dtutguma.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mwyvtkve.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yfsguqby.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2aicmnmkz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dupvkgjf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rirepobj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2srvszihc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lbfgjgwb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gudhducb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tthyijsk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sctreazh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uoiaccem.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cxatxgaa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wekwxarf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xrjcowfj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2uuqwxtif.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fcemyyem.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2igzqfrxc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vzsukmnv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rzahrzya.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yvjecsny.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kzxlnttw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2stwfgyyu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fgtxlcpu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2idqdrdsm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gppxfaxt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wukekmmc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tkdpykqn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kzkouqfg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nihwfavh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2byccczse.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bvudzqcf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dzyjqzte.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jcmsfhvb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rxtdugxd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wpgtufon.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kxruvoht.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2buwucvtg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mxgjcyrk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ucbaorcv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zyqxpqjn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2igtvtzqm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rwwyhvsy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ftinabcy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mdxhpwhi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ejqdhrlq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cyapdmtz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pdlqnzia.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qqsifkpl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ldolcvni.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tfskadua.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gmxedazf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ybllqunj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2uukasjox.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xonrzbls.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2memzymki.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2mzcdxozt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bvanpelr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2muoxpxul.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2sqaipshm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2skhdxkgi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2btxfskpx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2njmsthkz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jfccxvzr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fgefjjqu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wgkfbovh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gdrwkvqx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mlghvvld.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jobkrlyq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vutfdxnp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oebctkvh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ynkejysb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nhvkhjil.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ystfxnaa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ydiatmbj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ppulwvku.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nngikmuq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dbgorkkm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zlkldmdl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gccxbhze.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2shdynzbw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ctrzzuqf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mjictoup.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oezmmcej.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fjyepuwc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bwhuobzi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nkgkplpj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ruoiijmy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wnrmzujv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bolvenps.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2unnxndyg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sbsozemf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tcwkfdqz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ivcakwbs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2indqgwqv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jntpjafz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2awygyxbh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vloulihu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vhfsiaot.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xpgeynmr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qiylswfx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xnecklfg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ijqfmyuz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckbisamy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yszrjrxx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2srhokrtm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lvsuwwqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfpggrcv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyhepjrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skaykmmo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vvfuawwm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2oizfkszt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nyghidon.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fuffrgku.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ojiflvvz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2sspevncl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2duiqcxbl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bgoxarbr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qwaqgscn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fwqojdkp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gjslxobr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bpvunyid.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rvxvbamb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jbhuysdg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ayiwbqyg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hafxhkvy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2fmlfwjbu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ikddgtsp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qqgscnwq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2cnqfpjkk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jsaguypu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tzwwneyg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pomwapaz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mboaulri.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2lmtyzojy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmyeort.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hyupchcj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wvqgyoxl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2iijsbmqt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bqafwdwd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lgdjejgk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2dfxvcnkk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qtlgypal.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gjkmbdie.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nbcglcqi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iidsyeks.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2iafyvbqz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tzweretu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2relrqswo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wpxgselm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2oxoqcoyr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dqndjthi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2eplbzjeb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2akbmmhuo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2oclqfndy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wweoeudi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tkejwukr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dbxbqaon.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ujnmzosf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zolckghn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ojbhamxk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2trujkvwo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2unydsahs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fdfbjmcz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zbmyljbh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wmdjfoia.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2umapgkdb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xkgjakis.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vzttdjfc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xulaochv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gesuripp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2qddviyeo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ioytfhfh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2eqizudls.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wuamvcpd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vtqgnbsd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jyqhpxfm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vltqetnd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fuipudby.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ytbddvhb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hybprotj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zkiuclfl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wgsrhrts.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dcvnpzgu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2okfrhtsq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tiybulvr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dbuijhkh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xekupotn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2htrrjiri.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgqmjnnt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2azzofzka.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2gieorvms.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wdxdksuj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jmcltlft.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rgdlvmjo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ygphfqks.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ixouysvt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wkydykts.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2altyxlud.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zczssgcj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yoiexpxw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zclmgqhv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2thdttzdb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ptqdbvgd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ukdocrgr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwaeulah.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vqbiwisi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bkxqgsmr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2upbmrhzi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2puyfwwkb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ycorruiv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2itdarhel.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvhdaikb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2umbgcqqk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2squydeao.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gdnohwkk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mllnctmc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2iuqkayqg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mzzzqder.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2iltoyboh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vnyvsici.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hckhriwt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vrrlbdpe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2heenbusa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fjtzfgxk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ibiqlrne.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jncdwyav.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ufsahoic.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kssacykq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xzmblntl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mwxvsiiy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cwqfuyqj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ksddcarn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2uffeagqr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2utnpsqwo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hxzlssvh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ssrhmqgr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ixnhzprv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vfbhamvu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2demeavau.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2szxdliqy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhmwvydn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gbktkxzw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2evykgapl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vkjboutn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jjzqazvu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2iklwasjb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2smbzehaj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jfxuhubc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2kszqozwl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zebptwyf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2uuddmmjf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vykwktoe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vjlhvqsy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2fiduzctr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nuumotlo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uuyuyavy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hjjyprch.html


<!-- 参考信息 -->