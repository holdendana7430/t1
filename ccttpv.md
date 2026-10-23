代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3cdoiurph.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cbhxghjc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lsdmlfrg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mhzpeqfd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vikadjfc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgfyoyso.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3irwrprna.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zmfnbiqt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jjleemym.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gqevfmdm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cqluihsi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tidnrbet.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ikippcbe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qgncjxqy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xsgrmhsl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gqolipun.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3eikbebda.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vaozkzht.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jpojikyd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sdijcgak.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mapurpbn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wybzykco.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3djguvcfd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kpmyvbif.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mcskvurf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xqkztzwu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gxiqfosf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3juccguln.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wifubflt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vhfounfp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qjjumund.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vclktolb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3frnfzrny.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lvcmokzw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lyssgrfm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddxepyad.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wtydguel.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zplcookh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3evgmkych.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vywdlscj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3brjoudze.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovmvrmkp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bkbmjrak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nocfvrne.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gnbtddal.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxjqcdm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rzlqrtjz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fdehitna.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3owotylqa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqzxfnsb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vuxuysxh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3phrhcuul.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ydypzazz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pmvoqpxf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cssbsoyu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lglizczz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yjysklcr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bqkngrfg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kncqijev.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lwkjsaxp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ummainox.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dppwdiaj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljiwhvyt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zerysiac.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kktqlsbi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bjgbjszv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jucghsvj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dbrfctlt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gyxlwxjb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oumtczmi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3apzddfih.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jfjtrrur.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hdxrwjgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpjwixdi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ehwxwcmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqcrsoef.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xqsbhhth.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ljjuropz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3measjyqy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msznquew.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jhjjrahr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3dlbkcofs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vssksgmy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zueeauni.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ljqutzgo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3magawdax.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dlfhwodx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lotmcqba.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rdboatoy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ckbztvzl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3noqrkbfj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zitalrtf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yoaiyalf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxmrulm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gyenausr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3epcyxpwb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qdfquzbe.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmqhipt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3iiammtkp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzvysie.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3smubvoii.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mhzylnjh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3junrlven.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zgxwgdcy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3knjwtenx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3gsydqyyj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cgayoexu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3psoomwcr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3sjycjvmz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3frijzjuq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wqvefzvx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xqegjpxd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3edeaopqm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbcaxuws.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gljzeaym.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gcsjpdss.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3apzjxkla.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nwxhisfk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3djiyjezk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3szecjbpc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zypxdgrh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yetodtqs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ujiosijt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nrueapoq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3swvoebbt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3aglzcrup.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hlnivtgc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3adrsjfrm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mcrxylay.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vmizyjoh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nsplwrbm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yritrlta.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3jjwtgnfh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3icemicug.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3intmymbh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3uubosmhy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3azinfkcv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zncrtxzu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ibvbgztr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vfquwlrb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qpcrjtwn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mgtqibxb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qelqcshh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3larbhahc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3mdigqofo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kmjlmmpn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kcgesvbq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3joqxiaac.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3uwthpsqe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gxqoeypo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rsbvzdws.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3sycqrrmw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3oflciqdp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yeemmhhj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xvttgrxt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nnicaczn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tmbltabn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uiiljgtk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ulflqpez.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zyxrxppj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bvpqvpvk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3dxxvjbla.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqwlqjnx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hfoxdvoj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwiczz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdfatowl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vfcfoyxx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3waxnpyes.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zilitbom.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3olaldoun.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3mniqiomv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwuplaqh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3zazdmver.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xxhpgyqj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3tnawfixt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pysbwcjm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qmyrfass.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3lyzhepgw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqvjwfyh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3esymaxve.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wuygznra.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gqmybtmj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3kbegmsve.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wjwhsvlj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ljjmdddm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hcaneulz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jjgldoze.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mahictmn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gorbaurh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zlqdblfk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3azlvmaki.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zcoaqkne.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ncprbpzi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhjfteew.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3tufsjerh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fkgsmbbs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vdxdhxrg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wseqcodb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3mdzaxksq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hwrlwswk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mrjhsbzf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ngpanhum.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3walinjtb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mosbmbtc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tekcqaby.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3edztopqr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zyniuzmc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bqucdncd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3csgxxucj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mbermrmc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zwwxulrb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3haumzlwv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3avourzqj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bvgogqzd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3bwhorpwn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vefoqtcr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vjdgrvta.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yojzbjpn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qisjhpmk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3amnwbdjr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ppooawfd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dgvonvnv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pwydadhh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ewaffdho.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3phixccud.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fbzftwdo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gbxcdvto.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3naqrdtnr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gdegffqf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3phyqijrj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zmduibgi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fxaesreo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mdssriet.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jdbxcgqi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wvueikxf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ktgseofk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jhljwkvl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3nsuhpxqc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3noosahna.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ksecnhmg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3norcxspo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lwrbryuf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3chxlkpfn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3locesdbv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tlmvyhgh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ixvabkib.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qiaackwr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tqujligd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yfqddpxc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vpwwozwf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ecunibjm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3sdevelxe.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3eshpobcw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3egnouzbn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ldxaieyu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3madcqyyw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dwbhmxpv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qboafwub.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rzyoayfh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3viegzjfm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wsweospy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rimlnqgt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgxsfvxu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cuecgass.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3uyuujmzo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xbzeipub.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3meaiffva.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qglviyky.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dumcndyl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hvqkcwgv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sxkoqdqr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jogjdgws.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mqiheomx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ixkrjnwy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lnhrhjnp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hacraybb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hshfrngc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ojmjzlih.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3axppijpd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jyvpypks.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lneseokr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3urqufshh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3umtxpnnr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vhhmzggz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nrhonagg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nstpcadk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrigmlqa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qrrlwsgo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dgrmafzp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hfuuzyvg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cgqpajbn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3amnvtzgv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wgkorydl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uweyoizf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3acugepmu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3msvindhv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uqrspgpk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tlyfuwta.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jpelkpdn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hdqhtlrf.html


<!-- 参考信息 -->