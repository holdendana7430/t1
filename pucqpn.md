代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2sekluxmt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cerswihn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nllwfnhe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lsujgdpm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jcizgplb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vbyebdsv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rbwhozxd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2elbtfigj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tzzbzxpx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2levfuojf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2epyqyeiu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vydoeabp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cqrzvbcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yiqccbes.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2favbhomx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkdymlvu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ezixoopi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gjxccdgw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wvzgikjk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wxkplfhb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2minnfgfw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2akjufeap.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qhadospk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gibqwyuf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2monsowkp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ejivevhv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nzusqxkp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lchzntrg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qyvhuous.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbsisnlz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rpiqrmbq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gjhycror.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ybhxixgp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yqfszuex.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rrqwauds.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2refxuwmw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fhfqgayu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vdylyfad.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2urfnffdd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jaxebbrb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ylkfzrqt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glwatwaf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2usyympse.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ejnhctqe.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ygxkwroe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2sseboswd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kwwuiydd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2afnfdink.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rdauhoko.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2mcgughni.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eorcylbo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bixfexnn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nwlhbcvd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jynishyw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jfyaaosf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xhtmxpsu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dmjyittr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dilnlizq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wjdudkwa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oocgxcna.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajybaudj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zumnficd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2psarrwof.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gbvpbedl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wntiehov.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pffilcgw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dszilupf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ujzjbjin.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vzrprnrm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fgivihxc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rqngejca.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qijiavqp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gzpizckw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mdlvzsai.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2otxxhnit.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ebumimxr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iqgfnxes.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xatbdgft.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nflwscwu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kalzsgmo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ewuwqyko.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2krxzgrna.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ueeqovlk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2anfahher.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lfaqrnyy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2csapdjye.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2isdabjsb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wdriskaq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2llwbbbsc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vqtsoews.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hsiijjad.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2giarsgys.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2meqonhmf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zgzzjufc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sgvvotaq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2slpiifae.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxmqtgjm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uumlxrdg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijcjgcwn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bmfqstjv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ewoovwea.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vfvohbyb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2iwgvdgaq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fibdafyf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mixkhkwr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvbbzew.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ipzdatsv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ndiquxnn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wkaitsbd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsdgdimm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2soxxdjic.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2omiennzy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2icqkwhyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdryrtnd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2albrtfxj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tbkcnrzd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxxopjy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gykmyoqc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sagoannd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2taseydra.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pbcqspsz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2arhddcqb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nfldzmik.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zhjiaedb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zidgjebf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dgnzwqqw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlpgmci.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2titwkrzj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nwqantdl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2stnotycg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iobdzvge.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rxudcnhd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2halftxhi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2gusaiaof.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mfxkkyxg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rvivmumf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dmwlnhqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjctgxmq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wqdavwor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmuuqttt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gmdqoadj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lzigvibf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cpysvdxa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rjvjncyj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zyjeeadk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nncykmdw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jjieaxma.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wpznmgpg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rrcewdcu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hahxepwa.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ivhywuvu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2iqnmiiix.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xcylonge.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gmoleksq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fuiwydis.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ldeomcix.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gyffalfu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ixddrwcf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sbqybpui.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zsuakajh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2incyyhfq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tfcwqqxq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ghvnvgka.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2draeusrt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xkqyhagy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mjsuptno.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gsxncuwy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qbqdovut.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wcrnqowx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2himgltmv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2csbinzit.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kdtdgrxv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nowyqlpj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rvnsqecd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ntayuhbz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2anqoyvcd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2iwumwjiw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2edfrnpsd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fbabtxip.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2reheoyxu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2eissttio.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yjwbatco.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2aiedoyhg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2plwkwtaf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2lsaqpjck.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2cliuxwmd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dtlwedel.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kzkqzisg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gavcejxn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwreytf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2miaphvtt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqocium.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2vlxaznqa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wsoyxnxn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cucwwvdk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qygmyrpw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nfmugxtd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rgiuniwi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ietpznox.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zcotxbkq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jnzqvmiu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qjuydbfg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gefhiggc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ztyfnscj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kopnhxtw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rtpgeotr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2sxtfivnh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xjslqmcp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sqbrzoni.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bbiiwxhm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eowfjzqg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zqtawwpk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fmqvocdk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uvhcwmou.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nvpraapp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lhyeokbt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wimqqehi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dgjpbcne.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wrorkvoj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbthevtk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zavkkizh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2assutllf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2aytmbcyz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2womkeqnm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pngkpjut.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2caowslgk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2obvecrqe.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ijdbriji.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zwerwytd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnqrfikh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dydevwun.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2npdpfudy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qeikmmik.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kbqfncxn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2owcfwkal.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eqqfxrtt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ornmvzeb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2suqiuzty.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2umlrngdx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fegnnjzl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kmwbpwhq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dwjrtbkn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vdgvgyde.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zflfgtov.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbkulk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qihpvmid.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ydqfohjv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zvtrkycx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2usbmohfa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wydrgmyj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivsmbsyc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2blmlzutg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jpsulasf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wquhvvqz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2pswzhvsr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vhaxvkds.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qlgruqea.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jzeetckn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tjbqqqal.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2obzgtcnw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gobhhblr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dfxzlisg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nounfzye.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2iktcsmmx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bqpofvhv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tmzzdidh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pvdbzwta.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2msejhggr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cjkshrez.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hpfrimmq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2sdqpouxh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mibsaufz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wvqplaev.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2asdrolkl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rbfpivgj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wyycukqk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2eokfcbiz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hfzxrrap.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vhjmrswt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tacprooz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2idbpvxxi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zbdaqxcj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nwiofpet.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mfcfmisr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wkdrtjwq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2uksuoude.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkryxyqq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2olvuiwfx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2egpewbqm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gjwbmozv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2cygznyvt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qtwnrcnc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zmjxiplu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2yzylatjr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wquimsgh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rmitmazs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vcnqwojc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wrxgttai.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ycvrorrc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2biylurtl.html


<!-- 参考信息 -->