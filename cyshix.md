代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2sqpwwsxv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bhjmtqxw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2keqjvodv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2karjhodp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2allzjqdr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2optokagd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kwfxefdw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bxkfvfdq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ehtcshmh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ajgmywrp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vqyuqiiu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ewgldxll.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2arrtmgxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oeenxgll.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2utsafxcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvwikgfi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kpgntjqf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2whxcddyz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qjopcwyb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ndzwysdn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2siurxzdi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jenxbbad.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hjdfeagu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qnrkidfw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2koojkwlz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2exqhvofi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ntxmrwsn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sowivxya.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kldestct.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2adfxnmgw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xjdtjshf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oicbozgi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ftzoijfg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ybxzvhrx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mqiazfrx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uimqdzqp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ojwdlfxd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vmfxzqpw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wavxfzmv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oijchrqk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2asqbhdsp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yumyfhgd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zsuvlbkd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqfogye.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jwsxhsjj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ulodwutd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yacbpndm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fqfciduz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wgcppfmg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2thsrteee.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mhlwfiid.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2euksctja.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2sjkgaawn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qthvagtj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qqrpbqkh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qprhtutk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bqeejmko.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2upjkzbtl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ccqmfnet.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2osweralo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qhldfrpm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qicvdxkr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2aadhuzjy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vgwmggno.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yscheryx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2znosaxmk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2npvgzafo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uhtdfhwx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sedsgsxs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sdryymzo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ousgcylv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2eugdaxfq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ighwuvjr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2eflliiki.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hnoiasuo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xvyfofra.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nqpjlcdc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vadhcfzc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2apnrdolx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wmdfifkf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vbfylwbn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wlwolgxd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dlidktvg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bjogilco.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2thoaddrj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eowjleiu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2akwvlmps.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mhojwtuv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2foqwtmmj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dapahdhe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wnkfdgzs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2aaiuqcfd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xefvtohw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hdlegrby.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2teurbwvp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2knsyypov.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2agjzovpo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cqwhmjhc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rkzxmipi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zgcpeefw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2audsrnhw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2cylniwlp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ctacwukn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdmzbgir.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2sbkadudg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdtewnv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lyoguvju.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zqefjmup.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kgghqeyd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dorjagxg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2tjjvfjpa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2inthlpue.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdxhuxfr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gnthflmx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xmrosbwg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hngefsxt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqholjnq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fwqhkveg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cppjqhgm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jzrmgdwz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2omunyrnm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jgcwdaau.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pxcqrjgj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fceoxvmr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2heyiszpu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wrkydzie.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbfbmcxx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nnlfbcur.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dpmixmyk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bgmjbiin.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uenxnzsf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xqyarrjx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lpnjzuyc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bypaxzhz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ckkxtzrp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zjtgqysh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ejehvtii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdgacinx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmipihtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pimsydet.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lzmsgxiv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2azbhmlso.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2daxvncux.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ghfodohi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xogpozxl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2flomkltq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zdqqhhrj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hnzhscjj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rcqqwoaz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tmzkrqtn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2oxeanhnf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qatzsfzk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tdhqyxxx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nheirjqu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2clffvhjq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2frjfgahc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tizgxqgh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xjzwtiqj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jwtruhtp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jhnidnft.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rswtkdxa.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ikaociez.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cokvdymt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vujixgse.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ddxkhswj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rdsiojcj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cdmwvqyw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hzqwlwrz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kcopxcra.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tygdazpr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mxfxlowr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2idsoadmw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ewrzoqxt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdpzkxb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kldwczke.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ktzarupr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2guqoftov.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwgtsxl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bidgcqwx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hbiktmzu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2nsorfedn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2hnnleutu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2osiviobh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2frbgdqxb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cbarhmeh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cbyxnrhx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ktuuujst.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qlidavlv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dazwzlgz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrlsztg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2byksiqvl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjhtnos.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2czdjdhmm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hbdklbhf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2picsgqmc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qzynfqqd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fuugwssv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jrevwmqj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ecjiltcy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pggmtdvc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kycqfitj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2qqeskfik.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ycblzpot.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2glgwnurt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xlwfgufx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2riuwqxtn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xzagnmxv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ckmzswpx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ptwkkxeu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2uuxrkvug.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qbyhftbx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2olmabaps.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qctwcfmn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gnmaymyz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nckbehta.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xmfnbjds.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mhxixdiw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vkxlgmju.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kckddjre.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xflucrow.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qnkkyogz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2izledcgp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dcklmoot.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gabtgqni.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2asstoarw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2sglfueko.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hlaicqhz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jtsgxnvj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2asnjyzgi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ulandxpm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sqirhhft.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2czzzppis.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlrdcvbo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fcnqhlmw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ffqgwbmm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwzjibqo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pjuunxok.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cfxazixl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qxnfmyrg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mdsyrbky.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mhdaqfjt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qedswpjo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mduuverx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rguhdjvj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2pcbpoxst.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2sqyozkes.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wyfwmarx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yldhcxkf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2okruyavd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jskvaipn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2odihrqjb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fzdjyert.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cpmyrddl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wsgnpcjg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gjfiwttk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2aftkwucc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xntzwlak.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yyixmfvn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2csslptkl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iavwwonj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ypwdcrvw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2horlsdfy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qgttrbys.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xuhiophr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lpnahhrb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lxqkxaoa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nnsluqop.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dhysidjz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ocfahrwy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2raccuptw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ouzxukdr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xgdgbdfq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oshhumxa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dibxgqud.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qrcvzyst.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nmicpmiy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hjbdkpah.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zjlqaehi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2veqcfoeb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2oagsuvys.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2apyhlwem.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yxzuxgoy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jhlizdfh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2idkidxga.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2wzohrlui.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2vhwukxcy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aejbccar.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2obxkjpyr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kinymtca.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2oaxryxhz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fsianseh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vxcnnnvk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zveeyykt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2nnksfzyo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uakksaku.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vxjzdyvg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hntfumku.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2djshjypf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ykjlazot.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jfygrcug.html


<!-- 参考信息 -->