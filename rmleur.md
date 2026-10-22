代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bxrcwwcb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ylqxzrij.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wwxnrend.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fxakltwf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kerxaofi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aeelivvn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkvomjmd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ttpfdsxf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fnodmpdu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gfwyvbmf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rgykuwmb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2arbbridn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gnytcevc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zfbtdyny.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2whijthnl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2svbrmypf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pvuufbwn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jyqcfwao.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vixbotqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2telgjqke.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mmqnlzwa.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nxlzxlxf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lfkzxcou.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xfzuuhsy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zxymqojc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aevydexg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qtlpljll.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yijcxuui.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rqphrxdj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdebikdu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fvfbmzxy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2obcgahvz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yicuddjk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oxbbrfpe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iukzsbem.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2krhnydcv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mldlxxqn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ffsxhmsf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kwuvpqrz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eornkbna.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nzxdkdvd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rnuimnnt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ywtwmotb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xhxitrrp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2arvorclw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gttoctri.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2usfpyokt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lkgbaxvt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mkwdgxqu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sufjlwtt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iapcunzt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zjltqten.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2aisuroun.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ijlyvrqe.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gckggflh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zzhkazrr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgmideo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqsrzzfy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zpgcukjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfrpqgpa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tnlsyfcf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jdbghfqm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qzodqnrt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rmyslnpx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2eopdlonl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vfkiyczb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nlhoxfed.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dzebxkdv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2kidltdkr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vrnkcerv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2iptmeodt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2snuotkdd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2whqoauhd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2hfaqfrku.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2sewswmmo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gyaqnrpe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2owfknmva.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2newfeoot.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fyhstfhv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hifggpka.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uuhobuoo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2seayfxbu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbeiggue.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tdvjjaum.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ndkuwtyc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jmqrvrds.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fuykhgwz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qicufnvr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2bdjjsrej.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vinxqlit.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2grhqofgo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2umrumubf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2iljbospw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2njaiaiyr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2erwvxjih.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2taqhxjwo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ahchpdkj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpwvyhmm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zgvyoesn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rfccgmai.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2itpgrbjh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jilkaklv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lwvxrile.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qggfgnxu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zogpzdvk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nznyrmln.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kxglxmis.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dnikhhlp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2hjzkfodr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qiwqafuk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2kamhemqy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tjsnbgvr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2cnizrihn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kbojqcma.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2iufbihlh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jvezibxw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2slwxxobp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2drbqnrxy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rbzgsgxp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fumteasq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2boftdepi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wtlojisk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rlfuatth.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tkopjpeg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tymyggtb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pgatpzyx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fpczzgsa.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vtvrkjai.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tcouusgh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zjghapcv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ujnqdhyq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2psabtgwc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2enmiksjk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2cqfgwawi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nruiufpa.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2klmpdsyy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tpflkhei.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2kqokfczj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2yfxokkuh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pkaasymf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xedcrmaa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qkscdlxg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2avqcwhxt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ruhxluxl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xjmfvhgx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2blhlzyvr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2vzipiutb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yhtuhiok.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bjklrzff.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpzwyqey.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jpoagcjg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vmiafvqx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lkcpmjho.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jrknsrsn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vtjzsmhg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2womdjrui.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dnxcavut.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2txghzywn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tqzpcben.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lpejnkdo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ooylupja.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mlfzrmmy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbtslger.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2apicwatg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mtlulexd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bmhtatel.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2glbiqioz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wltgujmp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2eisbafzq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2irxcfrdx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zkelwdrq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlkqmoa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bgwwwemh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ervvkjoi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2thpikhox.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wylhxrhk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fddqegvp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2htolfwwh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2axwabvuj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zkjeejkn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mowrcqbd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lqloigtu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ebhmotrd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2dzsulwnn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pbtpbbsp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2agjfonlf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hqmadrnc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2urvbcudo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qejiiizf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eowbxalq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zugjuudn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sgbahrpx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fkkussrt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2brgkmqox.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2npdohayy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pnbwzhug.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2acgeumzs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fuhxxwzr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ohueicnj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dftnezdw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2osdwftyx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ozonrqhs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dwybtxsy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lmnnznfq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fplipjns.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhsvsww.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yrpyqfvf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2svynmwho.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2sdcbxinm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2uvlofxyd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2plkrqnrv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mojonajp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dtebxncc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ehigvkvp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2smbttkod.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vvpgujas.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2vceuxljk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kdpmisgp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yflihyqm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rgvkuycc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kjeacjwn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2psvkugoc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ppjixocn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2woragmtb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2iyxxeaxm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gtqljoky.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2uubwocyf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bjjqjmhq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2lpihvsyv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qkdifxdo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2livtsflz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tfnbuiqp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2klsbsvrt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dbykvaij.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qmkgaexo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ouyphukb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2escuqpmr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kzjefgdx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2brfmjbjv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwfstpmh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtijquxx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ehsjowlc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2njqkljhq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnobxaat.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubrbbfzt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wxxayusx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2itsicpmg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vpacxswj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gwijblhw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jrcpoxmr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yswsleod.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iavbxhot.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zcvtftwg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oabpxdkl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qouejray.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2amrubzoi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cfasieov.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2oaittgjf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2asichhhk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2maohopcz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pfdxrndz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xsrzwcyt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nxlacymw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fxyxoyqu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2olxbyeso.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nxcilmhz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nlahglwu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2inpnfvfp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tdfzxkgm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kyqwsrcs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vogvacjf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2sfqnpubk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lqzqvyee.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iiesrthq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2btcizkva.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ktafdntp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mdepiklf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2aerqrfzd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qzvwlmro.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nhjmltfe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jzymqypr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fxhjwivj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ypjylkhx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uoumdgix.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ztwwomcv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uriqrrtf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ppjcpoiw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oxjavugp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zjwnxndf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lzhwxjpq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nnplzkmo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjbpyjud.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ezpesycu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rglhmwzw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mhqvbdoa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tiwhswau.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bwcmhjay.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2eecfugih.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2paduqggm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2licfbawc.html


<!-- 参考信息 -->