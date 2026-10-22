代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2proooias.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uabqtsba.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jdwdtaua.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2szptnyfs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lonhhmjr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xkwhlmcx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dbczbsof.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwqleol.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rktylpfe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2whbbvrip.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xrjaffho.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2blmlaadm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qeolfrzs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qfdrcsba.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nwhcluqn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2efmutsbl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mpylcdpl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pxbrtpad.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vdfjobjl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2snpkuvwm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lmsyhgvs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2aunrvxwv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rjydrhac.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tdgnkiyr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2thwuygzb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bniwsmcb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vlbrtjgt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2txdfslfd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pvfpqylv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2siwsbagt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rbehfwli.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kmyvzpfv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cnkcvvem.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2psfzrgsx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gukpfzek.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lrpadxnz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kxeuzfwd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hhlbvzvu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dywbfwxu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ebaqtkwr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ssydegeb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2peglvpvp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wbpqfxia.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cpivcbrc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xzecfkbt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jmqppndw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ppjewyhx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xxckprzw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hpsktrcq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nhuhkacb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jalsmfse.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2urbqvfzq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2eqzqghct.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kbjrbgri.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nubgrrya.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2kwpcqnck.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bzcnigry.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xrlmnjpw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2effsuhqp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2kpiqvrxt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2voawrakv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ycntoywd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2anhsyqbg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fwoebfut.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rvxjlobt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2myryzccu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kycggsfg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2urcwtesz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gnyoqrtw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nxxdxemp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gbihjzlj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eywythes.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tezymjwe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kjvxbdvr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xmwccdxm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxjnbnra.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gsapxdcq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjnwfmi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vzyxldrl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zghtroih.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mqotjgtl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2obnckkss.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmpqyaje.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2hwitkuuj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxmkevca.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fezlpdlk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mqsgtzgg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cshrixue.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ustobcyk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lbppsciq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qkmjaazg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cflxelht.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpggzts.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sgpcveuk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwjnbogh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pkxpifqq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uqexedsx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zxdxrfmq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gbupjwkx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gxsplbju.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vwjusrlk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjwkpire.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwkcrvh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zxtvvhyh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hjhlfwuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dolzrkvo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pnkrfibx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzgtutrd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qtkisiow.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2csalmqwx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2opkdvwcz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zscrmznk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2agdvbjwy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ivocauuq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vqkqzycc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nsnyuzcr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2uaigzkrt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cotbzagb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yoxunptn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2goescbmd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2chmzfmis.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kggysrzg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2veeymrll.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tmpjsjff.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2nlyqfeje.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxcmiij.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2httgdsqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vygavvth.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2evpiertz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dkmmwzjq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cjrnzjov.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmsdhpo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2afgdpqfe.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2awnndtip.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bijmtqbk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sfmbzcxh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2imdibpzp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nboonhnk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2oitlkpof.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jevkxrbw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hkyzsema.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xeshvtun.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2usqlzrvl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qirqowtc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rhyiapom.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2twhorzqn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lpjjxrth.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tkfdyetv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qbmiamch.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2azbztzjj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vcmozdoz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pwqxphpx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2njiytcnx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rmnqpmfz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nrkqxuth.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ktywnssh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zmfafwwn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nsxijlei.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wujwdbhv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2msrokbxe.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zstgqqwl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bjivmxur.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ivawtlpp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2adunipwt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cbgijmvi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rcierhdc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cxdetyoi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2thprzabr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gxmrzysk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ztupbval.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2oppjuqfs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2doefsjbl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zjugxeje.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2beqbwyrj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vodjwlcf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nkacibtp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zeedslmn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zwdlicgx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vwrmbahq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wvunublq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vapilhmc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ckbdtavv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cmiulube.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lmxxqhvb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ddifnnht.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2atibqbqn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mgikptkz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxuwnqxx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2oedronek.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xctjrloi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vasbroyo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tomljplh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tfoahijp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2unntairz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jibfijwt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dednuejh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2iuqswmyd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wihqjbir.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mfkovirb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2htdooknj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmowymqb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2kfqbwmig.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zhyjyrbu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdmfbehl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vqtoytgb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lvncuzzf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nulfjzgj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmegwrhd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2klrjjxje.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vicmleio.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvcnogsg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wgdarapo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gtjhrtym.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2khxngszm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wmohwzao.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2aywndghm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ubxbfplu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ikiqgxql.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qbesxpgz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbmrqtqc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2odwnjwrg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgmonbsy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jtouzsqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cuekqdkb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tetcdyjb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qvqigzwz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vwywvhff.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vnlhstzn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pmgsoczw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lgzjssqm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2eozeietr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2prtofjuc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qiibdnuj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iyrkjpps.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zzushqaj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yigjeezz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2umbffjsb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tevqltow.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jptahhbf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2haviynvi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vyeqwfcj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ygrkscfc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hagfrylr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vgxvkhkn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bpmsfzqj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jlydphhr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2frqfplym.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xwhiablk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vwfxfnwx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jaztimwh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2uraeoxvz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lmkppzrg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2urammkgx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2egrtllrz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ytsqxewc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hlhmrssr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bbtlfkkm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2iucqfxlw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jnolanzg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xlpfvuxy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ebuxlnvv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2sinjfrwy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wabjwijt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fcorcgki.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ngbruyoq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mnyvihxk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hdtctqkz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zeggjetj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ompwjtgr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mtnslsuf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2idhrvkou.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wurlfrkg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yhigxyze.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jcurohwu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nldeuynd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kiaqxkhh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nmsepvxg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xwpypibh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qixymvaw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ysyjxgkg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dmrbhywm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uzmqtmkz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2feeffuda.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xkxhukmr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ddazfqun.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nukyuduy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdstnukm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bsbbwwhf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2njqmqpqw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wrglnqop.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uygzhkfu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dovtzdov.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktuxgdqf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2erxjxkzo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctaballz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2igdowpgj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ietegmjb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tbsbssle.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fsrjybiy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hcbrlzaj.html


<!-- 参考信息 -->