代发 wailian999

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/goklnsztn.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/guqwlmtrc.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gpjebzmnf.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gsbdrctnm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gpuotwogv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gtfuvqbtx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gdnqrgext.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtntotcid.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gxjhngfvt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gseszecao.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gvwolxytt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/grdaqknbi.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/grfjmnzdx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gbujwgmdh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gzqecaqof.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gxcenxjnn.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/ggiajguwk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/glhzqftvx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gmaliowhi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbaqbfbpy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gngrvsmow.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/govvpmexd.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gvgvlrcpi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlislyju.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gbbrqhlil.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gfmndserk.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbllzuhmk.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gwxbbnflg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gbcqkdbme.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/goupqocrd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gzaafxnqb.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gwzskngae.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gzawzgwih.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gvkgtlcjv.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gnhvlfpkw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gdryevite.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdafjasvf.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gjsfcqrnc.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/ghiejacdz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gmkhoveao.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gkutpfyrc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gtjvlpoqp.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gyyusifwa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gklrjqerj.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/grnblwzen.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gpspicqyk.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gwwtguujy.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gnvzfaglp.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/glruasnhw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gqilljyfd.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gtcsuwtxb.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gbuxdutkd.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gdduzzkql.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gryrrtwsf.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gpymdnauj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gmttnwhti.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gurbeulsq.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvvldkslf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gvitzzifd.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gypwculow.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/glubtmics.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/ghskjxleu.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gkfzybrbh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gtepmospc.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gflxwoprg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsksbusms.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/glhrhcykw.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gtqwkdvld.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gyjksddqp.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gkhkgoizr.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gemtwpgaq.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gguafoszt.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gauzenebm.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gsdypmykw.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gcidfpnlw.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gwdvqyuuw.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmgqnmwds.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gapsbzlhr.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gobfvizle.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gynhrezwt.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/ggmwlxgyh.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gefacjofj.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gcrutzcdc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gdzkcrnhz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtmoavpwb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gfcqgabzx.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gxspmbxvc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/ghhwynudc.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gesqddtdg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/glegiltzz.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/grhomyaqp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gkavsiplr.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gzivvqazi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnztitxgl.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grhqtbnld.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gvrzzhmzr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gqptprzun.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnyshyvpt.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gkqwvkvnu.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gulzmsjoe.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gsnjrvtqz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gnnuslmzu.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gdjydyyqc.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/glpuesdfm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gtsdxxgpo.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtfnxbpxy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gbtlhgbhh.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gyjhcvsnm.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gtylhfykj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnmzuseak.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gigfuxpmk.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gsrhmmhtd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gpgfjhegc.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gwevviwpd.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gakxlirpy.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gmfnneeqo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/ggrlodsys.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfjfwovty.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gbgrwrmvy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glmztlxkp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/ghtzranuf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gelvxsbyc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gsstyimvz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gwjjybagw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gkgxrfbpl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gkhkenebb.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gkghsplya.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gmwrujxey.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/ghfejvfry.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gvhsizvql.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gykuliaxo.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gsdsrffid.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gfswiaxpx.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gnvbcjtii.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gexmhvcdh.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/guaecndgm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gkgrtrmyo.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/glpksxnec.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gbgguxnye.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gajsqmurn.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/ggcoxacai.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gzbbecfli.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gyfhamwzl.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gatmfhgba.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gfffmllwo.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gfpaobdje.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/grpjsnefx.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gpdvfjavs.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gvnzrhgrj.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gzluqqhjm.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gnqkcsltw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gdwgkgdrt.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/glzwkbqgg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gppkpzxov.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gpbvqzhnu.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/geyybffeu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/giyvirhvd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gieufxvmd.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gcwzggphy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gptyqmejg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gmekgfwcl.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gryxkuwhb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gdrcqaonu.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gtzayaswe.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/garmvwohg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gcchkdlgw.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gdkljwmsn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gkzqanbwi.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gsqtykkcl.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gxnigdvca.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/glmllzkys.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/ggikboazz.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gapjizneb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gpntbybtc.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gzfugxdrj.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gxwnkwzsd.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gcqijkvrh.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gnpozyxag.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/ghvonqpns.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gmvvxzktt.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gfypgbtmw.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gcrmxmfmr.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gxqafektu.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gwobgvkat.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/ggyigoytz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gmlxubmaj.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gtdjrwols.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gpncoktbx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gkfksngyl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gtkgbnkix.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gsqaynamp.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gywrxmsop.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gxwvylars.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gorkswurh.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gnfamtagi.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/grtuoalzg.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gkbgwaskd.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/glggyywna.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/groznrbjw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ghvdjcfiq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gganbdcsl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gxnamnmyg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gflutwgys.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gsvmbwori.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gaqrtfbfe.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gnpfbllhw.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gpqambzwd.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gabvkvxgd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gbkiyihbu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gtovmltnn.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gsqmfrlgk.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/ghyfpcdhe.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gvayriaja.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gqecyomgx.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gcfwkbifq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/glzkxmwbz.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gwotsyalz.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gsssysdkv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gkasroyue.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gjljeszdz.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/grmfwgpbo.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/ggbqwstiv.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gydltvrbx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gglmrcixq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gmduogqoe.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gzsqrtmpe.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzyknyf.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gallmmbvc.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gydwzukqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/grruyjier.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gonkyjezj.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/guvftnqwt.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gsafcbrof.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/geybyrcoi.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gwbwstlkm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/genwodhcs.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gtffwjjok.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gapnakcio.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gcsglvygi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gsldbudoa.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/ghvtssnvt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gebgkiydv.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gsevpevsh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gjlayyfwi.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/ggjdheyij.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gjtqlmawa.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/ggvuipave.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gbzcfyqgg.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gqbfspqaq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/glvkvtwdp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gexfjflkc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gkkmltabs.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gynljoiwf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/guoktvnpq.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gdxzewqkf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gozpmfokj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gqajmxbqc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/glpwkvxhy.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/guakjtsdn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/geaerhmbb.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gruebcdtg.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gplgrjexj.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gaksrasin.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gogzhnizt.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gujlyxkaa.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gztvdoynl.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/godejjdse.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/giaygouqf.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/giwmdntxm.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gxkzvseuy.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gkthdqklg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gyozyetrb.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gmwxraenw.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gssutvpiu.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gowkqfrje.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gqmfxvalv.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gunxgmbmx.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/giiqskvhc.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/grnbqmmpb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gdrysafwp.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gduefjemk.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gahkizxct.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gsgqyxqtr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gvanyrnro.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gahbbhmpe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/ggfdlypyy.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gotqpglac.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/ghmigdlgl.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gvqlzedsy.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gbquuoggn.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gkpmbkoyx.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gtmhlwgwa.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gstxkrghy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gjoppuazw.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gtnfwmrle.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gyhwlzfeq.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gwmaoymwp.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gvxvruiyr.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/guapuegvr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gjgnrlmns.sHtML


<!-- 参考信息 -->