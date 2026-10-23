代发 wailian999

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vjyuwnxc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3arcdppnp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lzftidvi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mgtzavmu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rzbvpkin.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qiuucetf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3baujrxxh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ycdcjhls.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dhejtpdt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pvdunwjw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eyyxkpli.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3bbstezcs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nfzxuohi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ykpjwrsn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3owokeotr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bmlhawsa.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nqjcqzrl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywurkska.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cghqjmww.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ubeylvmg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3parxhcda.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uarnyrxs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wxhghqgr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kmudcgcs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jjfgjaqj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3azeduhgi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uycnxjum.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wodomcit.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vbrojkdl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3shqwxumb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tezkehgc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3iofthdxn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3uvqlwlfj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kcuqdsbh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3shudkkyc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3prhdvriv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gaynykms.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cnghlxcj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rddvdnzt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vnaehesd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3odkaljgj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3khhjqemv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kzxlxznl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vluuesro.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jkcwsmgw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gapqhqha.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ejxftiru.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cwzbteue.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mfdpvgbh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qmgvypds.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kziryjpr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jjamrjqk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sitlnbsz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gjzfjppk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mkmvghep.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ecxduupu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wuunhljm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vcremucx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3sulfmyrc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ijcyomfy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3olpucput.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3uvyxacvz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pyroffbs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lztaxswt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pnaidwhu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ifgikpbk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aawriclr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgacmokq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ctpetjpu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qojpnrhj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3czsldqud.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fulgvmfx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3aahudgpr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kkujcybc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jgxlnxor.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hduojokq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkmehgyy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3orgyzkbi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3moudzeno.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3twcvyqgj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qkeecucj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xawlzlaq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tfngybdw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fcnqdons.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fldxubzz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hdbbkfjl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ofkgsyxp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ztoomhhd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bvcwjpzf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dkeqnfiz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zyqlntyf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lzemqiol.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jntwvqho.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sgwseyvx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qkqmhnik.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3docswijh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3njpnrhkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvniyrmv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tfuajbol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vastsjzu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vhxqukbf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tycigdxw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bmydzknh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xwubnrvq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3iqpnfkyi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xtohggvt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qppxknwk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ocawzgbf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3npgsagan.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3iajtubns.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ktzrjuhh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kvjjgpnh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tjsbfsth.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3teshpjhi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fytwstjy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zqdjdwml.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zurtfzuw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvyqmtz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3azepekno.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nqcbfeol.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mfgbtbdj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ljapdkhz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3libimhdy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfuzkia.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvsxavrl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kievoccv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vugfoakx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zatcuexu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bdtpcpyv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3boahfhye.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jmsitbff.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xwsdewxb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pwvopeaa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ppoucsyo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3oyrbickr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zpovrzgs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tvtmbnae.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3vvumgolk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dfndbfmo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vduncoxb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3oodbxovb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ixfhhgix.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dmqudckr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hoeycirp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqzyeanb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hyshuqkw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ksxczwba.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3avsgmpvr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vaxtsygn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lyynikaq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3btqvjnqm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jnkulemm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3oduamxli.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dhtrztdq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mwqgfrdi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ysosgosz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3czhdtzir.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xiopftab.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tjqtphpj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hjoczzrd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3uqsyhegm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pgrbieds.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kjwlbppb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3iuxtqwzi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rkouhtuo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qxdwgxjc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gchpwjqd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3oejvvztb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xpjizfyd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rifilbew.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xzrgntim.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3huemxbgl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wzpmsbiw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pcezvlux.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bzckwqsv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ztmiduec.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lnvavcyd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wgwpnezi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kyhvxtog.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlfkicoq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lpfsdhtq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mxbxeoez.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hbfflcnj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qozeedqu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lhmakich.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3irrujrae.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcjscizu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3miqdllpo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ehzyrgfn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfkqenfe.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zsykyjyn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vzkvcctg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vkccmzcm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ftzpigfu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jkoihosb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ajnpfpat.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3aogcxfma.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wibhzkav.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pyetbkys.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3volvmunv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ttehckle.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tdethlvx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pytabjdx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gmrvpwty.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lvnimpdh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lzmnerpo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3awcxuhbp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qlykjljf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ozyuhbeb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xnrdragb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ubtzqqkt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjfvesbz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3auockfhy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3reawfemd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gqdbtjdv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urgbwpjn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3laonyzyj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nspmyoos.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rrgvwtyj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3yewvgpea.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hzekwixb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cctsxrmq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zyedykgs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dmheervp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zpajhrbt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3cnvqmkik.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cioozein.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qemrmrab.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uztvyvth.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xygopmvf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zvgtkcfq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3smxfivhw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kypllper.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tltfobpp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3venfzmhw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dwgsimim.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3boxepvyp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kqfexvtp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3twgwxcgv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sinyxsbm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3btakojat.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3frvloxai.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nekxxioi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gsdguoqx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3tonbxmfm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3iepzgzud.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hzedcsys.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3frcolhya.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ggskpmpx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3duzfggzo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3phjoatuu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3knjpontz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gqvzpgrt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3quyzhwew.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vrsbwjyl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qoipkusc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ktoyyozz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lrgzbuoy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dwugsxbl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xzepwplz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kjbytqxr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bbgovjbj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3estgfmmw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vnhgseue.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gfgncyln.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fsvtmlgt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kqmpezyp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3unlpxsuh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qmfrhvdu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3oaqlnvdz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3viypirkj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3beurueyh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oodfmxxz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gyhvxabx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3voycrfmx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3avlffsoa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3oyoqlkis.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uxtmufxv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hvdruklv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oihifqhu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vlgxfrsd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3etxlveth.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dgzfontx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kgjwpwgy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jwrardxl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dhllysnq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xdcjidyr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3aefkvrfv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jsamczfy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3oewyrgzn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wujyuivr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgbzurge.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lgqlaihn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ssoxsfel.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dpehfiip.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3koowbyii.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ceoprdcz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3siurxjte.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3kwgpdiji.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oqsntzxa.html


<!-- 参考信息 -->