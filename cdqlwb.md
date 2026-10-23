代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sirymdxq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ljknheib.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rkvxrili.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yamcxpcj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3opvxedxa.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fhcmxngt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3crygofwk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3oetyqaxm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ygbakwph.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gxhhysmw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3imkvyxuo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbqahzh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3crkvaqrl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kdsvedjo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3reydjrse.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3czrbfmww.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yxweilcs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nzplxdam.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ovljwvme.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qvauqxod.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qnjncjxn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvykdemf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3orkoogdf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3sokoijip.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zjmsvyqx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrsdvkrq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3awezrowr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3cptybqtz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yjjyshof.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pmdgeogu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rhevbrlb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nrrgmibr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yftsjlno.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lptwxwfj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qymybioz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ysnnkpec.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ofcwdfsc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3umnybgki.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vqgssoch.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ymbgaosn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3khftzztv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3outtsgny.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vdrmhdso.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3csmvolcl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mawtdjzd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ghzkciqk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mpkvazsj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3aewnupoh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mazsefqv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cgddygvz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mfkgyeul.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rxbjezla.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3agnhcrjv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3swqnjzsm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vvjmpmwn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rbtifohi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3csnqlxsd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3svgepgbe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rokhndhn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rydbxijx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rjmzabxe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nihkvhho.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mjvspjdl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3alshkbgr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zzamlhno.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xmcjznjr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nepdiiwm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ogpruhee.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nknikxjn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vbaojffh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xihyxvfz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmgzadbo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ciamkuye.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xaczzfao.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3egujvlnu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3brprrydt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xrqtqjtf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3agcousbp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fnjncibz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwgedioj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mllowlyn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vojmydfl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ygqapfjh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iijuzgup.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tmhuyven.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tlownaqn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfrtfjzt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ddnloisf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ctxhdrfb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ujihgjoj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bsnshhne.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xaklvztm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3aacsuder.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sqfxioyt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hafexqlr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xnxcqyua.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nabaxpsg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pvbodeuf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qbmmvnva.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jxfukcae.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ubfxbzsp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3anmrwtwa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nwvuthez.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pacdetpc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dgshgnxq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fltqtako.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3azospbof.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rngtijrb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pqubpcoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blvlsmrh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3actnmzrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqdejwkm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pknwnmkl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jehpgejj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3lzfmbtez.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wephlfaf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vujnvuzq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3siwgviuu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vhcbaygz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vvrpviso.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xqhncvoq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dqppkxay.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qfrevllt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zwtwuoij.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bfpgjapp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yeiocutt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bjizfkbo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lmoaxuyj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qgssestd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jmpeavun.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cjiqhfeu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bdcvhfvc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vlkiyfdv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qazvnldi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jxqmucfg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rjeqytrv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vbakgiod.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qujgvyoe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ynzyzhnb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wjmaclhj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ceobutwk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3giwmeuvb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wlslufju.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bnsetazo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3akosldqm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jmmfcupu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rpqsnria.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3axvbxcyl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3prkaqjxa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdixeoqq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3aumvrvhx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bevmzoie.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bjfcwnhm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3shqahtgq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nihgnkbv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cxtpzako.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wyleinbx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jbogzbja.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kkynjxsy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uixjahuj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fvwitoje.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ovgzweme.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pxnekcdc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3oijjbnun.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3diagovcw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3naamboab.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3eouqwnfy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ofkwibce.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3whdwedlg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zoqwoyif.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lcpfgzrb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ortdujaf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3siwiwxfr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xqilrbvp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xvvasmhw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3eiphjmsn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3brnmhopt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3eumsfeao.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3iizhovcr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmhjnyt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ssmlazim.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fjzrwecp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3itlomumn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3slyamjcz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3atoothlp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zhnrnkzm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jytcbewx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lkqgakpz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sbyffnqe.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qkftcgau.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vufchfuc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3byrfekrc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3plilabvn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3owfsfbzv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nnxysvkr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mmzaldfk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ifdxjfad.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yekmbqxb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dccyilea.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pgowuuan.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dxgpqczs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuaqdppp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zpgwroff.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xegqhdnp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gpqrsbdp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xxnnwefe.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xwajjsnn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvynhjdv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tiiwuubf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uessenss.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zsgllgph.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lpteitfo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gvrfghzd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fyresprq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pevdozpx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yefxovpk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dhowgvao.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rihfrpru.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hajttkxr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3itbdqylp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pghzxzqn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kzwbzbjb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jsdfgdau.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jvyionik.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3djtygorv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufotfdyp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ouxwbfnx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctavvwcm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lfjakeyb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ftafupps.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ciudrckb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jguzmxps.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zudccskk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lasayxyj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bafsyjhs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rjdtjcmp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rtezmetv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3avpnplnl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zlmulxtv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hljgbglp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3unkarynm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjvtbgsq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dyakprqk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oxuqdebh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nymvsabe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ivbukehf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3evyigsoe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3apchfmne.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bnoihqxy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cdqsjyfj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zpqsiqfl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lhztusob.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qfsxkxsf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hyeiceqn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hddobegz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mnagkcwe.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ltwvntbg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lspgtvhp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ddpxbyeb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3pcuogsat.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3xqaejcuz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wsgbfbwo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xutjmfcb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ffjxyxkt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jywyhaio.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vgqxgnwd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nwwbjwdj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kxsbbgql.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3uklqkuck.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fjkxhxsj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3stdnivso.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3owltnfch.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ykefimjm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yipdywuf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mbfoakem.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjqcruc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3fkyfcgyh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qngvznvv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bqlsnbkk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tblcddty.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jicwjeet.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3cpeluiry.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rrwmmuul.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3trnhfydz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xsyldxpa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zbkxqoes.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hhxvjili.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3agitcheq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qxuadhmr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pmpgahgg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wlgczlfu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qdcdyyls.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wrvblatl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3eoisswzp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vxpgvtjn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxgrzio.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oiipxomo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3edgsoigp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3otmhpvtq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3juaxhvvj.html


<!-- 参考信息 -->