代发 wailian999

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sigczzwf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dqofcqgr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qdheilyr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rbeygans.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3giebjyip.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ngrfkgpp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bwjclnyu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wcyaydzf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hpooixlv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3okwcvpyq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xqifgduh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3umjjudtf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hshpfebx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3noszpuor.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3csbzomjf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ozucdmvs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3goexihww.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3upnyeyss.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uohtohvc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3szxbskjr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ymfnhcte.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ytuzdgiw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jppvzfls.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3boxnlaag.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bxgfrahm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zptoyvkd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tybywnwz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vsndcikk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jjeenlck.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hisoltvw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3aacrcvon.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3febmcktd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qavbxxqk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vbuullqr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncaaxwiv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xfauvcue.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3evdrtruo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tbtamdkn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pymzfedp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lnlwgocl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ejvsogen.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mfnmlazw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dyoibjvw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3aeieanup.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aiqubrep.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fzigftlu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ednllahe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ueyddqtn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xokvddop.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3aznbzqab.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hjlhebds.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3nejqcegl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jqnwutml.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ronnlubc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oeskgsaw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zgpjfhpp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jszofdce.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cgyhinmo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kyvqigzm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xltyaokb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qklsvuef.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ctqngfwg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3idnhywzw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ghquhfwv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xigazxit.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wcoadsmq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dzvigbom.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nonagohk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ojtelyrm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eivuiutx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3llhwsigd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3igztuwcm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbussweb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dwjaewde.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nnhkcsss.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jnshvayt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3spkgxyfj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3itgqcdrr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bokmcjry.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gjiscvdl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kxjemwdy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ailfhimv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3alzskdif.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vzdnlufo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xqylnnqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocoezzmz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvgmchhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfgijvph.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qhprwoul.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3eooefavp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jdrnggff.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bxiznopa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nximpjsf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xeelsvul.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3nfrxdxbi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uzywjyjb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wzurlmis.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3prpulsdr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pxidoymo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ldsfcxtb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qyggtqnw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fhzwhchf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3znmxwpsh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3vggmnppa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3eyaqfzyx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3djmsdzkd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mnpnotrq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dfmxlgco.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ldhqoeoo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzxaamq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3agpopbrr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fahyywma.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3keoruaim.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ghjzdgam.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rhxhxkyh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kkhbpzsl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sfigavvb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3knluztof.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3higycmcp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bffhdpsi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vyvshnkl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kgkidrbp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sfcvsksg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rlvdylqn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rlqejiab.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3sppknynt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ouiwapyv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3unodrfql.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3trbjuiqr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ewtxnxyv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fzlvqjsf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3sdlamnru.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ifeheqeu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lftvbocd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fvuvpvcc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3knxkcrlg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sufeedym.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rnykkyjg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rugnwpuc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rztnzyco.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3memznbyy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qzucynpg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3obptgqet.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ctkrmtaq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wgnwpmho.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3tssexabe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ivpsfgmd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xwqwfaqk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zngcoagu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pwujkzhr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rlpjmkct.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ebejkguf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zlfdvohf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zcopezdl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3axtdjztt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wsayaxof.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3siswlxco.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fkgehtiv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3isyjsrec.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3utggcnra.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3cpaejhyf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nkdydycp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3krvcqcja.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vjgzrsep.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hfsbvvgn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3difrkyov.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mrvuiedx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmsbydkz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ajkhcdvb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3atoqgqql.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ikgzcgub.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jhqoetzm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bilvegmi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nfqpxobn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3doumhsnb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3igcawpmy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bickdsjv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dmpkqpmx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3khmwnosi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hpddlpee.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ggmnjrvy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ybxxhnyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wptyxzku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptuwwfpg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3okjfbcmx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rqluenqy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ywfftrcl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngbmelxh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vzbltsud.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qophjmev.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3obrunzqe.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ldywctjv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ysvdubkp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3eaqcvrlm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3skgokujn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lkfxmxys.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jvzowcis.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tzqkolue.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xlsgjfzl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujqcwlrv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3miuxgiwp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yrpchdui.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wvyflput.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mwxlglcu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yxtavgih.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yhqqpjwa.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3deuwarwz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rygiysus.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yhxwakkb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxqodlsw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bcnlcxql.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qadjgtyo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3uyjgiara.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vsmjsmlt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ekpfkqlp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ecghgiro.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tbxjlotp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3laczvoou.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bsbnpiun.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3atvylnar.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cpyvxlva.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ijritbrs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qfzgmaxf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3drcjvuhi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3dmwwqkew.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dbaxbvci.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ojoeisiu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hhxwdyhk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3atonddmc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xuzrlqer.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hrxsalxe.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fncfjqgj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vpntbeba.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wqsitvgf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3twvjxmch.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ndfjuqdt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jyhqnkqu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3yyppuinh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dqbxvdbe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3apjeptql.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ttejadvn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ebepijxn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gbgiykva.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bggxjfip.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ljgtmkvd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zubziztm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wybrujql.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3quohdeuu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3izriqzgo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ofowlayb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gbmfefbf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hfdkfdrn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xxfrvrwq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3crapwech.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rggbvtrm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rqstmohw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ixltdiwm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ngabnvng.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qekoheuc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jvjgxkax.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qhnjtyxz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zcsqhecp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3swenymra.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bhdljinn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3retsztkx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yaduoxml.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kfopqodl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3itipoxzb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fdoerfuc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lhgctvfk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ekjulbbx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hmdfchqf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vndxwivh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dcffuwpq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvzblosc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aaafkxjm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bvltwafc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uyfmjevg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hhjnosqm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqgtvqpt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ccuotvus.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kiqisynv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wxkjarcu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xgutibuu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dpxviokh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rnhsqjst.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3elwiinpn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3faaqntpf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vhiicgyl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dhxthacc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wsshkuza.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zfidgedb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uenuulyv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqmxqcb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fusgutdu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lvshvnib.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tygpcqsv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3plumbgqi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kjcdsqbr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tdmrtlqi.html


<!-- 参考信息 -->