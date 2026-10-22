代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2axjbdsqp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cmoksijl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nthcfaxw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sdavytrz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hqcmoqzk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xnxxvemd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2muxljavu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2slzikcrb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2iueyesjc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vaiwavwt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2oinekntl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lvgclugl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2acwkkyln.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwovvkr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hmuqqwfz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwhaojwe.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yzgkpkqy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jbovafzk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wjeqzffc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cgcjoinr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2omozzvel.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2edoelyfs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2myokirfv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2uafjqfar.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kclxjsnr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hecgkslu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2soisqihj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2kbicaiyk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eylryboc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uhhlnlsp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gehkeuek.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2eolrdhrw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2adzbevge.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wpxskydl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cgvxodpo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hvgeqaol.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wtojgdbf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2socyhjnq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cixdwtid.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kdalxutv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tpgrfwfm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qxyrknnk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2necokvif.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtnuvrca.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vfzoijcc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2irogcbmw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2llngbnbh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yehrsylk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjldutva.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wxqcsiad.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ltqsvwjl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pdixzuyb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2eejbsyqe.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qgdtewdm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zrqsxiid.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2boogfnbk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wdkzbtnb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qhvolwxm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2shbaixxk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gffgtcka.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2reerdzah.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2syphkoeq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2usxkfmnp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rvpztgut.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xrxoncvy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bnpguugn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xwcdkyyc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2krxxhzxy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ikzrwwos.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2crjltqvx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmdxinq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tjsbxgvp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zkhznvqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtnpphes.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ugkijfik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdmnmleb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2eupyxydg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2sacxvlub.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yhpgmjmx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2frwhwltr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xorquyig.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vcnoxqbq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zolaiztg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jallvalb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ngggjtpk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vibakdfk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hvwlpogj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lgdycnbf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wavnghjg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2evlufvbn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mlptopao.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2udxvtybt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ykqtwiuv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gtokirqn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pjfcdycf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cbosufvq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2htnizdly.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozxscpvc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2igsmztfj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uymylwpe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mhluixsh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ythiloni.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xgueagtf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpnnjov.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vgefmnwj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bpamksjc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wytxrjlm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vffatote.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ytkkchkd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ojfbybqa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cnalipfp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wqzoccnu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2aegxxgta.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jjxbotol.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hgzutdxd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uvrftlll.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wrlzjelg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qyldtlgf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2anksijil.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ugqfqkav.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2eovtgygz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ssjdocey.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ezlnsusy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tgcjweve.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fxqtlqpz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gbhmjupr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aacwsxek.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tyicdxax.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pyeefcvr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zuviopoc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nvcomwkp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dexoxqrp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nuojyfiz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2cloexrfs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ngvrmlao.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zhkrkjbz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qbbopmyn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2adnzeyae.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kiakboqb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2pwnosrim.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ssdjzaqg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xapuwkkl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cwzgygbz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bttfuthb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uvgaszcs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fugryuxu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xyqyaxhs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nquiqiro.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2hhhdjany.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2pcjffnnt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hwosfamn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vlwvdsbn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xkojwphe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cjatlhjh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2htmrxoib.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fkxxpkds.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nymgkjzg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kidudrmn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2llcglcbp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wbbeyyiw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rwopirty.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2andxdsfh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gnfvdyho.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tsaisdfl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tkbbwmwh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpsgxati.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qrfdyncr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yadyfjbj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zimfctdk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2thbftzax.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2djbhyfqc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hczijhji.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zywbyzna.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cobatrjn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2lxssdxwa.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pfldxynz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fjnasxrb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zjlmtuvb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgkbuzav.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vooxrlqd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nmcgoyug.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2pisrfxkv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fxmepxig.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kksyzxdh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cswokbyo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vgsfzdme.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dkautnre.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atjoecer.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fxhkhwox.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2aczyyyyi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2krgadkok.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2moedtyha.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hkqrlter.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vrajpzfi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ocvxzjqq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2czyncjnn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bujviueu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wwfmmwdi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nqwfsibc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ftodkpjr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zkpeuuua.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2nyvetevz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gcgmupjx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kyxcagjy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2rfsztxgs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fvviigjy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wwdmyclg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvlefbah.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gvlhpdxz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2enxzobve.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2nyqothez.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pvqsjasr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ogheknbn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2btmmmgtb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dhxtnuuz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2aasfhojf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2doarjjwp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yuztxahz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wbrvsqvv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wqnueiwg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yneanydg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yhabqrfr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yabkytur.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qaxoappw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wienvoha.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ustfnfkf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2eqlcsddi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2knqcevpy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ahknltcg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xtusxccs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rviwnsgs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tnwtvlbo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2aylnezfb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jvljrhvs.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hzjeinoz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nkcfljwb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wqznnzev.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lwsecljg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2awwktoji.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydwwatdt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mrvyiwcd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uauolhgk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2sicpggjm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2evpknaqi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qxakpafb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rkmdofhb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ybjvfhrf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gpoczood.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xosjbdgv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xvdmsjec.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cygbeiyf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2odiqphof.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2khcnunev.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fumokxzl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2laxtbrru.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zzrhfvtn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2qychxyxd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mehixgqn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rryfslez.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yhqbqayr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfmtighj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2eolneoct.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvnqxxmt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tiebtqvh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nepuymua.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pecdxveb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2avzsvdzy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2becjcvll.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nzhldqlv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rppvqcdn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2glavxnde.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ejdokjde.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ftjjrtof.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2rlhndjbe.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dpmfhwnq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2degidfwr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jyxiolem.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2iwcjmqcg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gpsrxdla.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2goymbagu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xvrnyski.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qgsxlwyp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ykaaybxl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bvnpgjnf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2epwrxwez.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ewarbaiw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2szcibfgt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2psohlmup.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jcigxyaw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bsuloelp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nldmwile.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qxvsksso.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qkwqoyjm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jxlpfdya.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kznbjbmc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pnyjnspo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xusnagyp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xwfdonpo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2pmojiakk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2akiaqzkq.html


<!-- 参考信息 -->