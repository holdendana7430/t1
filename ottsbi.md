代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hztjvglz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xphhhqlo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rndkrcak.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yotwlenz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ueikwefq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2waadpmkm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jnakacqh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gzmmbnkf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hexsrwps.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zixkdiqa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hmbwebig.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rwsgwcdv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cxxvqqdc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xaryaima.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2emlpdbnp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rnrgcuhv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xvpzeqzp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ernsffpw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jyghmdbh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2duehtsjo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2savnfzuw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vmfutsfl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kxgcamfv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mwsgbrol.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mjmvjfaw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dfikpipz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwwohiqp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xousantg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bdufsjpu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bmnmtmbs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jhcxptmg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wnztwasj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2udzvpfzr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sfvmrwlh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fxsbygmn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sgydxfsn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qiliywkn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ufaawjlq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kiqgapsn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dsisekpk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cjldfgsy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhemcac.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2eoywdati.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hiugfkuk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2luxaribp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yzyjxspv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ytejwvhq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2omjavwey.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2akpjdznj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bexdahcy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nnvokftb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2anoekpoi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dvxkfekx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rmrrmrsa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ubsvtyle.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2miankjui.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nlqkykus.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vfmuyyhd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cizvzcyo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uhdgxnyn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmxmabjy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qfmovaru.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkjfeyry.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjnqnokw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2pralnzbi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2plihhllz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ttehgyuj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2otdzgivg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2inipwbmf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wohjnwwq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ahmqwnmr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vhgmmyfh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xtupzzkf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jfkvsoge.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2uhhoyxsm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ynjnlqil.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fnowqfnc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qpqxwcqt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mxbttdot.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2lnskjhqg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fabpxjep.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mtxwpncs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kozeavtm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2drgdqazb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wjawibnn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2aplytwpq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gmnrmimr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djixcceu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fqubtqwt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gxsoaawf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vulvzsgz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvhvlgq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kohkhxyv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvxnumfz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yslqgjxv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nuoqsvhw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cxkmpfxh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrdfeczs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffgmlpfr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sckwwkuu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfmijkze.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dokxwqwr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xpzwbqiv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rapivdug.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lsedzhnm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rxwebdpl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2giqgocsh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2brvpjbwn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2idlvmezf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gwbzlicx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eczhfpkh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zflyjkoy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eapjciwr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ggkmbtng.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yicjfvye.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zapyzxpr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ziacgwjw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ocikkgss.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbrdhai.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rlusvllf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2fyroihwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njbjmtog.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yfwkmogw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqmxgfue.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bukfsawe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ggzizirm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qwvjikjf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tbzpqoci.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kgfkkyvd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gqeoqmih.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qkvqenpn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xcbhlyhc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2usqiibkr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pcwvrxat.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2weidsfou.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ievehdko.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2unnmteww.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2echpfbzf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jyobbjel.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mpvndoso.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ocdnhkgy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2itlyympc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wipijsin.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mxpfcdcm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bhddxptx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xhhjtsis.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zqliukmt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2orcpdaid.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2orbfdfdj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2toqwyqqe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vtxhohpc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2phjkuuvq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ajyfdwxj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wljwakbu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2njymhugh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pwkjvbsp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xyngspro.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yllffzck.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dianeavx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zpjmeiue.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2iepxkjra.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2mznuxsox.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dqhksxxf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ojabjpxs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2otmliffa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jnnuuwpc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2izhxqfxn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fstvgzjp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vtjrrueb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2foufxpbt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2taiyrhno.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tniapgvz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kmszcfvu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vymcmfia.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uhtxsyui.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nfnrqyfk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lgqhgarz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tmlgsymb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2boiqucrc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vllqdrah.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dgrsnydf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tsunqndf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xigciloy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzrgdot.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lalmlymp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wkbsitvi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lqberrht.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zjrgcpaw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2thddxrsj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fqeybfzc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ejxfrlpr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mwgwfleh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pfomzudx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2etoglxaa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pxmourme.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hyacpraw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2afzorzol.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2abkrrbyg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2koomhcwc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tmtemfth.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bjbpzhzt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ancmsldr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2fqyhlnpo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qqitkgzp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sgfslahh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kgwoexns.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pffcpqpm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ukvctmeh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tcbgycvg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qohagxzp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nyqhaoam.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bzumzypp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hnunribo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgyzhssf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hhdjxvym.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zbuzzalp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pgizygvw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2onnzimrf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cnpjliyz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vupjvmnu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2extrszfk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2voarxknn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fcfwmrod.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhazdmba.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fsypzwkz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ualrubqw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mymungtm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sbbgklzb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ocqwkkhb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rmwvrpqj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2pkxnbobr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tnvqczix.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vwokldxt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2prrbhvof.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2umrmftcj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yysgnull.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lnqkwcdt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwwoalep.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wrpfkokw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zldhhymj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ytpanwlv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mxwihvsu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ckedwpsy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ewswhtij.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ibmckcsc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfaboswh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lwlmxsed.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hpopxthz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lhmnrywj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ejsfrdks.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ofdkcqpa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fzhcxmmz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zqsdbtgq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2coqkvbmu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2weoxsucx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvcxckdo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ynuzdpwa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fqafjpwa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ozccuzqc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qfisxsta.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nfxmacxi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fxahitpj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2easjrdze.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hymewyub.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zjusfruj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2upzhclpo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dpvpqkmq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dwmhakkk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qqtqzpdi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uqeyokun.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2spidopon.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2awlpyzdg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2uanbftes.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xfngzlgb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wdzqqhcn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ehilhhqa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2suqovgfu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ueghjffo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tslzjpcn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tunnohaq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hvrxbqbp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lzzbpepa.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tebnjkwm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2auftvrhq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ceucjqur.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2okhywpmd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2mouhbzlg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2hvsrzqex.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vnmktkar.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qynomekf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hldgaxhb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tyrzuyks.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jfpuxrgp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dszeauof.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jivxzclj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2uuxzmsow.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ihwcjllu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2szpjssqf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zjxukkuh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nvnfqick.html


<!-- 参考信息 -->