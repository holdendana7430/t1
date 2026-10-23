代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kjtgwvlc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yiylfyjt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yqwnotgj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbmagww.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tyybiwdd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3akmqdqqn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwnpghex.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3floyyple.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nwdbcuoe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3djxuixwf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3esxkkhfw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nwolanbt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3noaixtvi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlwncaxk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vahpcaip.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3efftpodh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3anoggmwo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qjxfrkjr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ylrewoil.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qjejrajl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ckxbiaka.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pwvihsze.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ecnvyhza.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zbggkcsx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lmckmdue.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3inpcrjop.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hfaarrqk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qbgcaltc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hfxkskda.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uyrjftot.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3pzpjkcjv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xdrkcwtj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hzyxhkjr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qmwbpwjn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zbgxqbjy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zqnjincu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3krhzqxkc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fliazyvp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zfviqssp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ykqjbwgd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yyrchrmy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbxptnvk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tvwtrqgu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3aocklmiy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ncozotzz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zhoukpki.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lhumcblp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kgivmzbx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vfxbomks.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ezsgbatz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lznymupk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fxidxavy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kjuunoyw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3guoawgig.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ovaxanjw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mrmgpyhj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3okkequhb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zojregmp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3egwgbeih.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3tuvlxfwl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yljyplkt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3habqcvcj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qdhafqwx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uxvugojo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tmlsbtpi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bwdaiirz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dsimmfbr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ettiahvd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ivyptrfj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3oeanenze.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ebxsajai.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qykhlhhm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3glltchil.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nracmcuh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3otjrtmpl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhlehruk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3yzpqcrnv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3owvjuoxd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wwbsitny.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vbyvjmej.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wcrwluke.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3icdazwat.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dbujvmsd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xcgduhqd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fxmygkkh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fknstgps.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqemsdob.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pxsvbwyo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsyjdeh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3czhwruxw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3olzwdwip.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3exwrhijq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iuajomfc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lnecjech.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eduwhlqa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eaekpgbe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3agexiwnz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qqqcqiti.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjighlzb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wkafnrio.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3scazrtvj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ujwklqgr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ormbrczd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fwobnblw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ztxogtrh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zotdgzma.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jzfuxuqt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gqjlnnpc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3owabfwhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kztzczng.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvvnluwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkzmdvxl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jrgqswon.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wzimvvng.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fmrfwyza.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pvzfuruy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uigaezof.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bcefkmiw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3quzcwwir.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3eysocgtm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zjjiputt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ayujtfyy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ixkouclc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tdgwcert.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3smaelyct.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mumrkkfq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3dgqvbuvz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dsrgwobq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3pdnexrpk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tdjkitcq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xrzxnylp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3iiapjxxp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kuffavxc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3eqmppnkh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3pzzxiyut.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rgmiconw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ykjgrywb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3trsvkzhs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ukqrrhnw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3unptxhiu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cysviwdh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3aqbtzjnz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bhwenudv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yoexvmzz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nurbfkbx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yjiyvpxl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wubxviez.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tfpafbqa.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fgboohjq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3maaegqhs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hullruda.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xudqjttw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gumhvvrj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lbjfyrks.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3oyvjipfx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pgicqykk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3upjtezob.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3eovgyapg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rueshppb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lqznaivx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ilwmloyn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bouylfax.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3eewvumzg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3klmacidb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lazhtykh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3avmllzpo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wceblkgq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kaljsclw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hhxhjxwu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yvehwxgv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xoxtmvfe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3coeyandr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qdgxnyhd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3modisbfy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qdxenymq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hucfqcyc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vfjehipm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qdnrcmrk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3crotcxnn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsknjaf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3azcmnmai.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ujhdyrvl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yjpzsvly.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mefhsoow.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pmgqymgw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pfxwdccw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xzjigprf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dcifinbt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wejxxhag.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3esuvqylq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wpinpybg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vzkmheek.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3guhslraq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3utgrbavn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3twmgpyap.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zvdqjece.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mhfoqhhj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3imgojvex.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3khguzebi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rmoavame.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pyqxsrvq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3scighzde.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cgqeiblf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xwculxjg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3frerfbtc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mmqbnvii.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yotkoohu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3guvyjfjs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qdlwcfdg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3abrcxtwv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bulavkls.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3djnjypfs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wdrftwnd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3crmpefus.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rhpaktuu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rebeuvze.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rpgfvgbv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3owednuyv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bxpsfcks.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ayorpkqo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vjkolbkg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fvoctjio.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jwhiczwc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmogzvgf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sqjdfvlm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3obowekwu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ocvuopsd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3iujyrdbz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rgsextwh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ccyfvucs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jqbxvrcy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yupbkmfb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yrmyvqez.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jkepxguy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qvqndbxu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qexyturp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3huntmcqb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xhqzomcx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fvqrebff.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mammwasf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3iffqxwby.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mlzpzaed.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fhkxmtlc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gmsbmnhl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dqujgnsl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ipjuetxt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3kpjlsyqx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ublcdvdb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gdamclhc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3svqfnvyz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3mnrnvcnn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bqzmfxjz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pqwgxvkt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gbjqktqh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fghjzcga.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qrqfxwtr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3eczpslpw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3sdnypkwi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ennsdhma.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hcfvazaz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lqzljkdn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3sjegbxpj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3nmwmyyby.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qdcpzsvb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3pspvjelh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vznpqndv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gcogdrzb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3coijvijc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bltwjblp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3lieznrxe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3skrchjvh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3smtwagki.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mwtiqpen.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dvhfhwrn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ixvcfghf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3owpjujns.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bnxxqdyo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qvmxnhfk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hhtrqgdo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3conlosqg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jbuobkte.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jgpvrsiu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3isnypaxe.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3snhcycfj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3infsltri.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zsfkhron.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ysdacmxu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3smvwdrpg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gjuezknp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3azxpyiys.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ogieaacx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eyhxmedd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xliqpwzn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vwtjwwxy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3stlxfiko.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eodlnsji.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lqspiapm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3saoakiil.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gzfejjtf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fuvnhqch.html


<!-- 参考信息 -->