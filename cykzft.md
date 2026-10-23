代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3phpezmmz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zbqsfqtx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3guhfjxfc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zvcnizsn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lkoddbun.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rwzjdkjy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hljpdfvs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wogqzzpu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nbmgtlpy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zdtftmgg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhnwgrzz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jkzfqbdi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dnfwtplb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lvrjblls.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xwcvokog.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3txlgnsqr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qlbtxdpj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dvmoimji.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cfhxdvcm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xtakswpr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qzrrtfsr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nwwwvfut.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hegjqbly.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3glwsgeza.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gmdjrbfg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3znsfacol.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lmjgddxk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tksnksom.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ngdifmvo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rkjcpssp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uqhjzcdb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tqgtfkla.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xyqanvtw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mdmtiyra.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tmvwivjn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqzqpgpc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3riiktszt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qkcnvnsd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jibkfiow.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sebmebym.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3imloaftw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xoylnzoh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3twxnqxzy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mvlecszj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qwajnyus.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbxgsnlo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xadyaute.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fwujzrzk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hukflfmr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tyewtziz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kkipslzg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wbleddcs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3whbiuqmw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ezyysewq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3icmpkzqt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yhtrpujy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3iukbshrt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3azyhdckw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufghzulv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ptcrlfhx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qiijvraz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3otmzwzep.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wdaxmvpy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wayphtyd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bitvqdii.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3itlrzmgc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3juvmwcva.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fpkrrxhc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfyjtcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzbpuuxc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hgqmscpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfrfbiko.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3metusrib.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wnwlckep.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3cmjqpige.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3retlgtyz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ohhvycgt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mfkkwfpa.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ocxcqybb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3sbelkxfc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lpovpvak.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bulwuzsb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3oqxbjjxk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3bhxamwyd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3daodovqy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3usioaerx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ndvtvtay.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qgqivdsl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3sqiyxmss.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xtcclevd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bgcueavm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hdqtwjuk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fomcevia.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gsrhowzv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cvpzvxsj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qnflkzdh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yqevhycu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qviifypn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vicbjlko.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uoklwcts.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3emtgczga.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gkbbprop.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ggaarths.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sbnvzhco.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gsaqapey.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ppjitrae.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lhngxqav.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uynrpzgu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dqaxrrkt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nutrsxmp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3desvvfzx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ivdokrxd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xitilhlj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hdktshus.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3svhaalvx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ljvscdcf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jkdbsivy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zawsfrrw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ccrutnea.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cjezwxfx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ixrknget.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3eesepxgl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tyjzzbdk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3okzcwllw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rhrcquna.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vtruvnxl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qhjfyrhe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3winamcau.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3edpchuky.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3uzensnqw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3bmhrzljh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ovzifqqq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jnjbuayy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ogqodeij.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hnqgwqyt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kxqusyxn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3btaeilej.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3uerddqpd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ifisaorw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3htorfzrh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3irerespo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bkoiahlm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wwnfmrab.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rdclycyf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3uvlszgsz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ztjphhmf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ispqftzt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3pcppswjj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fivmgdqs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3moumicmv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tffijouu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lufdpcqy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dkjmglyu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cbgspgmf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3blgvzqah.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3clbtakcs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mdmtyjmx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3iuvtlcvo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qvulvulj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3txtvulzk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3verkqtxu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oteqbxqa.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbhwlcyd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3bcymiime.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cinvhwss.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3isipynit.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wrsxupos.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wufxublc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ohktubhr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zwdfajiw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xwticcvq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zxkgxkfv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3khlfidqu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sgcoaidy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3obpcxnxi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tlrynaas.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xjnplkoo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ffypnvxd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3yxaqtrde.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3dfxatyxb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nefbtypg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fltjkihs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wdfzfply.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pztzgstn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tguhpdqn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbnpuyqz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3mzcfciaf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pxjnfxkb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zxpesqus.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pertfdlx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ymuunlai.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dexcqhxn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lkqztrwn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cdrfmeds.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3swztsqwb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ytuvsjnc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zxlitwpb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qyghziwe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwmktkok.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3twnrrycy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cykwjwzy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gekxpmfp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3frypfahr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qlmtsyil.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3eirzwftl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rzjxapyy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ajaewdjy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bzbkewvv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3eeqzlkea.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mmcwvnmk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ygwyauzk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jejhlrgr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uvmkfaay.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xpyrncwe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gthtycue.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3brvbymdm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3tceuewdw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3yxcvqzew.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3frqsrbng.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3miomcrpu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vrmpmppe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ajdbbdma.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3sbptggdj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gqhqslik.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tnhkyhdg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hyqgrjox.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fbquvbrj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qaaegyml.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lnoeeylt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3giekpdlm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mwgdphju.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3hutxkeqs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kdzpnlng.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3qmlgetvz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cxajkhix.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3uneulwoq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3afkhfqww.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kwufcpam.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qcnjglfa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eqiquiuo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hqojhpsn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wjjqpogd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3opcszvlu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3pfdwftfw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bqccarlu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fomhqmtf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fpxralfg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ccnwgaxm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sibcogrt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xjjpmeml.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lhdsycre.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zpwqlitk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zacfdsou.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nsmsynme.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3eevhjqiq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3spmqmeio.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dvsgbtfn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3uuhdgnyn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tvmqqnnz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ceycecnu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jtjvblxv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zgiobdiv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ydtchxxq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sehfovjr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lqwftoat.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ifofqrou.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ohygjyry.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3usbfazyb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qavpktxd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3olomdpjt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cvhatbed.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gtoexvpx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rucmnxfy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hudimlee.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3cfrgprgd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gvwnqnif.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cncfdkld.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dysfkjsj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xobnttjr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3agyzpxns.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3psdbyvar.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mclsvuyx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3psusqpus.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3efgcymyl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pbkrviyi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqzaurk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ckzpyaym.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3urrpwbcg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xyaprlcu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rouijqpk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3yjmhmncp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3crmphrgx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gdhngdxx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yjpcmgoc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xykbzwyw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aehlpivw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3pymwrhzu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hwokckdm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3tsxwuyqc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wddoqwqt.html


<!-- 参考信息 -->