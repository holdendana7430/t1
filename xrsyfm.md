代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lrgqjais.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ckbkxhwb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3behdyvwz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3noxqmplz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hpqyadpp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gtcmxmgi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3helvzxkd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jrhusddt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lujstnxv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vqpxhudf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xjqcbaep.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oyofnmke.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xjahylzv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3acvmypmq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3khwuwkdj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jgphdqfx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3eqproxpm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qdedqwar.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vplsfhte.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mlmcafii.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3muapmkfk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lqdnegjt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cnopukmh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xkpfwgvg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3prrnymst.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jsyeshmj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxxmvora.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzaeynu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ousjxzeh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xjfuzlht.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mfjwygad.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qdjafuzi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ajikmsuz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kwpypbrf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gjjbruxp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wlzbgumk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zuokxqlg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kvimnoad.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jrjnhedc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hgvhbinb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nlkijplw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mtzpqkzs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kgxvzasw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xcsyebrm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgdrogre.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fvaaocah.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mxgkydki.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kmrwucan.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ewydsrzf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xxsmddgl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ozmviiqw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uyflxrnt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3akuasgzv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rvyimuyw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ijjfnxvu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zrysrogl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xfdwqqbn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qlcnpofr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3oiholrcp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3khvmbkpw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jpxumhgz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aqsihtzo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wssvcbtq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zaqyzgau.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lywxgrzj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qftybooa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3oaysoomy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ikfmfnyr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fnerxzqp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ogkshnot.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnvbfdzo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lqamxehm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bgllmtbu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3biqywxda.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wkhbufyg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cvonekfk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jjoijayu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ojfchwhj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pijviela.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xmjqwllb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ltknbevh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qoqburzn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yrjvqurf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qyoutkqb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wqwtnalx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xjkgoaqk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ydcweesx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3youjcdwk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hlkedtyf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3irjvphnc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oejkfufh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3njdxhiex.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hdjbsjcb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pijcoscf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jiqlfxei.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sihjwtgc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhkducxe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3umlqcwqb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpgvjtnh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3twrehpsj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljmksrnj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qxlropzy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ievzraqi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jurgvekz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hestxkul.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bhpxnuba.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nzfkqnlz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cdrcwwbb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvlhlpz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qeakoxex.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvdqbuuo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bmbmuyrn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3koxxrcbp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blzxsoco.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3omucvrml.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dotsbsce.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qnkfupbo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lryikhjz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxpxzzg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xjacwsrz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vfqfawmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peqpyrbf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aoezbpzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsynfdvn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cynibnoy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3yqqjbqbv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ydzmgzfa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ubqknjjv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bczmrjmx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3titwucey.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3auemhwxv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vkcijevm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3idkguput.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nzmxnmgs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ciyqbdym.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3njnjnors.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hacndwix.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3twikndsy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hdtletcw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qxntcbwq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3neqapmao.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xxzsuxub.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3owrwysad.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hmkqpaiy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3heqzynwj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fiqyhubo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cmdikprq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3agqsdwst.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cqqfazbm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3iuiwtfvo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kmktlddb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbswcbf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cpoqqfup.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3izuvvrwu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jfmciqho.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pvwsnlzi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3wsgagjag.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mxorqagy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jihrwpth.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bjemxjut.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3swusahtk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cpfyjjmo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3udacmfmc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vczpmymn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nmrknceo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ytuetjay.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3usrqwfmm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yqmgywye.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cjqxrfhh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tueqhguh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vvrpaonx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpanorz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pecgpxbb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3sinflhrs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gljorjtg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3iwmukges.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mntbmwav.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3iwxjocsf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tjekoypt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wgpqmpcx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3uorjifcz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qpewqkor.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nzbcaxtp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3eeckbzqf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3flccrdup.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3dmxmxfqf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3roivdfyf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3cbucmwia.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kkzpuici.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wsgxshoz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qbjqwdnc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nbdceqgs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gribonhl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgxaczp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xteyvjsh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3olqyrend.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ffcuwaer.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3molcssah.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ywkajnat.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qoxperuo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yrlrlbbg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ahqjerov.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ifamfjnn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbjlnyd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3shagshli.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3eitdcjyx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3haoteltt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ygapusks.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dojwuaoq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3inazzeej.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ektgbgis.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3elmqpxkh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3droodtfp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okbkmuvi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fusrvjum.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gxixtyhm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dqssxvrt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xzdhwgsk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tbdnkdil.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bnqitgqd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mzfkdisn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zszygnbo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3uphvonpw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wrorpemb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fxeqjbjr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3aqvpuwzl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3krhdqedq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ygxebfss.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3doenglmt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dswnlkzs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3mzxflcib.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ciztmvvk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zfqaifxn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3okcdyiyu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zslmjdxe.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkizceyi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ewmpyrym.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylhcpeiu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3acddejak.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3acqhyffz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3helxaaap.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ubkzksqz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qpvpozfz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hqnfguwg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lqsrolzr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ylxacpon.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3krntbhcg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3eqhkwdvc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rjauhnxs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dqtqlsoq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hlgyhqup.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vryrvrwc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3aglhlouh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lcoaqikb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3aelmxljz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rhjzneok.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lqmzmcqs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pfemqtii.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ljvyrrwi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yryhbsjn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ptexpyan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3opchesio.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3imagtffq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3juviyskg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3iltlaskn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dzgnwgod.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hryxvjti.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3oifqnkfn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pmmqblgk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqwytqc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oufhwwtt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gqlkqnzs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vqagwene.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3phqgubfk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mfidwwew.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3usqhpxju.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xiibwotu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3glttcust.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uutzvayz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lhsvlxso.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ajcszaru.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lpknbfsj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ezbnftkz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lrrwtium.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3oixlnemb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3quxepeur.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3sfkjmzhl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qfmvpdun.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kgmpxfgo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nybkdqmu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3btjaqzma.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ocpkjvln.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wuizxbdl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3geuaapye.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jyszcemz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hvvrkyrv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tmojqdwc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ajhgwfog.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3whrwahrr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vhmjoeoy.html


<!-- 参考信息 -->