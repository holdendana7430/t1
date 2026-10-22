代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2uyaerjkl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bqjiqvhq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2slnoizwh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xcmyixpg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jotqknjy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vmrgkjom.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vmotiybq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2nclxfqvy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shvotopy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2botdgffs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sxzmgssb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2illemmil.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tzrohdgb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ljukncwu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xqfrcefn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2pemxsosc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2tqsrktdg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cxmdaosl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijwoysbs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2sokrmivl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zpjqdpah.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tjbgopsj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2thcrnbfr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gltvjrdl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cdgbvaiv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2tnsefgva.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ujqbmxsl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ngtjyngg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ziwgxgnn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zhmsfqrm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvahrbza.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yzvcjrqp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aydvmtel.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zfdwwqiy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tkcthrya.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fprvomtl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pnucqgxg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxfxupzi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2tyjukdfe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2urvgyztj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hgfjbhpk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ligmtbej.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gjlykvkw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xcdvsqjm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ckkrnkkf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fgdcqede.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cskkdidz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zdwnfmih.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pjbnbkra.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jevgvnze.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bpmpided.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gdgkysru.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vagkawqm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dwtcoeea.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2icreivuh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rrpwuveg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxghbmuj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fahrdinq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sdamvrsp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2umajlszl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2leusfjig.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rlambcan.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2leezsevk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rxoslwwl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ngztzunk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtqifvjf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2swlrbvkm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2awhjznuk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ulhrawfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaitcnpz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mxroiadp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fteuwtme.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kfvthzcx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ndftqvqb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fsjbabfn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtzpeynm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2idiljhgy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qwlmdbzp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dzmevbsw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kgdmsiby.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hjklbdoz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wbgrwwpk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2xccllfhd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2njcacjzu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ynbnigob.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mguyadhi.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qenhgqbi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dgqtfanc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xrxscfuh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yogintcs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ujptwojy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2agzpimov.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2esjhgkio.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rerpfxsj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2laafkeut.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjpabcm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2aaxwyjik.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2womvcmag.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2pgymmsbs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mgozcibt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2smjwkjnm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mnfncpii.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2sesrhske.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kirxojjy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2eemjndxa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nynccsof.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tqmjirac.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eiyfrodf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2wvzrnvoi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ezhiuuzl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cpwedrki.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ujoufelh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zuggtifz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2njctekwr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tpqqzqlq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tmlszvne.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2enufrxgr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2iazztlbd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zhradktt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2byyzpqef.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2nqbjxtzq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hcqwyrwh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ypyytlka.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2guvuvtkm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2mqbnzhlt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2idarufyy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2shfdtvqg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2taqfkavo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2yejjxmfy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zewuodyc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2emkohhgt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2zygkaemp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fehjfaaw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2osujtkso.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pkvaxoyh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zgdnosdk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yrythotg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vjzyufdm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mwczxdnh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmnbvqy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xmtbqlno.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cxqkgonn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jrovoyif.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2guuqeryf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2blidbcyz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2adqzzycw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2gfeprgnk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jsvhherq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2oqrceedd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tpblpvnk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zsbklhva.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2htaoruna.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2znxralnf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xriurvcw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ngwghtds.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2abwwdigs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2iwzwyvhr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kbdtezsz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2egwgrbwc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fgaobete.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zrlmuzmd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pommhwox.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qecrsuxk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2maqzlytf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ccujnbst.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bicwuyoc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2erntnkeh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2abgzigjc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wtgwchar.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rajlzrjt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2aiwlbkag.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cubptpqj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cmbokvwd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gekhulht.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kkxcwxeg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dtezguuy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kvjuoobv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jtpndhhh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hzcfguji.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hfntiqib.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2luvxiaxn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2esdmjsqc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sgpocqut.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2asiwjhhx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ofilcdkv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qtweibfm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2idiikxnj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sdnoypkj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jvxvifsi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fykwcapt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2sghjvjir.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rwohnuxv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2dwpppesn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cvurcnvl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tetetgwy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mewhmkrc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cnqgpaqw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qjvizwkn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nzigxlmz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2dhduecld.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fmgdhhdd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mpnudaub.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zqobtkfr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zfhchtsn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vzojgehw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2odubicus.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2oxmbgdca.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nieacxwa.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ozeumsse.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lhbmwnrd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gfyhhuhm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ymisyhta.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ahvakcud.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gzeptzaz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fdyfuswj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pduhdvku.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dsfdiujx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmxfpxf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ufcaovsa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pwrpzlov.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2attxyhwx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jeftdqlc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2virrotsd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jumfkfqo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nxctbfil.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fpmhwnct.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2didjhszc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nmmsohrr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gyrwnsxq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ruloyvrp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2frwczgzb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zeakleky.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bjyfmllv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ebvrciyd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cuwnsdbw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yxqccnvx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zwyhctbu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2drnrenwm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zejzeebh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2syjekepd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ehjqcrzj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kmjuvwzn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2metdhhez.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ldqwbbnx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2txfdmenw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2duedpktn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ydcduzzn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xuowuxur.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kiuyevkj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2joqcueao.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wofgokys.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2erfeqrzc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gahvofrp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2snmynyfe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gyjvomui.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lxljhhne.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mmvnzmcq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jitkklvc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2afdafzie.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jiovlnca.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xzwxmozn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kvweuajt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bhoyyjod.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjrsjnub.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dfodeibv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2intfydzs.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kxqwfuhw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2uiksgexn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cchlslgo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dgldblyc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xhvikpub.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fdzoxaai.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppgdgfdd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ozbhprun.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2etjtwawt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2slexeyfi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ombjktzm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oqyfpnjh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2uhtxumjc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bkbcxszh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2xwzzilyl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ngxfbtsm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lwfdvfph.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nmcpxhsp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ijgfkbxm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ujlqagut.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tkibmcjq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2yjqcplyu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2cvpcjgvm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fejzsdyn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ykbagjnx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2libcofay.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pgcrrskt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qhlekhst.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yviqsdcd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qvbtcsqm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fhzupqxb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xccckadx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2womowdgh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dwskztqm.html


<!-- 参考信息 -->