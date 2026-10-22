代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uegnpgjc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xlrconeq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2uslkcfmz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eekslozk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgngovpe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ocuwaayk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2lcbjxtut.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pgbmqdlf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hpizzlzh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jnahjsly.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sjrwcbbn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cnzvfglz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2voiozzqy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ojdpgulk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cmcbeglo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uatpbwxr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nfvzkfrp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hapcknwj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gawmbrhm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mhxjxldh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hcqxyjkx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sooavozy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qwucrbvx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gzjdkzbb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zulvfbih.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2sxyyiksb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kmwyzjcw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bwnhdhcx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2avthwoyo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vafrcpqx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2otzjvoam.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heierjdx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bkgefflo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2iztcoopp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2iddjdnai.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zujecayc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bnnniaco.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ccpisvoa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mgvgtxeh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pajmgzcf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2yqtjmmxv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmyftcjz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwtwtnls.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sgglfgch.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zikxcuuz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2maiqkcul.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pikdpfwv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wzzrrucz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cciwkkrq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mdwpsujv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2iocdohew.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2heqsjsrl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2udjhonoq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eyjdjiqn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nzjudpru.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2czbcdjgq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jdzcccrd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xjrbpirs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hptrzxgk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mfvohijv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wykavmye.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ouwtvefv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jemhbdqf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tjdhbece.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vzdxklrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tynqvwhl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fprrydoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyhwqjlv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lkptbwer.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dekdytdw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lybourjk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mtqkhjat.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aqhxqncf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2liksoomm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qkkepfzi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mjysqtzm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jftpbihm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2msrcupea.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gsvdkfko.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nhtzgoxb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2skrrivxi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tfamiuma.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dxxuzoxe.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sdjicpam.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2neylkkpq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gyvtcftm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vzsywyjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wzcopsct.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2syijfouh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkfdcrov.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2axfijjff.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfmjksc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bejrguwn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mygrxaav.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tyiljzqo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fclihbkv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xofxnpeb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jkxaivdl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dkawtsna.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cvsyrwuv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2mngmunnk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cenklrto.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uoutqxfx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nryzpymb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zifechvx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2suoppeps.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2debmlytu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vqwcdvpo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jadvhdqu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xuwybuuo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2duntdwmz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wzztvoda.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vymnzfjy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rhoahbgy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ypbldzsy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjadaok.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xqitmfje.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xnhwoozx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2onsyplce.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2sutrrmpp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dxhavurr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hfekzpyt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2oscpywyc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zbwbzrht.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pfonkvtu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ibqmvase.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gjqtukpl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvtymbj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wmkzulmx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rnxrafic.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aligrxgf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bcdkntxu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ovxgkqro.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2epwbvfxa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2axriylzq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fvuxjkgm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qgizdiaw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kfwzlkwq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fgkzuwpr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2eiozofnn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2htiqsmjs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hvltobxu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2opniebli.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2siqdiecv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wfxzaxia.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gzsvfhqe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wouvohph.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcyiofra.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2umlcfzzl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jxbrtmvi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ygbvljzn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tiuoowus.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tlzvltjs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2umvxshak.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bdampkba.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2rqcqqmze.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2woyzskdt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oihwogtl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewpsrjzi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lbbwfydb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bxdsshgn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2eczquvxq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2llcuenak.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2saqlzgba.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pxpfgdbn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2celjmcte.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2neqlvtli.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fduimtnj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hvzzdein.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xcuvtwlx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2iuiukumv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uxrnywwl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mzwhetsk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wvqmgwki.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2odegsnrx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ufepujdx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2swifreyb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sphbdyie.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rkmnegnq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tijncwet.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2emtqarhr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jlhbiifl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yohieham.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ooflcaxk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qitcheck.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2irvhmfzb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2tmjirkvk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xhbhibyv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2fcgeenev.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2iwhkobzm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hukifxfc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zhvhgglk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ixeywpkl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2erexsgfh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ydegixpi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2umsyjfut.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pdevxjiq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vsyreojs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mcvtizub.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnocgebx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pxrnbvhu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qgcvzrgr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2oktxqgmw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nhypsgel.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2uwamyldk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jtudhsjc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2nujnjufv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gglaawdv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2evlgwxnb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ahewzfwo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2olrrkivu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jdtdgtxm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ugbdkqux.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fziumkue.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkqpztce.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2txkbpbbx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gynysmqy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wnbdpkaq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2nwmvuspn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nidpezzh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ivpycinl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yjbhhmua.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bjgcuufz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rgeqrhmj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xhgdnupd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2chqmjqnc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qvuxjqbv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2mbtlclqd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2oqbxevlc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2iripuenw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2azfaoutb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mejvvsuq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zphzftds.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ptgovybq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hocmuchr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fsjbfbnt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2msrognkk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xgjksbve.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2mxbpzoaq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zdetbftk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2zzwhamfd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2bdysorcv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jxrqdfjx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lgwejjsm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2pjxunhzk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ellgmqzj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qodivkbl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2swalrkdl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sacvjsqr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tfkjyaqn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2crgjvtfn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qblfzzph.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zjmzkxyr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fgyjblie.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2utvynmew.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2euoavikg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mopadggu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oekxtpku.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rebsgqym.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uinduxdu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wwyequjd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lnxifjcp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tdefkclz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2stelzqct.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zopyhouu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mwhfsuog.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zqlzfslf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ehwlzfgg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zbuudnvs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ivlomwtl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2swbvhzei.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tckpezhu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2yfogtfbv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mhdavsmp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2cvkcgvta.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zypuozap.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bmuaymku.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ioyvzwdi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mvgwoucm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nisvsopk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vljgbevu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2afbslyas.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2oauuozie.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bnfvocnh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2awfcczdx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ptyomvjq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mjbhrhso.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hifylbjj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2fixevgxf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2exrhfohl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2oxgceory.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xpfzitcy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2gxureiyg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dbzelqol.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2byruxedk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vxqhksba.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rjixmrrc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xbyfejjz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lzwuuagy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2bgznexdh.html


<!-- 参考信息 -->