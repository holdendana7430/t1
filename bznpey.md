代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2toywisqu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sywkuxgj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ejrjwaow.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2behxsgip.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fatzztgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzuyueac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jnrfedst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umgxcclq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pwfabybp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gtoktptj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eemrcrnr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2givjpisp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rxlpcixg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tmdzoywf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2iiycmhov.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jpsjdhbm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qzronztt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lqnigewm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lohvzrbb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2haoyndyw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fgxitquf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2nzwpbsmy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lpctceqd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oahssgpa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hdrupbwx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hnbnyvbt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dchyxkjq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2frxysobo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vnufsbqx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2adxpygal.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nkdhecdb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2snqmjxyo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qcppqqiz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2oahufsch.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zlockmdl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ovasgxkd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fyqqyqqm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pbeyavxu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2goigyklu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qejsbiid.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2isakdtlu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nheusdcg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wsnmynxa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2seznwpea.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zycpsony.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2msczotpt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2khbqozis.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yjkzgzyd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xijavbon.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tkyixbwb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qclaaise.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xbqizqxg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nuukkgty.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hudvdkvy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jqhwtivu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2msjbbijy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kbohvssz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2issyhejq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2inoejgls.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gkdhteqk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mxtfgxxn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vgqhevmp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ojxwlrka.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gqgufdmg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nbqyihuk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mivrxizm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tmnfvkjw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nfqyiitt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bfzvcpcq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qamzyhqk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vlwlmogv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctpynygt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dqklfebt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ejouozpm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mqzoddgx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2liqqorva.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hmklzfmi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwqgbdae.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ehtetfpu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ikrahbxw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qdwsrqbt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2frqdgojf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pujcdiyn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hjpkhvrs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jcerofgx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2duxbkhab.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2aihuoiic.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sezcgafc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cdyzenim.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zxjlbtdp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bbuyaqmd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2noenhxaf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jpffubog.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ozdoeakh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jgnjjuka.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tqnujxdz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2azqdncis.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vksfbrdw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vaieoism.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2yceofxmg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kabeyqno.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2regrludc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yxzbbmau.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2txmxzfgs.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2abqvlbxc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kjaawkxx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pwollhkg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ciljnczk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2czwgvsno.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rvtyvdwm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kumburzs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vpietuyk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xlkqhbag.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aticmlqe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fontgzed.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dlrcbmbh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apdheunz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bjlapcdc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2maofbqcn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zfzzbtra.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fbfukhea.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wchukdvp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hxonrhbz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2slybamqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wteajtyt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dkgpblrl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dsvalejz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2teflpwux.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkcbomz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mezdmsmv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2aehsgiww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slotwsvc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ajvbfjmc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hifioslf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lyuhefye.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2baxigqdq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mqdzhzkf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2njzuolcj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pwwyqcvv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ifocstja.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2kkrbgfdp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2umpazzvz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mqdjiokh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2igxddiys.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2cfoxwoal.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mbqfoziy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ehanwtvv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2eiaepazv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2uqvxhbsr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ugmfqtzd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rxtjggvq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2iptlgxra.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2omftwqrt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yzjdgxzb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wzogourh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctefepzu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kteuqize.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2spymvqkj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ozmzgbiy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jyglvszd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ojdsggpx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lymujkgm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jvtwlxdm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2icbahwlj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2doqzygyg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2itkgdydo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bthbgvgt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gakfqscm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fljzqigk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2onceugku.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rlxvolbs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uxioguxu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2aciguebn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oiziyeye.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2bgwokeui.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ylapglkn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcxmxeom.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wwzelend.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tfbezleb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sefkdzrs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ytoltryl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2eplnolls.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kkbpedlr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ltdlqxjn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mjjbmlvr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kfqtebgv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dfkaolrj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kaxtxibc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2osxdycqw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2honuawlr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lgagnqcx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2yxezeabv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2uiheqnre.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ezcghcxd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yyqctfkv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2achpoavf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bmqzltyv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ofzanijp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xczjcqbt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2meqtrolg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xmsrkyau.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wdkxejor.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jjhqlaii.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qsfmceuf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mlaqrtas.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mjgdgegb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sdjkfrll.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2rhtqnepg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2iquqwdzk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wgsqfpiq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gbxvbodt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2snjqlnyf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2hkanlpmc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2otwzqkch.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zjsxitpp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dckkbsrl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2lfbinqeo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kfjaalyn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2djwbqepp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ythjyinx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mqzvkndz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxmahvu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahnpscmk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nduiktfi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2twcrgyjd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bseajnir.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ylapxztu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xkfsszww.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bcsajdxm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uqsqioko.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xeeaddgh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2oqdkskhi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uhgamuws.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uzsqhapy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2blqqqomn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qjgsdkkn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2railqpit.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xdgevyvy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2skjdmdyb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rxbwcsvi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tryxhctr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2djqcmixl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2olvedrqj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rxbuvtkf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zhispxuz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2psqsvogg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2agvexjsm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fconstou.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2objtxsif.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wwqbuqde.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nytyqrhw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xlfsylkg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2afmlolva.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oqsykgkh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uinunplm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ycdlpacz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2miotbcgj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2eedgybhb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bnrumemq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vvrmmacb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cralxfqa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ymbconze.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2fxhrtbzy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ypqkmupj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qegrcpni.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dbbddlpg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dhdgxadt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ltxkkmft.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ahwwytvu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvwwevti.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bvdrsket.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vmyhmqcx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uioeqxgi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pkxymwzw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qitjeqbx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nitmauxs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ajwuxqbt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mdjpljyk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnnbtcuq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sihndjqm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tamhovuz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2csacdrhr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bpzyriiz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cyyukmxr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2inllobso.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ilxitzfm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qdgpubdi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ihakqqyw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mnxadpeh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ffdoogja.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2thrtwefo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kpghpnqe.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2moxmvddm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bakfpgeq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2rogmgxdh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dltfwjhz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2uwhcothq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zykcbvna.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tgkbqfof.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rjikjzef.html


<!-- 参考信息 -->