代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dxlxseem.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sdiscmyx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3abwkmcwa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bgwccayh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3sevvikrc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3brhgbhfo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mthulcei.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ehxlpwvj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xcpojiwk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xalmpkzl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3elsdgzgb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3tatxoqll.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qkizxjfz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ocfvutll.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hvfjqdok.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vhsuvnwh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mawqackm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qmpbhjpq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nmnwgdbj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nghsbhmg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzuhmyhj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mztlzyrk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yuexdxbg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmsbkfzj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3woidopmz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gmggsytg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3epzklcwj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slxdvwzt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3thlaziff.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pupgfaaz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3byjpdzfs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxtguwbd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vkixxzqo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3efodjhqd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3homlpdos.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rlzzrozp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycqpwvrm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxfifzhp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oemnbjiz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mdqzmwup.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3agtrrdfk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pmiqpahk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3peastykm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pzukoeam.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xwgcpnny.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mnkcaior.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jxigjwvi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rlojuyih.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3snsqnjhh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ioganfqs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fotdwalz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3urtkrwfv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3allradbe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bneqpmmn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ruxhxvsl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kpgkgoav.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rlxqclua.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ptqxpeun.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sfticuot.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3geuhfftb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3qbnwtcmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ginvosbd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3olpqfxeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbhlkzqh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hpcqdtul.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nhmnxguv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kpfkvdxj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lxtbzimv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3aubehccf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yvtoihod.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3stgayrwr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fabjnlfr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ksfreswm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dptswfpu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3okhieuuz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ebvfnxpp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3whickfsq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bofshzlo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rtwzyrfg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wrzadzsn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tiacahpw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3spmeghbe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qzltencp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hyajvtwt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wamxssgk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtnaphyl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3fgqvqfdp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3toewzrzx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3djccmyxn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjpsbhq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3eamcekzn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pizkblzx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hgkqfhfq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cbtxwxck.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3yeaeurjb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3syucvdss.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3sjawghsy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3etimnjsh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3uanuyqvu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eirfdzmw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vrsoysrz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xqszvvws.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kvfnxydf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hvzgucxj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wkczplfe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3urqyyrqb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ylqykrhi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jspuitel.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmotirar.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dkvwggio.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xsulmkne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3udypjqeu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lufswbsk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbultcb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ruvbclyt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qosyqekd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hvbdghzy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3udohefhk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sqkmgfqf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lmofpvzr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3czcbthln.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hcjfyskm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3brkmljas.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ftkhxsyf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3atvclvqw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kqrmuzco.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cfawqjzw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3juujhqpz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3iinyelss.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3meqxqejd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jxdbrejr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3sclxnrxz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3zjsxqlfn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3utzmbhrq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3dcgryxsn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vkzkcrta.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fjjzfzcj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3odwnwhso.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ndocnwki.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jmtryagq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sbbzssyz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jdefscpn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tsgkldpc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfcxdjic.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3kvgplxcp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qsdmgfed.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ouuiqtgx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ezzgoahm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3depkjmlu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3romxygly.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mdciotmf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ivllmsvl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvazicky.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3asujfqjl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxzrprpw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3isnnyegx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3inxwogwo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3leknqfdp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swwqevzh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opokfuxv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kxczbvgp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jmaimvmm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rfcrxicy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gcmswhqt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pfgckqej.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uaucdnfn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zatqnjrl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nkksadld.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wahioxsi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wrdkpaib.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qplvzudm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hxjznzza.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ickpsuzn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pjovgamu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3djxivpii.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3csxgjkfy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oqcgtuwj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zfowjcuy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kijhvmjf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pmvlxyud.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dkejllkw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqjedmnj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gmebtssh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dhnbfcxx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jvoyojwy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3haebgsyn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pbanxudv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3eiocqitl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3frodiyyb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3drtiimfe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3msnhlepn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3joecjqwv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3leacydzv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zlzzratw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bbsfasjo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ceyuawol.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qgaqzwor.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3duyxfdql.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qurkhpco.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3iaewnsbv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3oqkxtgtf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdylakjg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uwuuuaph.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cyddtbqp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvnnqwmh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mgvcnjpp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3emtafrmg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3hoxqoebo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ywughqxk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cruiqfsa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vkwovndy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3lvhorzte.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rucwigdw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3frxqqfsr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3knayjwbx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oxhycjdw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bvgteqyu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hbkszabv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ntydfssz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3fkirzvax.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3htrgynax.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tbvoajpl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zoenqzee.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fbfmfzhd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ybbhrekr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dooxuglq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ditbxqsg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3sxqclupz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mtjuciyi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ynlzvsit.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vjdisfwh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tixnhzui.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3naevgsxp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wbpezhof.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ritxpske.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uhttzand.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jumhzujy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3myrnxnrt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hjffpajf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hausrugk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nsispfxs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3edsabolf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iqyphhda.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wsgkfxjm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3utolaqkg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3cppvwvkg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3phntxold.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ydzzjpwh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qtebhyfb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3aaxokipr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tiskcffz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yrirkggy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mltrayoo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3huemhbqf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ognigroa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsatsrtt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3sxyjykxv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ndigprjr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3euclcjjw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3apitpeoi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yyfmvhma.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zrzacwin.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tgzzpqek.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3oemwyfjv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3sqrozrbn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3flilnwgc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hpsupxyu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3sekfklaw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3behekxbw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uwzttdhi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3iheysjpy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pfrmscti.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fphrjegp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kwqpdjir.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qvbzojzn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3znvognmy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cjcuxmyd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3erzhvaly.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fjkdcbrb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ajlqbdkm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yhrhsxmy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbdwwpe.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yvmdogni.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3jlwtkpvx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ozzzmjkq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3efvienfa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jhvyedpw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iozhuxuf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dpstbfep.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qcnlvute.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3apsbkxut.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cpmfmftq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3riljjlss.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3flddgyzr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hcmhdjim.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtidbxkm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dnotnkop.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ykxamwcr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cyimsuio.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qdvzxiiv.html


<!-- 参考信息 -->