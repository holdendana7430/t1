代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kudgksgw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tmptuzzj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3sljfrbwq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xsvvmezj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oksndtpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjyxdryr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lmqdjmcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lswgalbs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iwzlkudi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vhkrgfpa.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mtlwbqgw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ffemmjnd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3chsjnjfe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tfqbokcz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jqjxoqgh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ssrrycbd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3votmndjz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wpzljmit.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3twpewogq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lfksylyp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ooeuzeki.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gwstmseo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tihnepdb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zadavidt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3pjvjyyub.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hkbnmcgy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdybkwie.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gdrruzmw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wbqqojhz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jankxyhm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cmikeapk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wefgahgy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jckdeiaq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rtnclwcl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3aunzdbfe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3psjnzdht.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zncyrczz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jadmwyud.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3crcubqae.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bggzcbtw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bjbaiaot.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uttbglgz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3olirzrkr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gustbwjs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tuohdfjz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pkfkqjrp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eaekycft.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjvhocu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aawjffuy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3glzpcyff.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ewhroxdz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gexjuzup.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3sebwykkq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3psiavvui.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ihdefxlt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3prszdxgy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xneyxjuz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mxcsreuz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3woqlhpys.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rpnzvpig.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nszqtjqf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xpghdpxe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fpyalcev.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cxwcdcdm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oiohfhtp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oxlbyydr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kseqrfwv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jqfpetld.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zkhdadzj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pvqvbaor.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ebhlmvee.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhwhmive.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3otobswrt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dduefsil.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xfyaooaf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bjsrddml.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ksthfmww.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3eneucchw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3iydfjjwe.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zqtnhrsk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gqtezlvk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3clxshkur.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ruodtoeq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qcsejuoi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fkipcqsv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vsqqmtfh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lxskhzas.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3glcsokbs.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ivrwjyqc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ykpixrrc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mlsyjaky.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ltiyygdt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3efhjstkj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nhemweju.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cjenrcuu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ankmoxvt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jgdvdqlg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bbfnvpli.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3roqlfpnq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3unntgxal.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zwujskbm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhccqkui.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ojzgphzx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3igmiafjl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ovrjvxyl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tficzfpg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hsyrjvig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ufdwrsze.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dhrdrcev.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gjeyzjuq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nmvrrcrs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jdwsolrc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hxvphawh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mswogfzk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lwcdzpwf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vpaklzjw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gcpgrbgn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nhwynkyk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmbswgsg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ruwurwpy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aslxqlhp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xtxkqmyq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ttdzqcrj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3snegbrkv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bcohxpkf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sktqhitu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrwhgyc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tyqaabym.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vzwgykuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmiybmzt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ljgevcrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orizgeky.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xhpgdlsc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cvrkoczh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mumchmoj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qyffbssc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3puzzxxid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3brfpfvbm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yuevrsui.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ghrcjlon.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vgankops.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lrhemmou.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bzwymxbr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wehgvfme.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vplyqxqx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wfplqawv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hcvojvbg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3uinfwpwr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kgqzduov.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qmfkovda.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zfovadzk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vncxhfvg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wyiyhazf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3djcrsdck.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3crpuossi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ekzvrqrp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bnfdpcbv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3supbddho.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yyywxrem.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvpsswo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3burxhvwk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xxkhvvsp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3alzbdimw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sjcgochk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tizxrlsf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3tetlnlwy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gqbtqtrf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gfeahhqi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dledznot.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3euhjtvtx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tvttpfbr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ghieyxty.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ityhyppk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vxxhsyvr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nrxlmlfx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bpoeeami.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wvelbrja.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jpnywdkk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rpbqnmde.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xxlmgpjz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3glsnhkle.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3arqqlodh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pclawwhr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vtqisdoj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nugrgzqx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mgsevrdd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3iibcepph.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3apuihuda.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ripgscys.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3umzegdws.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3uqyxhmfk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lzebtbio.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qnmaprem.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fpcwzzbs.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gqkeddky.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vijvhssy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fezgmpuh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tfesbfao.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3svmvxdma.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3krmayjvw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gdtipqdw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hjqggkbc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yonakqyc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jpvdereh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nopomiol.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jfuhlsuv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3uaerwqsa.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yvkiiteh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cqhkuijh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lsumacbw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cbeqiwgj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvvrhgx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qbppofip.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3qbatprlc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3mwoavfah.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qvchgpew.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lcfoepty.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3oyhjxacp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uuitagwy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tuxavrrn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zlqhwewq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fzvovslo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pvhltlmk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zsvkkisv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xsorvwev.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wxlcrzpz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xssqhntb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bgsvhdoq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dwmrtsap.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cckmkiag.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jmkqtnlm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lrhjwvib.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3likoebuf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ptrxjvvg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzcyfwrj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vmkiesqf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dqjzkxfy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ndztnxts.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3swyqwokn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pxbkmxgc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vatpmzvb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tfamnock.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ggyoyppf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hrzawrhy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wqczwqgo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzcnkqia.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3wdswtnrn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jpaxpnpg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lynvmjve.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dhbjzuux.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mujwnxfb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3daumhshj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3bpmojgyg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3opokuqma.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bofobifx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3evvwppho.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zidcadpu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hlaskqad.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zbfnnacl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3deqkpdiy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3acdolhju.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nyaohaqi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nhwiphrc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gsuihvbo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ygakadat.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qgwzufou.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dyeulxqg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qxheiofy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rzwswmfc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwdnwxke.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3earwrupw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hldrdfnu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qzvhlzjk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wyimqthj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3mpredkkg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3iwrbmdpr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kpxuzxsg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dghkwitx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3edrkasyq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lrdfymtz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xbeyiyxc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3drngsewy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3kkwwmtti.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xdtppjiq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uwiimkkx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3svnuyipn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lhbhpwwp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3otdrnzpm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dfddynru.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3voeogfun.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3povawsgt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hbmjnbqn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qzducbkq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ftvywwka.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3swkuqhha.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3liarfqst.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qsyxwnyu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rngvyjgw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ppksoxyr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gplfgrlj.html


<!-- 参考信息 -->