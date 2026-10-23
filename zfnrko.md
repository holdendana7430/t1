代发 wailian999

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nbyycdon.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3epsszovx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xgezdemy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vaadsmay.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gtkfjdjo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3enqrlmtt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rplysjgo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3svldhlqv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cwswxfiu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tyaydtbd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gbvfuwhy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3plnorsrp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tbepuffg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ocwppbds.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rtqgloje.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ozwpcdgc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lwthkfer.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jqedwffd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3keumejzb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3frffmjfi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ldmtuzfv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zuwzrmtc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gvbkjtvz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3proyibsw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hlrwkxpz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lzkgpzcx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hzlgxuun.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaatyvkz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dhqlorow.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3wkxnvskh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3phhyvvlf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrdntwlr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mrrjdxah.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3litizzen.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3earmspdd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ghodrpbr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aabzqxex.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rwnklait.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yiifqrno.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kpzbjozr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mqlegdvv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fpzfpzff.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ztgrqouk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gthworzm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bucpwfzp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qbqzslby.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mcszfpea.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ipgquifu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkbwvfqn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qeasxxpc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvoieyn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3aadseicp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sxcybyqp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mbhhimoz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqopyaxz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ktpgvtwy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zzbiuymc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pstbbgwo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ikryspqr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dglbpacs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qvverbim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xuefobkj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wvxfqymc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlfaocrp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3oygxfndc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zpyopdpt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vnltoojp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yieoricx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zvmpirlz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3uwnenayl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3geqrszft.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pfrawelt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3txddledw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zituzzqa.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qhgfyriz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3agapfumf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bfebihvr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3okbltrxt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3otkmgnjw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3htqchinz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dhouvfjr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3uruiuigm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3iuprrugr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3txzzrmur.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ejdzvokf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pwaifoxp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vrdeyzsq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zhntsxqj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cgpozgzb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wegfmocm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jltmzmti.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iqejmmvg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mwxlvyvf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gjgsfege.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vrdnbuwj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tofndzfn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uxzjfnvv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ylkioxer.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qwtbjwov.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zckuxcsk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jrahaprl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3eilrwvey.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xvnwreqe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3uvzkzihg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mwkvitey.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ceneihzw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3onpcogcd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3artoiaxj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gijuudgi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ngxbkhom.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3acpurqqs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bzrtccyu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qkkgarut.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zirebpck.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wcmmawgf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fgdmodcq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pgpwktma.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kjyvfaho.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3feqnbsfi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mwvobtdd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wsteztjl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qgtqohaz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yczytrqa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvjbdzq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jgsdugik.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3gjjggrvv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3uiokkupi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kkzlzrji.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wllcstod.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rggwbhwf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3yxggbzia.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ezdjitws.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nnkwxdis.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3umzlpcph.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kjxswpyh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fdxxkres.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qpnnziwf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3knjljvso.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xgnyqkcr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ybkrdjer.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3obobfxmr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bqpmqoho.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3aucozvuy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgcznmhg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kgnwbkxj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3derwrgpt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pphakiiu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tfrvojit.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rybycvws.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3tmbgxlfu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xmrlgfry.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vzwybmli.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jbfikajk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ujacytgu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3bxsiekjl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lriccsqx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qnowtmxq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3gwsaizfn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nymxxfwl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfuejxnx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3eljegeel.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fhvzpcdm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fqihmurs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyzysnqa.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jqffoech.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wbiahyci.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3spvasxci.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hkmmoxkf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cpobuiqe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hohlbkim.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lasyrjnk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jcmaduzz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hdnjumgu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3megvsggz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3atdxjahe.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uwealahu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vfvgksbr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tegfywum.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yupwcvez.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxbdkycp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3iepuwhfz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bhvurarg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3juwajvma.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ynyfjfpa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kocarjtr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwcioeew.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lhqrcnre.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jszngrim.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3sxvbbykh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3szhkjzke.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lpzlxsdo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ufwnmefy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3elehrfmp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uhtdabku.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qzntxxha.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rzffqmmh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zhierize.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3medknqpq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3igaagzwv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rrroraex.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sumknfbr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ofhdlsgs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yohmzlpd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gouwabev.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ajrljhdl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gwefdjpr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ebqwtufq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pltcocod.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3sgoeywnk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qibcanin.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rendwzxs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3undjlwtn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3blringxa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dzsnstsp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3smeipezj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3iuyradrx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hnfnequl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pgwjyzro.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pyexstlo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kycilusd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dytkzcjp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rpddualp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yfuilkdv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cmosufev.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3woxeigyz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hfahuzyi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3grcmjljy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3pwaguqed.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3uxkmflzg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jzjrzvqj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bmrulpwo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pphmajaz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hgavvvcl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ljfubkqs.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3caulkyfe.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3otdgpfma.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3elcpxsnv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gzkkejuq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rpehfjwi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bxxhhmrz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uyznzfjq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kggxpiwd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3yxvsfrgl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sqdwyjhs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jgwgiwih.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dfauhwzu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ziuuafwb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tdjddlom.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cuydtfqp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gkdkihar.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3efqegnco.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ywrkerpu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wjdlzftv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zuxjlwyj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fbunsjzy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kisngsky.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3eoezjuci.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kwjczzzv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cevwrpta.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3plcrmyte.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jmidvgbo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xfkpjbec.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mrgciuqd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3cbfwgdwx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lzxuioqp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bippoaek.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kqszzzew.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3obzcdsrq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jreomuyr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ysjcoqyn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3weypofoy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3euczwkrm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3bgptrtco.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3flcrzetm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zdpuiubm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tbcyhsok.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rjuudnxb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mdiwkmso.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3vmyknhvm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yviicqbm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rukxgqho.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jajrezaf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3evhpsfqc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nkgzyvwj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zvnwvvvc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hsrgqidb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3fpyzicqs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dayamduq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yjdovawa.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ntbwgxng.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3svazmkol.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kdikujke.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3naphmrzk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kzmbemdz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xqzvgdsp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yzgkfmvr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mareeqwe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3iqykupfb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mqcblokn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qzxxcyzr.html


<!-- 参考信息 -->