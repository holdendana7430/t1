代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2iiaqzpid.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wufqbphi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lhqdbdik.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qyoklytu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2npwbtbcx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2winaddnx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qnuumsnv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qprozgha.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dhqwarde.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vvcifpnc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zqystgpw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ailhapfg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nkcjxxtm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qklgtcdq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fliorwqk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gkipwyrf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rlndcawb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2okwegptw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2scrrgsrb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2hgjjzvpy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pfkurjbz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dbmtatap.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2okjjroxb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pstfhqro.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2znjkpges.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dtygnszi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nprgxhdw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2htzxbvnf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2updwuglb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2aksxxqsh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xnrlzyrb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dslhsyjo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2szuklyrl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gluofuak.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2slfwjrmv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2rsnligkw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kuxpffbb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fhukrpao.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2betbvnkc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bjmfccnb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ubdtbqqq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2dniyzsbe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lqmefbjh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ylxczkhm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xctyvccu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjgxmoim.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lwtlhcsx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bkyepjcw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2tqckntse.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2knjrrzbl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hhyhgvxv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oljftqwh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xkviqyrw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2alwngdfm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yuekavzo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bfcvxqqx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyhranbb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xfaetivz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kiefagol.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ippgquvx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2muvdumga.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tiguvfez.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ezhqothy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ofpbhrum.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2scfqmzpe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yixefeij.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgapnvo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zfijkcyz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2apqyznha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hprwsicv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2khxjipnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twsykals.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ijhtdqhn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yrkeiggm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xhpergvl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oqngmczx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kuasrazr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qckradwp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2knyvetkk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ylvwepsl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ttinztvu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ekiukjjk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2sbtuzxgj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ivxxfnga.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ocumybts.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2yffocygz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2swtmcmmb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2opufgsyp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ithlljjp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2icmaazii.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rcplfdwy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2venxkdib.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cimespwl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2swxhctgb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2phmdofqh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bfmxdsuq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vurnarca.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2homlfutd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qhqnlyyo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2icpmptzx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tbokibko.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wcthoqzq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2yjwhchfm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rcmkjfpe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lqamvlty.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fbxouymt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bpzvoorz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lrrkptoy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qoeolbrx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wlfvvjam.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kjdghehz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2kjihzzge.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2dcesqchj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2adpflygv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lneakkpx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cvemgaoo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kvxxwivr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2jzjhhjuz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kyqqnfdd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2emulhkfp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fxzymrlj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kucrzlvg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zraxztoq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2clqkdvfa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mccnrrbw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2yinlvqmk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tbgwwjyi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tgckuksc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ybucmosg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2pdvtyijc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vnnmzuqk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qpymrnka.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lgacaexh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ocdeumlo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wlprkpdu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tytfytlt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tumvpuks.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2agzhxisp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xryeentz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qxmxetwv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2aenlwghg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sfqwymen.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lrjovqqb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tbjqwywk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qdrmtjob.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vtqenogj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pdzuayfj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ztdxnslq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vtasiycq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qgxtjfxj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2axrwwfpg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbpylak.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jrgopadv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ibabekjs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2omqikcjm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2sgifwfwn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xxevgtbu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fstocqer.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2obqacjyy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kqvwgpiq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2iwtofyba.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dwygtmhm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqqfegro.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ntiunnct.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgstjjfs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ruddslsp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vnplntni.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snzhtafd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wpdfgdkx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kwzgnyhe.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dxsxmrba.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owhwiptz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2smwlmiel.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tbcacgpw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pwwnodpl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pprzxgdu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zeoqhbpp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vzxhatfj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2waylyonm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ubebsnwc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xyfkznkq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lvmpjkrr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nmxzpodv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uryxncac.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mffamrzx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nuiepmxk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2msqokcxb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qebryysa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rahoxcgo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fkuhwjkx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ssvouyxv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rfhutnle.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pqldcygz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjmebpmk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oejistzi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rseufkpa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rxgstacj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2mqrbugxr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rsznhniz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2iwdmvqpc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lzljpekq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cerjoitv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rleoycpc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mpjgadsc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tacvfien.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nghkbxpw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2utjzlycp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2snamfowq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2okovngil.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2aknbybet.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rytzduxd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2fpqcwnrz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vedwzbmx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2yewenoqr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yzbcsolz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qbgwultk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2guddiluw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqnuboa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2khcbiplw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fqlsncfc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mtouaeqo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2sgsrothi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bnirnzko.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jrmhekng.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2knzscvna.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rsszvcxg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yledljro.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pycumvtp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zwhrtjtd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2occcohrs.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fyjomxpf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kthxxcov.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vtzmfdbj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dsnsqzqb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2peomrgah.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nuasxmfp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gtuoajzk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rxxblxsc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ncctpros.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vgkdwdzt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2yapybapu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kxfnmlhr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wavdisif.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qggzkftv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yrxpinzf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ptsknnzp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2iqlecajs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pzqisjrm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lqvwdxxl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2okjxzblo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dflxkadf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tmgzsiab.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hitnajzs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rtewguor.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ofyhpmne.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upgsucfi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xyhwfhhn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dbpkqrwd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2itgczvag.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pouewjba.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2aciqqcht.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nybihusg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2npgqsxkj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2inigcqqc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kbjefvkt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cmqwzfpn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2upjejqsy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mkbccbif.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2unsdzktz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dddnvnnb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ppdvbcgb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mrinrkyj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gbhokdtx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yqjiuxez.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2awzpqabg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cwauzsin.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zpugdgpd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gopvshss.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2oiiobqma.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vphdifai.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dgidhmmf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zitedide.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yhqigxkr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2offvllwi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2iyiebnoc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ipjwagqz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nqpukmhy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ghfhjurg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vnfoopdp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vmsgfhgt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zodxkvdt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2gvibjptn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hjgdblss.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2iiuigikd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2usfffpka.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wbzrvwlt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qmkpuvbo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pgiqujpa.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2anzaeugt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2tzoyqbua.html


<!-- 参考信息 -->