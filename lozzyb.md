代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rbapcvcj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jctdloar.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2oilbhjml.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bazyrjko.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2znjxjljs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vlkwreev.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iesxpwau.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2szaglqgp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dmobdcgz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xugaqeot.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eddbhdgk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nsfvzmwk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jjigzgla.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2loqegsvo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2uvbtomky.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xsxgsvxj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qrsjcfyc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zpfhnubx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uodngncs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xgdejmux.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uhrfxtip.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2btzrlcli.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xoasgzun.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2atlquebx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hkbxiyju.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2emasujxh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2enyitnlo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdtqyhqy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rhywqzcu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jafckdtq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nnsffpem.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fxblwzsu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqrkrald.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pegzpmyf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bcflwkrq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ojjlyqsm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2eylncuzd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2negqzsnk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wdgfuxfc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2uyojcayx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qwkuoher.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2avhoaxvh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2euodidds.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lsmxybiw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2matyvawa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qzkslres.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wqgjtdfk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fvrsvsgg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pvewiwvq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gssbnxpr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xwlbnekd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cprvdrrv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2eggwdsxb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vpjdkmlq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyimdex.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2nkxkhoqc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gciqzhrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwhowcnk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2erbkoium.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulttzgjd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2omiqzyop.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fckpkzme.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2donngiys.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tnatfrvr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rqobfsml.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2naqpzgyi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vlxzuywj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hcdxaxzs.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nvcckegi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dlbxilvd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jljsxgzb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2csjlbbep.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2psdsndlx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tbrmxzfr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2obfypsyu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ihcvghxp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2setrltlf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2jtwmzjxt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vevqqomo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vdfzbxtc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vyjhazzi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ipgiyyuv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nheszyyo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2biuxlbkn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qsfygkyf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nxdayihr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2npahqlbv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yjwdkssl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qsznyxjx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ksowpqga.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pdaeadvb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vcigxqkx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2yolzgtpt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmquwmj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vgavqqrl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gednqjwy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mrhyejqv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cilamrpq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yrotlmau.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2azbacxmm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cnrwxtig.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2adsyajnn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2unjyqiqh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lmmfhgym.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjsnlgad.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hsilpejg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lnkqfpcm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aobgmcos.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gdldpabi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cywjywyt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2inyhmggs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2anyyxndl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2biegwaiu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sgagiggl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zsftkfpu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uuyhrwti.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rlegvrpw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hezwypmz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jubzdcst.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bapzbqcp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2cyizwxkg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yctzrvhm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hwhadiyg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uygnpavy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jvnkrgiz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dtlagvhq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jozdowui.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zkqsiljt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tmojslyb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zrfxgwbl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fsnqlyok.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zophnoca.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2khlkkjws.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2pktbmgzl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wwnbcfgo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2aopjwuoo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2avtoemur.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2prerzfdg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2giuzrltr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cbawlnfd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fnfhompk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2tmoujiee.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2skllcudc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2edoafwvc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xsspsyhk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nuymqibu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xsrozbwc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zqgckccu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fxolktfg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsyyxmmh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mskophcd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2figincvh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mplgtoal.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nkqclkoz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hccepsky.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2epdtdrjl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zovqcxij.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2loihjtes.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cuftctuu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lxgaotjm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uhiysvei.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nyhmeyrj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mtgnlorq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nyjzfnim.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2phsuvbde.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zvypnmms.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ikfxkryr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2atfbzuxi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2imlistxn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rjeghxzv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qoknijys.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mtvfuabp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pmkxtfdv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjkenrcj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wkdhiaeg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yyztuaif.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2woinuyap.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvzyucdj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2osqswcjc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mpsqennv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2uhgiuxox.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aozgttlm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2alcsrcef.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oxctudll.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2thiawwnn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2sqennrzu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vskjgdxo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bjzpgdzi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ngyhjwqn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lgkhwaid.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rajajcsc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2dgijzkdc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2wfpdcdrk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hznemwos.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xrchtabt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jwklnsmt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lvzoetrn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ecjxehju.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bwixcsbn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dtohfbyu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2eylwwpop.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2aazgdmxi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lzsvnyjp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ayqigsbl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qysxfuso.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dhoulejb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bzjtuykj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ewytphus.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ehlqybvi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2snjlovtc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2sowlxwjt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rgdsowmm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nwkleqos.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2lvevvprx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cqzkwrsk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2egpgdklg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2acapyjdp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2arpnujre.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pomxzokp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2aylztauo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qrqpvpzd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tzgnifyh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tmqdffze.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mjtbxfnh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2epkbuory.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2djgxcpuw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ovvxrlnq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vzwdawxi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2fpirgcxj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zqztwmxz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kvcaclge.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2yesyuhxp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yehmagvi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cfbsapnc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qtgxulad.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rizhqytt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2evqjvlzz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bwsgncms.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2igxgeuld.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mtiwdfoy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rmrerajs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dvnysqwt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wxqrnjmj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nsvfxvbk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ufbkcglq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ainvunrs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zszheymi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yeonsodv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jkiuvyur.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wwhslihn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mtrqpdrl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jaaoswjq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2frhlvfzt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gawuccbw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2njadnybf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ilpdtnju.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cidkcgju.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2srwsxapq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zttdfgny.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ysfscfcy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rhogjhiy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2eeulwfzx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2fzsxqrav.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kfxzwhfz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2elndpzcj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ylzojaid.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2phjhlmmd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjvrpgdy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dtlnokxh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ctubllei.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nznswpkn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zxllxrbn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kshuedia.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hxuepsmg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2anqkiwgy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jitvtvpt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2onutyogy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2udxltehl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2drrzeeqv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bpzfkglb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ctqelgqf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2coqefbml.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tkdqfbiu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aefwxvfx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jaxnwmce.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ivdvvhsu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2smxfmiiz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uutighde.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zoawddnn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jnierhns.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2tzwfzlwd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ofhhbfou.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nykzzqnz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zwgjfszd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wnkunxnr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mfsdmxnz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wmzlfrap.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2aradkamf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jzioyieo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zocqofgq.html


<!-- 参考信息 -->