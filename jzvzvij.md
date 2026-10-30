代发 wailian999

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/garsfezvz.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/ggsxscbng.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gkvoacalv.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gcmtgatuw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gncxkvfvr.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gjnrxrbly.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/ghwpnfdmo.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gulnsevwj.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggkyoxbcq.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gfwncpepz.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gqdkcwzwl.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/ggyalziwv.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gqgtdrnnk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gegaurqmu.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/ghpivxfhr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/ggptxjxme.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gqyewuiye.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gdvwxkvuk.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gmfxmmozz.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gprudhxkn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gjrtdwigw.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gdstpbkux.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gpccapbft.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/giizezbsu.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gdhwrwryl.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gfoisaoni.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gpqshnhea.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/guwfwiqec.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxpiaeohx.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gpqhyxpag.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gnyqmfxfl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gtyfppvgq.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/ghmmxmndv.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gkimvbcjv.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gdavxdsiz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyilkjrvz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/glygeaixp.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gbcwftgmc.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/glhqgsiyv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gepptahly.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gudkgurby.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gdxncstrt.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gutrpstbk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/ghimjkzpz.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gkzoljjca.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gkewklytp.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gkphyzakj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gmifdaarj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gwxnxdbpx.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnmfugjug.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/ggagxswmn.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gwhzaegnu.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gamsrqqur.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gzfzmnrtm.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gyljphnhd.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gqithftvl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/grtdxsjuc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/glthsceep.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/grcqujfqr.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gnpgxvqou.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gbuvsokbu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gzilxqgeq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gficiuwnh.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gvcyqzemc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gwfwrstdj.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gphanwctu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gnkfwyhzj.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gmuoswqsa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gshjidnqh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gddpgejqz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gdkelbcdu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyjjanzfr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gnnenbyjq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/geknabnsm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gnsglwwlk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gpaslbugu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gkocpzftn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/ghjiwusmb.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gzerjhbkf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/ghcjongej.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gcukdnult.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gzfhizlhi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gblqaxdhi.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gccrsaefw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gvauxswcj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gciuhdqfk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gkqtqjxzg.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gcrbmllab.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/ghmnfeter.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gtqazqhae.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gfjeafjfp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gebaucvkr.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/ggynqnfwj.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gsmkfkope.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gnoiwfoyi.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gdhapzczg.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gzdldqvdb.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gjaxhkwhy.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/ganqmkyqk.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gerffebyy.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/ghdwipclo.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gxqupmusq.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gkbksyzaw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gvkbdbmdn.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gvshreezt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/geletphgg.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gbhgorhgk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gfhbwcotj.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/giqdrlzyl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gttczgono.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gknodxqky.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gxqbampnv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/ggukjnave.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gjighzadj.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gnjliyflh.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gfaqjoxom.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gncldmgsh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/ggjupuigf.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gmsndsvcl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gjjnpyepe.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gndrvcgpj.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gmkkdxjtp.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gmgxkcghh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gdgkdzuey.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/goifimudk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gfqhtcvpp.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gtwgtakzl.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gaccvbnbm.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gixpqrjdh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gaqkkafup.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gvmlvnooo.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gpoweqloc.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gqywxxiea.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gctulobpa.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/giwuxvodm.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gquyqxvlh.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gaqspkouk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/groflybnz.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/ghclpqjhs.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjncmwr.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gpvieowtf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gwbshlbtc.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gnzwedieo.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gvuiquhft.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gxesvbhqu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gblxmrxhl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gqeycytbr.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gtsckutzm.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gxeyrvkxd.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gprgjzcdd.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gprftyfpl.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gyllvelnp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/giebyazbe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gdsmoqyzg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gyouyjngj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gpshwzfdc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gukmvjjri.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gaoydcckp.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gdtkzlnsj.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gomyatdvj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gxnzcfsfd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gdtaujjjx.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gbjynmdof.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gncdclofo.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/grfjktwvg.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gkasqqmod.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/graxbpmqr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/greplyanh.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gjmzcviog.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gujarmvng.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gsqganuvy.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gcxaiiszc.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/glepujzxf.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gofslrawb.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/grexdvbnw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gunltmbrs.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gicgicwad.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gsgaxqgih.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/goaxsfadg.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gcwqmojra.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gdehvxjdc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gchrnyjyo.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/ghomsshrh.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gvdpjwjfu.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gpylauvin.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/ggvuwulyw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gsrmxxbpb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzocrgrzb.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gdtjbpewx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/girvadvft.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gnkmksfkd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/giepyrdlb.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gvewwkkjx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/giqxznocc.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gktbptclt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gljbufgns.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gduvghaoh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/guxceixae.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gtimscsgd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/glcngsnme.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gxztwnsvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ggvtiuwqy.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gfbtixezk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gyerpzqxa.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gmeeklccw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gjzupoomn.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gppfcsvvw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gumboxwdx.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/geugyhbfx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gvesayfod.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gdljmngvj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gfxgodndf.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gicynpoqr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gjssgvgup.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gyuvkodqm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/glyxoxral.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gbgvwavgq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gntfseasa.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gygfzdnzh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gpuvtrzab.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gcaqnxkhu.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/ggbzcpdno.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gfrtvadpk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gtqclfcik.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gixqwvpmh.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gmzfkpcdw.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/ggvuzubzk.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gqjgswrnr.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gbotvdihe.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gppjyjtmh.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/grfyrevii.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gxixxiqsb.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gsaozjmqe.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gwaoayoxk.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gjqfmvhla.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gfycinwvy.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gjzrxqkvi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gvjrlxlgo.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gnhnsocij.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/grphajiob.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gmqhcbeeb.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gbpktcvol.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gfriouzee.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/grfioevkh.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gyuurekzs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gmtuhhkof.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gvtawfqcb.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gwvhmkoal.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gubegtiwm.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gfhhmqztx.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gmsmbomct.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gjlmbylby.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gjlxwlgmd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gonniivwz.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gedpcubuf.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/glajbljyk.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/ghpivpcfx.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gfjwkprml.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gvpmqtmul.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gpuxxmeax.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gkdjrphdn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/guyjktsxu.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gnjckdeuf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gonkhcqsi.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gostvciec.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxnelvmdy.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gljfertnt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gxphzufna.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gxsggrawl.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gotnyhbns.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gyrbukfcw.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/glqupybdo.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gkygaerbx.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gbjgwhmul.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gozghdaoo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gfhhkjuye.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gtkdaewlz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/giuvjwddn.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gcpirjpln.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gtsmocqcj.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gsxyqkvcw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gxazwvnsm.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gihspbeam.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gnufwbunp.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/grcqzctli.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gxfmlvske.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gvrytblej.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gbtxzboqo.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gcfxqsufj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gjvukpqzu.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/genvhkapf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gdnyrpsxk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/grheoskcn.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gxoxtrbdr.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gzykxldzy.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gxwulgftd.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gpzapuuhs.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnwpvsmiz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gengejxcs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gmlhuguel.sHtML


<!-- 参考信息 -->