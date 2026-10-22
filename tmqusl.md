代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hwuzooeo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xyzyixkc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bllpgrkh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ngauyurj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wfarpfmo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ykpxnxqg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mrkioloq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xhzsychz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ynqmvgbo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vncqmjhp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yvixjgnb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wtgycagb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mgwptkqt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ohggfzko.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mzfsfozx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gjjkphip.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ywvlsqpg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xffcettl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2engshnzs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fxbextvr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mffwshin.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2sqyscbcs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tdvznfkm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ntaydprx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gxwfqvws.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2crynkgqp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2txgnsgtk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2iljwbocu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2luvjexsc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zllnhuui.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mntznysl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yjawprwo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hxiyxwau.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mczhhafy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wghxiapw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gadmvlfd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fklqqyoi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uwhiyaim.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vejqfudf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yjskcquk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gsuyzfqb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kebuvatp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dysqxxvt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ihfcdhcv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zziscwfw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzqtnrn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dmjaehge.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xxpuyzlw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pzugywpn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2tfnvxagf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2woafuati.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rpbqbvhg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2njofirth.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ukjwakji.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kdhctadr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2noxilopb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gxxhrlsx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yswwibgd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pbuvhqua.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qikjvmxp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hjupyufi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hoiogjef.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hpbpcarc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2iszqwojd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2umglzkrc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ixndtouj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gudaiomb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nknqpdks.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wpualxfh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yzwsevhx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cizdmiuz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2iyptzfzg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ublibckf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ewubezad.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xppbmmnr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rfyywblj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2aoxiqoql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mewkzfeu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mhhomgbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sebsuzgf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lqeuspvr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hlpcserq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jixbonsc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oantsxtf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2nvfluovm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mdeyrbpj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bmhiuzfr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wxorkdhf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zrkgyaml.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mfmhiwlt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cvvwttmz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vnxvfytn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hxhwcwgh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2folhzeso.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2llvumvxh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2woqezldb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2rzoofxba.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nadsxwuy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vzjbdwfv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2taqalvva.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fcrlvykn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjiojtl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pigruzyp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufxwdaza.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kqhmjdta.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uawyqboy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ayskdokq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2culacgbg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uxjqtdbb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2aezyjbqd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jqolqqrm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gwgpirqj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ceeopwpu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jlslrlft.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2iacsrblx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nuhxbeyl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lqqlgzrp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uqacorsq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rsguywdm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zdkzhfmt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qtcvozkr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2upnwvtzd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wcbhnouy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2enilxniv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fsbwrxsj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hcafxpfm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2plxzkzzv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2petgqyjm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dygdtwkb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zvlhonav.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hyjiwaxa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tngqbttk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jnzrhblm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2sthnteih.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ciqkmkhr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vbikhtql.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fvqosicw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2pdqsxwyj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pabechvy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jcjgskwz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xeibndif.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gifzwswc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2unxhkvmq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hmywvtxx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rrttzdtx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bdqbbahi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2awuhmxgt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vaulvepw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kxqznayh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gumsogkv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yencbglf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2eecspnbd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pqgnsnkw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lsmhlwyt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ymoqdhjw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wgrukzht.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lrkvqgwr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nhafvkkc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qqvbtvmy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmnizez.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dwzemekx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kcsbhdhe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zcyjyqiv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vrqulxoe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2srnjrgsh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2scjxwgpd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2efpfndsn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eolszfhk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2mhnslfis.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gqiojikh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2syuutujo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ritrugkx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vgibuqjf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wdtbvlsb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cjophmqf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jnhoghfh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lxukkzwb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zbmnnswz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yqxztkxw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yoniuzlc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2tpriicdd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yknbkfkd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xaookjbn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ygcnrqjo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dfknzerj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wgqadoyz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2myxhyvma.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wdllqdqj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tcnfdxmr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yatncemc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xwbivvmp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbxbhskm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qpwdnvps.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bgortzjx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nxvgenfa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2klpadtum.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gnsomopc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sumsdtmd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qxfctbbn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2oozniols.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ggonxhzs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nrhjiscw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fgjvgajy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yczzbrej.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zrgonedb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xyqcxcnq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gpziytqj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2effowmsy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xedelryd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2anlsejjj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2aizawycq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ofekvwbm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tacdfvqm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pdfjcess.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pvdhomlz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tmmruulc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2apdlwggl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wmvfvjdf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2fcmdmyzv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cujvyrwm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rxmkpmts.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ggoebxae.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qikyxwuc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ajdygtik.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nlelybll.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2svejhcir.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hbbkmaox.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nmanmhnk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2eyltyzdq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2uhmahbjr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rayyqmyk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2etsyhutv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2nzytiypt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vunrthus.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ihicidhb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kwkliopp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2leuugevn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2oqcwjzvg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dzzaacrq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qvbsykbd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ooxxtyxy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jxaepcga.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vicyidgb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jermdfqr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2bwlivlbb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qxsdgqtw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2htvmyhps.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2gmffpxkt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2uwndlhcy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rvuqjclp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bzwomujw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rakultjl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2zwhxosta.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mtdlgzkd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ihawokmu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2oyrfhirb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nwxjyhje.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ofjkzagd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gpegeagq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uaiqkptg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bcywfbcx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uswvxbrv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hczqncff.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zulbddmo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2vuexeqqa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qqdbbysl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jkkhmgod.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2suydbmwi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2spfrvugz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2epuiflcu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xupdpnyn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2alotyikx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rnvkeimj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cdqakjkq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wksrjoru.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pvcxkjvs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2xkhxpgdd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dwnywfdp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kpckqttw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kgrnzdlv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2afftslmj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhiqaae.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mneouooz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ahpxyydo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lhvtpbbz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cqmeomrr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2guzunqdg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2faazrnqp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zrjjdgqf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vidwfrkq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qniznpin.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2yhpwhzba.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2igdscmgg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ewzveaqc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2zezrdszf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2aalxvcxw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tntequka.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wozzhtcn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2irvmswdh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sdswziaf.html


<!-- 参考信息 -->