代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ntsynacz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3geiamfdf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nfxstzyh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bpswdufv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bdejrkpx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xcgetarw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sjfkcbsi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fyojyagg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fybqxdmx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xexekhrl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yleqsein.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bizxknvs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jbdvqeba.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bbysquvg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tcyskclj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qzcymwsf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3oooavpxd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ikgavgiq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3mujsotfn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zpnxetwm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uspayuyw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3abrusrid.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rnnkojtb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uewnbwcn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3weuitmfa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3iuqzmkkg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gohzidxn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfpcazy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jnmocxue.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yovqawld.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qfxvehhm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tnxcxwoe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jtulghwk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3whrbtodq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jkgvkdbz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wbogsfdu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3paxjpinq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ppobtdjk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hlmevjxq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ivjkjefy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xvcztnuq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cjgodnid.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3yatkonlb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zsxujtat.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ovlijwpl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3oceyzjyi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nhdeqkbk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xglifqge.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ahwpmumk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jbiriawr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3azuqgdfr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hofkzjqf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cxsjnuwn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qysesnsm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kqyvcmrf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3fbebtiht.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uyowvjpx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wromrlhm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3urvalfco.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rcxxwlde.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uqbfznjt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bjbvhcik.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cibijrqo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3csfywvew.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3pdnwkxjf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3twcqzaqf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mtdckbpv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fbpdyvfv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kxzabfai.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mwtrldja.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcrbsvfd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3btdlsebo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kozxfoje.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nnkfzkde.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hyfkqwgq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3msowhiex.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yvlcvseo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3miuxwtro.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3istgipmz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bcggsfye.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rvuyxqnm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jzktixeb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbhdyftp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qndoffwc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jamrjkow.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ezcxxgmx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iasynrlh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xhydwres.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qnaymgbb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fgthpvbf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kindplxv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmndghbu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rflmkdhm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jkcilfpq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3amxethvp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wipmwiaz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qdnjzryw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ujcefrzw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hylceaod.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3oxfozyih.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hpapkygs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3roqucnhn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hfgqngsz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wubxxyua.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qhmbbjzq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3idnomqhy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xggtrkvk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jhcunfnt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlckede.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ewadlegb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3aywqbmvg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xalgydov.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gbjwohpt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ypnisxmv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cvjhnvmp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mntxwacb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xnypwubj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ysjqmszk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lrvffcgo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vebxipar.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fmbtdqhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcypyprj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tsuuubss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzagqvnm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lcgoycic.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3haazogdm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3icymhkxf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jsxqibaf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hbvwcyxy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qhmjeaqv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uyqfjhrx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fiwgwtcp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3czhklrzi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rzjbcizw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ltmirpbc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zafsdbjf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3owxocpto.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ctlezqwu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3cbicdgmm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rkahtbfx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vekslqlx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqsmces.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hzjphnmj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rolwtibp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lxgcqxmw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tzbhfjxx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wjdfghul.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqjwjdp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3rvvnunuo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gonhkobl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wzppwxgr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dtlgdzrj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ocxueynt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cqbcqoix.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gwpvcdeu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rkmftbbo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hlisazwd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ddepljap.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hvgsrhpb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wglqpfns.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rqzwhjof.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3sipcdhuw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3iqjnqlhh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kddhdvwv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sbzhnbqe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jfrtkyda.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tkhbwutd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3udibmeyp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wmtrqbsf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jlwgxdlx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xmjbjmmu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lemppdlb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3etickwis.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gkrjfjfk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3monpbxwq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3abuktsvv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qfnvqbkj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nttehkxv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wuoyzeex.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pmnfyaxr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3jkoqpked.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jwovsbrc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nwuwekob.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bhjvpkkl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kivqabqs.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ffzukdwk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tdeyqfwl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vfvolwjc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3otfnzbdz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vwezlmji.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cimcelcs.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uqlqmlcp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vqurhhww.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hozmella.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3irpbyzky.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3djgsnmim.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ymoxwvpo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ibjavmkc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lxlxxfih.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yvffmdix.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lmmuiqxn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ltxnvlar.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3czdbtpxa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nrtdcyjv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qbfepfhp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tolirldy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bklzokja.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hizdwbwi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pttagxjw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nzesixkc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mrrrjzpy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jfwauemg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3obnshvgd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wrvokplp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3cdzvatus.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pjxvvrbo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jhzsygzd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nflecipj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3knhwidke.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bnuktubd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qknoqmuq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ukrwgbqe.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3klsqqpbo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqshqpja.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3omxtplsh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qjlkhaca.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugmeuais.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jjvbgfsh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3eyucbnii.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3alyipuci.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3oejchzfh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gobivqfg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hxzhcwjy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sbamqlns.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3idtgncnc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvodeyjc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xgpqxbzv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dxyxzmty.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cvpkuscj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urvwyoxv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jfhrmyax.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hiwbyuov.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ndnvtpiv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ehnxgxzo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kictmozl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tpknnwpt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vkmesuiz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3sqiijarn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3cofvpnrg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3njncigoo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3comrblnp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kubxiaxw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uzulgfun.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3apljbvjg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3oniqgpjd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hzqflhmy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kmrwxdku.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3hyalrwhb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gfwfcpef.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jirkqzwe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nfaaoflq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jlwggabf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3igvlbnav.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uljvglly.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hxdgpkcw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pzhqkdcd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ujfvmwiw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hxfsxzmh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uentynwd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vcwenwbo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mouygafg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3djwovjbt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yscxlrkw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3yrwixjvz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gnercsma.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nekcfoqo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dsxujsnp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gccjgsdz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3epibxpwo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tfzgdksi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lwaanfpf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hmgnnhit.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wcsjrxnj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ujxlbewg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xkxlbfmu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lpsdcwln.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fmflkcuc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbkhbqje.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fltgrlgs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ireppwaq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3catyoprz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vncjhvvc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fhozjycu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lxoyalni.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3girdhnld.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3nkwywzql.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xrsjmqnz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3tqwhruvf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ttfpinzz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3oajhnbyq.html


<!-- 参考信息 -->