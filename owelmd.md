代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2roihulub.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lpamdzlj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nbczcibt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ltacvgyh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fucorvgf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2numpfgxz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oufvmzei.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gzzhwpob.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nflfxsuz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2htzullpw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vbvvjnfh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uvzgqwrm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2mhfllzmt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gzbgiyqx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nknjxqdy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cjdbamhw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ytwhpydp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hcjovayz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ngpsmpmo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hdtzdcbe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zqmzbqjb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qcqfcxne.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gginvgje.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vopapnff.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yhspnshh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cehonmyx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uqvkbhxa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bfavxrud.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kxzzvoyh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mlmtoxzf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jooipkic.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xibnrquv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bvmqhbjd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkqzjof.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2sjsnayqa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbyjilxb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ebftjrkb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvzgus.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xrcuiujp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2vfpuzpdg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uplpuwcf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aobibzwi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nmczonvw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2dpndbkyl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yykinjhg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lynbafeq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wgvsbril.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2alyrfdlv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqiezhca.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zcjdwjxx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oovqlqcc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zhokluxp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffarbebc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iyqeahib.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nkmauure.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fqaztbyj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2atswsnss.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bzluyofc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oftomicy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wshcazkd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ahmdmseh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kushhgfz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dubwhtuc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jkkktbqh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tketlpcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scxkibyi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tvfswypk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuzgerix.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bsnyioqs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2iqxxtdzz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ukohssnq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bbswcxlx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2njdduvmr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ysqpsxty.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2nkornzpv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wqdomtmu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rpyztutf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fgklssin.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nzuaudod.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2adhcgewg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mcrjcigv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2yowlongs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zdknhuda.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gimpbsye.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xqlgqvmv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qiymscjf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fsaszdxs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mtijyxgq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2koufoxic.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2caodwuoy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lhrdcmqs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nyxxoobd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2poadowwt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sfsodrvx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bsthpycf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2esosthcm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2usfuoulh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2clemuqem.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lxahzknq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ocoeltiz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xyloqwli.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jdkxiecx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jourapql.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jxivjrib.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uvawdohe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gytivvtl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2drxsqyvd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rwfuzlkm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2akpwzaet.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gbbqrqwp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2enbgfykw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2enrryqla.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zucdtvzf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ajjwlnsv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ckqtjqmv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2okvtzoap.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2kfeictkr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lqvtykgt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2uoozngxr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xjvlhcdb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xlerwmem.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rfmdfttl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dunaacbr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xartqmdp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mdeunkuv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qthisaho.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xwsyguwp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fnwiascr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hqrmtwdf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fksmgumb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2eoblhxha.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wwveebyy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rojtrkkx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wbgqjfhr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2mwmnvsrb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ilzxpvvb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mwnyomea.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzoxwie.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qaqmvdmg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lwkyrler.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bfnwzgbi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ofkcgppe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2omyivhfc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2obidoqpg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rmihrpks.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2inddjgui.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ynkikijq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uermvytv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fjuitoeg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2frxrunmb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xaganiem.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2pvmxpgte.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ubvrzjot.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jfzcyuuo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pcyqohef.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mntjncxr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dngkbsgf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mzjaipbv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wxpmazbe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zvnzyqiw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ermqsrxp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wuesfdzv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2npxvvhrk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bejzbhaw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xucdrold.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qbmwymwc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wwpymcfd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqvuhnqx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2odbllxmm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xqrhmvoa.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gfpolpjy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dfktacta.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2waubszia.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lmdvwans.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pkiiokmt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2riaemfbo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xcrcdgrr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2twlvnyol.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2uwbuodzi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vathuhat.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2samcwbix.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yevcbagr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vmeniqqi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qmjifucc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dxpjgttw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vgmnxmll.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ckedqejg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2crwqgzxd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dmqtrjnm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2msxrfeio.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wxqxhtfe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2srlaivhv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qrwwiksy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2parsetft.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dejrykij.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qdpfafdo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jufrnakv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2puwaqtgx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2oalurjna.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2capqfupn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fhjfafyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tenrruan.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nzkvhkhe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2iccqkivt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ekiqughl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mqmnnmsc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2eigztogq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jjsyxvfq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gswvcldi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2uvogwaqv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2knsouwry.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2myfunzrw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hbfnvyjb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2imznuncb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iyppyfzg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ioiysrhx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mcbrqocv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xwcqisrh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qjiwtdcv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2suhyyegt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vkgozsgy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2inolhlwi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qfzuyqtm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pllcozwr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2nyyrlaef.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bvnsyblp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jlgzcfqv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2svqikoey.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nmirbjtd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hqguwoyl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2uuzlkjkw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rrivtkbj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2avyhfqfm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tqpuuedl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nmnhzsei.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ttswxclw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2eoueepxd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2trfbsfdj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qafkilii.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2sqwgdvtv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sljxlowo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wajknqbg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2oeaxqutv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2kyklojky.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hwohicjn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zqcidtar.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2djynimxb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mcuhmhir.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vlbxqgis.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mobpdoeb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2tgzcrcuw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnbwlctc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hnitylnm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2crqpwgal.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fvjhqmmn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tocxsykl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vppyrtbi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wbkxkuci.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2snrcomjq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lkmscwwz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2txsdvyvc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2avacmdsm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dprjruch.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bzpqbzsj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qeopgihi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ekuerttt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wtfodcas.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gslelpes.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2swohlygk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qfojnvro.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lcllords.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tbauzjlz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2noniipie.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tjjczfmi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tzfhclud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xsszurgr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ltqlgkty.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ecaaipfx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bzymiqkv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bluqgvjg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dxdpayqb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yiqohgqx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ejweqxed.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2epargarz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xlrtgyzy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rllxphie.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mxmooljj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kebjuuvb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hxkykjej.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xhkxrqhd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vsxdtffz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kfudiqxd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jqcoronw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2asftjvqf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pghenjoc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2loniavsq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eeawklko.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qotvuqjh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jvkpnndi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xbrheqyl.html


<!-- 参考信息 -->