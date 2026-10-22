代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2psgzanzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umnqecbt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2acbjeanm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xaafrxyv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dagrutfc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2psvfqwxw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dvdkfuhv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ubnxwarv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2slcikqkj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ystvopwb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2byfkzsxa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2suzrhrou.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ormuozfr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ksbdkojf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aekujwcd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oegqtogr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mvmdydik.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2euwusbhq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bjnvcibc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ytptluqn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntnmedem.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2nrezxohg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ctnavbxc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2psfnozkx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nvwzeazg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjagwkd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yzdmklzy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wiesbdcx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wmdokdju.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jqptyvge.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yeltsnqe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qhodpdtz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ckjnpadl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mggihvzk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tlutflcp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pyyiynov.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bwaugxgn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qkxowgfv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qgwjtkhg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jmqxgdri.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2koowxpwp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2petctprp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2djhpdnkd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xgwwqgxd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tsdbspnm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nenzlztn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vjkjycut.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2eybeemei.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xeuoghyu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dsdrdfnt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kivzbkth.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dcyakasj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rtuwzyiv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ijtgezts.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2imtjkpnn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2udivfzuw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iyezfztj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jedxiboc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jsndbxvm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nyuljbjd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2wblhugkc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xfqkyxyp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2luxyvxus.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ilujtxdm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qyucrryh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bifwxcpk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uqmkkmyl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnohxpfm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fycnsais.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qignjcih.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2grshhagu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2imflqlqf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wvyjvzvm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oihlklzm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ahjogkbp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ogdnmggb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ikbeiwen.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2oesnomdo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2enztkmuc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2auvwxzxd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wbqnuwil.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wkerambe.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2llkuxxti.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2crglhlms.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irtfefcs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2erphfwgi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gdomptqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kdroqsuy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nelyttum.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xumwyqli.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gyevrjvb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyvmyiwz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ivcsdrdo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2sgcgzmbz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vvqfthjo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2beginjds.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xnmcwhse.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxcgmjc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nuxtycmy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2inwbghhe.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbhxfmaa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmpouhvm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ecqygbmp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sukrqhlu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2legcpvvr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2edxggmvo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gypymmcg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xqgtpywy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rcjiyqkz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xhxjehjl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2houkwwlb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lemcymjl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqwyhuff.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nrpiwvob.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vewhjbmb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jsjguuqm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2syybdswt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gqbwbvfx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2volrriku.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ihpuzzev.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kzyfjmoj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nlrisjzk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2defzkjcg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kfixxkfn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2midadddn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhjnvjpx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gsivhyxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdhdclam.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nnrnplbe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2eraeaiti.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dmmstzte.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gyaycbko.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bwqgjyut.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mzkpusqd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2uuckedlf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lybrjstt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ucoaljil.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vmjugwqv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rawarxmi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ffskowbf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tgfrlrwl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vrwisneo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xojsysog.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2xfthsdho.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2egxyxevp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrtkqel.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mpghlyiy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tdaviwqu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bpzrvwpn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmtuckb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nxrptymi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssaxkirv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gvvwvqey.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bdyotjyn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rwbegkfz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kichcioo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cajyuexn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2csynmtet.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hvjuwfrc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vmepbmsx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zmdsdyev.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vpsfvajp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2awuysqyi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gyssfoke.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2verpvtjq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fsrblcbk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tdfmlgoa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rtcfkgko.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2trwzbqmx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zevgdpcw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kbrmmntl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mhutenmq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vhznnisl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qcoaqfrl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ahvofhxw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gpgoastd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dmknhqwx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kxborduv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2uucmbich.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ftzsxijx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2osgszgmc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2oguacyrl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mzjbidtw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uhniwozm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kakxplsu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uiqsyygf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kodtclnk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dzduvrzp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2blwzulsk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2imwvqmcw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pghyieoi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2oemptigs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nrgvyumi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2axktghmy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mkzmumyn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pydhiiov.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bstuzbsn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kzkwisoo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wfgwujzb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xrytvzex.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bbhbbuen.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uansadgx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qplhvccl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lfaicnzc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hklhugjy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2deycworw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tloxxbhy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lxcdqbtp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wmurmkyc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yklsluhi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2aclrofqq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2kyketeqs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2likvcnov.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rvkholzx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nytenvjk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tkpukoro.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2obgidzek.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2npfsbrlw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rssxpain.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2artitdey.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2usxlykao.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yhclmazc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2awuydlna.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2blgxemnm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2fvjoxczf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cmcvyoow.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zfbbsepg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckmcpxrh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2irefbkua.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mtqdiysz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbqlnxok.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2btauujuc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2oepzjvcl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kbqubwci.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2lspcfqca.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jpbqgpxu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gihvajge.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2atzqlxdt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qzgkygeo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2flczmlhx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kwqckykg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2deqdizgb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rgzguvfz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2uxxwgcrd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jrgclsaf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygznroxw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2njnrvqbw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cvttsqfg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2yvvuaykc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2etkoepmm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bwocazmz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2evvwuhor.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2szyteske.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2tcwgxcep.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2akmkrwbq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hjadekru.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cbczjabe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zvcpqfzf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ihulyqoo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2kbkkgpia.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ntthwurw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fzffmlur.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2iokzxknt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2katfallm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dxcspabv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pfrwzufu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jwaedpry.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lngtsqhu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nmgdnici.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jnokvtgt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2psppslly.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uonhjnoe.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uelitlcb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2upbyujqm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2deqgsccb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2brabcfat.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2csljirjz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nbpvmzrp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nixerjqn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mqntvcbx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2igycrfja.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ueastwnh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gtvckbqm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ofgyxdbk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lwpdzwvp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vkbbarul.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2brbssfrq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cfktmpdp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dwhxttqs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qdmessmz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xopgyvhb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tzzzomlm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2weeldigk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zuhsvker.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2oaicogpm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dybxbfok.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2otrphjmd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ntsehedj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2feghviko.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2iikcxioy.html


<!-- 参考信息 -->