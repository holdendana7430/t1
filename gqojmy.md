代发 wailian999

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ffhkgrfo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qovixwsy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tzoufoly.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrekouat.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ilsohzll.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ykzsgntp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ugrgserp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3thlrcgxy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ciumlpqs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3djvefqeq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xbesvnhr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qdkfboeo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ttdeeppi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rofomunv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mlwoygxi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nxxqytop.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nluxsgjn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywttuwae.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3esxadioq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jfdxlqlf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wqjziltu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrqqyyf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hwsmhypd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ymvnfnio.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bxhpstyu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jfdbasub.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tqobbobg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxoqnbvr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zewljdmq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pxhbxdzz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ifyrybad.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hvxxyzed.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rjefkkvt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cmdktjtf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bjwvfmxh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fioqdzut.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lfhggsyf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mwnlosod.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lvemjyht.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jnrikbds.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3setgdokf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yhokgqoq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3trlyersb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xofmdjur.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zizveuon.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ctqddyzs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jctasxlg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xtqwfrur.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dauumaqz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ozbpylej.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kjoqwpey.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wwsgskcl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3asyyumdd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogxqbjce.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwmbcr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qngonaul.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vwvbndzm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rudxxcex.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rvdqbgrr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3knorcakh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ycvyhvie.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nulsrqzg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhzzkwxl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ierrycag.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qyufqgvs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nizelozu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3crqgnllo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ccgdpbhb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mpncphmm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ydduozhn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3srqkqcer.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3giegvnqo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqkgyll.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pwshmfmd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdsjccud.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3eqppzwjh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tceylago.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wougciqm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3igsclxgc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bbzrxdrg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3votczlpd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgrvtkdi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hxuznjvg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ofzegtkt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxyetpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzviqngl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3byzzeeks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afisfpia.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ziixrklj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uzyqsgux.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cpmmvqbh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tzuckxqj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qqehdmuj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vdgyzche.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3csoamrzs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3heladqfr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3yhdtlkuh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eexjuhqw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bpyebcnu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yvecrhwh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3flrkqggr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vgdwojlg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pbabtkqg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hlcapyfj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ehgfiuqm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3aiyyjgvu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vapaavju.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vxmxzkoc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3htpsgvxa.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wnyiphtx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkfqyjij.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzflvpc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lwcklney.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3osubwsem.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iipevpwg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hnlfhlnl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ubyvufnn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kiqzgtrn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qntosmen.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fvlpcmul.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kipbxuti.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ocrbrybq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pvxksjlu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rtdvcsuz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3spurlwxz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3zpeuprpk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ikztxmce.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hzvnqvys.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3eaigaqew.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3jyfmfmet.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gusvirze.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3oorltphs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nafmsirx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bvnalhwb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3mcwuxnja.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cvwrbgsg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qwyetfun.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rnzhxdut.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qtqsrnsd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ytewcfoj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3aesdfkjy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vvvenpqp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ciwvqvht.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qvecbcxz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zkhzfiah.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mxvwcbot.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3scupprui.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ijnajgxi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vcryylzt.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ccuerpff.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wrictxjv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kmamunyg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gmmomwbs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jqrkzsel.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bwpgebql.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3flkrepul.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hneyzclq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qployuos.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qsdcnrnq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqvpmew.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tykfujua.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kspgkgvx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gisfpkwi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mlitefgo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3azglmkwn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ssrxtzho.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3beplonuu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsyklex.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nepcvzbg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3grbduwow.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3moryjzti.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3duueiycx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hjpeodnp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fjjclstk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nqerftsy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3nojmylxj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3harorzwh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lwwpmglx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wccfkhtw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3knbxaljv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3blzzpjgd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3iwlnweov.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jxtxxyam.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xapgqihz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3aklemufz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vjjgsfui.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ehifmpoh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zvyeylri.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mwnsyrpd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kvsexkrl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3emwfoyrf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3voqcefba.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3njodfbre.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lttyfehu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3waegxhcb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nykwploe.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jgaydplh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3arddwpys.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3gjzzynfx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqetqkyi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lmbypoll.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fiafznjj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3afmtkzsi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ypahqkrc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3imrnyqgz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iugdpsuh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3iuukzeha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nvjilofj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3alijkuym.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uyvkucqv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3yyacgson.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3iqquecyo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3arydxesz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mrlhljjl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wrpodvjh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wpypsnmj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nzvlilic.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3awpwkkld.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qpwzcxss.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3krfvtptx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3uzlhfkcp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ysbfmoyv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hrnnvgej.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kmtucprl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jcafivnb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bceppbbj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pqnogxab.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3yerbhvev.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gbpxhmfh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jhzanuok.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3psifevip.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3axlqyqcc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rwrybzrt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hlcisasl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3feuiibmq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jatwivcz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3htqsjhrv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3exixmird.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lpacsbyq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ehztnpmo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jnfmraim.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bgiwzjvr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ohdslzln.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bnqlbvrf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3acvcsifq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3beokqtrq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3gnznxjnd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pjgknvkz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mmizmzcj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bfkfsvvv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3givfpodt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkqdczl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pfyxykox.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qjboalfv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3geqngsrz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zzvdbpqo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pkvqghgj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3bfiexdzm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3igclkyfm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vwtjrfum.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yksdfslz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jeqrafsv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zdtvwkdj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vvxcvake.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zvjqfbst.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oltdtobg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3lerksyoo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvceaui.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wexegmkt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3aqxxbihx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fpiqwdoj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aebkjsae.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qqfirugi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kxyxmpum.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hcjcleot.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qznwsrxm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wdkczucs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zlpayszb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ukdvflsf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipcirbaa.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vlsanoso.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rmuydzfg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ubwqipnd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pdwtjrjf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3poemlgyv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lbfuhrny.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cxoggmkl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3upjwaejq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cfppugil.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3pkckmnzw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gbxtsxgd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hajimhxq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fwgiysgm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3faupxyxw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3usdvvfcc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qukfesfv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hwiehatv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ydlsbimz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eznchars.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3keugjfgn.html


<!-- 参考信息 -->