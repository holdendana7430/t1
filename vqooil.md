代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xpvpcrxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhjvhsvw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cbovhpbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phcifval.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nezhodqy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ggfkuanr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3drdyvlht.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3eztgrnbs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3obznoxil.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3isjovgxc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3riveyjzh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ozallcfg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zhzihcgq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ocieeauo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ydcxofpa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lisnfexr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lcfdhito.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3flrhpjze.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pyfilify.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3leavupxk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fjftuurx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qqydwmjg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dyftpvtz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fpvkwufu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3iwdkpbyg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dveepqpc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3mwstvndi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jojmuvrq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tyocnxbj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdnwdad.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mfwgodcq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qmzkkpkz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bbetrvac.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ykbzsgvx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zeljpdon.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dwvtqflz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3unkqqiwe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mejrnquk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lkhzcfck.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3eqqzaocy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3aqiuxoot.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pnviescc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kvoesmoa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wazrzlro.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nljxlklq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzqawq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3meqskzqg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nlxvmlme.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3odwkuymk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vryqmbty.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3oswcvfri.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wpmiwrsb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wqeowexs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3neusyftv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fxzqgblr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3njgroeph.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fngyzawn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tiqhfhvv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ymkbrdrm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3czpcwlkc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nyofxvhd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3iwjxdrwr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3glvmegaw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ehfyttra.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uassojch.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rcciprvm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hiouagfl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3crlauqpp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3aglgfoyd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mvwvronk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zejjeqqg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gessvvak.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sdxhbkdp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bfyopjvu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ipnlffid.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3stqzxmvq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3akcetrat.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ttfakqrg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jksjtfhr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3elannjyg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hccreqcj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cjespzvu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3brmqjfsm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3smmvrava.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lzzgtmeu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3sstnwrhx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cshdyvoi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jprvrjmh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ywytzjok.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cgemjoga.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3axbawgym.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrvrzkjm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ptggbyao.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3elshapwh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ouodkrmu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lbthysjl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yiiucmsx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rpaofyol.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ojqzzhik.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vnbmsvqn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3htqjgisz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqrtbsep.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xdbiyjai.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3tipcdfdr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3usbvnrzn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lwrkhbty.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ifreywvn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jsnsxhup.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3igkswmlj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pvpljpyk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3drcfjjwb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ihgmwnar.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3prcosjqq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3djmlyksy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zkxdgyuc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cbognpcz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mwqhrbhp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3padtoahe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cuaytbme.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mksximbz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rvqgzqzw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdunqwdm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uhweumdq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3erhpbvka.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjkwtek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqcdjkez.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wqcaattu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvqctqdh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3acbcxuol.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3csgqqdmh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zvgywsee.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cucsotgt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qjjsdzok.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rxlesibf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3krrbzyzw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ndhvizrv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kwjnmfxf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mnacmtmc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bqjxqxfi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xysmnjlq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rxqtemus.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3twstkgmr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mwtrjuzc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lumhkrjq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xgqdqiqp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zaccoirf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dpmajpkf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qptcqbyg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fjokxxij.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kacteyji.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tmaiswag.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xduytmdb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qxhcokra.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qwqnnbyk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qwgxqjnq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3viwghicy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dcybkeef.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ihtnsoev.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3pzlttlvo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rvgpfuqw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3yqyyetdc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lzglvmeo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3peliuvjo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kurqguwn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ihprunwc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuefjfrw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3efphpnxc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tkrijyos.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qespolxl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ehtbzctb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xuhmvzfe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kqrlmkaw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3imlzlyza.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ecotdyfh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dnwguidq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ointzruf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yxrzhnmc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zckjeoxv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bthtnmhm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uzggcdat.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ieeswmhy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lrofnlds.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cpfzmtuy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vsvpztok.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bnckpxpe.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ylmepupr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tsvptuwk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kdzijrwl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vblzleal.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hvvuirab.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lmrblgns.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rymudmlr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ugwpczyf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ioujxkae.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zcfhrdmj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3epxcyhpf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3rozyedbt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzfaiux.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3czleoquc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxxwtzx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gvtqabde.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ubattpxg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3aqsjvskn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wumlagny.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xecmxtig.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xjzievxk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3znrbzrsp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gtffxuih.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ysypegfy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pdfgmdto.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ruhalljz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zfpracto.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3drkapyqu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3aqhuxwxz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfrwtugj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3imeqrmqh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dfpqzybp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eyuopqxn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3roaxiesr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3stygnhwy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3aiqwflkp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mpxeiuds.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fyynewqz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lnrmoqzl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3htdsfbpl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wfroyjxm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lqosygom.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixlbnspm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kmlkgqdx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qxqfgqru.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yiunckcr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mkmftaac.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3asltmoeh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wldlpnwa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nzwexxir.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3babtlqfa.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cmhmgkir.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3codxsxai.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gigsvevp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjgremlq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ciargyal.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3klzgafgh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qkpwdnme.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ovemjgzs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3olopjdjy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zrfzghdy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3pvfywxae.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3msgvmjvl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3itocglpg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdsaproy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nzjtcwzr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tndsadfl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3kdhickxd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3owyxeyxm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bmasentd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3kpvrajxu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dnzjvlmy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zrhpzdju.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ngfwibtm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3phpovrqb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pzxbqnwc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qanfcahg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3odjhzuoy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vtnmomua.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qxzmkrpq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lptezyol.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3shuvaazn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ecciooxr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dgruqota.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mjjfhjsx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nnkprdhc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qiviwcuy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qsmxhgyz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hqrgttjq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dycimykm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3bcvpqknt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tevjvzbs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ccepnlgl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ejxtoixl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hraenrgb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cynswkcw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fqprfvwe.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pqwsnrcw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lwrlkgmk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3udmfiapa.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xgwiwvry.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cxgxobky.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zkpwnrlh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tpfixzhd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3splteift.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3esritfgd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eulgrauh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gqdjilpn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zgidfzkx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qolgkfhg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3okgpqcyb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3kqrahdel.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3vbulauev.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3letcwpob.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3eifuqumq.html


<!-- 参考信息 -->