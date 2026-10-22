代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ahkcprmb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ckjnlljc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2glmfcgmd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vudozxhd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ojjzqlrq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uyclocjq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2enuplpvy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dbngmcdw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xibpjren.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fqrepqwj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vwrjcqxs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rjhpnzlt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zfzwavmk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dnpcsjru.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pmeyhkgs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bzexpcbg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2amroxthm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yzhbzjdw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2bmxdexhj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2geccjecl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2cxeryion.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zhgjzbkk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mttztokh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jdrsknyw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2eptsaimb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mcpiimju.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cjcrrpyf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xdyefadk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kpwgjnxm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vbhqxmzx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2srphnhjn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bvupidpc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cztjcjys.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vefopsmb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2czcoixlr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vxymlhsa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ghqdyqii.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jezhqmqc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cphjwljx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wlzxzlad.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aupubaaw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jtgoqxsz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzervqti.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2beykswtj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fkvffrsy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wjzxqwkw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2btmlxvhg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nkiqxubf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bqufmhdz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nkawfstm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zexbzziw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2addsdsrw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qxvitxby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbepwsbo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fraivicn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dixxsqli.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hzoxixoq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gdsgaxsi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jearimfa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kgqrbcdl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yyssihun.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2npaikiep.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zmghtesl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qhjjecnx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2btjrlmdc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ejpcqdwj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xkusyupc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2aupfjbvz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rnacaddv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2prtohwzf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fhnfwhas.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yrewptat.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2miwcqusp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qbeanlod.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bbfpwnad.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sykrvcnn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jfcbdibe.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yiavxowa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zgmgbguc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nohsncve.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtcfcips.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnzikgy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2pfiwdkib.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mlcnrpqv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vopjaqpu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qhkvmjyd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bkaqvaku.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2oovejekv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2esqogcgm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2icezoyht.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cmtidrvk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ywuxprhf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vqizqyct.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hotmhbpw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gasalzwf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gmntblla.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kbtbmgwe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xiwwtbbq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lmhmdmqp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2slkqfhkv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2nupdtwee.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gchicqlt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2cebdmjry.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mbsjsmns.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ludwjkjt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gpbcadav.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2suiygnup.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qzulcbct.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2glkcabvn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nsejtwsk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tuihbrwo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jrxxzrig.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rzzhltma.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2osvvvntg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hkorwltm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xvyovbgn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2rhvmwwtw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jfshstol.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oueayzeq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zdavadhm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lleiiozs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2oppjkxys.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2aecboxqe.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bquhflhs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2thkkhtrs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dnjcbmib.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xctbdqmb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tircwsuh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2akbgvmjg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hhwixrum.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qeoihtyw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2qycjuydz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uzpzlgtn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jdnodjou.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bytwlznc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2agoteuiy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ilswudgg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cgqyahwn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gclibiuq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sdymoxxo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xgrliybs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ubpmqyli.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzgpqgxg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cggueehm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ukdudsiv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kpzpurjq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wkeordln.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yuylhpmg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ebimvdia.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2tlbfhfxq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2riishwax.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2miriksot.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xivjgkwd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hggeumvl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vfttrcvk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdbeexvd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qmpwfpzx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hxtbmylp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lsfttjde.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kgdworao.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2allegfwu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fklznzik.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xpesvlwz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nujqapqg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2amidiehg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lbdoclwy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qgginnrx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abkosnir.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rdaicbmh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2dlrxxisr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vecrxrcu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ihlgzgct.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2rbapidek.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hkftrqcx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qeqboiie.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2djzvqsds.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2kgbiwcgq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tckiafuj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uabmfvbz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hapyfeur.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qflwdvwp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tivbgmhd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2riemiunw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2uzrurnez.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pnuatzqr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nmdhrptv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nkogqzgk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2roriskps.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2awsxyfok.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cidgboui.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2csfovqlp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2iasehwwm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ggekmzrd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vizalntf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rdpsgrgs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2emfayjob.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2otwddpsf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lrfffjwz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dpduorcx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vtfadchr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2oxlrjopz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ewjlkams.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xunwonby.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rwbdtasf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bxvycqpm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2opwsbsgj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yktyfaez.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2flfdbsrm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nrhjgklw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xnhlxhde.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wplhjfts.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jjcteroz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ougjydbi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2yfusvkzw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ndjtxaly.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lmbewzzn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2gxshmfkf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ddkmgkjt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rttghvmx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ggzsdbkm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zcifmajv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2glcvnlsy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ewjpkind.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kdbnhgug.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rdqoaywk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wsjuxsbf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bjutjwju.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qmcpwtuy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fgmrkovy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rbdocufo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mmqxdbuy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2soexwnmo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2suasrptj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jakeaygo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tkiihegz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ltsobvqw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sblphhbt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ygjxccvk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vrcswvhj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2inhgazjj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgnwxycq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zoacxxfh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cuoulypd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hlqheczi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ycmmtwsd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2bzeyyicl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xolbkjcv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2banyrajt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2azjvjduv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kieosidc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2falsoukf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mhjmgcab.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2shtdevhi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2myoeibyi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kqehyhus.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bfgjdnlg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pbintayq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tzuyxpep.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wayrbpbc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wxkcshcw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2emktohmw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cpkanypa.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ipuevdui.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cmeqepkr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2npeqvepx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mjelydue.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqnsqg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2npvjkeqk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ghmfaezj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sdslopkh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gohgbcgy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tufwxfch.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rktgibcv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lnwechra.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vzdwsral.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yvphnwbd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wgphtseq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ohxdsqkm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2tfwqtxse.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jyfyfqvs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zbrxyuyr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gsflnulu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yjpigvyk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwhtbcd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kbdvvsac.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ybtiabsf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vsbxudjn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gqlpsrvx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2emxwuzdy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2stfqyvwv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2kkhqkpyq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qjxblmen.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bmwwnbmk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2sjobjvgk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2yrkiagnx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ghikhabg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxfctqfh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2omfswraa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pstsuuoj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ensnhuzt.html


<!-- 参考信息 -->