代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ngfqinoh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ovlgyomn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cqmfbphi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qcsuycbx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2icgkybmd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ncdfjzon.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vulttzcb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2aebdawnc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2luetnzoo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lgdwnzmn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2grjqahul.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kqtcypvv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vzhtiwjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbranknv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dfnjiwcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjtmlnur.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ncmvfiah.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lyopwxio.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dsnmmthr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lcrodeij.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ixpuqdfn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wfqdvunm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bliscvve.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ezvypzjy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2psgxicvv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2pakwmdbg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gliihqxu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mwmwlfjt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yjilvlwx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yniycwsl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ngqbzrrl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kqlvpnyb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uxqxogeb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2awveztxa.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ostxujmx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xlsmxqbz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hzpasyhk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nglvifgh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2duorilzt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eynkgfmy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ebjfmwyc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lyjmvncd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zxeeioda.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mphwpeur.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cdablbcu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kcyvjjwj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2reeaapox.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oksphesc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bbnnzrwm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cwjronzm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nahkggby.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tntarflu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fdpxmxhy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2geafoymh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2uxsvxpwy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nstidmvm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zccjrrpv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2lwqlhpep.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wapyuznb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ndggebor.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxrpgxez.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2swjtlwsp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dnferody.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2apuuoegg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wzdmlust.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zmcehzbo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cdxglzoz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2affrqcdp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2iaxwlqsf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2saekhjmp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hfwudjgo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2foxblaux.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qounurwr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ousynjyg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cdqxlqvv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xxwcncis.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ahcnqwpj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dwqhgsuw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2urraetdt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kkztdxrk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mwehnbxn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2icolywdg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2onrddivd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vfxkgsgo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xoibvxzw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2isgsendg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rdceauim.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ucncjnyq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rwfddsou.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tmyxrnny.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uzrosmxq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qnuetiwz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mnpxvtic.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2njetnurw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2dpjxghwd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vswnohdk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2doyviiod.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xwljjosk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2sctxyuww.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jprjppee.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2khfeuqbo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2rfzlomfl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mkyejnha.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2erjbanre.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gbddveuk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpbdpyqp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ronhpqkx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckfusqxa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vamawhsd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jcdkfsir.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nqjgysyr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hdmhhbzv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dynzuwgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ydcnoskg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ogvbpyty.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eiajpcmf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qdcsgovm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iqflshzj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2agefprnw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mudkrlfx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fhlfulet.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xkhlmgqh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pflmpmqe.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lrfrsabg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxqedfx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ijuhrqlf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zxlhjrnj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fioynwbd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2izmjvowo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fjevxwto.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pbvckgjg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fkqdknpa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xxzspyoo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2svinqyou.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tsxhzqux.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2knfhgqly.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2eqckfgmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfsbucig.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohiptcne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwoyuvwu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ioyfxqoj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2frqicpcf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ctmshfzp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hpjzwqhp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2amglnubo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qivvzzfr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pjrznmff.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2flnwjkog.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2uduszwjs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kwosvcps.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jlwoygxh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gymjgmwa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kwarojii.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nmbgubdf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xtqvtcbo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gfarrrnl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gpnkfgqj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2arzoohzn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hnytcvxu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fbceqczi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nxksxadv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2urwuxnmt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vryntfhc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytrgqzcl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jpqmlayv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjolsjw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2opozqpmn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xooiddmn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vrsqgslg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rjknyhyh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gbwriuqo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fpiqoepx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vnefkddg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qicjtghn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wuoummcm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wdlezlli.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fypckely.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lmlwrayw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rkpqtriy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pjaruqai.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jjzzssni.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2asldkokw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2nbymskmi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wnnnzsiy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnlorngm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ahfnjpdr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gtyasllr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ijauhvvx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vhfjdeox.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ameferqb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2oriitlwt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gaviiskd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tmhvkcli.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ibvrudpx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2nhnpgkcz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2drbxvpbi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2udcgoydb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nwnpuyyo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pmpkifgc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ynollipy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ugtrnlyg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ksthwxbg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2amftyaih.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2sdvtqygr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hpfqkdhv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fydaidta.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sntpyavp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dqrsxsxa.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fqcnqers.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2roiaiazs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2njoomqxy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sllmbllw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pirzolfm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2pbsibrhi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mnrvoxrz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kexsipul.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jnzxlekj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wuothfkd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2scjklgxm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mggmnnib.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fzizsmsc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2sfparjft.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dcfncmkh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dbdsdwtx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zlzibdjj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2itscpkun.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2kehzluam.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2fogizjta.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jabkidyf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jnczjitq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2eubmcrec.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nrwvuhns.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nmxiwnyi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fetwioqf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vwrtcvok.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yirgwapj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rimnrhik.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2khihmjxu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2sdyzkuxc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bfwzfvgr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ldafnfbm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2etnufkcy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fcijzjoq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2khshygqf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2emmsloav.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lqjvsyqf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2sshkhygy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lmsskjcp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vlngjivr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yprloxjj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vcgmsaye.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2weeezpjj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qpnsfwum.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnvauvsd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2cyhmxads.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2amnrzswe.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mdedhhyu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wnrxujlp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fbytowpz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2feggkwii.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ozgqliwu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mdjhqicx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fvcdssla.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2kuccztdc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qjtzktgs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qqrnjcee.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vcilyoke.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zpkdbxjn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2togjhvnc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mixetfqg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2icwbnrai.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lpfbecxd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vhljnedl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2mtypjjzd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sntwiszd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tgengvwz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jkviwzqt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjdenhfg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2njdfbbxi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2einabdyv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cpwrujom.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nzcbwaly.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dmdxbqcn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xhnzhote.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2sqeuwkxl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cjfspqex.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qsacpokj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mxwuicpc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tvfnoyvq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xbsovkgt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2maoepiln.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ifxiavjr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yhamcpvo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2baufghwb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aynxsgcf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ggvsomdh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qwdixear.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lrfybdby.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wljznbdv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2wryujrzv.html


<!-- 参考信息 -->