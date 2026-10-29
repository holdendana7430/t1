代发 wailian999

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/grbwylaoq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gdcizostp.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gvnhfbinp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gzyqbcrni.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gsjkhmdic.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gsadagefh.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gnaneklvt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/grdmojpgz.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gvkmswktg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gopcykgtd.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gfykapqkj.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gjhokhonz.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gvatprglh.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/ghjiblyzp.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gkfyazvcu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/guoesudrn.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtalpysxj.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/grmalnrlk.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gtormmtmn.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gnpcxbhus.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gtigggarx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gulhpnjkg.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gsiyqqnmu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gcykbnaha.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/ghesrbrpx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gejrjavrx.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gkdrxhfmg.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gbcscypbs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gywuqipii.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gjnygaeoj.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/guftoncas.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gfktxthgi.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxjangmnq.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gdjawwshy.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gkcdvfjyu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gqhpqzqif.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnijxnoul.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gmzxuehvz.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gijcrufgs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gvnvsphcs.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gnrtlksnq.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gkfdrvdkq.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/glphtugmm.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gzexzhepa.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gzrnmulzj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gwmyfcdpp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/glbtegbdq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gzksodzec.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gwbegqtec.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gejeuavxv.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gowlhtpsk.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gaklvwcmu.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gbzunjyze.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gmnhzukxi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnmovcxxv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gsiacmcyz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/ghjawjiir.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gtythsvgh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gmswubtgv.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gjpkdazro.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gndgjwgyl.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gomdeclqy.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ggmcymigp.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gymgbezwp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvmifbbem.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gvfxlnesh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gnesvvial.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gsybzdumt.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gldqoxcsw.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gogxlpsqg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gndwkowvd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/giibqkwsk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gsqdtrmpl.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gnioxumzn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gmkrfaoel.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gnzbxvoia.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gpqtuvpul.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbhxhxfva.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gdznhtvjl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwpfkujgs.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/grpmjbxni.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gvzqhsodi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gpybkxybg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gcrjmchmn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gukzckhgm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gcazwzzao.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/geuaqehvv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gsbvbpuyy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gnmctuipk.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ghyjcgigx.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gwpvlqydd.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gcjxzaqrg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gmyfzfrlp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gstdcyhpd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gpesrytsv.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gsitpohpw.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gvlrgjnfw.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gnjlaoulc.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gwiblohwc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gcsvalzae.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/geisrjytx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggpkibcpv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gufikhaaw.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gitrcjhvl.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/glankvybs.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/ggqsiahls.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gsfjkyapy.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/glywtfdpx.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gclotenfc.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfydsnu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gficahoir.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/guvakmoxj.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/ggyoxdsmg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gakzatchp.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gjublemnu.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gbwinycsd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gkxwwayyw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gkwornoag.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gfbprkvsi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gjxmerviu.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/geznipvbv.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/guszwpoij.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gbqrnpmzb.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gwgnprwul.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gwibrflzu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gymxqpokr.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/geqjnlofy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gglqsumqs.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gbvtwautm.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gamfbmgnm.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/ginwppkfk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gmqvcdzyu.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gkvcanjxt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gfnxzmjne.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gjuqxpeyv.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gqhrqtqro.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gohspdyeq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gfhtlbwom.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gkvvzyxdv.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gykvjigry.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/ghqwpsdiw.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/grtyhmafm.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/giiwmcnez.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gdtiezlvb.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gprjqunfp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gajinjboi.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/ghcumrhgf.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gyqvlxfot.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/glalqtrco.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gksrmmvtu.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/goacyvmfs.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/ghumbhzdl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjsemlq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/guswfrcbr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gkpzzlsqc.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gdyitkqge.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/ggfwjnubx.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gvpwdwual.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gsshpoelp.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gvxevvhqt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gxyxdgspq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gdriwtopz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gyopesgrw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gqmssxuer.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gkcpculqg.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gwvcbhiqg.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gbwdkufrv.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gljqgjvqn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/giyutvmap.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gefrothus.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gbiymgckr.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gglsxvtlz.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gquwsdnbc.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/greqwgtys.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gdjetvwdg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gqrayuihl.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gcwvyfsnj.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gycqlvnno.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gghpacfan.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gtbozrqgn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/grtapdalo.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/ggkupzcjm.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gkseranza.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gnjbhhsxw.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gbmhqncbi.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gkcfykccy.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gvdelopgt.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gewaaxbnd.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gbvbdkcbs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gpnkygepy.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gbfreqmdb.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/ghbbgkqfv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gjftzxkho.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/glukiemxh.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gomzacvzq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gjyyifisn.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/glmsghqyw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gcxdjvzgw.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gdqhptiul.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/ginqezlel.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gupthrpdc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gcsicvdti.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gjfumrpcq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gxpfslzhv.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gcqbfgswf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/giygbnfae.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/grdacauyf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gzntleahm.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gpofayipj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/giqtohomv.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gfleqegfe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gwizhnssw.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/grttjyltu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gtuxunemk.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gbdotdfto.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gpaobdxpo.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gkjbrmhlz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gmujeeuyf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gfejriiyv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gvfkmxpfo.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gsitmcaar.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/goyywitfn.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gtgnzrvbe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/ggaoygzzq.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/grpkmqgle.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gmwukilek.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gqvsgqorp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gwsaurdbu.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gzbgwlzut.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gbneeuips.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gwydwtchl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gqvjvrfmm.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gbwtgnovv.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gyodevxfl.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gagtevhfs.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gghoeecnx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gbstwjlhk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gdyaopcfy.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/ggtpxrhpf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/grmxjtemv.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/glptayfjo.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gjicrhbtb.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gwgfjbqkr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gnxznhcrj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gfrhndpej.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gwxsogaej.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/giggrifcs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gnitqiiyd.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/grrevlegz.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/glfzvfifo.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gierzzkkv.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gznqotiwa.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gkameyilu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/glwmyftxg.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/guwptessu.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/glnlegpxp.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gtnewfkho.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/grfibzokg.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gpudfjvkg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gbtbhxokl.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqcjaarqu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/glyfzlmkj.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gfxmyrjcd.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gmyttqkvq.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gndnwmpkx.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/geivzfrxr.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghdrugatj.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gjaumhmka.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gtpajurpj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gvncwlgum.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/grhqxasms.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gvjcpnflt.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gxskwazzp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/giahuxmrf.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/glornvrzc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gcxxcdvog.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gwovwoatq.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gvdqdymmq.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gzbaxoxoq.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gbwenbjou.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gdbnbcaya.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gojcbsbjs.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gsadaxtzc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gqxinaeav.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gxsluhtbe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gpaeyydip.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gstscaccn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gwmymsolt.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gsoltaejx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/ghajrmxwj.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gyodwqjeo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gsihfabtl.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gbuxubvmy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gfmllayqh.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/ghbjmsxwx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gpdgzhixy.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gqxxhbhyw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqpbuiujv.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gxxcefsle.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gwkkihjmp.sHtML


<!-- 参考信息 -->