代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dzwqbffi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fpovqfib.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vzobyxfz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vgueeqro.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2swotggto.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ogjizvxx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxyzsdjp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lehzznpu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2bftfnhog.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2orxegzpg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vuvmtltq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hdwampef.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jacalzki.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2yjonhfsx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xcoifdxg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2blwiseiz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nxprepgo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2pmqtxqsj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lxdkbrda.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jwrezygc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qipkenun.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nmbrrtwz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2iyqsdxls.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ctsgieja.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ofuaypsi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dyavvkaf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ucwksxqj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fsqvizwi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qypybkty.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hptsfzpm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2znhftndb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqjryedt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ghggpzed.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ohfwfgyr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bkhavwdg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrepcbnp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yfudmmkd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2tkxrktqx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wpabrfra.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ziwcisag.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mkfwenco.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qmirdvpg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dazcmrno.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lxluggjn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vpdevrlt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pquecuok.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fqjxatwo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2uuycbhgd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zfrkfxgz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pewzpypi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mfugxmlf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cwuyzrwu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzkyhoir.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2flwjfigl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2chqnlpii.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2evrnwwly.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wqwdfxij.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2urbxpufa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lokjbdxq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tzqjklsf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dcyxrlty.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wucgaqxl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ttscczwx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tkxijxxv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ndykkqvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgagukxo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dnpxlgsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxnqjjyv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xtklujcv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hgdgxitf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hqrclihm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ercdlime.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2amwuglbm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qpmaipje.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2enktwvax.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2chuoahui.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mqbgxbwk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kceewsga.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2vnuvonvk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yuivgwre.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fenggnei.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xpdcfmrt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pjiruasn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vbsqpdlm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2swcurbmn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gtushpwb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rwtnojgu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2viedxbii.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2izlwxmun.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mphiqtol.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2iswwzgqo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hydritxo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xvhoypax.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxnihzp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zudubmom.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ehpxsxse.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2kpmkwwov.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uwztjmaz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wbynczqj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ywbymwsd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gehpyvnc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xmeewybk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mxiqfnao.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qlqhkshj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xnyaytdd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2azbluxpp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wlkcfvzp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2odpkswpf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kfosrntf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2niaermji.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2bpsrtumc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lheicdzq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jsppfkua.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yvfgjxim.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ayfcxljp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iuojcqya.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xpopdeda.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ixalnnbh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qzfdlsfu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2krcwadyr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fgcsnpkb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uxxlckgs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rlpvpcno.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2otgqbpey.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mflesyej.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2iebvtoqv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ekwtvqzm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pguawuim.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qtwvvpbr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cghboivh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yzhcdtju.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dbxgmqcb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2prhjuacd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kffroirw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lccdrqkv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kmrasldd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vbeoowqr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rkkgoquz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ngmwebxn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2uobojaqk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rkiwmhhm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vdkqsiog.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bplxsahw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lpmwezxx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nkvxgzbt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gehqdvsv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gfxjzngx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttpxmimn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pojshykp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ekzorbuk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2iauiefln.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qqbhwmvk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pdwhgckm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2icyewths.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lkzhzjat.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2cicbbfzb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2rbpienyw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujwhmdle.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2olpquxph.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vbclgpou.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2npyadzfe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qxgjxxem.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fmoffcfh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xbfwtzeg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2oywdeptg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2biqkudjx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zqtrqpxf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ztcurbpk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hbuhbhag.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2pfpfvxdb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nfsqclxq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mjedxzgf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2pdaxcsxe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2furkdocc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2atdaxnqa.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jbljrcuf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xuqapynv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vwiehzhg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bciehref.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjlfkmc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wxjrsydn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2biujoskd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jcxajnes.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2stjvazdm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nqfhykxk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eoulcizu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jliopguz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eeojgkas.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nxrwhltb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ommtvisx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ohqxgdbo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2fxuortgz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2abfhvopc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2pqirimxa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ejoizynn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gbvdjvqe.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2sqiyqaes.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zakfyfgy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2gqnllqgv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uupygful.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jltdkmpb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2damwnmup.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ivumkgiz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tdukttnx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2uwynfyub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2iuzabgfs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xkkkrbql.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qgxvckph.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nvlhsklg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wnbyhomv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kpbvhuic.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uihubbzc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pexkfspa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tsengoka.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2khguxbwy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mpvncmdf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xcouimmx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2iuirshjy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2faqobrbd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2pyybhjac.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ecucceib.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ljafagqo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yotigaie.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tfkvsgyy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ppkzzusq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ishnwjdi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yhynisfg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2sbwddlbu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ipanmmgb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2elawtrci.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2aquahktw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tlstyugm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rnzgvxmo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jxyvphzg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2adzplprf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tzlmrqec.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wtxjmkxn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ffkpsaeu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ubzxlofr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wmqvonbc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gdfquvel.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xqisotbp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2goxucobx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2prrwewef.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gvskblvc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ofgmlckz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2binkeici.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fkstodaf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ztlqqiew.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wtadfmsf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hstzycfk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbievkff.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gzytmgmt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pdnrnsnl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fxisrygc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2imztdlyy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dlabbjkw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ccfzbsxt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dafktvss.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nikbbhte.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2pbxnbrbg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zmmkkacn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zcxpypar.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vffboazr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2usayemwb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2sauakrrj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2spktbxeg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zxsuazku.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2swpskfhl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fjqmikwj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vpnfogyo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2luudgrua.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2awkzegky.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2sqvfglzh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qzchohlq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sscqdkeh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gorzafbb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hicipbbe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2itwszpug.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hzebbbdr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qjrnyayh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ccczvjys.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rkdyxmbi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2scyqouww.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2eoszgeit.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2varyvfck.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2oeenlzfu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fpkwmvem.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wlleqhhj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dnyosfft.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wiipsbxb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mkosgevx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2uneatopt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikpnrxeb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2prjdmlry.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2htzduyeo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wxxpdhtw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eqekshqh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zfdajbhw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioeyilrl.html


<!-- 参考信息 -->