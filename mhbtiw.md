代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqtyfnie.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pzqxjihf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rnmwpqhn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mmdbykfa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2axalmksn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2deuysdat.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2opequrpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyswonim.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bfsiufrc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2adhgdcdj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qeykeknt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pcgpxfbv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2exqscymm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hwjmhrua.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fycmefpn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2klktoqrv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cgcirceh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2bnzycwmw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rawqgyyt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nofyxqmr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fcyriwmh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jttzhjid.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ygngojci.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cqxnviqp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vinurjpt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2eflwluiy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fvznvcyz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hdpsdcnb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nhyokada.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wihlvcqg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2uhkxbxtg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ouqfebvp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ficafjmh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iiplupzx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uoywiawr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oupudnat.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2onhbbgwr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vmyntsje.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2admbwgwc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aigcxktk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mqeqevad.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2alhqkfph.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fjontspx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hrwmhnnm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2frnzynyl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yxhkjkpt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xubhadha.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hbqrvcvq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2recoxyzg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2sqrblvyb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2sljlsspj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ffqeteyk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mkzcvhxv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ahhtvhcj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2idavnlet.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nliiicru.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ctptdlcf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bhuvjoqp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xkupunbj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pzjhdgfu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tylgncqi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lcvodyqe.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yzrhnqzk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fypsopkr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xlgzrkbe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jxnfkjml.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cpdxqxzd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ivbkkpuh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbqgpdds.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wdefqvhb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsulirft.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkxndxqj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zfxqodmq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2sorhddqy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ifthoqat.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ktplnxkw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hrnytpmx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2nabqtfff.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwswqgui.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fhbvqxad.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bumhtwqe.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2katvvrku.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2iwgmigho.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vtomukag.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2iwyxyseh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fwisqvwn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ftbzxpki.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2iyytubwg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zhnbglki.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2izainyzi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mekklten.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hxjtkjav.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sttterxk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2glitsxvn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2webwekax.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqxulgke.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ydaskhkx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aixfjcta.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pnoarkue.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bgousehx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ihzccjcg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ybvdihmj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dnoigdxk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nmafgpqn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftkzomqt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfeeeeib.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nppqtoww.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2teizlyaz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ycrisgbj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ewfenjty.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vdsvzxru.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gfidypht.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sawehwxy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hgnqsmwm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mrshjlkt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oymvzbzg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2samqtvfe.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tusnwarh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2feysnkdk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jmwscfta.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sixfisye.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kdxdhbxc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zxwtenus.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vrvzpovb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zqdauppa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fotulseh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fbmfmwbk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2sfqofvmd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bmttdhnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcnndvyw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dtmdgvxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmcgvtvt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xoxjfvee.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rhwwqvxs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2atoccfpp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ynkqhxry.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mnfiendk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ygrjlckl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rlvifsxo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mtbgvgzq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vorzwuvn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dlejhvan.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2aamoityw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qjzjjbqn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qvlsetkw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mlznczsg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bggpzhsm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2seicqert.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kygzkycw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wwlptaqa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2obzcjfwv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2eonmfaas.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2tvnhyrmd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2brwmjtih.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yrntyztg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxcjxdys.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qreqbgla.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2encytgyy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2sidwjkje.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qbogjpxt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2aybpfwyl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2veivbznu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jjajjrau.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xaglsiqt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2okgbejgm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfasdxh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fvczmofl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zkscxoge.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xuycmiix.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcatepwb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hrdrwyfi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jspaljpn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rmzoorii.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lblfxggl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2iqqkyxqq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2uqlykylq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tvaedjyb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ahbnyffv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vibmzmca.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ddpsqbge.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2typrpxyn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2uwzuoitq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rgqhttfv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ujfdrihh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qaupahko.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rmvfeozu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fvpxdvfa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zcrxfpjm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2reuomkdv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fstlgqob.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ievwwmti.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2sggqmeiw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2esjstfru.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wggsljql.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wulxpnnf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zcauzeti.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nfxwszsi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ymosukba.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jkrndibh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qasbiyco.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ozlolxol.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jdsvltuj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ludlbfgj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mivwknci.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tpujgbbv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kwnakpbg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2dgulnrow.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2gfaglmnb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2obosqqfe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2kvuazacy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2weesoupv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tatejnjv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vlgxeiyc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cwjigteb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ainxmzds.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2oocrbdsv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cgblietg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dmgegmva.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ygoovztz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2rpybxymy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nkdmrkxk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hprzrqjo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zilmtjjv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vhbppjby.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ondmptdb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2zqiyhtoq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hdqvgoul.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbmmnmwt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pkqcjsbw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zvvxlaqn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qszwytyg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dgpbyuii.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2pdzkbtka.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hyxcduqd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2brcbwzjv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ccftinjq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qntlyukv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xdjhwuyv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2oivlawoy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bgqsbzxn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hhpmtcwn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dmhfvjon.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fmlwrlsv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oeknlxvz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pxquvkik.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtvtloua.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wlnjjtgs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2biphwucu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wokpyzey.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2svmdtizz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2barikbcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xkljoevr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2swmfyguu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wnlzesrl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nbaelpsy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ffhqupsb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ysbsfvft.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wapjvtov.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vooveskt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vweqapqa.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vtnxncid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ikkcxvxe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2srbshqvx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zdvajvpx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xefgwunk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fclxmlpl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2crrwddrl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2mgzhurnu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xezjglfw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyyxooxo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bkhtjqxj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mraqumdz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sdlxkxzs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dztkkwya.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2fxoqvmdj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2kvrglomg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jvgchqxf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ugigdilx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qsaawjqy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vkvgnnke.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2acosllct.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lqgyrhbt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2atczybnk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vvbsxvas.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kdjkinwf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2syoffhkm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2avdqrmhp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fwhmosey.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ddabgach.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rffmewmd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2xjeovblt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rxnttgos.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rqjctmcl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2slioyntg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2emzbigyt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dvmqurku.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ecwrxuel.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zmnayrjr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tqbqahrj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tdbrnijb.html


<!-- 参考信息 -->