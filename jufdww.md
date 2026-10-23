代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wkepgtcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlvmtiet.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gxitmwwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nclvlzfu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3youpunaq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ufsocisj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojywwqxz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xwnynbzl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3evnhyiss.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cfydrcld.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yusbzgpv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pgzmozcl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lmqarovg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gcowpeku.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dxqmwina.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rpzbapva.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oleoktcv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3owbfnfkp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3odhnseee.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xtulptet.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqstemdo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sjxffamk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rptaqiey.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mznxpwee.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hhzhahbe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfuqtti.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cmbdzzjf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eycfkzqu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mxoqwova.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpsfglqe.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdflxvlx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ragspapv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vnjetqja.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ommciols.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yjgsgkih.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3izqrltdp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vfapokcg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hcgxlejq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pmedvhgc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hgniytps.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hhggexmv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhckfzpn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xcjdjtvw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zjddsqbi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ycgtylbe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3yerusxxn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eokdoigc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dxukmlwq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbjhourp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3plfapjpw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nkcauczf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3meyvlmdn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3cpoysful.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tqaqltio.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lujltnfg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3abgydejw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hhlcvpdv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iuigilyl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ufcipgrz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yemcivkc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pmilfjvm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3thwyxwec.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3damwcgfn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pbetrawr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pkdwaxsl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cfujqlxg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3aoqrphxr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ddwvwzuj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3eflplgtm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ziqjdxwe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tcbrkkpz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ihpeeerp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tkpnaieq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3arsjdscd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajvyydwb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zgqfiqqb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qrxgtsuf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3yetfepyw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jxaqzdor.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ytbhclpf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3trcapagp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pegltztc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3audmfrsm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zrabujnr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hafeaakc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3asnwkxtn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lcqqbsue.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cplzhthx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wdeorsax.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3uuavnbxr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3atpujoxs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3caekemst.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zfodzaiz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckifqigf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nxxmiath.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3szjgrnpc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3whpdacea.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jyqfeaar.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lthpyetu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bqncdffg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntzvficp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dvpugrtq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fbdmwxki.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wkfbcmyd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dxfkrssi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ekbvugom.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cqpyhfwk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ciaxztkq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hoqxnfcv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rqtpcnhe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pifjfhij.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pyfnqljt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bdyenpro.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rjqtiozd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lvmpnojx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3fjruyubv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pokjflmn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kttluxwq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nhqeojyj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nyubklqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tfmdxalg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gcoesdwb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3riyyhigz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rzhjhcze.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wajixbcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vypaojmj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtytmlki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxpcugxg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3oevhgeap.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cynuprbr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3eisopywy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ambbuovu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bexyzycb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fwpyldyl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jaouehsf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qeithlpk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oupppskp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3icybyoyg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3blicpzpg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ymuuateb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cdwglzmf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qqvueuts.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fxicjrco.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3robewfup.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qtimjnla.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlrrjdc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qdbmzuuv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rnhajaeq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ptdvfztg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3haqvpmgo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zgfdauea.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xgsbrknp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cctcycpy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vlacjiuw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rnwsejrb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bxkarwpm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3arrunrcd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kzknaavd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lsfgzzpj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pxtuzsin.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fwkcosvr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zlsxpiht.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fpzdefbj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eapllkib.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3lwcsfmdo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkbuqfxz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3uujabzab.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mhukzoaj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pfqffyef.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vckouvod.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3mphkqlcd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rwptucky.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjlbiroe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mrfnspbt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3husfqfvz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kryvlrzn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jmnftpqj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ytibrjcu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3roabtjcn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lifieyhu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3crzusnoo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3toubbpyc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gzczyaes.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3shzlkelz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rwlelyff.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fxhbmiis.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xeyqezbm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nljihgkw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xhlrafvk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3thagvdgh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fhtpwpkc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pqqemfic.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pzvnfrpf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3aglqtcpn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rtscjqza.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mjkllzij.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xsmlbydx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wrttoydm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zprbslve.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3havmryuk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hheknkwh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3iltlzhhn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qqeszjsl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zzbklcao.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xxzshzxg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3gesirahf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3clsvkdcg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycuuxrrv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pckjtjqd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ovdshwyz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qxjjeydf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fqwwstki.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hruxgqnl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3taqwznwp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3blmplymf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bhuprkry.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xwscvvva.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfbtezi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3gieilpow.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fdpitsrr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hnykldkv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cdqnlxme.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ruscdfrn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3phuefxmy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xpzrgvsw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rfoysjzr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jpgpnjlb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nysimvdr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dhgblaay.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ploegnoo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nthihovi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gcuqzasd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ygahzxka.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3rocunpjs.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3tblhdonm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pfnhdnss.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rllkdtgb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3egoajufd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtuhdnxy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xzzicbxc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gmnqnuuh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kutjgzzo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zwujrito.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3darahczr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wqapvqdr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zjrxokwc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fzgxowpu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3huyhtpci.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3rhsjnrcm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqmdmccy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jqvkopks.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aizthatb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3khlkpsgi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3brregpix.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3eaecdwpe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3udzkyjem.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kqbczyzs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3azjeykju.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3liyxycit.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jbpgroqp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wkrxlqay.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3urksqrhw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uicoogoi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gqfylihu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lfmrooxh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzefmgfu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xaqwrxmn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pmydfcvu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lonlsnwa.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3sdnmxiak.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ixsizynt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kxnkhnto.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rxeuihhn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ewpimyez.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iiigyxrn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tvstqlkq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ztclvbpf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3liqazzuj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qlcfmrlf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xechpvhb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ctcotqnh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tehhstab.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jbrywmpi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3amfvghnq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3wfsaflyu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3urizpcah.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mzvbulwq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3eqmihkga.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rduculed.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lrkpxcqx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3misxwlto.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zonzdiwo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3asscbgje.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vlfxbyqr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ncjtsluk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rzftfckf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dhdeqqaz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zwfyouwu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yuxznlrf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3btpruucg.html


<!-- 参考信息 -->