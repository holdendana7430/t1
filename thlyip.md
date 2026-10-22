代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2furitgya.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bdavjirh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2sloersmj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pbamsscd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mgdrnmqr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zuxgbrls.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ydbnridt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ftkolebn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2edxghamj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ucfkkntv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bripmgfw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hwbvxnmt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kyjxvhlr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mullworn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bbqjogxy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2utxwmogx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fgnwtloz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zkgfrmkj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ruryxune.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2niwidcqt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2iujmifmn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2glhyxnxm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nbterzug.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uyxdnpdv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ldtqozwc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2oecdhnqv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ksxqvsci.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2aalsqupk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nvfguhbz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fwvxaipy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yjaslbnr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hohccsat.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zbobbfkq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jhukoyaa.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2evmnrors.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2scnjqbhm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2auwjfbfo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uidkjsqd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hvsmogrk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cxehcixy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2alszshff.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbkfxztp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2oylygjgt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ytqhhepk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2sbmtyvxu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2utbaqxtv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ysqxmfjg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2oiyskcei.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2afefqbfm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymildgtc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwndapzg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2adutfyts.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ytzizydw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dstdkyxn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cqgutkdq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kexufuqg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dalkeome.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bctbicsu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tfpjzlih.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lblexbuo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zjdpdqyg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lwvoarpu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfixfwqf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2amdcvixl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lpvkribm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xxaigots.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xqdqyueu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dusfqjxv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bjcjklfn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2adlyqgjt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cnlyhnda.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2omiynzhb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vsewnnyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzpcvmsf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihxrrknp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqhousqp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2imqsjcyi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2icgqzsmr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2veqtghiz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ojjhqmix.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2supylfph.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2kkciwjgs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2chliswck.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uwrqjbee.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2kasxfvtv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mfrxjbqf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jzvndzjb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2plenlpjn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2robuyclt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ojaecvwr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bounnhvn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hsxliaoq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ddxwldla.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fjaaqmqp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jjfzfunf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2umtkkoim.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hxkpqikt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ubdlsfgj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tgrzmpwf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ispdfzpe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zhnfsatq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xekqdqjj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qxoswvhd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qzoeppzg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wdhcrdru.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uoefddja.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tmyfjhgv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ahkdaxeg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fqwnzpnv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qykygzcs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2guvpuais.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vdjtherw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ejcolncr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2insdypob.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2xmomeyhc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wrosieqf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kkzucpup.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ifurmyhc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jvvddodg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lcbxzoie.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2iskgputw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wieyvyop.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2knlqkxzx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qqtnxckh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zecksgue.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rjokyduw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dvooxaev.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2svivyvhl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jdujgbli.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cgoyjhkn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pinvaeyn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ncsbhozj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nkauujaw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2abuyjhis.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2prxhccot.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bfhjilvg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bzyfsdgz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wdohbebm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vkzbyecz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2itgtdwux.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ezwegqrb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bjpousgm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lhwaqxfn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2igjryzcs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2uprnquiz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2uduebria.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2syjqzkic.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tnhaedji.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qguxbkid.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ncwnfhhw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2aqskdueh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zhfrehxm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ndhxmqat.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2hgjhzrbz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ifitnome.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wimpqnoo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rsoswgdh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ooekqukj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ccobxcdk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjtlxvjw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mwijrara.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2hobfgyer.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bnxjorhz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2hwtkhzwd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2usparsaf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2feihobwy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2iqrccbsi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vcrwkfbo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dbfnjgrh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xslyyyxo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ladhrrrd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dxaompgw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2aoiczsyn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xxvborvv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2myxzmnti.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2eaumbawk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2eetalckr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qfkemxak.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tlygsuea.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2glasoqfe.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2whdpcyzo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fweujtpf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uqvjvabo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2dktagoka.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2trkfxpss.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kajpejnn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxgcnvaw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tgsyqzpk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uwtvwvwi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2smiiiwmr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2uonrvufd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bglqxuez.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gtvanzog.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2maehziho.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2hcbyobya.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cuhgrkpe.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xpczzjgo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oimuebgi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rkxrsyts.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wgnolbsf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qmytdmlm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xwyqgeco.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ctmpzlxc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ofhbtddx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zvdbxtml.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ivwjstnh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2juaqydnw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jbxdizwq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2qlmayrvs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2axazwkrw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2karqquhi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pswdvucr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dfpiwuqt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gjshlclc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lfpttujx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bjrsrdjb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2roatcicv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pzbupfrq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2guazjyzt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2itezydqs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2spjtdlsz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2viabuuil.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uahzgqyk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2iukeekso.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tvozupeh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2skqtuwum.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qzvmvyot.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pxkapoil.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mokzfhbx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gmkjania.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gzcwyrvd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2twtehbhu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jcysvhqe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vjzlelsd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2licpmphl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vujdwnet.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mstovzhw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zaawjmyw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hbedmvct.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qgtvocoq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fdlrrtql.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fcrarxbw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xdyxcwem.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2oielhnkk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cjrlqgfv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vvzxexrt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vwalllth.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rjakwtfa.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xcbxhxfd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2divqympd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2axrimvkw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zwvdctug.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ujfeejtl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lndtjozx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2cctvugun.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2klfixpcy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fgxphpmo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bdtsybdc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2juxcbkbn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hjfqrfwo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ukoicxlg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2loyuyicv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpqrojqd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sfvjldqh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ruyulton.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2slmruhqw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hjhncdgj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hdxkekdt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lpnxmfxw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2znzfbxug.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bkzyiatm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2eykprvtd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hultutzh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zpqtdvkz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2tvxpwgen.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bnmpygrg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fmxyehjv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jlzejsmo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2njpiqdud.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2bifgmtmm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hjzuafsw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tfrjyqyc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2uowefkmr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pqwszpkj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rxjgpqqg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lodyydgf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wptouxnu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2aeiquwbz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tkvhgtxm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2toaxpuul.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dniebgge.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hxggfhod.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wumvyjwj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ieqldqqu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2teqvrmws.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qpfptcwo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hcwwukcy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2sveyhtko.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2cmcemsrk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fxaywrhy.html


<!-- 参考信息 -->