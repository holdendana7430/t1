代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2byqksvel.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tnsrwzjo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2drapselb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bayukspl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2jikpnxhi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2soswzyew.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rogjdbya.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rgemvrzo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ndhawpxo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2unfpxlji.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwameoez.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fsjkkcla.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ktqzphrm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kifwalzo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lgfbplkq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ihpdvsyw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xojddbcr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rolknaju.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xixijiep.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2dogzjtku.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mhcsuvrx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tsblubzy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nekegnxc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lcbiezar.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lbkdrkwr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qhmpdcbv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yfdkrewq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cjiqrsxb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2yapdktti.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jbkixqua.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hoipulvw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qsyjnawj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ndogiuce.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oocourhg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hvlaijfr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qvuptoyc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2csltohkv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wodnvfsu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaoemend.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qcqzwwls.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jnlkmjcj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fxybugdp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2plneiwuf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pfsomzsq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qmddoobo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2chagfswb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xlsfxmtf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ntmfuhbp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzchebkf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jdzwjlgt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oaxqcnbc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tcbuufwe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ainyxqfu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vgliktrz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xampalwm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2caqldoja.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oqbmxmug.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xlopvryt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ojfeawes.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2egcgwghf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jqkoaish.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfhkgtjn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uwzvrxrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uefneeox.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qulrzdip.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vrntswqb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mshxxuqj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2njqsysnf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2abfkjctb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kpdlxbqs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ocbhgfxi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oihdxvln.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ubgoddzs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dbxbhcgm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ubgfpinf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zviommjh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nppbelpq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ljreupzb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ywcjvnhb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2psqkmvza.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hitgbzhh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2efegxtkd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cdqhtill.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2myhjvmbb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hamfrzaw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbrirclh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jigsaxdl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2edimltso.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bpmkxkcm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ppnlmfhp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qdkmlwfh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hhawibvy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ydozkbvl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ruvlewxm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2glszonkc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uoqjnvaf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2blxubfko.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gipnfvau.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2djbopqxy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2koturdic.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2eofzktrc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xeafljyt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ihteplma.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wlnafthn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rklmhlfy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zlvhxccd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2bdvjievq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eopdyhji.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdulouxj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2dhdkssed.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jbnoeypt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2byjipaop.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2sawudrxa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jcaxcqin.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ijirgudj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwnythv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qhotfbku.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wxwmajtd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jbrhchvg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2puwmuttf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dsfobjzd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nbyemkgt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rlxqpjas.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nnjdstqt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wmblloqg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wckknjkw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2btjmncqg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2amfonbqc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hlaruyiz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hubwuhxr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2sipcfbtr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2oatplcue.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tvwmsxuk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sznnewwp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ibbuvqvp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nodvimcw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nemiedia.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bywaobia.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2idljapqx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2iirktucq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2whetzfub.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wlrfwqgu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fmpfzvye.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lffkeosw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2kwywsiip.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hfdpkiey.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tdkfhasd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ljbrcpxe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qzdyzctj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mibrkxqa.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kaukpwyj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2assvodjp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zodvyiww.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pghbpxwa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hpnoiywe.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2sgmoprvq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qvwkvxwg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kucjpvyv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hmfodsqv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2sewufjhu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kzxtwkvv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dgxdsjnb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vyiqmmhm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hnfinuaj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bqkwrrrj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xoxfdoth.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xebwzivd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mufkpcis.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lstezbov.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yijcpqux.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bapzzjqy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qevdaoki.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wblciury.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vtqvwapu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wijqzfwn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvqyrly.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rqnoiefe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ymtarxnm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ydlnssyk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bricywor.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pzzwijdu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bmzxsfvg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2czccyfza.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kdjqgurl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zhnzmckw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2irllqzlv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fclpabmk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2txmpljfk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jiuaggzl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yteoxspr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2lxsovioj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2uyjhmgcv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kagaqizq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2waeyjvau.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ymptxnby.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ubgmihgu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ymndwmrq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tihanjxc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hchkgmxi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2puicxqzv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vvcihzfq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qsdqmkzb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zanzryic.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ebptrnpt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dwyvzzlc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xbeikekh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2djcyuttq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nwvdyfis.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kkhjevma.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ijxqwfwi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2npriohgq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ktoijuuc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2oxmsezms.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2oslpwgna.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2veamljsv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zhddelyt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ugvoamop.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wxwtiuty.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jhbhzdsi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zzwbyjnm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2pncjddsz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ylmqkgxk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2prdqwcvd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ddfolezr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qhrwkzkx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vjyybatk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ykktygph.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gmwxodlw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hzscmhgo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hpfncpij.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2swhzyufb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lklylhrn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vfgdvkml.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2tczhmdiu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2tyumlxiy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ljfoyutr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xdxkkvry.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kxfmdpxh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2egtmcoaw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mbloigmg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cbfzutdz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ynsetobl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xrlumnrc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2myonsshx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2qesrfmvy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2culjrpft.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2blvipilj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsoeabiy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2uugsyodk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2guynyfts.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpaqxglm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2iokcrvtj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ridnkevl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ykeglqry.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2nlnjkrsr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2souimvnr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2apskyrfe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vfygbezh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tqfhqpkf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xcliwzsw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xubjeahk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fvncrzrs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ontjhctk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fivnzdfn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sppibley.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zxuyreey.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ergwefzk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wydxfdfz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qoljeayd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bwbwiznr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tddfzvoo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ejthbuvq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ehnaiqbj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kvaldkuh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yfrrstaa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zmzqjawo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nocyrdnf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yjsmgmaw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2rdvownne.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uugtpams.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vlbiuymm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdmohab.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xrlmgmuy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xotcnryc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ybkfatij.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vnowpgdb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2fhfshada.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zeaxezhc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kdldnmpu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xzwfzamr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pjrbxmms.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pnjmprcu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2azvrdphb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cvfwtupt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wdxbzwmh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmjvvgqd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vdhrvtou.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ymrdcikz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2uffskrlv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2counlxlu.html


<!-- 参考信息 -->