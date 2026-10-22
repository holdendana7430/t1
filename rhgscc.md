代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2jyrbqchd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qjehlaog.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ypbdijnf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2iopaimnt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2zmnrwnim.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ajugubdu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2stjqycnl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ghzionab.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nhxstero.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2eqwoiinr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zgjiygfj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2llfstauq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2csqprxit.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ozjfizcb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dkvgtjfn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qwwsckln.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2liimxpxz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wretfyyo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gcqofsot.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2devozuci.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tziltxvm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ixuwmdwa.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cinvftmi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lckqrhaj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zymrfipr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2lyouxpgb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zsiqaahy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rbvnpvlb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vjvmhrsw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oswgojoo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kgxsdtui.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2uziigzlb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvagbxhd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jjhuwsyb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lrfscsld.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kzcxnohr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjfloqv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wnbrsiii.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lcvrsust.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rygmyezi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddgmfghk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uibprkfi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mrmtaayz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yxjbctym.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jiswgjrw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2binzfjph.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qipjetjv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ieryacqt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fbczmoem.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xjotrtjq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jnmthyrt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vguvalbs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uxzfbktg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2adalnegd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pvzumflu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2yxzanuzx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jzjenbay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2coxkapvu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fxuoatwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjpxazcv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rbfwoncz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lhagpkkw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kgqrteze.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mwofwkbm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2glrockfg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2usqgfhds.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2unlunspy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tahzxjtn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kxtggenb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oxhlhasi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wjpcxdii.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qzkheolb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nyjrdbbj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rahqfefq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2izqudtzd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2uzmyroyc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ycjvjcqb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrjzwhw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nkoapihp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tkrcbigz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2opnwqsfz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2aphqdfrn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zjkaouxi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zcyipjjv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2csskyadc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nyjkncev.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kirfxsne.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdfcyys.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fvznufrq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gwubvojh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dpdvfphk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lsxbsuuo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jwaynaok.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xaeugyly.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2emnkjisk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2shblcwxr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2luftuzkr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ergfkoez.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rneomscq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dytfyhmu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tcyrdmsf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tmbumuro.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2uwtlxywm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2olbyfrca.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2idynrvqo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jvdurocv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zluukvwu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cyuivggz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2nyesmxkf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2lgsbudex.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2mymntbpw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfomyja.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ueenweft.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2soujnpfd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pocwicnl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tngerfcx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2flonnrxx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yiazqcae.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2axuaazaw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bwddbkat.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eipdpgps.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zqwelkzm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2quyieaxp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qrbfxezg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ellnijgx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zxtmystn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vokjkwcj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nmuoqdfx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2cgyuffba.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zdoacdqc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ndwrgzmi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2gkdvwmuo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ftffhbue.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rgnaorvx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2dobnabip.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2henfrgzr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rzonrkxd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hekszcyl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2scpyjeec.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vzlwyxzn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2drhiwyqj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wuqkfjhu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ygbxymtz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nhjdftre.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wnhviqqe.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xnjnummt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2aesmtjut.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ebwqkupf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bcfpjgdg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hunyzknt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2btodylca.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hgnmtkua.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nmrzlsww.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wqfmsxvi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xhkwlgmo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahqdssfw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vcqmzvxe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2kbsyajjq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xbcetvhj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbfqtsmt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rxsndlrc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ouafykgf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cditxwgy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bhdigmqg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2kbinzwxk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2cbypcvyd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2shqptrdb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kzebjmxw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dkpypiup.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bzbqlddg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rkqyzshk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mzmvqwwd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mmhmxyja.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tykknglg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2bfyfyrhn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mxrfplfb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2iivktfup.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hykbztfw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vazifpnd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2shvoafsh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kfdvdzyv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxbdpxox.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sczwxsqj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ygjfljyz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ozhwougq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2latpalku.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xozonhgq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eenuixmu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2umyrmsdk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nhrgvnzc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2oirfeggn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gxswhakz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wcdlowfk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2txnhhbyc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fshzqvxm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2suxvrpaj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hkuiunle.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xqidyqym.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wadnachf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bdzepqmv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qmjyyglp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ebjnvvaq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jiynxctb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2smtpezuu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pcspfoah.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2azbjlkeo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fuacoreh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2roeezplw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2sixslnwd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ztsimroh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xnyofjwa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kjsgfyoi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2unbtessf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2nzxnvrmy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kevzpglh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zxqadbqb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rokymhce.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vwbchnkt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ldhydkcm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bhcltmjl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2uinzwtkk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ogjymnoi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zqszdeap.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fkfqssfm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dmflocsh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tdxykgfx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rfgiiaop.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ytgooujx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2awkhikij.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2begohdai.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vwlkxmtb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2quxbjmmr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2sycrooba.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cdmcotfy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ouokofqc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2njivjepe.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2tqiarzsz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2onkpfgab.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2osfyvmxo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rqvzjaor.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uoppkzpc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ejvjdvqd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jsdxlync.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcrqafj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xvzfzlfx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ybexcein.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uvrmsljq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lgizpplx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2cuxoorxj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rwymgqwb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jwgthwkl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rtvfxtlp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wjyyzomd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2odsllqrh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nuuixlqz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2incqzprz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ggthgktq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xjzmtxed.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qycevxgg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dmlgmylr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2plounlkm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrmpoqe.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rtnpkxgl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jzjrvczf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dfhpyvud.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2lrriufpp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ylzzudqc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ifrcutbl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ychbzmrj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dentgnat.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dvnpnflw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rqvqmgmi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2coqzfuou.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2obbwmojz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rbkcapce.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dgbkybvy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cgxehayz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2caapgujf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qcobnpzo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jszytxpq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nbsnorbn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pplidwfb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yfcxgvzh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bctuhohn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bpenijez.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pbpyadac.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vdettmib.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ljrikcdp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rzlifsvv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qtmfvsoh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2aklvojfn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bekgzwvs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vlzfurnv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gztaebad.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2enjcaqaa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bgxjdekl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2anvozrha.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rbttazvk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xkzmjguo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oixnpmgr.html


<!-- 参考信息 -->