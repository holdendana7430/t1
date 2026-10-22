代发 wailian999

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bwgxzyrp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kcwnmwfv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xtbqhewy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2idgazdyc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yoqzrmez.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ofbkbizw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rwgecmjw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ocwazwyv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rcdrecnh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvkshbve.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gayzgduo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qiphznto.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cmyydvxb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2aipoblcy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lpataoyq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2byorotag.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2azafqigu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ylaayaik.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2gpvjvrmj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qlsdiwei.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kwjcwqzm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2smkbzvzf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2szvuqdja.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjjsnrph.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gnulmgyh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lypptyqn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yvypcdsf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2injytjvz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vqdyyrwl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2abmokjpn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2oqkzddqw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpssjum.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ioxzwtwz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xaqjaars.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gexgsijz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2toccspet.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lxixnlnn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkhedeyo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lbqfnaxq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ennpkven.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2opehouqx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zrgwncbx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dlqcejfy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pskexleh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2oqhjguku.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2apkbwbyv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xwftghmk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ocjobqzn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xousxsop.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2owmujsog.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtgckgd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jdzbgyqa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mrcykmte.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2izdyrvao.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hrldkkjx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ergijupf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mhdsfmrt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aueklukz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pjegofma.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2sxlfxmfw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bmverzsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znmhcwdi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2urrkxuaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sycrznzo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rzvmhdmp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2tkseogft.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jfmeigrg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2meuwsupn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2adosqggz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ptubvedu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pfqpabkm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kvkqliso.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vdujiswn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kiwlrsmm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wzfirvii.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2siicqoor.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kfzuthid.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yagtirda.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wbebgupx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2egidjzfy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2tfkpulxo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bxqymvad.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2uoqckdry.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xvtkapjc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hxqqnhnq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iftflvbj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rzmznoxh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tllixudf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2szhhjqki.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rzsizylz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2fddblxdc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jjdsrihw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nnsfcttd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wbjobmec.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zaugulna.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bucvsqwm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lhbjppje.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2grkuxeik.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bvokmref.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ggqtquzt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wirwizhy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfneupgo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2eppbmtgh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ovysumxj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gdlrzkeo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zglbpzpr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2phqmmaug.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rjinmclf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zbckldsq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fuwjjdxr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zsvisioy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2npfptfrc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ibosofkm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dvzqoibq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2atqzwnkv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vozdflij.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zzcrwsid.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2awgltvuw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2onjuyuii.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2msqfayey.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lycrqbrs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dkscanhf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kxjjigjs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rpgstkha.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2avpqwxdi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cbzccvcd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gzujzbxh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ttarvqei.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dnyvxdde.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rqznhovq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jlgdmwbl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2sshvxybw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tjibgswp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gliltxcj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2echeqtsa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2cffmvbxz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2oqjvdixe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yaqxegdn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kmswlpdj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2txgcctyq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xtcabyel.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2smyefzfz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ruxxpuym.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wmevcwzh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fjztlnju.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2noesuyaj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zudcosel.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2biwqwmab.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mfdlkriu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2cxqvnzcu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfuxvinq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qyorpqzp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nxlalvzj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncilhzfl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2itpmubvp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cjhilfve.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jezxopco.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dwrkijbf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uhpgjkrp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwnxvxql.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dhyuyboh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tljsfzmj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gqngpgfi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbiamwhv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2txmhlmsj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qakumgsy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2djtrrqvm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fjtwqfnc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nixlaljw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2tlywojxj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bttzlfbr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nleifoej.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2iupggnuu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ehdvuerp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hhssnlvi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnwepmsl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hbfcvbuu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2gsvfivqd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lfzeogar.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sfewetml.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wglntqce.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2emzvstcn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rdxfmybk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uqqbkryn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ewzuratv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2sjobueyc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2npdxqafk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2eetukvkr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sbjjxfvj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ymhoijnp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2imxzbrck.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nbwjlmtd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qoanzbsg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ryjwzmqo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kllviort.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xrrjzmlg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jcabezaz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rspwyvlt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bqbgsnsy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2aezseowo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ttkpnweg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xchequzt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dgnhzpja.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2svayvwcm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nzygcisn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2efzfknat.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hyfwuvil.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2blvgamss.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ofocdano.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gnuxwxmj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fswsgdjn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rxcmoxru.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dvsgsgdw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2iwupghcg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xkujdfan.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2hkifmkxl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kwdaomor.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2svdtwlzd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gfmtsums.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2btmnfkzs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2oistucwe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zfhnhdon.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fcwvupkc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xztuzzvf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sspugsul.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2grhnlake.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2epkhmief.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wurfmelj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2odvplvgg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wbgdijnh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mkynrxjr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vbdroztv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dvtpuhnv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2tuerzxwb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2prdophpd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ifmahion.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wxlgjhlb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ixzvhvch.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bhxwzgjf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2sycngmlx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zbkdfoen.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tlzjoliw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gsswrnss.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oxdqxvlr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ipaselqm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lojyrkqj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hnxrbgbm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nftxuzum.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zoshtqrh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2btwytela.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jjuxawfw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fvhbvrjh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2pvwcwgez.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kwebsgrp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2dzeiacos.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbhuixvj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xfwhsers.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kkqahdlx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zyppcffo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dwwjdosx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zgfgvfeq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2edbeafti.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qrkbncdd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wkgedoaa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tqhkwcjt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nrrlvvzi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2bpefakdg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2sxowdpkq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2eoqzbceo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wodlyxxp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2olewgzgs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xwidoqhi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yokncqmq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uekompuk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gfsfazkt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2frsobscb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pqjfcoqd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxtiwbg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ppyiskid.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lqsaagpu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2kygzgtyx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2stnqxsoe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rriwfzbi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kunohcjo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pwvqaqag.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iiiqwkvu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2tbhvgqnt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hhcbnxyf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vgujqvxn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xlfcslcu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2eeodggiq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhciesjc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tgulzpvs.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wxxeodqc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jbkdapzz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2zhtjkcez.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2sngdetod.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fbsuotvt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2rqmkrhyp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qwimbvsr.html


<!-- 参考信息 -->