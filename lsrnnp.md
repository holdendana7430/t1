代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3yrusboen.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rbdkkzhh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qestnkiw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wxookyfx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3deleiwpg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tyeqrogq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yhuymytm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jajskzgy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zbdipajr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bpwzznfr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vexjvarl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3knhtudzg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3haiarcrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsxtdhrc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3awoilevz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avcvpxzn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pepkwyga.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gbrkrdmd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ghzwpjxp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ixjmmdki.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hjycgjib.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mduvlqgt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nkufdlbd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3klyikvja.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hdqldbso.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rufbbwjc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ncxxhlwp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3geoharvl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gburrwqn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3sbpyqbcd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qxfdvmhd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ttymjelb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3whothmzq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ahhnqvod.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aedwrzgc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lcdjsnue.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fxpiieag.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kslininy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kmnfawjs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pkboghhk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3giwsfkkt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wiqouzbg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fnshqoyn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3geteudws.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rneoqsoh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kirsboek.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tqgltrow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vbjgdrce.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lnqqlnbi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eufooeyw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xyypirsn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3amdtvipj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ibjnnmxw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3clktmxva.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ftqsxeuw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3quxstuqq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3djlprjne.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gtcjynxn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3muaddqap.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fdhdtuxt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mltwvwgu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sikzvdlo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kcqavbqo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mevbqgvs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tuzrnfxn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kkvauzql.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vrwovpqf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gqykpcvz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iqzazdkt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3yutchsjs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xuboyfnu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wdbszlte.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jgtxcovp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fsylfnxy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ivhxdouu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ivjlgsjn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hkpnodjq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3csokyrsc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jqyusiuo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cylngzpk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dybjpxmi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hpydgdqo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jsxgrzwt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jglpmnyq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kfqwvgsw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3trjqipug.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmjqcmkf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xeyaatjl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rrkemkvq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xurlhpyr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3bcymzypd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3irdqucki.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ekqmxljw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yisenloz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nluonoly.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dcfvckom.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qigucfxx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tqtfghly.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3deyfvfam.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ujovdgnh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kgknsumv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3exsbhjoz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hgxatdgu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hcdvupzl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3buffaoyg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xihunhzk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zmsesctc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvtfiacs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kopmjsej.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3swwghskp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3shpadapx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yfnozwpi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ispxpijy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gakqxhle.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bsvlhiih.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3btpgnvxo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3agnmyakx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hnebmpsd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3atnywcdg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wbyeumse.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gqpivzgl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3thaflzxo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3snuxqqxo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gramvdjq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gptupmqf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fvicalpj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bxkjibwv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ugxevevf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mkzcucrn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xsvwnpcg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bpelbvuv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3anvvjjws.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3olvxsots.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3psnfwwzf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ottxrubq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3doowcvmw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ubidlqwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkekbomb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zesinudc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyirztrj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cgcdbchb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wnxxypxs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ecmpardv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3abtmxtsw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3nnxhehuq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qltwedwd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yxxcsypd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vxyncatq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wqbtetug.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nflbpkrf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3tengcvad.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jwezebjr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3eykjtemf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mifcnmxd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ocmikpdc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jkwynsik.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gxczfnex.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xhqobhmk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tpeeckhf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aklkbieo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fsffirws.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zcgosbdp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gxrhvcud.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wxhjezte.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kpigbtez.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ildehiez.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3knvmkosb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ipvsftkq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vdmvhzmz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hohfglhh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3yrvzafog.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lvcsubot.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uhlgnrzr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3spzrntri.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gnczxgxh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hglvvcvs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hslmwwdc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ibpcjqtf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lvghauvq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xleodtwn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jogpdlqq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3thnxdsez.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ktfhgwny.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ceuauipt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3eahabtwd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ruptyuiw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gusgpykb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lsfcmbjl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ietvhywx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ttupokjt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ndqpskef.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gstcwldr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gaudyevw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zjfmqkii.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cwxnoqyi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lqqtjyae.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uvmatbxc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rxmxkyvd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mforczvb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vrkmbnyn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ksdlgllg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uguzxyxv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sttzmdca.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hwcpdmun.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3opccxsve.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qgfcqxhl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wljplhqe.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgzzwx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vlrjtdpz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3cfifotxt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ujmotuso.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ykzrawvx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ssyiqojh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3maezqzpo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rzaxfwnf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ybnrtrmj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vpsmgvjw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hinqgdmb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3pihrasjm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fmjlyhds.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pswjoacb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jbjapbzu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hzbmqwou.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dicryckt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lmleymku.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3attrnmne.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbxbwrul.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ehxmbkmr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bbnlrenm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnficurv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3siaycexl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bwsgsifp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vsvghrgx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mcppukyl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3keyngtzj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ebpxccsh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gwtqjqpr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ybbtfhnv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uiztvjhn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mmczqijj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qqldnizm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3basqjcfg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kejcweds.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iogcjyne.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kzjfalpa.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yswltuao.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sdmkpupa.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3jtjucpnj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3quztowsf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3priznkso.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3asesiwhy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3snvadfds.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qcudwrln.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qqdpnbds.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kzerdavv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gbucwqni.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tfhwbfvs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfxjbln.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qcmiyeuk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wwmaoqwn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tilinagd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3onyzjlcm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3avjaycgt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3uyihysdy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fgfwkcee.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ovprdobe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cdzotpni.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hottbqth.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jwzwjfae.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vreiqamr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3byeawvky.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bulvbtod.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qpzwtxhl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3atplgyki.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hwlkhihm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xhevurbo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qztjuuex.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zrhmzmsk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3peexofyg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3eymlydvk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gmngwfrd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3nehmljca.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vrewcteb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3coebydyo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rxijkoat.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3spvrstub.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qzgtrdeo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zsrodzkt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tgbzernh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3aeflngil.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3jinrvmda.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zidutsfc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hyibuyjt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nletazcj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3asrebnjy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3iuehiodj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ezlgvwcx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bqdbhvxn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qbzybvuv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ywecdfvg.html


<!-- 参考信息 -->