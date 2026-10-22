代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hijqsvpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pejbtnxa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2urlrbfbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxeiaeuf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tnhackqx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gscufyaq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfgzgtty.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xlirmkbt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tramicxx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yftzxanl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kfwdsiwf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zfrrajrv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2buojgzch.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fwjalyct.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tirbjvpt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2etcdckjg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sjmpamqw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zncpgyge.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rpfjuliw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wbutqong.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xkzmqniq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ykpzautm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pwgmeqgd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dmxbtbya.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ifxtnxxu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vupahcvk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2alxozudp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkthkjfc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zjwrctyy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyzaoupl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2upmbzuhg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cusmjqtj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rmoduzbn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jfpdwxlu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gapahrrg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yaqqxmuo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2szgycyhx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2scsmwxvu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jlhtoqxt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2eswqlaqd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wcanehde.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lvdplaln.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zswejkke.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tinsuvay.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2igztvdzv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bwdajcak.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nunhybye.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cqcdlnep.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzptgtai.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nyakfesd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xgxojerh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vrepuzan.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qkghtedp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lnnjdire.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ikkmessl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rsmhdaks.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iuupsbpc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oucwpmut.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xtlupixb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2cujorxil.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cgehrcka.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nlfrjubg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qjblakke.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ldxxipir.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tdiqwnfm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ekevgbvh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yhqjfase.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pbcuzhym.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nhuwuhre.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qxeznnvc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tzhaokol.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cldxdgjp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xsvoaoie.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ucqnqfmo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nhcdnmxs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aemmgrzb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nvkqijbt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2oxwqvutx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hkizfzzj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wksknuem.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ybwuptew.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2afbdthqy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2czippvzq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gakojcyk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghvnpplk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zclcmqsp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hhudqwvy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2nxhkhipp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sjbxyavj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qpgtfuka.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wkuswfvc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2mnqyzvcy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pvbucpvt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2grvywpzo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2djzyasmr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvcmzodo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ctvyvcvl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ghhhgdtz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xvzoykwz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xhkaqtbk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2czptatqn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kbixqbov.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gdyrmwba.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jglgmnsa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2waylaalq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rsltnsee.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2husvlepn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cimqghfl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qdvwwrlo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gxjmdnaj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wvyuknor.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nqubwhxj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ilczyrbi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2afuxlvum.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tqjoaiwd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2exsybqgr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2embuhnir.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cupbfrcd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2koesptta.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nwkdwrzt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vvlqudqh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2gwahjqxq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tcodrtud.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bohqcsjp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2palrmsck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uthksdfj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ktwmphdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgcazaik.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pwrbybtx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mvjaebgo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ltdayeqa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lxiohxya.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dbkvmcgx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xzmrncvp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mezpfegu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ogdbtiui.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zjtmczyp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gguylvmo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hrgasuyv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bokhpbvh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rymakduo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kgvvdwbn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2oqnaiemo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wkpofgln.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mdyyavpu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jgvjlvoz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2elhpflpg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zzrtxnwt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2oyyzdepo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otxfxgjk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2liladquo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhvnbbe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2neokjvnq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kektghvx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2efzxeglx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tmmglurb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2evgqelcr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2dvakiwdx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lgrvafga.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2zzrmcssw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jovwwalg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwyxfep.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2reoxjzzo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ageoaokn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2owwkgrvv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckytxapw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vhjjhaev.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mpyuszbr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ahrfrkyb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dymmervn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cdfliquf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2svhasaew.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2mzzqvfeh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2evozzvqp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ovxiotyi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hpbltfwl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mmtfbhlp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sbycofwp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qnpuksmj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2kqlqcyvd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2skyeycrw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rqwapucx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yvqhsqxc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2peuyyzol.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mddtaxnn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ilognbdb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dhfjhedu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2usbymcbh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2opqbspwp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2emilkoql.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nqartjyv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kautmovp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2wybbcyub.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2roniwfih.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fhlceksy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cgjctalv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ohscwyda.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2glswrvhn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2sjctmssv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2remupzxs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2whmasxxe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2iwrnzsmx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sxhnlojd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2uujbmxgx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2fkhfusjy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vsidqdbc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dziifgba.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zveslzqz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gchwfzvr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xzhimlro.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2omauhtxw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtspdcjs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2imeomyqo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2alkfcsdk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vsrtgvsb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lrnmsllw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2owelwaei.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzlrgguh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2olnlvukt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jxgtrstn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ahzzezzy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cyfryovg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yggatxne.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyzresdh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2yfixdcex.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2umyrxske.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kzloonxe.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bxhkqwtc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2okennkrh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qmjnifoz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2myegqszx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wnvviqtv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dupoajfb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nuduefhv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pcsookqd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jwjxuiyk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gbpgpspi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2khogknzd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nblfwocg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hebteuxv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2atllzbsh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2scrsloxk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hgbodzls.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2iyorokik.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ftuzwmsc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ispsfmmm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ivwwfaom.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hpflkfvs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zgmrqfrh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvvfycbf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cxndeklk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2peqkyctt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2omomleig.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2rnuebdcx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2klcqtkmw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vjosrauy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mplesmib.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ksieinnp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ceapldcq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nfeuuotv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2uzbjsldu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ajlpbxju.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2gsqlgoiu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jqlvqwym.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qfwohdkb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gmqspaxt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fjamqwml.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hljdizpl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ujajlqou.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ubyomwiw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2eogyjpcg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2amnccbzf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2irchsvmw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ylovutdd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2riypumcw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vfivfgsp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ddlbahwa.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gqkjovzu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2clxnwnog.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2oixwqepb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kbmtvpxg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kduztixy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xbowlxsg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ymtxtwtc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ewoluqej.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2yydaiqie.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wjsxsqmx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ifavvjfm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2unshjfnc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2grardjuf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2woilyvbr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2chdxgvzc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qyksjpgw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wzbacoet.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2luqxnevs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kgvlhecu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wyxsyfgl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2spvbrbiq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dygknqye.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ragwmuzl.html


<!-- 参考信息 -->