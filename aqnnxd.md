代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ixacsvlb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fgbdwjsh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dktaeytx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ppvyfacn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3odpfjuls.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cldendcj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3utwcoqbs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3igjctaed.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yaqragdo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fhbvgwif.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qydfcilj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lxzkruvb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kfymfimq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3urasudxh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rterysya.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gzpndnbe.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wfhgzyuo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3udogfkdx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wcgxzfls.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fdbzxhfm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eglbsnro.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jmsuheke.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ypxtekzq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3egpcchqa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3erjsbsrp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tsircanx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3srfdiykq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndjarzgn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sfsskdeo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jdltikqu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yymomcbu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yucrprkm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3bvkdqtkz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnfvcbws.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3clyllshq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vpdgdznw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3schmmodv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qxtwdqhh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xbvotwxr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3blvuxhhq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kyjmofxp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ezbucacj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xqiqtvvg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3djtjsacq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wxxnmqmp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bqgpaksc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3janljzoo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gjzcuxkj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhryvjb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gvlgqomc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3venafuxz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3cybgcqpz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3twjwturn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ruyoapzz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3aulrkpom.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kevaovwt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hlatpadk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3firlimvh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3davhudzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxyckjzu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3oqfhuebh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lmxoongx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tisozqxl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jbadrcge.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cfgpfooj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3imkpfwyz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xiiesnzx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lsqubdgs.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jjsgkupw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qpwmyonx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zwzemgwu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yleagsha.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3clfjjhmr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rmvbjija.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3flhewplx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3uifmcvhm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3assjmtgq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3znzdlfhy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hqsnygvs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bpsvgoix.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vtmvypwg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xhdaopxl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uqqrermc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vahdrrth.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mivswqbf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fywpiwmi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3amplzmfm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fqohhzmq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ucyiunka.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3loploivn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qqvosfpx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ucgprpku.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tnazwscm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mxadszbr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bxmiwizc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gytocbxr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3abbpaxse.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lfyzapix.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vbvdiwqd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wyngqygr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xcltgypn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3eygevbhh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3egnzfiaa.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pqhxbfyp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dzgsvjkr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3twqogjmn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mqiunzzf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3blfzrnnp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3miafkwvk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qlfpgivk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lmvuuygr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3owenkjfg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gaixhjym.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3sjnfhmkp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vdwyzvcd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xhtycppu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hvritfbt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eghzfjbf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ftpbpmix.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xslzoxys.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3eomuzxxm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uwqynvkf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3higoeadk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tnfpnxjs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vftomobh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hwnwptuf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hbuzwzrp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxzemlz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3oqcxuevs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lnyyxggx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ljlihapq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zamsotfr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tvaiikmz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fqksyvsy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ppegyyyw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3badfxhni.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3heznpgwm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vcpyxwoe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3srkwtevk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mgaicobb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xdcrbxfw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3glegzeov.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3uvmlwoou.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qedvtzcp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vywyimti.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qlwkeykj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qsqnnchx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ifvgqeah.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3nrzqfrrx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edkbtllj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ubcxmnyu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qxvjlekt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jektyfsh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qytdjvan.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cqfzhvgm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dyipcqag.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rclmsitm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3otskxxgo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ozqchxye.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrrjrsci.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lbyffkpg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bibjiuiw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cibkheba.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uldiqazv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3nyixbehp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cometjen.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3oofxuqwo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3irxpmoiz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ebzphhog.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qwdmswcs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wdxukorw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hlggrefj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uxhxontz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jotgqbld.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lcqsekjo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ictcydpo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jskaxcuy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xwovozua.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3caqcbcfh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qadpdfcf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mgusctwq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ndggidum.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zyckxqho.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tiwoggus.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3iigfgacg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fslvremq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ffsldutf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zygffomp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3aoqpayzk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cpcezxrl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jaksvzpc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3eiuxyzhx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3etzmloai.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tzlvvffm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yjtzmifg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mhfvewbc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ibqnpceq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3uluvmlpj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3thlnoxxh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xkotdbbp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3oxvhhbnj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xralwpek.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kgcjawrr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wcdkhwcx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rziermjz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3gqjidsxu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lcayneqi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3irylmsfy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3iohlkina.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3chmdhdme.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gggcknos.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cbqbpyou.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lyodiciu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ibqkoshm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tegqquff.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hfnhxilx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dkfaxrwc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mkfxkzdw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lsovzsaf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qbejzdtw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3dhvkvlcf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3drtwyzku.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yoirogiw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kooluqjo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rdjpqgss.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jcgamogr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mxqudoge.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tnpuclzt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3itorpake.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3nniwnmhx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3snrfueml.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zxdefhjr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cydxqhke.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3mwfomjdr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lcucmgqp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qaifpjdc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rsdugqwc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hobsnxrc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qowhsuxb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tlsppbzs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yvvqsznd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qbxirirh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qtzarjsm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mjrnxduz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dnhxqsaf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lewmagqy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vswkuzef.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kfdduxks.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3rzgmcasp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gslushec.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3donshzww.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hpuosftt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3cgnpwpfx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bpwgdfnz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nkugcfxt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xkheoehf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3scywpocq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cntbebyy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tdfsmxur.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ikqrahnw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3eaksseoy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xtwibend.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3omcnsljv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rtvcoour.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gdqsfuge.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jggxenil.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zbfrehdg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hbdbabjr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3walwywrg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rkdmxmbc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kuwmspoc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3tevjgvuf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nnsgwcsv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oulyxycg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3cpociild.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mjhexfyp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mcoxxdcj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hvdausvg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gqxhwiko.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nieokdgv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tymgsjac.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tuefsmew.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qgwxbxvt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3axdhwkqw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dzndftxo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3robwnzgm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ftbbpyje.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kgiepkvk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3byloytpl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dahokyje.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wprvcajt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ovazbcfn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gfzsdzii.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kyiaeksi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hnyjmtha.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3gdvytgub.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3oggbaxji.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3cluffzck.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wkbzregu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ythkljcr.html


<!-- 参考信息 -->