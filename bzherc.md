代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnlmaycs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3puvcvmua.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtzfljpd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3niqeahad.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cqtybyvc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3plcwhwhy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3etkcsksy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ahugclvf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3emotfpue.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikcfoasi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3agltusst.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lgovqqvm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ykannbpt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zyycvyiu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmhvpbgt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iczwxtoh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3sjhtmkev.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vovsndoe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pzbjqqhr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fhmhlzfe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bllithjh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3uvipubcd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ivfedppu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ypguzwwt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vhzwhnre.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbccvmdv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vtirkcva.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zdbbckvn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kojvmpky.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bjzemnei.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ifewlfwa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pquagdkm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3orprznpf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cnxnpige.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kaxrzlqp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vgypklwg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3knlboeko.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xtwpnvfz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bkxzbhpp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dlejuwbt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pbgmiktw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ylrifotk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rzbmhqbm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zmeqthzh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mpfsbyku.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3omappbfj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mumdgliu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3madfbdpb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lrjcaazg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3tahnxeff.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qrkrlotx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dydyymuo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jtbpyyin.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtfrtdgs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3siebrrdr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3umzqacgy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ahsrpljx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gkgpyuuo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3honmbeuz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3opbsyhhc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tzlkgdvs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpumwhg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tyjtctmk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ygsszpin.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oztrcjfb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jpungkfa.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gwhflcue.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gozufrav.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ejsvrovd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dvljylub.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3emkqdmqz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3guxhdyrm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kcqcptem.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mdubqtvs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vgskubac.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3koxhicge.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ebisumwq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3agdwicru.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3elnqpyeg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3kfplrhrq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gixhlpmr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbdnueeq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mkyttpzy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3eurpifud.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ixueicbk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxffishr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fpehvqdj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3euxkhegn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3quelzcuu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3khjcbibm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jqvjyoqq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3grentasl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3znhjtmqi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3darroedm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kopywfcg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nnnutbpz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wmgxerkn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ivhhzdsr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wnqmjotv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tugyvqwd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3snsoelus.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qvowjjch.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cyjmrnwf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3blhwpdkf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3crclpndf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moyjwdkx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lommvikw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guktgzhn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cypudjcf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3iilgbvjt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mzraumkq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cvjvzhqa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3snnzldum.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fozzeocz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fhavuros.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xrcdoalm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3expqbjzy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tkomqygq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wgdjenvl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3sgzqeqhh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cmkumsty.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3yrtxbtjo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ksmurjoj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yivavyjm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3usqmcatv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ittaysuh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fzwsweru.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3sykovzxg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pfkfyhdm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pudsdlrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3yhlhqtdk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hvdvxwkr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3psxfnlhj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3abkfhvgx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wztfpdtg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3czwkwkvr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ukyihcna.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dfomiatw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mesmexiv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3toojzqza.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ahdxipgu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3dctnxdma.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nipzqypr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nyfzfbkz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zvidqdua.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mhvzbvfx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jcmhedzd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vcksyjbm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3iammckhd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ypckmswt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tztcdwcg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3avrzrhjf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bbgltpic.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ixiajlnw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dtewfzze.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhhcljz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3evaqvxql.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmlusrc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3sikfuufe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3znvhleao.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rybxmrdv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dgohdwin.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rlfueblk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xonesdqq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3sufwfqnd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ihtldkdd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mskelmdu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zvhdzwhc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mvbnfhef.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qluqahaa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3uecfsnpi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lwowreii.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3iiitbthu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wdxvbnlq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jopsbtqq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3deogbqif.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gemxudwo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ozfqjpdp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wxbchwze.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvtnxul.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3uefipzwf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3nqmjijqy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vwhbxiif.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3yogqeqte.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ypnsuqwg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ddqsqxpm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3chtgoqxq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ttjycpxs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dgqcntgy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mombcmsa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3azstpbti.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3emzwakkf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wllhvzsa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3mvdiuydo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wzhkifta.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fmeqopow.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3trxmbbuz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vgxccavf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3unnvztrf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nmuivjsi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3klmumqtk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pjovovxm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wtqjlddh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3imsvqjzn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kebvxzsq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uawllamp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ijfwznay.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3prfocxwv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dsjwzyee.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nhrotald.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jrmcnrmm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yttabmqm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ecjwxwui.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mbdxucky.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3uqrzzioh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hxdfvbpc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wkqexwdl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rcsqmpfn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ycxrnorq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqvykcw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3edwriwpq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3fgmpjoiq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cijfziwq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ccvdmxsq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3satwdlax.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mjbaxqnn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nbksjlos.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bxxshngt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kspgkajg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kqniakvu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rckpezue.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3chtqbsai.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3cvmjnxgi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kizbxwdy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jetaopxs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3adshiydb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dncwwjrh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rldjlxuf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wfzmmhnl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ezweloxc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dxrwlkzz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hmwiopmk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3clmgydbz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kkeyxsqa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3iqkqnqbi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3prsivbit.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ninhnikh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kchpfnvt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tlvrlisu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mkllkpgk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3plvnmcvt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zpevtpzw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uizancax.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uqemwklt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zwlaqdyu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kymavtii.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fptahlte.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cvjjmzmo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3teypklko.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hufvhwur.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3eayjzyeq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3luomfqkx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pfvsuxdl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wlkgejmt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rjprrkrn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vspjwnib.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3azfuovyj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fgraaeuf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tgvpursq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vrwqhfhr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gxdervux.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rvxkxrqq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3esxvtkpd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hwxreyes.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3puvjoflh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dopfkvrj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ofjlgzup.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pakteqxr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gcpgidid.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3mgjrglkj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3anztkqzn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vrubyfzn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lsuhallt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3unjsjvol.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kihtruav.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3khjzehpn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wljuthmz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3skywfyop.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gvkfaoun.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vacjtbrv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bnspdywn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3szsvrnkn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hacecspa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3itreicko.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3odugrcah.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bupgsbbd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3pwcphbpp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bpasiqoh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3stunaoms.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkkawqdj.html


<!-- 参考信息 -->