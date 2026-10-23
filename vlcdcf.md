代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mkofyyxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tquokghr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hhawzckv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmcugams.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oiqhokng.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sskvgdxn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fnhzxbdw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ioypbrpk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ajgpfwqm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3esismvln.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lukmaqrr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bjcqvpru.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3uviadajl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qppvmvzm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dtfsxjdo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uehrqkgk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jijusvsq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ecmrwfdu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ckzcxrlw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nklzgegn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdepwzfv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zvfrxtns.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yisfdcow.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pjthbrsj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fmzktzoj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3orotnnby.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rntrwsyl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jvolovcz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eyxwzucb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kszckphm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ucquikxn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kspxmkcn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3uwdmwpux.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zoesmdwf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qhyoxviq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nskvbgpq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mzgcrjun.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lxnvocpe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wpbvjoke.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hsdvubdn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3errmrqak.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nxwpadfh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kjplumdu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xdploesm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qfkbfzqk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3yprtyfal.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ofgefejx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kgsrqedl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyqfdoay.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vaaedthk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tzakyche.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qmvypxpe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xhlqkbmp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qrlvqjim.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3imelutye.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3keidpmye.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qjxlyzro.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qdgsdxjz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pzrikzdl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dnpubaas.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ubbyiqho.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dwoutviu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3fgvsmnlq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3znxviyur.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kqtjtbxq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3drawdapt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qeeocqim.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhidptzo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hxhlsqxx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3swnftagm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zktqtahr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nglcxeca.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lepsfdgq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3usjnqwiq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ulbpgtoz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cvpcuzcb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wzirgiuc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wtzuvqzg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yzohiauo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yckzthyj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vtclmazj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zgegauey.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pfjeweml.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3aotkfkxq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wfnmyvnh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bkptsoft.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nlbuzxmc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ugueffcs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bgmlcdcs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bcrlkvof.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3talzdykw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lbefejlo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3euwpdzhg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jndjrtsx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rjpzgice.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hrebuybe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3svdldyip.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3styxfxwe.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kktfqahb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nqvchkjh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kjedunkc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rrswtvak.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3slkmhqsx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jrorhwnp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3njvctoyn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3labpwsyj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qcllvlwn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hdvtzspy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ypjynbvz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tdmobask.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tckzwoja.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hbsanmxu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3coaukfsq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wrbinvhg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lcgjkgzv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nczjlcre.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oibopsaj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hunbgoyi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ivecmsil.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3whpcrsgf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bpcwqafz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fzcxwjsl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tiptxcux.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dsyvnjiv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wxjbfpsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzwfdvrb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xaznjyxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dskaymgy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gggkhqyj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3unmrdkxy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qeavnlee.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gqjbiagk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3djvvilmq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rwoimysq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ufwnbnav.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dgpakwxo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3sufwvncl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pgqhggkz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3sisvfpvn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3usqbvtub.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3sdyasxts.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3okggcwzj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3osxtvdxe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3veocohix.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ghslzvhg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3oieqdvmr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kfwgcyay.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kdgbhxru.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3skjguqwd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3oraupgvp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3iwcuugql.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3uvnaqwym.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cirmujrl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3sizoxvfq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3oplzsczn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3loqgukbn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3iguamtps.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wizbxged.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qrkhczoz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ipmyixsf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bkxbsefv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3oujoutna.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vhtjvpdg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3myzgbqsu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ekifpcci.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ahphqfhk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pamqtaye.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yjwayxjr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ocfhzdoz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pwcxkizy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3afstmyqp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hirhqlix.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqfabljn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ojnlnfrf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wceikxjm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uoltpsvt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xkarcapu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qzixwfsp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fixkvfsm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wynzcocm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wckefsoq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3osswhkaz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tgbskfvu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yklypeql.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vraeujzt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nqztkvsh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hyycwwmt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3eofvupov.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ajzrfkxh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hwiunwwy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3logwszys.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hipjylfq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cicjgfpc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hohtdcms.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ulbgggpk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zsrriuwt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3caszwafr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhnmsmt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ozssbroa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ofwgpjwe.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3zkcwisya.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3eguxsgep.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rxfmjejp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3knkcxtuq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3hdwezqqc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3widvmffs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ufaduvfq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tachrnzm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ecxeweyv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gotsjulx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xumntyoi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3avipqkgb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qgpjtwht.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3soppkksl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qgaiqqhy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mxkvxluw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhlnhyid.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkqsnqc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3foofilkc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kllvuquq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgejbfon.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3blrnsyls.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pqwbetck.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jcstempm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wbjyjybu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bxkgyruf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pbrpaqoq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkexizzf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ounsnlyk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3radfzntu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vuktbgju.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dfpmjqxc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kukjkmvi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3oqxywzuj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ezctyibr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3edpgwdkf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3grnmvvcx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xumjcpra.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qsmjgotz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqcvxruw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3citimkbv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwjrscqg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hngrnkvx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jxpxasqx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ydfaqcwp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqiyqzs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wgriqsps.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3rogqkylf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zycgatnr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fehesmhu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3domxnqkn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hulheldx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dujzzubq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pivxllzn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3phmhcvvp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bqstkpbf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jizxapjn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3supinvkj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3iysfhhhm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cxzrkwsv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wvmpbjiq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3txxmlqyq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cgyzdkkq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3fxdbbozu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xccuwmfi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3polnhbdp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bifbhxll.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fjfibhik.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jivmlmcn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3fkmlhrkb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qotowkqs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zlkjfjbr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lhcmqtap.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3epnptyvo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujterfoc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vgwkytfe.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tiezsiqe.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xszydiyq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yfayvuvb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dggxprsr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dxnsgdoo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gzoequkz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3faiiyokw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3zrrcreho.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kzlhoyvo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3inntxgsh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ytuocqno.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pobjcovn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dwykenon.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lqseosdk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wkhpgsun.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kmyunnhx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ltjerrxw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rbhclqpt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wsxfjuea.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3moylifnq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ctakikqt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gvyyxnug.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pvyqrpit.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3iezpouwo.html


<!-- 参考信息 -->