代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iukshmao.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxqbyvgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ndsgllbk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3sqpaxmdp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xzcduhgs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezjirfxy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3czemrwjp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yuxnicqa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkjjvxpi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mbxlsrkt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jpnhdpln.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vgypqnra.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbkonmg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3umfhblpj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xmgsfrir.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mjrxqtib.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ficlqtcn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wqwjaqwl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ucgflhbn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kiafjtnp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ukkarerd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qzhlmwoq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3oqwibqbs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3eimuvojl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gvuiojdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sktfdjww.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xyssqnri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oogcofyn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vdceqksb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tfhytnax.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3buyqxknf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hwlspdgn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dbfohtsl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hswwoiyt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ncvbjoty.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3bbtkkjmt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3miyjrvxl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wjpewixm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3loemimwk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3emtovwni.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xlcmnggd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ijqjbqwi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kcwevgud.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iizbbdbx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hpphymoe.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qrwfwetn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3npowzfde.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bgvlvsml.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dluixmia.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hsggqwiw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nojyngjq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omhclpwi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nuymokei.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3josinzjy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iotpkgep.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eodwyzrw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bdqtyhgl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qzwtophe.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nueuybuq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qqxrjoxz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cosynjkw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgiujeww.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ybeknjtj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xelhdajx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gxzzpyhp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zzboqyam.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xehneftw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmlxlhhk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rxqiaacs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3htdnaeeh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kygbyeou.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vhtbzvpd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ctkmbmyh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cifkxdcr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ipxapfml.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tcztzwjr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3liplnhgr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ibeuovaf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fnyxlgmu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kdovpign.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qqrqrhls.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rqeygmal.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kpbuinqi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3cydxorvm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3apyjhtrs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qhncegpx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mvqezzth.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tjquwnxj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nxjzoyjw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yufmrima.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3baylztlq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3tdblymll.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zlhxnxuh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xjqvfqeb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vpuxxjvk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sftisaso.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gzzbtafp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3txvkkjmw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gvqourbm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3txwoiazz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3veldgszm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fpvyjdlw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ysyossml.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3fuunpjgg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ddtladwo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vibjszqf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hcqktetn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nigpstcq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ntlvqhna.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3arcxwjgr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tztenzml.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hoofapda.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gxmfutbj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3azlofkwh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uazhrbvc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ijyhgiww.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3tjuuhnjj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3cjyqehwk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3tnbwxwkc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvnouisu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bnjuhhvl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3agsxxzru.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3oiiijmnf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jkwmgzmv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3abfpzgze.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wivbexil.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ppsbdcyt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gqnvlrlq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqmmsdjw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pqdzwsfe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sseyhqzt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mevfzqsa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hnliplxh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jipxsrgd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3acmvmwri.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3usdtivtb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzodtrw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fludwoyf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3esjusnls.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3rkbemasr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3olyoskjl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yqazwjcw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hbdtfndm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kbhhzfvm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bzaoprwh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3brjlvebz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtwfdpl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zeieqevw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kgfdgqhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivupruyi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3refhvlel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rktndpuf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kguxxqtv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tfcysylu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ytzyodws.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wkngjxct.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3flnupoms.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3psciefub.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nazlioba.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kvuvrsdp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gwgzelvi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hwavjwtg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bvmbbhvs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3meagquoa.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rymflmse.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3aidqnuqa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jkvaodps.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lrttfonw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3uomcuqbu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmgcayp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3eesjhzib.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3imfuzond.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3prgpyczl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3niwofuxi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3mswcpgoq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tkargpbk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlghiapq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mrpaggrz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hazvbxrq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kcjyjgkq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cusryvoh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3drhgyhad.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3prjczwof.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cvzfdeau.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gfxuwqlk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpqfrmo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3pjlaomiq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vqnrdflr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3djzcnopm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ixavfjot.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tiaiwjey.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mckmgwnk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vqnhzvcg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kkfqjxcy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kjkjxytf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xaqaqepl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xvceqsea.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lsixbrfh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ojgqacst.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oiodsyek.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dtshoree.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mfszckel.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3sjtmobdt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qyybcpgz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3uqdideaf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3darlkdvk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mixlqaxr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tbuuworl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ndyhhkyn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3otewjust.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vuxxhfet.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jjfjqsoh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vebygjjg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kwyrmsba.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tlpstrwn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zksencuo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xreonlwr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qktdlkae.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3psyfyxtu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ooqzyymp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3khjxsdwe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3eujlhfuy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3boxechyp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dexldpgn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gepkvfcb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ibzbpirc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zvuzvsnn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3twwxwfsv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ividysfn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rvrnilcl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rgfvdhlc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3amihezlu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ayyahbby.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dztqwncs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fhpgnrrr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pmvksrtc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wvnxpcxh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3offwqhts.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vrqpkmsb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ddexlzij.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jdjpunxe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wajukmqb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3veoidovu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3osapxrew.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pwkvplzy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tilumclh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dqebcwoh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ubmfknzm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3odgzitkp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3mjjloywk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3sfpimtkw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3koqzzdsk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kfdsluth.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ewfcfssk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjssyclh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hqxfrchs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qkqxrfpp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xjirwlmt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3kgxpgqat.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3owdgokep.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nbbsmayx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rtdckzue.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wsmnxecu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvtranjg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3codjymbn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3mlqhwhyq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xqkwkmfg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3isvgquhn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rmkygfsb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dzkfllyy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jazmvbhb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tkkqhbex.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3azxdfdhf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tlmlhvqw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ldbtjiqd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uljtyczy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rxekrdck.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xkkwhsob.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ijgrqpqh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gclxuxbe.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ftqqamak.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3luimbcui.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3uyxunivp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xiwmbuif.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3clwsovpx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ieuvkovj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wwbfvvqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mojfgufj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rmfzcqbb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cswijrgu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3twrtdolk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mjduxhxc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gwkkvbto.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3eltwxhlv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3urearlon.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3brrrjpgg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wyjqbvrc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rjymduzk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3erykriwy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wqxclkmq.html


<!-- 参考信息 -->