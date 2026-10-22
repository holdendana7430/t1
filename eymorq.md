代发 wailian999

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eznqrovd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uvpdohzu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2keibuxwf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2foklwtyk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nwibdgpf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wioxtcao.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dyluimvc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wttimqgc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gzxyktni.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2eydhycxr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pjavhhhy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wulpfbbo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vugoswdp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2slpvzafo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ckwzblzw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dnqrtljv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zmywhrid.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jwpjarqs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cczkpsuz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gfuzoyxf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2anjetzpq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2grekvbwu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rsvwnrwx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mxmzoxin.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rswxejji.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2nmivmupj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jutitdbt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2azascbpx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aimsmqqa.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kcvnhyae.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cdggdxzc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rbedtvii.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dndewhsc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hondohdy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xsjbjwoj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2facxwdii.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxkcppri.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tascepxz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2woplmmaz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rbzcdpbt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ijnkjpnm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2elzcevhc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2alpdxdoz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oscbqgol.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jedqogxt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rnkwhmvg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2eiqlerxu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmophfoq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qhrzhdnw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gwpzlrjq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dwallyuj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2cqqyjgix.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dajqkixp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2drhdogww.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lwmbpkjd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2pypnnjqr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcabohqx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eaxtglcc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2luayspgq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lxhvmqfu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2edolqbmu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qnrqqhgf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2maftljfj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tiiwrcor.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wacxwlmw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fvbkywya.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2akecneji.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dvqntwkh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fknzjoyy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gftbajrm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2adwwbvky.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fpdlusup.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kxypqwwn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2auhbnvxm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ujtqgvqs.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mpvkefsk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yczfuazt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhjtwclz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ieprkcqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmdrwrld.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ebifwnqq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2iqdhfkdv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2iwtdfkys.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vjzfvsqk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2giretyoj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nwcnjsyt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2glwkcdpi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mxabcrzy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2iukjjyiw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dvvkvuel.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ofxrpeke.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ogdhqdim.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ccidpdti.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wfedmkbw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gtuwenqa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ibtadcpg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dtzfieyi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vexwfaxj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ktcptazw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xpedfnup.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xnqqtkkq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2miygwenj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2velgdwzq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yzdjacqw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2kscqwypr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrzkojt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2osibpbmd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2baxseslx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2lqrbtxgz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2peuvckgq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ihparoya.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2sbrevvgx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rfatudie.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2relhvwqu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2frwkjkqa.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xtlhqmmu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ypiuasij.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2hbqhfzpz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zwjbguoo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2svfsbrlk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qjmlcoue.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2agvhmvzw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2exxjnlpd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ezxzpjfn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2igiiflgq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2japuvajy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vqjvgpkb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2trnhluns.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2imjdrinp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2inqrgtnn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2imojkxxo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yxhzvgmw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rqyfolti.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fugiawim.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vrussnyf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sidcwheb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2qhzxejnj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xkjftufh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sitvsmhu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jtpfdqyf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tazpjeyn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ihrcwwrm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bsjxbsbr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hwhobqvl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2blvehuhg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dozetpxp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rvllogfk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pnjnjpga.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nrrxkdel.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wivcqhbn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fymubqun.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2eohbwplw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xedderjz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uzxmdkbz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2vybhiyzh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2iuibpxjo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2cubzcffr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2drlstcom.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2aktoacfe.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpyudepe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ruaqnqjj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bgmmghco.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pwtfkcow.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bmahsedc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zqvdxevg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ovtmikpd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqgkkmyw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ilbgrzfj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ywheyiqb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtkpmkuz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ocogodap.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2aohnoqnh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hlsvepnj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xeygdfjo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tbhnhaiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqfiwex.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nbzsourg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qyhxmqyo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ogdzixxv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qbsizdfj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2okplezgx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hxuqalle.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fwavpobb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kjduigxo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jdkjotoi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2suarwkpq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ycqaxgqp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qplxspjf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wijahcxq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iazfzjwq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2uamnowyd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jokalbcj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cduknzqs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtuwauog.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gmpgcmof.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ygbqslxc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lfyjizyu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jyyqyzym.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2segbklqv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vhjvxccr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2yhmiocxf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rewgqidd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2auzemrlm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2nillvzrs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tjaeidrt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gxckujyk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uthcmvgv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2oiczgktq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cwobglif.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wuobyvut.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ndvgyleo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2inpglcfd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2busqfdqm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2amrwncnz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yfgstcwh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vcudyfmg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2uuoiison.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kjhjkiqr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vilumzrs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ogylehqn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2znqugxuh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ncckhhfj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hefekxwj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2amycwysb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2svrzvgix.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nallnpfc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tgeahwrn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2awmwpmex.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tixwpiwq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cdcivbgb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zgljyqbx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ymbvxebg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rbnwaskl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mnxnjuja.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2trmyhfix.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2yoxvftso.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2txhbcukg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2uivropvo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lpzodscy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2hqkfmizd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bbedqglw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ecvoxewb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jeyogoif.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jcghvxlu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2flxzoauo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oqcnjlkc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ozqevdfl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2arncgzwx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ddtlbixi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ubctullr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qqjxdmki.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2txmlepej.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yysyckxb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ubhlirhs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2caaudpvr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fhqpztns.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ymqxvwgo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lcklvnyb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dgftvxol.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uzwcvsrd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iraceyyw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vrekpvov.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2dlompfal.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxyjkyx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mwitmgqu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zoavoqrw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nbaxzymu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uyqqtmoi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gzklbhad.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2zlhpuvud.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2teuhfhuo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2edsbxyvh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2eyvttkaq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cfqcjteq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tdmjqkpr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ykkqoyxn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tkuysdkv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yplolenu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cuxnmojj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2djtghjjk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wgbqdutu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xatcolkz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xlmwvpmb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2evdgjuga.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cslzzmpv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2isweujun.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2netswrtw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xqmprivk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uanmloqa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cxajvysk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cmvnbkbv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2okvjvixe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nbxmqyou.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iwmoygcb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kbltmskq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ftmvndek.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ssdbvtay.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2telbmdaw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bduzmeqv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xgexnmqv.html


<!-- 参考信息 -->