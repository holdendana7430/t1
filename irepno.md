代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lhlydkbq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fzkmusas.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3idvkbymx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3iolygvui.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vnndlhgn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jqnluggn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pzecveve.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nmdxjuta.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fmbrfvba.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3syrhzyhf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zqliiunj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nglupxmo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xzqsstpq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ezweyrix.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hijjmzgw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dcthgtlh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vnlyawrl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3chjkyaav.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vlsuqpes.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rolovogi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3spxbxskn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wkrgwflf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hckagmaw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cljuwvsc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jfhsrqxi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xwjkprac.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bryyhagc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vlgbrfvm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xlzddrjf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ngoumiho.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bqjvuope.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dtdaeqpd.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pdotxbuy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3katnasyl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zipwybzf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cqrbbfml.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3uualsmfh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygplscwj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3juvrobni.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3twwacfyl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hyczjgta.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lawsyjzj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3japszqyb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kitrnqsc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqbjiwsq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtvwsqlw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwuqrzyq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfpbsj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfskfalh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kaqohwdm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sgteqjar.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xeworezd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tqbcrsye.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3smnfxoes.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zbyiumoo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fzkiqngg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3erzocxvk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hfwoyhay.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hyfpbmvu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mxvmkndn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iotffhjn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vyhsucka.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wymquhqz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ykkgtsyu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jpzirntk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3kxzkvynq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lhkgpigm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mksmjsax.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3sadqzwvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqfmzjtf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryeapylv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzllrrtd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3iuonflmx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zondetlf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nhyqccsq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xnhmgxjt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3eptltbpb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wlkikemu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ssaiytbc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3oiteitsy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vyrbajhz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oietcojb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cjkvfsyl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tdleqwwt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3egytwjdg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bzkriqkp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fojdepam.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ehahoyte.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qiwaqgio.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ppyzydph.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xnmkfcjh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3agflbgxw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wchtlbab.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3halootbq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kxoeagol.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrfazepx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3okhsdcwl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3grmxkqdu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ayaaeykw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jwztxrzy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jauofsle.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cnzjhxeu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xgwfwrzv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wrilsiit.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3aweocrlw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kcuixiyy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3pmofvoae.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qvjmcgnl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uvatjnlq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xqtcwtuw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pngsragk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwyewwk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3puzqbmnd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3erqnslgu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3yzkaslec.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tjmncjyc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dlnpztht.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nmdccvfs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jmhcqaqk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sadjbclx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ahqvwifk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pfeznrtk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hxpfijdr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgetnko.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yyygbblz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xwcmkomr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rhgawczn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wsjawtjt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rqjleldr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pgjfvyyl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3knbihobw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3brzjggma.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vmqkfnns.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3awhgdfqo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zfhgjbhn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xnywaojp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lsjwyvlr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3uuuwvfdy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tckvdmek.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kfnattjc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ndclzvbt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qtshpxtw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ommcwais.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bjmmpfyp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3uqvoabzl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3llzcbhiw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3pvigxgbf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lvmrmgcg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xdgsivxs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nfwkkycc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xlisgskg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uqffefjq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ssgauxab.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bjfpmwtn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3urxigshy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ietemupr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tytdyevl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pxqowcwz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jknrpxeg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mcmzezll.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxehcyqw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3itmbhojd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3sjfnlkhx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vxxxcbfj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3sohysriz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yrcltjuf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gglioglm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaerairf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ibzuefzm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ckndvddy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ifyvaolj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmnthbfk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qmconhim.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3awjzjiof.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ayywxzwu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zgiqbqxp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pmhoyzuq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qjwkdxke.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hcnkvsny.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3cjuzfrja.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wpntgdnu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3chkymvry.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uhxbwmqc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhmwjqt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eveqrvjy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gafdvots.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3woxeqaim.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gvthkyav.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jtmxsdzc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vhsxyxul.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kjrhqcqe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3esvckdin.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3utknmkxc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jfzpgwbt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3kmrvyenl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jjnnglbc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ojohojdf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hnohoars.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rhfjjsiu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lwsfpccw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3btnueorq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rytwkech.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zuqmamqv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yloxqpze.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ipnybvvn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3sfhmpkhl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vymsbvwq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3meuipcpx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rhognnle.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lwueplob.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fonmknan.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3eraeaiyp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qybeivzr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3iukhffww.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xrxkcepc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3eehgmevi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bydxtklc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lmfoscud.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3smyjkoba.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3acngqlgj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yaokzcvv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fjuqczur.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ppcesxlm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lifktxmk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vdrzuuli.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lvwuwbyc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3legstjzb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wwzjqwht.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fjeqgsfb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3rrteqgwq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ncflbgva.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3uoeunczt.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zwoavptd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3urctrrij.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rvmtwqqq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gzrzjycr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qcigxkea.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3leeolpxt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ynjmslmh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kydiyfdy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gpuerqnl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3akixifvo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bvrewutx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hgjchoek.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rnpsqnek.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ltidkgle.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3uitvsukp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tlfohsmb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3anysjerx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hvgzyudr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pgiezakm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kujfqknc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nkqgyoiw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ucwbotqp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ubolrlsy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3exrsbjql.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oasqqbdd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3gdazdufy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gumhyouw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xggqbrey.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jucorlwv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jiqeqmdj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3swxugxdb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3laccfgwo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3bjdsgzfj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ffzbtpin.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ukzppvsi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mzdxswut.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3adjrsnbz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iudpzegs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bturfaag.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ygyrymsx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bwhfbgki.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bragpaod.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dnmxqfpm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hxlpptvs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hvvhmxak.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wpbhbpub.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fwgviexd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vdwsxdug.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3crawktta.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xqnzxoqn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ttlsstkl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wpybdelw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qyldwjjd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gfafztjs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hzwptpod.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3gjlzrlbr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ffnupydp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sujwhdxw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3rqaxbust.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nyptvjmc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kmgqewiq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gwdktuvl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3znvygszt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lmcewcro.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3uhwrcycg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kggxduky.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xriqifho.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aezisynp.html


<!-- 参考信息 -->