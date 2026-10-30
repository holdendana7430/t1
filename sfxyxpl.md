代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gdkynzfmr.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gklujbycg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gezzzpwfe.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/glfkemixm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/goouzejaj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grjixjiwc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/grrmddmgm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqvfkxust.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjkpzkfsw.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/geefjqatn.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gayirvvux.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gogfrzpou.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gtjsqjnqq.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gtdfrfsbk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gdaixnjwu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gcrgiypxr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gnxvfzhka.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gefuymyyz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gsezshkuo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gntboktrj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gckuzpwkd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gfvyhvsbq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gjurhjiho.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gfacpacjc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/giujzasro.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gahscvhfk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gjknhlate.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gmwlbtxxf.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gjbbdphiy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gliukjnej.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gniwprcyt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/grvgqnogs.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gipzwpdha.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gyyvweohi.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gchpslpaa.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gktawaxum.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gvnwsbaun.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/geznetlyh.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gnyjnaphq.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gabjstzgo.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gvpmmripl.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/grzqvroji.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gwrossrer.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/garmealcf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gvsvptgrf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/geengckjn.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gszguzyuh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/ggsinmool.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmgtwsbgm.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gqmqansic.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpmznsivo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gixxqvvwb.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gyjzuojcp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gddruztdi.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gpykkflpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghwdfbzko.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/ggyiapjyv.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gprbhdgcz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gsxiifcjj.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gfakyrokz.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gkpubpupy.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gzsgvyoua.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gretfgggq.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gugcrtmsp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gnlxhjpve.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gjlfjjecz.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gbubbxtko.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/galijwghj.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/grtpkzfjz.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkygeejuz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gviyzszbi.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gfxcsgwvd.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/ggrsatlsw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gkwmyhtus.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gohwftong.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gpnrtmcft.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gnlaixgsb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmcdeafba.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gagxtnfhv.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gythqlezi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gmcmbnqqb.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gmpztyrfd.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gnoksxbkm.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gmzebrhlp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gvcwuulbg.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gszfjjbqa.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gxxlpyenh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gwmhbsijj.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gcurhrocp.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gjwfrlyez.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gjnctdibp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gvcoadllz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtyhwrher.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gusxowucr.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gbpxbftrr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gguzlrqkk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gjqrjerdl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gzycjxgji.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gxxcfciqy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gkbtgirly.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gexmbrhpa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/ggeyhgnmz.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gxapelboq.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gdiubwxal.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/glplfbauq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqhnlvbty.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmejncdio.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gqnlphtjx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gmlanwsss.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpzkvhyjf.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmuqgkynu.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gzevfhuwe.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/giywimoau.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gogvnzkht.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gyntmxcox.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gvlnxqvjr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gytgzsbly.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gqzihjyco.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gqvyghyob.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gzsrmqzav.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/ggrmvjoxv.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gdqslscar.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gifdnxleg.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gvssvxmnh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gquagnjxo.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gbwnynmuu.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gmgnfozkh.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gizurgpjs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gaappppin.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfqesildl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/geeoinkec.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwkygqjfh.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gcsemukxb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gyhtsxchs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gahkcbmdn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gbmtgcizm.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gbnrbmfny.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/geiwimqvm.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gpnotkmgn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/grlkblhns.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gxmpgvyib.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gofxuwfee.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gwlxmwgeu.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gvxpiihog.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gyxodrmdg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gmhxgcrxo.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gameshxty.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/giurgapuk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gjhvhppxg.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gytxbjxzl.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gopbscyxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gveayrcby.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gaqsolfpn.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyccjtskc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/giynnlebx.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gecffkgpz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/ggsmzylzs.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gqlzpftzv.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/guxaevwrx.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gvgtqlvnk.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gxqilokmn.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gijnzrddw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gpfaqqvoq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gyucpgjfm.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gkjoqimvi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/glpyziuma.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gjeossxcr.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gktejwqop.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gwuzmovbi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gqvxxtdle.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gzpwxfnxd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gfjscxsqy.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gjcnzcxmj.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gbzwtcvxm.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gelphlzam.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/goztiknqr.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gzeyikonl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gqbjunpkf.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gephyopaz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwvefdwzz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gjqkmivrl.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/ghetsmngm.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gjqbgolgf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/grwmmecgj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gpqrvvkhh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/guebltqoz.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gokfivnzn.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/glwkftxbs.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gfkhsprvj.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gcofyixns.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/grhwbqrht.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gqfqpnujx.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gdyjobzxh.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gudautulj.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gatsyohfq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gdojpnnmo.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/grjcnmfns.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gyxdulnuq.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/garfwsflk.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gxieaotrm.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gswlnzrlh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gbbnlxhur.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gwqteqzmq.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gqgerjrod.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gudonhyxq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gyxbajgjo.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gjzojradm.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gsastisdj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/ghtmdouvu.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gbsknzgjy.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gcnobkmxw.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gppfbaqdb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gfxacmplw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/ghbejyngj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gweqgdquv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxokwec.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gajerbgtt.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gtyumfvxo.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gsgwovcwj.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gbkskmrli.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/ginwzbhkq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/giuegkfcu.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gkdzfhesi.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gruxqufzb.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gymgwcbyv.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/ggaiedgux.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gqfwsyozj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gxbhponcp.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gmilogfli.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gpinxiumm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/ganpmxuwg.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gmubworxt.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gvtpydest.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gptshlbwx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gczoxdwan.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gowpdibor.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gfnjczbgs.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/ggifvfgdv.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gtwiukocx.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gltoxdmnl.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/glxzkqxlb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gjszuogsp.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gahxutcjx.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gjvleiyck.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdzzsxesy.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gzneczind.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/ggoqetpme.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gywaeaojp.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gowexotcw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gqmrtcraa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/glruzsfjh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gcegmhqme.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gsieinbkx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/glgkbbbdl.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gcxqjuvlv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gryspxeov.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gztkvwdwd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/grcxhczou.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gtvmimyex.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gdhcndbmm.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gkbcrskdx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvzqdyuwf.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gsbuefhfs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/giznpgiti.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gunvomqxn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/grwhmmuuc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/ghfxflryz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gcqcnloho.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/grbengrxo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gevjphcnq.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxgfpfs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gkibsrwev.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gqwalkcfy.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gtdxukpfw.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gjrwxxova.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gklsvbndt.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/glrcbpkps.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gvtmjgeqx.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gueivbzhd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gcampesos.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gyyglwpzm.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gqjwtxvac.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gvlmxhupj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gamhmxtee.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gkamjlhre.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gsbssllxj.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gqhxzeccu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gxkkghrpg.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gjbunvzrp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gyxbxrcyr.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gusvmiupy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gmenczqxi.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gvkoersit.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gwsynmiql.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gisquynxv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gwtckgqgt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gfmztsqks.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gsatexvoh.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gmincwmut.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/ggvlgczpf.sHtML


<!-- 参考信息 -->