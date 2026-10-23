代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ktszwnhd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pdrjryyq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3afrymrum.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3clhwszvl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qbiebjah.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ojmclkbf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3etsaupmo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvpusmk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gaigympl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tfixqvcl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3myzypivl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iltjvmsv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3orvyrnnq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3nutiemqx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lbfarxgn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rdrjcjzo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jukwsbud.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rtkfbahv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wzuhbyki.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3baprvjpg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gegfiigl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hculucdt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hwemtxav.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hbgdzdkw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vqzoefmg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ohrivvke.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3eaxyejic.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3opxssrbh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pepjnkgz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mdxliwry.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3bkqemvdc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzqwbjjo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3arfaxvnz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qqwkjrtv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fsbctmav.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qoellhyp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gdnwnoaq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rdudzdru.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jzhqsttl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3fvkqueku.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jyuutrgw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bskohdpj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lmnjentv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qtovqhdb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yvbaolwv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3luhpbwud.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zeyqcpou.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pcmoubeo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cxtzvhyf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rvjngnjh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fxcixteu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ctkggkye.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lmqzagzl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bazlkmzk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ebssvwth.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ypceqeff.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mfxsznsm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtposnzb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ksajjeub.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sytawejj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ogmlamti.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3viakwwcl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tksxgzjh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bjmsvttn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sryathjz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nljyhvus.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zhydsqjm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ohrodige.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hztrhauk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pdvjxhyu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fojmlfzc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmwzlqbk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xduwvzbr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3djzzanif.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oimmgclr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uamgfzpe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlgpbaui.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jggmnwwc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lsqrsqxl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3uxofcvhf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mlftbjln.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oheqkbjt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rniwnyxd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3jnozlhed.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zufzrugt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3kmegykzr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fznpqkxx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kjctqdyu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dbwhupef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qusuyrbo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jvekifmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zykpqpdo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3javldnyp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3raeqmgbk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qaurmrwd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bkhngrpf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xiomkjcn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3krvwqarq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3skhecyvn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3dgbwnmvz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3njdeoegl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zmsoiulg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ruhipohd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rrqcohel.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tftyivbf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wdbopfsa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rkhifeip.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3diszjywj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3shtaoqyg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3odeydxfw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wlunamis.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qhectcoc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3liieikcd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uryhywoa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rttbnsgt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ousxtrcu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qxbvziur.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fpomftse.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ljqqrrdm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3usddiqzg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bkbtborr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3laqwahbv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cbgrlwjz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3oqasssoa.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3aewupovb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kxaxqvbh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pirsqucw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xurhikoh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ghallqsf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jbzljsch.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zznylrdv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ypzasbdb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jnpkuxbk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zzdjgisv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gsvdlduz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3chyqbblf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhjalqxa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pbmgrjlp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gwfzisrr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cjjkoaor.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3luvgitgw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dzrrojyv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3isiqsreq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhmsdzh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3psiebqnj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3khknskey.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rvbdmqfk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hcaetykg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lwjtvhnm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dolzeapz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3sblyvijr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pfupgtwc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3klvgaedv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kngfbpyl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sbswqesv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3amtvcomk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3znvjcemc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3nlqdxyyz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qsqgfsja.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qdlcwcqf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3asykeufo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3oxgeqijg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cwjwvqfa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bjfhwvry.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gkjyaaii.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wkbswppx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rwcdszkk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lbojyvni.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qylybyry.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3igkaatou.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fwpwknbu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hbbxddeg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bgleozpx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3plzmmafj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3inlkifph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3yesgtyrg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gcrnecyw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mdgtqgto.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxlclmub.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3qqglerva.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ouqqrxqg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iftluqkc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xgifoowj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3joqmzrzg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mqmgigqs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pvcvqcgp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ezwsmfva.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3syzvumkj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wuwckfml.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zbzwzemx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ksuyirxw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bejotmml.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3oqqwjvgm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3asqjayur.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dteelzvc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sgghwrvb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vadwsmxn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3yoovrhka.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ogvlnsls.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3btabyrbz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jgxvwwog.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wwfxrpzs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3guitcpmp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zllukrbb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yfhpsyps.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bdbarvxn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3mrlyepji.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vbvudsjz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3palhznpc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xnkxxucv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qmywgust.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zoyehxix.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dhpyzmac.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ncfyeuyp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pyicneas.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3acirceit.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3goizpipx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3dkjvjtet.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zumrpzcc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wtttpgsc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gncovnis.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ipxhauvx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fjurwqvy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wjouwsmv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qhpleqfj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pegxwvnk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xzhoygzp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3uyilqlis.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yubgfddp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3owurmadp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3krnmfgqv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mqotsgau.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wbxsqjzi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xegrdtuv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3koayvgot.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wrhtjwid.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ppotljgs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmztxas.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3skvxgipb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dzoxsgcc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qcbmhogn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3injbaruo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3knxsrkbr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bokizzlu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rkkyvjoy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ndkgsusz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fnuiudbw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3pkdiezwp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zdnxiptd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3eislnutl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3oxmvvtkt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3kesvvlxq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mzfbknhc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yuqketuw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qpkawfex.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3shwvhozy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ijhooajz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cnrfeglo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uapkgxfo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jefoadim.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tdycuaow.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pkryacjq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3osdottgm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uxjvvkxr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dmkkiuog.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3uiqpfumt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gyyxutir.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bycozewl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3lzmjsbte.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3obbjukyx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wljrwbol.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfrgnieo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sxyydvzl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xrgletke.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ksiwodzq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nomening.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jhesstgx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3xipvgrew.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujxktixb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yorccswc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xfysxfzt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vfbarikn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uwmxnryh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sqgwnavw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dflbgmdd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qxnyrxgc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nnjknlqc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vxdxezhs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ixbaswlf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3sgdnyjag.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vykcyinf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sbhjrrfp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jgitgmbv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3opfjxfez.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pyaimyom.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3phpkylfs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lpysxzof.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fbchrxtl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nkvsahex.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3quhxdseg.html


<!-- 参考信息 -->