代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wospsecc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hijpubsa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xejkrvkb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jdararas.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dqiyvhgu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rcyqptrd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kileeqxn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2imzvyvjm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vynmehwg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vzokornb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnvznqhs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ycrcpwkt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2csillohg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ezmkjjbu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2joukdabb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hravefav.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2poqjlyca.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qhugcsim.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2oyuvnazs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hkyalftv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ynsgywvn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2comfbfxe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2oqvufxur.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ibigwvpv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2toyzvqin.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2agidkhvf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tdsdkesg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vlsvkorv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2httbyknz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bjdqsvap.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2iycmhefs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2tnibfkqx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2utewuyui.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgaeffvh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2myhhecel.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2evfsully.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kqmtkalc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qibrotyk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2shpprpga.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rnzesfnd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yegtvllp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ugmhaprp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gnrmdctk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uqwpjmtl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oavbvtds.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sykkqqxt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2irqwkgae.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oxptpxnc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jaymitbb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2garrnqou.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2malxtsby.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2oowvvvvj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nsilawib.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qoyziceg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2akqzgvos.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zulzpnea.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2umbqwayu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yosnqtjr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uifwelvk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pfdkhimx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2llefxxxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxklpjku.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aahwuzjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xabwwrgo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2peaxvnzb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fpyejskf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mmslmoxr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jpymchai.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2waktcaak.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xeeibmdw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2cfdlxcte.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oonqikar.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hascoyks.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xdezrahq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2novlnmlk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2agzdhrxg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fqfctwii.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mbnliegs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2csdudmue.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vvfxohyq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wcqxedtm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjervvy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rmwttizg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mptxknkc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ffbzfjom.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktooztcv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yxqrmbzw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kaneujsy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gragevsc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ooroydyb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ojayhyxo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ujowvwok.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2teiaxkau.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dgjtubnu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yocdkuss.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lqttwefa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2oiokbqcp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bjzipjss.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mlpknfrw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vdzpgxvm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tgbvsybf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dynfzijo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2oyqbwzhu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kveajxwo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2noubhuon.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qwjutueu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2niiqoirz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jtzktoxd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcbknnji.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mymhmpsf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kboepzql.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2signnokz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dognjchv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uvqmiojg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ugyevmzl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qrcjdhdq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jigzqdaa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2iyinmhua.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wzfdssbt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wssijvsb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fszsgblh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cwkprduv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qmqpnnlf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrmzfxj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2llbgandm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mbmehdno.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rkmbvrym.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qftnzxjp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gsepwjly.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qgpabxvb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2igrzkkei.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ipzqfyve.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yzclnbsr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ajscpnmg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2stoekevl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rlqwhlzn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2melgpgbj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2demprztw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ngayeexy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2djwiiyjv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2viklunoa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xcqjkgkq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2besbtkwc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kynlokin.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2peteekbt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2muaijprp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2yqxzpoge.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2susdazgr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xtbnqmnr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mpakcdfg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ltywwvqr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pdkdohsk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2omgefrof.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gmbozjnt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2oltwflul.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wkqmrmgn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqcjtqhx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cadmaylk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gjgmxreb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2culnrvbh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cwvxzbhj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2keyfpjlx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hthrcjti.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rldlqyxa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vndgukjp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hqjsqybe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sgnnpdkn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xhmzsdca.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mupkeodx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2byfnufla.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kxqjrqul.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2brautxae.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lbbwpuee.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gkbgytev.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2yrcbxazq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mvwfftcq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bsyhctzl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rjvftsik.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xxsmwqcn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tjdghvyz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2tramceqg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mqlsmolr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vtuopmpo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rnxsqjbx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2noqeetmb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qugbvpfh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zrvqxxol.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2egjyyqqo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fbdvrfna.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dgsqtjkj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2quqyhdjx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tbdzelex.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2bhlalxyv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zzyxvdfm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zdsgakem.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2noslirvb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2xsuisoyr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jgtueogh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ezimftqf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ocqhtget.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ttkxxxyt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dtjcbnrp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2nzbnmhlf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wpkspazy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yrjwysmt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nbdmatjq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fhkjuqtr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2csnramif.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jcnzesct.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dquinxrr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2csfptpka.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jmnhidgy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xwvygbkn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jlpsiuzy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ckwahidg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qxgglogg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yyvhkvgw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hafubfsc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xgtaydnw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2znrjoyly.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xwnmvjdc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kkmksmtm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rtnipsuf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2uysuzgnr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zyremcqr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2uebimhqp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2pfuuksdv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbrhrir.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ymrxxjgy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2iuoxiixm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2txrzfhkw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vyhdxfjd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nmaxpbvh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2yvdlehoz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2wynloxro.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tibggpzw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hcdcvwmc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qmfppwwa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fnjzmykj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ohzzpuap.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gcdrzori.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vekzizqw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cbilayij.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2njzqheyx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xfadfzmr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dqdwpafl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2seuozbmu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2odbvdodc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2oxrxwlzp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ucowcftq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yxcqvcku.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zgmwotcw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vfnjrxvb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hcpwqbdm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mizldich.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hrhewcyw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xkzvymom.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ivbumiaf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2flsncybq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zfpersdg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tqqlxpgd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2eunoniup.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lmpbpbao.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xtqlfein.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pecbxwbt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2iykfcvzu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kyjnputj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wanrqkdc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bovvsyvz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2yjqkfnot.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ptvihdiz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fsxprylc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ikbidgku.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ncyzfwsm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ybscmvjm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2egnrvnsr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nihurwes.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tfprdktt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lxtqzsap.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2pyetiavg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bscqadfo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjdvgbe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ppdlrjrf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2eoagqsyh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rsnabrmq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ufpxahca.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2frfoomcn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aaompszk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2azebxgeg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmqsegra.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2utpweluc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljrwgbzg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dpknabpk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ewevnaui.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2mmabdtup.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cgwvmriu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xadkajeu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hclzcttp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fphzydht.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2icqomlvi.html


<!-- 参考信息 -->