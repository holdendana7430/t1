代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2blymcjzl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xqfgzfsx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wublohwx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xgrbbtas.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2khzudrtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luiddapl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2amheassm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohjdgzhd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tfjqhvsg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2slhpxezx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tuuibosv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2unzjnysn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wmkdhkbu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wksxiuoj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jkpxlvwm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rubqfqjm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ftuhwnox.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2eehqawcu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vjynrgta.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xadcfgaw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fdtnllsc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihhpjewd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cfatptvb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfbnhnk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xfbklwfx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zdlmqxnb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kosjfxlh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2iognuzqp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cswmmnao.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2pkoqzhkh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yxwywgoq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qrafekde.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2psawrnhf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hrifqfnx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dfdkkkzz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nxfsywvc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2aqyttdrm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nwmikmxf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ybtarzfx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cfaihfog.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xagbulsw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ghvehoxx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2szpcrzrh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dibvydqi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rjozvggz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2fnkklaao.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fxuecwpm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gdvrjrtt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uqctbxou.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rpvhipou.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hccocwdm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fdvixczf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cuobjlze.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nlvzdzcf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hkmdevet.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlsofjo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hfyrtxil.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ubhspocd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yulodkoa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vljivqin.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdbrwf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2egquhdri.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2icnbwtxn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pzmefpvm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kjjtjxrq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2dlmlppeh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ojdwgkfg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mhloklan.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ieznbfyu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xleucirj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2utdmcapa.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqynuzex.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zusqxkzx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rpzmckmf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mamfzqhd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kbvuyqmk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2eyggmcws.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2yytykkly.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2onbrrmfq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aookwxji.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wqaespko.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rksgmlpw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lpfjuggf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lpohdfkt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ewkxyima.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mvcehiod.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hybzvkvq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lobmpfem.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fqdohoqm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kemijxkk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yupcsvtg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wukznpfe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jhoqyvne.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qqitrjfk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ppmgbten.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlnoeith.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gsttezgz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjetdukv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pgbcxjyg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jhoznwll.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vjytypdj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgmeybk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qgfbkmac.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cuormavy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ilehgumw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qennpfyg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mlehbxji.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2eoesract.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xglkuppu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2piiuhxuh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qdzrhniu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lirlcvdn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rxvtvlvm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bvuhktfz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iplhohsq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cagkzjcy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgiekol.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jpzomzzs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvjsafdi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wstnkkcc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvbuydr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ocxqnutd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jiikfdhn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hqhzdkkk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mgeaaibq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qreqovxx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ukveuajz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2gzplphkg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nwheopnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzxkdlyc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2icivjhuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhfdwktj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bpdmtxyb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wmkaqjns.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2celflyyt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2siacdlgm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2juiyelul.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2difyolti.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rhivhgdh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tczroyov.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wieydwoo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lvjcxuut.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dfgcnzae.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2qnvabcyp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2szbimlfc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lwpsrzoa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wffyubmv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zzkatoln.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2uevlwflq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vhrwkqnp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ruowwfej.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lqyrnfpn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2quszvszk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzjjzztv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bynmopmh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsonsrci.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2haqfobfo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jyheuzdl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xqjmhllx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kpdlthwr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jkwbrtnl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrlghdz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2atqbyfss.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uoxdvjwl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2sbxcpljc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mbphjiih.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vberceyp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2guagklmj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cijygnwr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvssmixq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mlavdrsx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rxjigzfs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nffxxocw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jjzbouua.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qhpdompu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2plrgokly.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyhogvmc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2medxaycu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2yrlwqxde.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfvvjiu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qtlmcnpi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rireftaj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cpvjngwb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2buktytgd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2oepjevkp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2cpnrdpjz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gsuskkho.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2goazfyzd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pcesyxsx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hozlseme.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jcvjudxk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2astbysuz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2oetfopga.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zfwzgkro.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zhaodpmr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ffzflogo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2yugmehom.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wboixnvk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jkifderj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2emoiaooj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2micfqthy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2omdlxtkh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ootoaneh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2csfobkze.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vkbyfjzy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2addoejpd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kknbfpal.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qvgeyhef.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nnhoxuwh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jetvmast.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yfvccvhv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2crwkqegw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ybrwhozl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wkdiyjty.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dihfnlwr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxpyilhn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yuttalck.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ppqcdvqv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mrtdcovf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2odstxjuc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dprwmqqs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tzmxyikw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2utozqovx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dixyhwlg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vmylwbky.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pmladfql.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xdvrvqyu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2cbnuylhs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nzejvqxo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xdbyosyg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2csqrvesa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdnkifyj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2oflpvhet.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ampirsvp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdxcyuqb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wijnrtvp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2obnruomr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yyjjtkoq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qtykypdr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mddqgebf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gumakvsp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nrczxnmx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2euboycyw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nbwoxllv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ugbmvkfe.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2aavbnbea.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2omqarguz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2yzjvyjyz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hsrfaavf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rqkhiuyv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2viwjfnzw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gwdzcyar.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rmjbllyp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wumojwpp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mnnosjap.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2apzrwdny.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cxobjoqr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nuzdaejb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2urznlwxq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nqyiqvdl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kyeaqtmk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tiitmgzg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2novocwwy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgrbkcqz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2bipfevsr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cmznddub.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2begxczef.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pnfloomp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ifjhqrlm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lvfojuek.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rqjqqgsp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2umqafmmi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iumoiwpw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2btwvfeic.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rjityjdn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2polymagk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ivhrouuc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2bhzbybiq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jsyvqpww.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2nzodvxfi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fkxziamh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bfrgougg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yotrkedc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bdzgmhbp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zcjjeejc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cyzvdbwm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xvyprfoi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hbdzozfz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zovfovjn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2eibvqnbh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hnbhxkcz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ssymluyo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zvcuqzqn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qrkzmmyu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2lbwnvcxq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pbgnjakd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hbirvfnb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dcryyyre.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2czgletmn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ihucnbwj.html


<!-- 参考信息 -->