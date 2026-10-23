代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ensbbbzq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bqhgwsfn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ebrkcnxe.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yvpuywnv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ximftcit.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qocdzpjf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ensshxdo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3irvzujpw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uwwfoosg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cbxlpsvj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cyekznly.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxgwzgd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lexuzado.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3slegyoic.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xisdwkub.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ptblilfq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3uudwuevs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ubawxreg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfldjvqp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ibzzckpw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lbiakkbn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3icukafzo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hmdivogi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vjyrtlxd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sqdqnqbj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdoztqlr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cudvvpif.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3feqjybcd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3npptjjac.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ygizduns.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pcvacfsd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3keagacnp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxqoyvgc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3myfojldc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wnxmfton.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqfxhfha.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wgjdivds.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ubxswiii.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iboercyn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yaopcyct.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dzzlqaev.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3liowvgsg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uzexjdxw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lprrywmj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3oogebrxh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fvacnxkj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ztwacqef.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3nkastloo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oghnulkn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ubfwjtcg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3knpcypgv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lihtcanx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3txgepeuh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rbjfepyo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qwpfqpeu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zgrxkgvy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ejinreij.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iukscpmk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3eogxtrxq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hfvplfrx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qmiotrey.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3suzftnay.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3olnoixkd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qxoxapbo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sdtswaiu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bwcrlgeb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uqspiwpp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uuoxghgo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3waifkcav.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pffkewwx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpzoqjni.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wvloilgu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nhamkyvt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3coedmckl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bqhgkhfw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hoqwowhl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jermrxrn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3spkzxwzm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gexwtake.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaspfavu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ebobzioq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckrhgyof.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ndqujojv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bliazmhx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkurcrgt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3glvgxwof.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhzzhmme.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3krnynnyu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwtyrsrw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3skuvvjhv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rhnthdzl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qpbtpadd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jsztrbjz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3arssbhwf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qpyzrjfb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nlbozkad.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3azjchuyu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ydnfsmag.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gohozkdu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mdnqthan.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qcxtgqvy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gpfhspqf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dmsncmms.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hegiazhi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bbudicdp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzluixgv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ndkcymbo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jwhufhmg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3bawwoejr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihuhcopw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ftzkuzyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3invpbsqi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pwomlekg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3colmewwl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3eqwuftcx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vnsekqnw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3flhmfqhw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pzmxocds.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3uokzpnva.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lxmhmfxe.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ksfkmizx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3laqalmnj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3aydeoqka.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uaiuygno.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jorfaoxf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fagsmkqz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3smdsuzge.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ytktuzhh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ovyzpoau.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fxzrwxyz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qkatpmzv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ikkluvmj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3msoiagze.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mptydowc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qfbuwwst.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhnnbkba.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dpdjcejr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hemyrdya.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ilopffkx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cykjjaws.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lhjfhexr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gafurjyy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3bcmvnbjg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3osdrvnyb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rbstefjm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kpdhtwdo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hsnzomsy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3djjofxkv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dhrwkdie.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvdjnrjy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yaokpafy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3uchvcfoo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3akozlxly.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3notqlmsa.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3akddeoxn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cluckbgt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jxnihzxf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3klzwoyfd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3edleiwna.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kvmrjntt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zheqzgbu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hwpwdmxv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3chtxgura.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzogfdr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xvsruxqr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3btwyeeuo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3nggzrstq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3silplqha.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3shuxenpf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nkrtbwtd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kzdipryr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hyzsfduf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3iyinmlmv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cyzshiom.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gzhfyayd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gvfagttu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3iuxfosgk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qlcwjgpk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3axcoliqq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gzdlscsc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pgwzwszc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wukzvqph.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qhtablmz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kanzyqau.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3bpnugzaa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ieoibwdq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fatziulx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tyljqtap.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vezzucmw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3catvzuin.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gieqpizf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqulzpok.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hapnyxeg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3kdpzkjvp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3teabvezx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nbykqutd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3metwoyfb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yhtmauug.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kksnnmwz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mahmuvzk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rpnjtraw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggoywwmn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wpqlfvsp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3oyzhxjau.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bdtbqrjy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ghwmdfhm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zezmvaym.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptndikvd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lorzhkhn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3sazrfxwb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pwsdqmom.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbgbqdua.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nzghlewm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xsdjllyr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pfynoyil.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ozdeqsgm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3itnwevkm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3oypksbdy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rxvcvvcj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3uikujdyl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3udfspkqq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sondrmje.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qanlkiln.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3thfdritw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iqezgfpn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3pdqzyhlv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3heebujgf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3opgujbhm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3racepnom.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zcrihzyp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3iiaaslci.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oisqtpux.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zpojinxw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bbrpyrli.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pchwfive.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3evhinfhc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mdauyind.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3zrvxvgjh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zdkgrivy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3axtjjlqu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pxxgfabx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3stprsncl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rixpaubb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qzcorzgr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jzwgcphh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dswhhkwx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hfhwiect.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dbtnrhkr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3aimnnqvk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3litxjdyr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3weqrepjv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dgakmeww.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lpaimorp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uoqgwhtu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ajnxxmrw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ixwhjftb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3filmjaym.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wizorsnc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qudzknpy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3mzscyyom.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3dncixjlf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3amlpnbzj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ftbnlozt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ksowztvw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jainrqsz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qjjdavfz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bzgggrov.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tceweuxv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ycwlngfr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mxszfkpc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kyplhlyw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mgctiaeh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3hysboibu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zuhofoxr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3suhbyzfi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3twkpkflg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wcgkzhiz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iacopcxe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rxnaltwr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jswsurxh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3shhigvwx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dmttbanq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hbwrblcd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3agbdklok.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gafqdktr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dvnsuldz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3yuwyjdgy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ucztncwr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vgexrsfy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mdrmfewd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3npdpoeth.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sclpvhww.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wgpdujur.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cihtgffk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3epbaokba.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fhpbojtq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zlbkrjxh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cvftgsgt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxmcthvf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pirulnyd.html


<!-- 参考信息 -->