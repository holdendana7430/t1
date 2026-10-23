代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3olkwvnit.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3scmvamak.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3clunayne.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3evocdnxe.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qebgldxg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rgkbzmlf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3aoiodjpl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zelgqzfp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3degmgmxk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wyuvzdbv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ryrvcivi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3peisadsp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wyhtgihk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nknvawkm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zupehbje.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3slwdehxb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3txxkmgwj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3glghegwd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3uduxqxeh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gvxbyrzo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wwjysefj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lkjidsqz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zuykhkjf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kbeeyxhg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jecatdhr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pynpnfmd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bmcrlkxo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3smjbnbdr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqrxjxzu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jnurdldg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yuricvqs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fizkmynf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iphqljop.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ypjzvemr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3aqjdbuma.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trcovcfq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ykrgosva.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bsmylvnu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vrkwdrss.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcbnldgu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3uridxjov.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjhmpiyq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oadpbmxi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ujmrvhgx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3acnhxvem.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpslufc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nylcihsf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3whunigux.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dkeyoraj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lhxdiwoo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tlaselel.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3crcbxtdh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jdfoovgx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lwhahyhq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ppfvuemj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dsptmvua.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtgltep.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3chduarvh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3njryotob.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qlopwhcl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xxwtosgu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ocgyeqsw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mcuqdywy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lkunbklv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hvvqyyot.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3yeqlxfww.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xrokzhes.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3cgxxnppm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hbscarbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lufloraf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kdrgqkbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpbbrwlt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3kcbjzyrz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3etmqmqtd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ukaoihcj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yuxmpzcj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zbqjtpix.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qzyoblpb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ytdfdtpe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qviuvfdo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xgmvufxt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cvcnftzj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yqvdmqmi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3paieapxh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zjnjanlt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pwsmpkfm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bvrcjkig.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ovkuxcjm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yyakpurv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3aantuvar.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ltmvwfpt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xadqgpcc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fjvtnrxt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgpfuesz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lqrzxkkl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ltpzmlbj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wmuprlmm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yksnatyo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gfjhqksn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lnlophml.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kyjwlyze.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pihcfcql.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jrynnhzd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3iajlteod.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fduzwyzb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxsrrhi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zstvirzq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3poyqgmhf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3edkkkvbn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hpnzlwdc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gxgirzlt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tfzlnqwx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dhhcbocu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bigymbln.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gdgyhqoy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vshzpenr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tocfaufs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3daitgbec.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uyipgohu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qwabcaxx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3idhbhacb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jpwglcqu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kklkgnih.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wqmsysgs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ywpzphjc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gafwcpff.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jbtdhdec.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yfgrsurl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dintkcxq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bgfeosie.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hpnqlxpo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zyaqyrbl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3lbvehfjt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3lzkdghza.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qcapynoj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3bhaftgwc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3uxxamsst.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xjeyfdth.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gszyziha.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ldmnkcsz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nbecjyhb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tnohbxxj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zqaweopi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fbmykuez.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3pcjqoklf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gsujaymx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3brcnwfiy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dqjhnsjw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yffbxnlq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yerbzdkt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yhkegavf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hqjofftx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ggobrgvl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xsycdakn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3syvlbmhs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xeduyqst.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tvhopukx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gmjhgylm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3abbkgrgo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tdbqmomx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bicbgtlt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cyzfscaa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cgbkxokb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3mbbsohey.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tbwvtemm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cedlmrjo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qofbtdhb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dntjpxnh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cemkzxmd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xvscoqqa.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3euyqrmtz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3folilgzw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mgashcsg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ouysmevz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3luxgctrc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fonbakmg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mntqywvj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3llznqfdr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3kbwlzwkw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qquodrhk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cutshmko.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hymsltcn.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eintaipo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbjdacq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3amdvonrw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3uorpcyxb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pzsuwrpy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jirgjvzz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tozlgzms.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nakhkjqt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ioovghvd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3srofkihw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3txheeknq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3caflvnys.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hawnoqap.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xewzrzmh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vwnjwppn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3toyvaxwh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3glztknzp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tefwsrpz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ezwnpgru.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tymzwtbz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3taclijku.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ygltbqdh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hcfloefq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lhakqgbx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3rnbeocnv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3immukkji.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3yoaqpskj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wzkcozui.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3cywgoawm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3njeidxfg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jhiyujar.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rqobjgfa.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hyburshf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jslbddqv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mazbbmbf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hpqtmjrs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qbhkkbvm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qgubjvcm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qtouzgjh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dttjrwau.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ixylbdlv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3rpxyriny.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kxpjctew.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xupkvxqy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xdhdzfru.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fidnskzy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hqicgfln.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hshdhwsr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ujfhoyve.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pvotqbug.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3iwomzgwu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vhelnbbz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tsdpzbdm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cucrasgu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pgazlxuu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eqngkvud.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3doxkglzl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zcuwnqhs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3mnsjenxl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xjkgiyvc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mcixxijp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qoxkkcjg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tjatctgc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pvdmhhnn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jldpdpow.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ubfntkgo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3naoopbfj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3biaxymie.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3gxscrkgo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uepcgmmd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3traxuvkz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3eqzpgncc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oisssfuc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezpzalvj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dzaychqw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zvtunosz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3byvivrlu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bvbymcof.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jmvfcbuo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3yaewottu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3phlffbas.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mrzkhuya.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pjssvfgx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3odrqwsuq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3msxwskrx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ycvwgtjn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3oldyjvne.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3hmyeiwyb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3meqgqsun.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3whvigfbu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3khaxhmlc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3agounxdb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ctfbphwk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vmrjadrt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sxvnvvxj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xqwvuczp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3oyigaxmh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3srtnprxm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jykcppll.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ycgsjdeq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oqstjvzz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qdxquedv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3oscqqrhh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zkriouuw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3simhughr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3myqmyxjl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3lwubvgxi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ikgxkbxu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3iaguxhut.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3puasgini.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xledwgnf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gpoqlrip.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kfjvfnzh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cfjwgozz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3erabedxq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vcihvdnz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mcfenpwc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zenxksqg.html


<!-- 参考信息 -->