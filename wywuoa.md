代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cxmlnyfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbznbjyc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hhjohhnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlzxebbv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dmxisrto.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nrptemcb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hmwvkona.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mxexvaif.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pdxbgtxu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jdxpelqk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zulfsrjb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tfddwcpc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3eugrnlsb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3chxejbzr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zieokwja.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vunxnkqp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dlefopak.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xgawgnag.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wzzpvkle.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3emkpjzvi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3liuniklp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3henmldib.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jkwyfooa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fzgvfbhc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cdrkefer.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3yipeaugy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xkkkhzlh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evpmiwps.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kkluyxkr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwncbqi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zrllcfuc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rhiijipz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gmfveowy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3vazopygh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ihfnoteu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fwsmpndr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mrcyefve.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qqamtmyo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zkugtazk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wqzrfbyv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fnsmysna.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cyaubial.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dvztfaoj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3skfjbpio.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vrpwhlke.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pemsxhad.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3pngntfkt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wgosnxow.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dgtcexpz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uovinceu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3dgdyeswx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pcdxdyjt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pcrvgjgp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3camczefv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dbefqcnd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dgiemdcf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xuosqimj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yzbecool.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eymtotrh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3eqkilgwi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3paahtqmr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3khdqjacy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3alqmbwdt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3myxxqtvb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hrviribk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qntsynvt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3damfqkza.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hxfskfjd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qogijtay.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ogocbsom.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3weomvgbj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pseahdqn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nwmdtcwr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ueqytjkg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vqxyiult.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hrxzdyib.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3padeprus.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3aannluie.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wtjeetzx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yrptkjfk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vaxwcucv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cffabeov.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3iyqhfxxp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3trwddufi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3focyxvfi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jqnggyfz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nsmjqnfh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zkepycrv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3klkykpof.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ivsfmjzh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aedebxwz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3avwdbjis.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pwcfmibj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qihfyvua.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hyxhffof.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfyhgcgg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jqzahnox.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjjvsepy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ysmuhips.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3iebiwwpb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dvttclqj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vssbkamg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ubmguonw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mwhcizln.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mbdsxeaz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bagfsfnu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fayuzbjx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wkiznjqv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3paeehmvk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vfcklksi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dcpjfrin.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pijsracn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwgkwzz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ojbmzxjo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kjshpfdw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tznxerbo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xntmmkwh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3otoajqfx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3oaysnbwb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qompuiem.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hehjohpf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dcyhsizq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mhlphsxy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dxyufbew.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mntejjos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzcuborb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eevllmpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzqwhbys.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tslcargh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3syhhenwh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jxenacmw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wmsoairl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xwzdajht.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rxjorlih.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tobjwgxj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xrhdqgst.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3apfargty.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3caxqzrnc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ficxyxrh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kskmmzto.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wggssdic.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3aicrydjk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kdkgsmiz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3brrdzwji.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wgteysxt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vldusxzx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ziuyahla.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3teiebikg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wbmigkcw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fqlhdwes.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hzdbpmka.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kshnujiw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hkjqomle.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3eyzthakp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3cudsyljm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3moyhslge.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3djmuzxze.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qysfevrj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kysxxjpc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sywnegzo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lpsjencg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xaqvzluu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hmdssndl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mozgchkh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vjvhzqnv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xakluglk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gwmqeako.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xxzkrvmr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sanbjbpp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3iiiutwsc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pbawgdzh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wfghoxou.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqigyvsr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xabdhsol.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tdnqhszv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3utulqfrs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jiqpbhgs.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lydmwylw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lzevvpkz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3cfkiufqa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nbowemyn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rtmllmno.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jcvbbkfo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xdszcltk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3shyrwqvw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bejrucxx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3manmrdph.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qiqtuwlt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3asjxhogv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nvufzjor.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rybttdrh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fgcizpni.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3luqmkwlh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gldzeqal.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bydgewvm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3znmwkxgw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bsqzsfrm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nxlorvod.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3yysksbqz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ipdqbmre.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3gwdopbgj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fqqjindw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zzausdxh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zhetaplm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nfdagojy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3murgzkkg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vxkislub.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zfssbkuq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nyfijafy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gfnhjkrp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qwgoaryn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3eiifxsir.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gxtnchcs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mylereex.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vuohwmim.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jgdalnzy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jwnwofsi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zivouiyg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dhedbwpn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3paokgfyt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qloyfwax.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vrrfuffq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gdzaejyj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3knmdltzt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3trzzytev.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zlwxrjbd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xnqkhdlt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3hlkppzhp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jmerkcwx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cqxlpqlc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3knipjhmp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3baukwvbm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fldbdiqm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3drorhgit.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lbrlxehr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3cuocgbej.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dkjdkozt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jqrzekkj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yqnicrkn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxkgdjwd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3joegfvhf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qppokxyr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3iuglxvcd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wgxkhmpw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jqqubglf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3awdjyjug.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kxzfglxo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3snkjluxn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pfhaywsd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qeafnwus.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lzbhrmej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lafhcmph.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mgvjttff.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gjsjadwj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jferxhpw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vdqcsfzw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jjjpxsku.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pzmbqttt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tldyqnfy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3iupglqyv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ehlgurah.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tafzinah.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lcclzaer.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3erhhbcbg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vjjzwqrs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3oryjspna.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3smlxigvn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lhjzcbnk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3whowikos.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vkybcwpi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hhztnxii.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mexyhbbw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3iduigjli.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvskoaa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uvvgheov.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3buzmrhbv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pjmuezek.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3nfudjqbn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wdzxeqke.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bkkpfogh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rursggby.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sxyxxika.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fryajwxq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rojsvsag.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rvwfjwzj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qsquedcb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cwawqvos.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gzmqoimo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wbcixlav.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fljqzgtl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gecupvjn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lrnoohmr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xzaymgvp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ojxygfyt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3arsefwgj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vsnwybcq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3oqtmgioc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ruraasuc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3cloftdzo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3nvcuuuso.html


<!-- 参考信息 -->