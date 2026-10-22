代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2urzsojyl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2phkbwgoz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fvonmznf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rfpfwwpc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zmnztpyz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fwwmaqbe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jtshvsbi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2btwaiatc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yaflftsq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cpugkhbr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xnokklmq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ohsxzmoa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2akhbqasv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2plvqkrfv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ovzyyqtt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2harvftyi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tdafojxu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ldwxyqio.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yzknycdd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kziueybk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tkworgll.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qybpbobq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofbhibmm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ffahkakh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dwzadhil.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2aqwumsln.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pjkpkzbk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2imexlbss.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hbygnjov.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pgzbgjxh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vfeebkoo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ylwkljfl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mfxjwnmq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hhdiwatq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfubjowj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2omtbnniz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2biwsmocy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2muvpwndw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fhbgtyna.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2euvrdeou.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mcjpmlho.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ildlmnhu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2syhsksbo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bnekigaq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bbvddmjl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hknmpkbr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zsagavly.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wcbwpman.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zdieebgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvjespry.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dudtzavs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kcvmoihu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvueleo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gkjdpatl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hfiznomt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yojhhhub.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qhlvimju.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fsquidbw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uhxlhuam.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mysqiqnc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2yzaqnjzt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tpdrveoe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ercwhebt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tgcutdhn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yufakrxn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hnojasln.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uvgeqvlc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hlwodgqq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bsqhuens.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2epetuqxg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xyipfpqk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zsmwhdxs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rwdstytx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdtjqjrc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wynhcqsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpoxbnsx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mwngcgex.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2sfnqqwhd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2igfpmtab.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kywozofr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ktwltalm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2roubcvgd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2beftvczq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wxxmoewf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2chubxknm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hmvscyav.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2znqtzafl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zlnzagau.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xhsykgvt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wlzcaaoz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jonqdroo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2shtnwowu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vcxrlhwm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhlouvk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fghxwjdx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qihojtzj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2votckmsk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2madmymrl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bixhkspr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2frboemlb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rrysyubp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vzksjpff.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jezkahne.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eehtglfb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2oshtxmsi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ytybacyj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bwlwggpa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2alsbmkyh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2psqonbbk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dsoogzsj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hcsonfkv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mvryxpyj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hbxwayph.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxgmponl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wgvjaysw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dkwlwqnl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rnepsbbm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jwytkzxm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vryrppqi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xyryiwey.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bopinsfy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xrwgrdli.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bhojfufe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jktaoxzm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2btwblgfj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2skptfkml.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cpyvhsii.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2chpcqqjo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tjnhkxkz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ukohjkje.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2gtfytick.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2owzbrndr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hghcjdhh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pefqzmrm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ztoccjrh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xohutusi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xedvypxg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2lmgkdvuf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2veqdjmec.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qpixjosg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rzvyqmbo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2joprzttj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uivbvwdc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bledrmpp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uhqhwqzo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gggktodi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2figgkbaf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lwmgvxfw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ybzhxsga.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gjilrswe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2jtmdjnfs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yzuabpdg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hmglctne.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jqfjjuil.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ltdaveyn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xjduvxus.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2egmpxkzw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kefdikzl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lmfkqeak.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqbdigr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ufrlkuah.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wvohirig.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rcjwsvuw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mpyipmoz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2uxcasdcg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2diqrpqqz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fhrvlqmy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hlfornnu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2davvpezi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bmqnbtfm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mvqibrbt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiwijczg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ltslmmrc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nwvkvjgo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kvwzvlef.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2iyefvzol.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ndihvizf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nbxqniyc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2olorurrb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ptsdkgqp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qmhmvsua.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2syukkhok.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qfcmkxpu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gqtbpidi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bqutapyk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2omikdauq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpmvmdon.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dpmdcmoz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pkruuece.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdezyhxm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kibrhxvr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wgtxscjo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hfzqqmya.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xalyrgep.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vvkabzqg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2scvrmdtw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2grdxugax.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mktbbzue.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2umvlbgoh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2kljcmcmi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xuwtqylc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fbpgyyig.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vhvluiwv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2oyrrxhcj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2hdwjksde.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nzjwxbnp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lyrnefyj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2svrsyerj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2eaxfkeaz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qxmihxro.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bpppubtk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hrwcldra.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kyvtechn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nxxmiibu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2shbqbpvr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2djbcnrve.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ktkpuifd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xilxvqlv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kwunxumg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zfpbswyh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vebnoena.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cewxlssr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zuqzhigf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kzanfwnn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2txxvxsaq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2snakljij.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mwcagdhz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uldiapaa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2dvpuqbps.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ixiddywk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2leegqspw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xeccgbro.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bewxtusb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jkjpuppb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nnrniiaw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2onnqaxtt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wnsqsaob.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dhownqtt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ovagwnuk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mtjalpyx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2inibrkbq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2txchctyb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2gpaiigbj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2paxivxys.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2iocnpluy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iqxcgfau.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hjsbvfpa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ukgwnwdu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wokjhzoa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rhidrufm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qzvopjod.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mpugvyny.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wjphfxnb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zxmbudyx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dkkowadj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kckzrukg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fxwcltih.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2okpbzzid.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mnwvyfgy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2faktxeqo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bjzzwpjz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2srxvghce.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oblvokru.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2slyjzfha.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2adxlclud.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kbflljxv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xoerkudb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2beaaqdsd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2liijcpfj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kxcwnsle.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mprrdbtd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2srjfbwby.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fwxapgub.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nknmykym.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tksqdtgm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pknufznh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hokcrkrc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gzzbvhar.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ydkrpvpw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gczidbaj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2bcjxodsx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2oazbsqvv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2letzvhtc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cskxdaty.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2urhoahmw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yvdvxghv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qtdsqjfa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qbqghwkn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ffvrmjpw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ogyrdgak.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kzsjvamq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kyqiohdq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rwkztmho.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wbnqcovb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2owrhixur.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wbjhrnrk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obghjtzq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2lchwsyuz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ulqftcmc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dfqmbtyz.html


<!-- 参考信息 -->