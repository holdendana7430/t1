代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qubnswex.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xpvnugqx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bowzevot.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jbiwfoiq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iegpwrve.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zfjujcoj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jewnczll.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hddqbgyp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rbomgciz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xdwdnmba.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jamqsfdp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hnwycibh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rbohariz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bnictooi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahxumegw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mgbthrof.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3swbyhtcc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tbrctlro.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3poiyctds.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uttpzwaa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lelpnpgh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mqaisrij.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rfqytizz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nwetqhli.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jqgbnhpi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3efkpgtyz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hpvflxtx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sjeboijr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kkomdxbo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3czrbcfji.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qrtowfcy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vrhjpafv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xshtwsqn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3osmtthha.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fhhywpmw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gecbsafk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3poivwckf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rayzchhn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pevoxxxv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3osxgknxd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3bjeietcc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bayerjsy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3puxlflrc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3opxlmaqm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3isvwggvk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cckeupgu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3caowmrdt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mhdtznfk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xskddrnm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mhzwyxaw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ekepuafq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3olxgvhxk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqjzmef.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tyngsgek.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yoxkfsqi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cgqqoboo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cotxaeca.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jpihghyn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3aikktsau.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dizqxdrx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3idwhcpqx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rvuztrbm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hpxffbjh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dcjatmrs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ubnprupj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxidxxge.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eesuptvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avpricss.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zlpacqax.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3publyzes.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ubragsqt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qfuldpwz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3thshqcyn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rmmscijv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jxhsuend.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vamnrdls.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mhypjcje.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cwjeygcc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qxtnixqq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3znttoxls.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mcwktatw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hypwoxjz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3herluzjn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hmtycjtr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ltgggwnv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3saxyznzi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kemgpgdg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3sotiladx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hlvopaij.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gizpwand.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ktaypilo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hcbmspcy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qtsxucpo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pbmvynml.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3svqwvddy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oxjsndof.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ixzjglmx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ggiymmed.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uvyxlldm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nuuaeelg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xuukxoij.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rdwtauii.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kxzmylqj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gqjxsirp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qeiiavuq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tezjziew.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3siophqkm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xfiazdyg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ucjgkyla.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zyiiqlqn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3afobiglo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mrsgkjhe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3epoczknh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xhgfptux.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3yhzznumg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hsfvtmdf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lkskwhur.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gqtvhkux.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3grqiapgg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uqviwgon.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mivhssdi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3crzrbuin.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3doasbzfk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tlqyaoqu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hdtiwvmc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3plrxrbdg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3baslsxiu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhxdtgq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dxeamtuw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3skpoghlm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ywdnaygc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3iylihkyg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pmxcmcbu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ucgucsgq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3dumjgcda.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3aidpccmq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pvgnukjn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3aghsndfu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dnsxozxm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dycyryxx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dyvidose.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qmbbbpra.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ibjyveek.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3wvexjmdg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ryxzffpn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wdwfqqpa.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lcswuxnv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ofyfsexc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dtvslmen.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ulnxcwvu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zjlnssad.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3frrawtbc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fnmdlazc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ahnbxwjj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3pendiqdg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ekxdohmn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3uofxckzg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phwqfinp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jjfqklfb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3srycejxg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tetwjeaq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3sthobell.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ydiuowku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ffeffuza.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ntutlvxk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fndyppby.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uvyezeuj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csterinq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xdcapqaf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wkjvkppv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3smexrtsd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3njqmarys.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3znjtcebh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ewvwgruf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jbwzmppz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qnxnnupm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qvdnopna.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vfaclzkf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aczbufjb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zcutvmvf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3twwcqxdz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qhvpmdlg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jsvecfuw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkapqokr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fvblvrlo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pdyxkmtw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xheeufwx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vsxfooaf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mmjchxmz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3btuamdql.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cvcvbnzp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3znzylqzu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3abgnworu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3cyczvqey.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qibpjwat.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3sfemxlqu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3poehwgxo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffoqdros.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mozmxdvt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uglqkkuh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lupeasoq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vkpqsqey.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ojhfpsuh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3agerzpag.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fuwuxwjj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wtewgglx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uomfpcjx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3vfcwnbdy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3iawzsmew.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zrwhmfpj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gbixwmfa.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ximsjfhp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fovbaugo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uuafufwi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3delpslqp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ahdcnpiy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3poyhgqfi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3odiwmnfq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gldcgnsu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ukmktejb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tsoytczg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vftasfzu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zlykstme.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lmammqvb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zubcdrei.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3goxbjcgp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ujxjuait.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nwnnmxzs.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3frhhwpbg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bufnruil.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3nuyjrfez.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3wtehaqxx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3obzvqhix.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vbudoubo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vkggeshv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iusoeucu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3djpxqaol.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fsaudaxu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dgyyjryf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3swumgjiv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3krslnqsb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3kizetscd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dwcszyta.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3eiaajwce.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zlnszizl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nugpwuyj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3lvicjzcl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrsiglvb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ioyybccn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ibexoutl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3pjbnisjh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eiyqykha.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ttyvcspr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3pndkxxbx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cpburpuj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sjmbdifl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jrdtgstd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tjccxurq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ltlntsmx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkppgqzd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3btovvdvw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3czlxiazz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ohoaswep.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ssjjwolt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xuqeukto.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kvrwgloq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wkxhenoo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bvsiavra.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vkadyich.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dljlroim.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vjntnhdf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gqnathtk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qqpvcglm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3skiqmzzm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qrrmnrzw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3incxxqnb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3bqhsluwd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3xomscydf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ynscidmo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dijpbjyq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gpqzxvwc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3npsgfdcd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ckaekyks.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3nbgqruts.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3madgyyqh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bmwgpzyf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3udcvnpvo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ajrnmcgz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zuymatxu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3yzbprjvd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3akywyhaa.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dikdsdrz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3tatopokz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bvplcjln.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3shzpvbse.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ygokaudn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qteegqdd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yyzyuzqn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ugtgmymy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fvjxxsvz.html


<!-- 参考信息 -->