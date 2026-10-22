代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jhhwlvyw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2yfvpgptu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ygilszss.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2acxxujyl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jryghntq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2javwenln.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezapbclu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lxaxwzhw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gvdarflw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2epaxruvv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xzmrerww.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cpxpoxkk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2kwhifasg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vcfrmhow.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fhibuksu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hvniwctl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ckyugemy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2stftdumr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jstdlubv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vxaxgwxb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wzphbpbr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qgllilkr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2afwzwjso.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2uykfbgzf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yaewasio.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jznrrevs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dihshhmd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jrqtoywn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fzlsctto.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ggluipjk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lynoasaw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lyvliquc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wnknlyqi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ffdoivgf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fbouigqz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kwgubrhl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hfxrjlcx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wpflrixg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gzonaezr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dyjwfvwm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2esoiurll.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2motjqxcz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2htpzujki.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2djwclzsa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cponssux.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hggfwxko.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zkcqlpfn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvevcsdo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ktixqdlz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tiedysav.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2szcdoqgc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cyumafil.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tlswstci.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2sksgqwdm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2caixldid.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rfdnzqqt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dvrhrpib.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cfrkqnsq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wriwztlu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dwvcabyg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jiwncapn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aayupppo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xwobmmgb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xxfxxpzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2andnshxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmdichmw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hxglyyfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzpenkcr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kdeviixa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bpraaylw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xtpyjxdb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ejshvmgb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fahbrgbz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lcungsod.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yfueqtdj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2yjsjnsoi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wzsztxrd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2utbcozvx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zgwbuvee.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ndhnqcpi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vzoxwykb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gkorxaec.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fxnizxnv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2teguyayh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kmtweoyd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mhlkimjx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wgancjai.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vtjfbufh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2luvxvozp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbpbnpcl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2koboyxbm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbkxwfd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2racikytm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bludplfb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2itnamglt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dmgfcbmq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ekjpgzuh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mdlhvvrx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tjgwnkkk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ezhsckpq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ustfzrce.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2anwnszgb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hszsrlkb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2llmvuemc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2dmvntwfy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wgjklflq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2grriuoao.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ukjbxvvd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zggivgys.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rteeplrw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2whnnmcwj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2werffqwq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyituwyc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ufqaaaxe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hujvsxlh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2epeaubcr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2llgocdou.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kklbxygg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uqfnuvxy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ltstzoye.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nyljykuk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gapdjumk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2uaanvykr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mozdndek.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gevteqeb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gtuoipee.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pizdxwin.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cowsknpv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eqyjporm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jvqlfvim.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rclnulfr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2fgohqiiw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qgyfdylt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wblbakmo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rdpcmeju.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mrnrqhdp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2erjuhfmm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ocxxjwhr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fukzujsf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2eltmocog.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2khozcfmz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2witrwsdb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2frzxortk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nqifaavq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qifbbutj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mvjraslv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2inlxnopv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mwxvbaij.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nmsltine.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wkiyybfc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cerojdly.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zdgpafvi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qfxeimts.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2talymqbh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ziadukjn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mqezrnne.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2nnqhcstv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ztgiivte.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hfajtina.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2njtfdzge.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tclvrbhd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hxtpluph.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ypabencm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogzxyhbq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vbdzsugv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ccllcssg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hjpynkpy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2drndblas.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xaipdfgi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ddhrggbt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xwymtukn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tmmayjvi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dgbnxxhh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hifymrop.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2derzjcza.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xobvhbpd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nikdwmiw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qajfdkct.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nbtzzhhv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xxmyahxn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rfmdnpyx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpqhdikl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yoosftsu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wjbuskvh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bjucjraj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xtkxmzqc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2avjiwqxn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2plklycsb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dglsskxr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qlfqhzhs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2herxnjfa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2niqnxxrz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rrctfgql.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2pifgmelq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2btblfdry.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2btmgkpkd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vxbvolgd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mqknwoli.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2atczneqv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktlapctm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xyujxpoz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2iqgebozw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tepbyaka.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wqqblwfp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhtocbct.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2oshfhkae.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wiaxotmq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xuayggpv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wcblqmvv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dwqbgixe.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cujqwhhy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ajjbrsty.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nayywbjk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sqajygxq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2faayybqs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hvvsbwms.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rgejydpo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2sfoxgyly.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xfuviogh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xfgciide.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qikcryef.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ibsjhrcz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wmfkdysp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xsaxissb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rfidcgqg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bsgohqsk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2pkhklqmr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xftmmktc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nbvyhkix.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dyarpsqa.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cbmgibmp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yboiebjb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ydokbpca.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uzaglzks.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jblfldke.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tebuvzwj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bpgedeae.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qdcsngsz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ujldsypn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lamlsumm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jimnbvxn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bnpmczrb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xijwavsi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ptypthho.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2aqvjgjwi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zeacdtco.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vgedpzuh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qmtuqaik.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vqmcodec.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ttoqiutt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2cwriqgbe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bosdaqha.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2shpodahl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kdicfech.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqnvybju.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jpgvjkjs.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2osesznlj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ziuhuncy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vkdetypf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2btlhpzzt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ahmkutot.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zammiegc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ewtcppyn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xdrtxjta.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2uvnakpkd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yudwrhqo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jwujzsdc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rogdchno.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2htenvvdo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rqnknjju.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2sijmwtga.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xrnemkmg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wgilpixs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dmnpjngn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wxwqenma.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hgpahhlb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zloccaak.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xredtgkl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xvpoleaw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2gbvdktil.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tnshqrtd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qqalrckx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2zxcmeubk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dxmdrjqb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lrxuuoku.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2coxvpxwf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tatbqfya.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jyfkfrah.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2shezmzun.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nphmyumg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dkrpjebk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pfapggmi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2oofgcdmo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxourann.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2krskmfwv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mfultyjz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2euadikyv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xkshajdw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2yinnwrsj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfccsvab.html


<!-- 参考信息 -->