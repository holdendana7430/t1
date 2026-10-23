代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3akwnhgeh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pdjstied.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3oerexmsw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3arrvjshd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ynlhgvga.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fldxctls.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmmjnwlb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3stsubxot.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yiyxaoqh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jxsdykjt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3yuagzoyt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vxmwssew.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qllxbfor.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3lsuzexor.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3domqmnxi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3baupmydc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ykpqjyyj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3soirrikg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjakeizq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3chhukkfs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sjlvfddp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3neyccspi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ytssxwzt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ociuavwc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iqnuyjrs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3efwesyuk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vusaevsn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeczszby.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3nncanvda.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qivlketp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xaajtiuj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ixdhihom.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3szboktjn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygaxqzgk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tpcgezxc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kokhbgtc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdwtgofk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mksiscfn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lrkdftfa.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lybourqa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtfqpgik.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hqavufyn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ajatrgxe.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qhricvux.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmqyfxc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dabcfmwm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ffsndynu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dotkvocm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qmsljqdb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gidynvzt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ukxnvzpr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lnbwpgmv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sbtetkga.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3favmryys.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mjjyczhi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kgxzktvs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqnsqiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkzsynku.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vxhxgdwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbtrxjpe.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qrijnyve.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jeaddvfa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zcqctben.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ogloblti.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mmyzmndx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bmxeuofl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ptxikjjy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3avdpyurt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3iyqlamdc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gdpupagp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3cbhqhgst.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hvsdjjzu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bonjcwxs.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qktuqimq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lbukvgaf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qhduobua.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xoxumahk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3coeemuuv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vgtzoqcz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mbhtslom.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qnvosdff.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wemtphuw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vujxyvdl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vsajyeqx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vcbeeedt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3trdyvvbw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wgnygows.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nqjvwonl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pnpazvgb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tgposdqk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hklbjybq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3eymursfe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pnnfiotl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xoxadjpk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lptbrhhs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3elkoznms.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3pczkqlsf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3vbgqyyxs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gthuhkbg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3omzouukx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ocqensym.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rpocqqjp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tynzbbtw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3cuorteha.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtjjzfik.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3pbhonejn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3skvkpbnp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dbpbhtyf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qdaodwuh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ohpdssip.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hzicpdlj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bkxxwhwl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zzqmnnts.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jqjnxflc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dzldjdab.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vzeuyths.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pxegkgzu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rqtjfwph.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yrgabzym.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzgpvoh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hcqeofuh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3iaeotfrh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fektqxmi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zjekabpb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jqcfdsxg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ibfctcaq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nwypnqlu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qtxjqitk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3tquxbugf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tztfuwbf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rwewqaqy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3osxerqoh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ryehqfei.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dmdtqrhh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qyhhwoll.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bbjtcqak.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ixcujrpa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rlesbcoa.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zeqtmgcx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uawstkob.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lbsimxje.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gcudixte.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lhlxzwrd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fmdqmxuh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jymclghj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fxhfqvej.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zpldiesw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3motiewfd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rmnjvfob.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3livenabi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3idsfpxsy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3luwzoiko.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3msdoefwv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pznjuzwm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lqnqhjgq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hewnvwol.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3awuyiltf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3tikfrvqc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ynadzdlo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhjemwsz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3voukcixd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3aukzdxrk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jqzlytim.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kuvbceny.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fxwawloc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qtfnqglb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3uwzqvoiq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3zykxapxa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vkjulgck.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3izgtymoh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3klbhasep.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcbtoxio.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3edekdszn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3pwwnkgut.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3icozpqar.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dbqeikgc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ffbfjxlq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bmihvazt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bmpsllzc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ngayhsnm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3noztgeho.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3slcwfezm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3uwdybfwn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3jnrwtgdu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3avgysret.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mmgrxqlv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hfjahqvy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3guoafgta.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hgvzyzwn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cldzazsv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gskoqhvw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wkmapxhk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3nukvttbb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3yvobkrdh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fspwnmti.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jserkrru.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3iwlmsyhi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqbtoukz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rfftbqgx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oqugtfqe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3donhypuj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dtwlrjur.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hgchrwrc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dherxied.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mexxxbgf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3olnkezic.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hsncftwm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3esxipozl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gaucvjrg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rcdkwexc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3horcjnrk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mdalcesk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ullrnrkv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3rusqdjno.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gfpwrkyx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lakjqefd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3twxcedoo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bwefzmyn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rjezzjns.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3epmdefac.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qjiutxpq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3afucczvo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hqppbjlj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezyqdtfd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ngpkevlp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ziqhhbvb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3klaujizi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3afruopqe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zvaslzya.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3njsepmli.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tbcuobcs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fgjsngvj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vwhqcogr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dgubkhpo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tmyojxje.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lmmqrebg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ovbkdual.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pveapodf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ieyllnao.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wpudueho.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ajpiroft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wqsmnsbm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3svcjejdh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vlyyytql.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rmbtwalc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3hxoolcox.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3itntohxp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lxqrbkda.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dseigobe.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3pfareoih.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nkknimpy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwienbep.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3okqwshmq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yxrasnry.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3udlmorjb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3urmxzxsy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3djmxxbko.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fplqnkrk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3aiclmxcx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3arpjadri.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3duqfnfpc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3askatbns.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3gyvebppo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xarunvlx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3wzazzxrr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ubwuiuea.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3htkkayby.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ncbjjlwc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3allmjolc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mtlknzmm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rcftjixt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3syvypyhd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3djajuwrh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tisbivie.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3tjccgura.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qvnheydc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fqsvpmpe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3huqjwfdn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3bfaqqniw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3pvescvel.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3eeeqabcf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fjveahlu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wotljzku.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3msrjovwc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vtevmtek.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3doidjraz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3enrsvptq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lpnmxoso.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jwupvznf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zwheziho.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3sswjgezi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3njqthvcf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rwlulvow.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ackezdsf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3zeotipgy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ygfagnrb.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3iahifwzb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jgfeetky.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3yovqruhc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3nqbtktml.html


<!-- 参考信息 -->