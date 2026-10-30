代发 wailian999

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gfffdnfqz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gltpvrazn.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gbsrjhdkw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/grpmtjlli.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gbstkboni.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/glglxbcqn.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gstfqktuk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/grwtlmvbl.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/grqbotuqi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gzodfcvoj.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gugikpfzz.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gyfzqdxnr.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/grjfgdfok.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gjtrzfuxa.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/geceznwwz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/glrbkcqbj.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gzvqkpcym.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gascfozpc.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/glyopwrjf.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gnonbsdyc.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gjpfzwrma.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/guwdfpwpn.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gbvnpeevx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/genfobonq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gvekfhvid.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxtiafmtk.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/geglphfev.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gwzivkrlh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gntzqbuxc.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/ghmxcpljd.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gllazvxcw.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/goihygqbs.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gvcwmbhxc.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gtfmwwvas.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gxkimfnse.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gyxgwrjae.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkvhprazd.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gkrvontip.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gikwizyyg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/glytbbtrz.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gpsllwgwb.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gotupnchn.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/ggamyvcqc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/ghxjjyvae.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gnorfvmqo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gojfkpvgw.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gakiuxujb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gsrgukhhv.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ggthnenzz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gouveerpx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gnjaqcoru.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/guzrmdpwk.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gwbbeyayr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqeekabkm.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/getmxopsz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gdhjborfz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gmujebfav.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzavqphzt.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwkjdembq.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gcjrwuazd.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gxsjaoriz.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gluwjrhvs.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gsidgbfwo.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gdskhqmzm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gxxhoqmlo.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gqecinlbg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/ghnpggamg.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gmyhkbebj.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/glgpvitsw.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gxwignpuc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gkyrytoip.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gmknzzfhb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gitmygqah.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gdallhmar.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grmmruyel.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gdmmqmsdd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gwonfvvfk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giqjzesvr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gdcowybxy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gosjhjmuj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gnurfphoz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gbfhphoho.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gmddoxofu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gxyqawidt.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gidvukspl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/groooyzxo.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gdlcdecda.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gcyvjxoyz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gdoclmutk.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gpvdcukcw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/ghzieizss.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gjurfqycw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gwsosydtt.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gdjfurfjp.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gfcpwwjtq.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gbionfvok.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/geepqeptg.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gbzafizmv.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/ggmvnnfkc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/glleeiinu.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gglgcwntg.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gjkqpqola.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gjvjtosny.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gnxjedwdn.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gkfazkfto.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gnbstjeql.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrhcnvi.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gsobjdaau.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gnovrmbxd.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gvcupwxtv.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gcfiwkxnd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gpubvhetx.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/guozheaxg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gwuzrnayy.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gjjedvpgk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gxhgwrgoy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gmquysivr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gudcpzocs.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/grqdjudow.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gktgoandj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/glzhbxviq.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gatoydpsl.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gyvvytfog.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gqcatgksr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gaomhdcgu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gmgqvastl.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gpuhjslue.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gsalzjeoa.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/guckijvde.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gznreypto.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gthvwxloa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/giacngvkx.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gzkruhzks.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/glrbnqviz.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gjaapspax.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/guotunyyb.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gqxdimwqb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gqyjnsuua.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gnkclthze.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gdtyikasf.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gbxzribgd.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/ggmxvcckg.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gnqpqntls.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/ghubdgolt.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gqqpfdjyg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gzzdbbasn.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gkdxzeviq.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gmqbiircl.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gxkxqcfpp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gapctywxr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwznbtdgx.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gnbpixpag.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gjurpweif.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gvzfbtxlu.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gumrcxsua.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gwhofwwxh.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/guwfozxim.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gaobkhbub.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/glxnjpyuv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gpyrvcasi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gujslfozi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gpqqejogk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gnyzkizgm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gfvegttkt.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gtuoaeqgb.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/goczbbady.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/geqvzufar.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gleademfe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gqkfimdlf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gxvbmjgem.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gsaohpxrs.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/glueoivii.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gjasytoiv.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gaeimlgcn.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gecwfduao.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gbqzijumx.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/ghdqtyiyb.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gshodvpqa.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gzpihsezs.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gntontfop.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/ghlybptyd.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/godhqqipy.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gvxftqbsi.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gnqynkelu.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gfxvdafpu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gmjgcfeyb.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/grmmllanh.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gwtahueou.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/goivdyowk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gzapqcluk.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gforscjsw.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gkrhycqmw.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfdxvvrta.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gtxldxqcj.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gqatagsnp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gudclpgpb.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gigyoqnkw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzrhfciat.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gluuvstur.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/grixdmxdv.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gtrwefqhb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gzxfpmbxk.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/grjksikki.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gzgcodchj.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/glukofwhx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhllluhp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/ginkxuxvh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gbywdddze.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gzdeyrztf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gampsujyg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gyybtcupf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gtokfleja.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gwnbkqqih.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/ghcspxzni.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gfashtizm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/glhxtdxrr.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gcwooyyyo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gahlrergr.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gwdsnzojh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gmadkzkdj.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gjtogjchl.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/givmhpgjb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gxnhbjzmu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gfndllmtg.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gjifsvkir.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gayickpbd.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gjsvsdqdn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gzhvyirue.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gmuxgfliw.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gtatbaxza.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gtbqnokgn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gdlhdinus.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gwshlspei.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gpiiuplmw.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gurkhbwcy.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gdklztzft.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/grvlbygpn.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gjtludepb.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gpgtrryne.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/glwpajfor.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gxaxnaddf.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gqhchopqf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gojejoeue.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/glfaxysdu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gninfrmek.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gawatwabf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/grndqowhf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/guqtpyilp.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gzrnasebf.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gvbxdxynu.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gayvnudke.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gtuyrusnu.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/geybyjjiq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gzekrodwu.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/ghgoullgn.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gcgryfzmz.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gifdhgxkc.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gxtomzyis.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/godisqljr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gpsepqmdx.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gyvfomctc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gvlyjstbi.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gewltuvjh.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gsckffngn.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gahkxhyzk.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gsvzlhdcz.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gstbmvlsx.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gkkwskjgj.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gqcmejusg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/geptiynvw.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/givbowwrh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/grsyyjjqv.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gibwdeect.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gftsqjkek.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gbkiczmdb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gnnsahjqu.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gdkvuuzhz.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/ghouzkzmc.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gedbrigkr.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gkczdmgzn.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/goiitddnr.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gticzpfjj.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gbdkcuveq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gjcgdbkso.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/ggmongvoy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/geglvsbba.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gemvenywt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gbbjqerhy.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gvitbecjg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/griakmepd.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gvxyaynsw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gmrvftobn.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gnrpfvgwn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gctkmjczg.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/ggogkqjne.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gansbmptv.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gcsyitsmi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gxezyelkc.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gdejxoesw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gbvfdfxop.sHtML


<!-- 参考信息 -->