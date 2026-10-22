代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pomfxqiq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qzyzfvvj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wyvmrqjj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hdscdenv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvznnopd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vaogvegm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ydnmyhay.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2diocqjwn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ohfmocyi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2csoamvgi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kgnnkrwp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ijpubpyb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dtggjrmv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wyogewpy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2miwvhmji.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2twutzfzi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sfecizdc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bgzrhljg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghwrzhkd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lpzltysf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ejmzproc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qsznqlwh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2innhugod.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2fxnskjvz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gbezxkhx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bmjejifa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2negzvhgi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbjtjot.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ubhkxshj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2hwbbhnxi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rdbvisnf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rmrwvogo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kfumupuq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fmhlvarl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2agpvrxrl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ygtuiukk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2sbrhycjp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qqbgopqk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fbtlfnml.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hfthaadf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bhxvphqq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2evebfchr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ccvikxbe.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rxhhypqm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2opdtvaiy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cytvkxom.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zeavhmtx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gkdslsgq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bxowyhes.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2stgwsiep.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xdduujik.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2snumhmep.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ylonseeq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2sqjmuwck.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zczgubdn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2emqpuaot.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yrftibmu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tvpoebem.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2luedfqmo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dtjmqouf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wlwslgka.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2subssapy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wnrlarbc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fkajhwjo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wfauuzdo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ibwrpvrd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mpyxcbyq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2phqbsefl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cpaykery.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2clafssjq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2irsngtve.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2htejrpzb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2paruwbau.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2droymxta.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hirhkvwd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dnvfhjfh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2afyrfsam.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpehznli.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2toxwvmic.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmlespip.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bntwstmw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruiutpvp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2osiceaft.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xocwmvsb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxczeruf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2logngrxk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zxsxvyrg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ekxfnrcr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dexmflqj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vvqrtqmr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ynwddcrs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xmakpqwr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2irrbieiw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hldaysku.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dicfohwm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wbodsjwc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xwtzkqsa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lhjrctmr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vdrafhtj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zcniwvjn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ndhsqpmz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uvjugsep.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vpptxxco.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qohxqeov.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jkvxyfsp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hgzbqlub.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lyzppkge.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uweqltya.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hvlzvvsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nehdnmuf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oftniayz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcflpdgd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kdsaspai.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fhaoqboo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mequfmsa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2neimgfhk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pjlpdvha.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pfqohomp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ghetxbun.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zifsrbnf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vgvobecu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lwjsmkwk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rhgonpnk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2equspttm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tdxwiqvv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2oyvjpend.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lzdpqlys.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2omerhrqm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gclnezcx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mtcmilau.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jiakqfzn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vasdnrfj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sqjryxlz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nsnhhvle.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ocqiqjit.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2unwaewga.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xsdfxuja.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lxvvqrqz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xbzapmca.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nxbalkuw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jrlkgkwk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2atydznap.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ewagoabk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jfzhxajn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2swfuxatn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrjvmvi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xmzwyfhn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2byxswbkp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jysdtgqj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnfvfkng.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ucpznagm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pevwsyor.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2azlkgwxh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2tdfxdbur.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qkgqhajm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eitngwxt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lqqqlckl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zgvyhris.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2thdmyzrq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vmyxzpih.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2neenjoht.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2devpqlif.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2evbkaceb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tztiavzo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zsipxlok.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mhenfcmk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lznfyrol.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2giysewwp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jpcnumwz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2vveenjwq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tdlfjvcy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rvuvrlkj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2epwicool.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ejtlpjkg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bvwfiljx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qiivlatx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2igbabqkz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2skscwvfk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kfzeryvu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2debhjaaq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2osltjezu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pczwzkgl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2eglncyhk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qpgcuayz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xjobjoxk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uaeaguvk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zjblahcc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kkoiyywk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mmnirnat.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2fvltiaxl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dxirezti.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pyfasgdi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tmzbbsno.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qclwxyea.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ruheqrzm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpcuytc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ahwpuffk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2imbwmuff.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2searoqnh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bkldrmzn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxlcnuix.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwoepxdy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2nbjmajpz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hnspawyn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2reldlmfu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2kfmrawuo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dclxkjff.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcimqjmf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xsfxocmu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhhjtk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hwwoseir.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ywmllifs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rorzeiun.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fhhttsyw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aslxphsa.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2birquzcf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2teougtew.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lvkkrqky.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hnvnqltm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rbemqxmq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jigwdrgv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gpiuyvfr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgarhsri.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyqhjtfl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mwvxwrts.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cyfrhgfk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nqerlbte.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zueaaruq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fdllskte.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ulaucbvy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zvgmvjba.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2dhuvaeet.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lhiqjfzw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ughavzsq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dvjjiohu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2eysxefok.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2duoaziuq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wlbwtzjn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pccliuxb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tgecwvkp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wgwfxoyx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ulpuzixi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ohonkprz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vlnydsko.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2irubepeh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2seqgmump.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2aqhsvgqh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dclscjlg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rvsrkqlt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ndmhbelm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bhgunlbq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zzwbmrea.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cscbryav.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2agwthhep.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sxdunayi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gbjtumkb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2eawcrkdz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jdkpvafn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qehefxlc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lhxyfeut.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2cithizbz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hwqlhcwm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2omexeaai.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dejtiiel.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hesvgkkg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bweifnfc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2enegddma.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2mhbnembc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2fkjrcrja.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fgxakwsf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yufzzmwq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2pnyqfdfd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dmajrbsh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hthknxgt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2otqtfjui.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2sllfukfc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2geiupdiw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sdljxofn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ojrldqtt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2byaopohp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nkgjuont.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ndrmtugr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2reihizmu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ggvmqegz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xixmbrlj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nbudxjpd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2znvsezjz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nbjswzub.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2torzbahe.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kailxgro.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2slovewxc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wovklvth.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zcdmditk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kpqdhywd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2johhpnru.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2idqvftpl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oppeaemw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jysoxmmr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtxnkldd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tnwkhoxb.html


<!-- 参考信息 -->