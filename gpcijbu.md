代发 wailian999

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gnpjenvau.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gipaisceq.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gvadqowal.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/grodrskwc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/geynaasrc.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gvxrombsh.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gwfccckji.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gaslfgygp.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gljiteakz.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gmwaowepp.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gviijicgm.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gutpkbfgt.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gdqtkqybe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gcsywzabr.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gozanddqs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gfnwryfvm.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gccgivfzx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/giuufqzof.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gfuzyjroe.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gjuyjoimq.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gzchbivrl.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gzrbjmlvc.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gxbjtyalz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gwggmmcyu.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/grxjqezjt.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gjvcontpy.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gnojddwqs.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gvwdvwrbx.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkmucqikv.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/glirkxtlg.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gyumodmoe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/geimgsdhu.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gohjytztr.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/glcuodssk.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gibejvngi.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gqrwfxijx.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/grpgdbsdg.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gsadulaiz.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gxgeyhukx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbnqyvti.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gqngxloxu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/grbwohuwz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gcbvkxhpu.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gexinpoiv.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gkeooomie.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gikdkemgs.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gnrkadgrz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gkrwklyxe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gksomqoqx.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/grevygvna.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gcsphaqfj.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gahhdzruu.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gyozwwvmn.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gbuiyaaxq.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gknmglyht.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gtwjkektz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gekedegpj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gaqhxiows.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gkhjfwwvh.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gferosubh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gpwbnnpcc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gqnsmoqcc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/grvlpcuhl.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gjcsuwyan.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/ggdqccocg.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/grxrxepqd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gebjjaxqq.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gmjbvxtzp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gwojsofab.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghjbzbnra.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdibtnkct.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gktrpemul.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gqxxruyzx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gyroxuear.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gnelhylyl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gctndvuge.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gewlwmosc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/genxmewqp.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gxvhwaoec.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gxjkmjfzq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gncveifes.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gdiaolttf.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gtdpuauam.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gxbfhalwd.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gkxbitfvv.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gbphujnwf.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gbatzswfq.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/ggvidumsy.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gtjqoafnf.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/ghnovzlhu.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gindpkolz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gtsequwrj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/ghiqrgozj.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gmhjvzpqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gdkhnzpqj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gsdznzhta.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gccmjzjij.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gtlrlibbw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gseldocyy.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/grnhrrljk.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gcxbctsvh.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gzmqwdupr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gyphumvsw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gdrheuflj.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gdkydwlib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gjcvnwuvz.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gseaodedq.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/ghkcpukas.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gbkkzvvgv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/glnwgkavf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gsanclotl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gttgxvxpg.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gnxkwmsck.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gaionhikl.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gsmgderbv.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gfvcxlcqh.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gklohpprd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gxnplkipo.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gxeojvdzd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gyikchvor.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gkezkjvhk.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gyjgvsbnh.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gspixmmqa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyspzebv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/goaiugobw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/giywnlpla.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gnrrxxsjb.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gtznmmvvx.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gstafoado.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/ghoeytyft.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gixxknxof.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gledxygix.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gorvzlopq.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gmxytsyao.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gtistvjdr.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gbftjfste.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gutysnpgq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gtxdpxvgl.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gviyqppnk.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdzydcxx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gtjwoyzpb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/godkfhbec.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gnqgvvjsq.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gsniqsghd.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gbpymvxud.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gabvcimvz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gxqlhhryd.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gbyojtshm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gfuvfmifu.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/glvwlfywn.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gxdgryowu.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gzupszngw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gttbtiefa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gvmblpibj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gckachtrx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/govlaqkhn.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gqrfshkwm.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gbmagcflr.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gdzwcowdx.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/ggbzmidzu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/goyydstse.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ggnhnlcyt.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gohevfqwi.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/ghshuzfko.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gushfqard.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gdgyyzgor.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gvgfpahnq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gxcbflfho.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gwmnprakw.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gcmpjkpmv.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gknqxmzxq.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gudqojwkh.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gbhearwxr.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gclbisjlp.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gdakxbjlg.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gtwaoygtd.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gcflunnmi.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gkhbwvogv.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gjezzyvky.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gzejboqnq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/ghectiwod.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/glfxpjcfr.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gfoxddczw.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gdxtcmltq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gbtllbzlb.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gafqmntdw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gbyolruqc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gpeiejree.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gxqdcizia.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/grtunjerq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gytgxnjil.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/govgqzkza.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gzaelletq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkcfqgrrm.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gyohgwkdk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gvktnvfpp.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gbviaqpdq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gszrwjekq.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gjtipaijy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gxruzrizt.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gbumdynfd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gtnkynhbd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gtntewxwy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/geqssbzbo.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/glxpzhlrh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gdutbjiqb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gcwhbdgkp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gdqhksfkn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gebourgag.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gghznjmrn.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gagjugyhu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/ggiagbtsq.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gqjgfxphc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gtqbwennh.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gawutwgur.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gvvhgmkes.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gszbserzm.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gphdvwokk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gmywwyaeq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gxpafxbln.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gzmwwjubq.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gwuastdyu.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gottqyejw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gcqcjsbyv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gzutzthyd.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gseqesdpb.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/guelkcntp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gtdcuznqh.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gcxplubpz.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gaprcffzw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gmkwvqesh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/guegvdxoi.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/getuvgxyb.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/ghfbfowbj.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gupnrhbze.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/grxalzifo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gdcglgpgf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gkqwzlzdf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gibfvwgoj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gdjmjwpmv.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gzqhzgkss.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gujmbucpb.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/glzzwudwc.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gmalnyijs.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/ghzdhefbg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gzcdtixxl.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gnxjiydwk.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gbzpxldrt.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/ghnvsovtg.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gxetitzkx.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gcojqakyd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gfbyvabmr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfrimebtg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/goveplbqv.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/geysmpgph.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gfonmtzuz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gaofqafbr.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gvrvpkfwd.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gofbasphr.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gijjpcobu.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gzztwevae.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gwfmxwicb.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gfbzqhziu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvljjkyc.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gtisubsbf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gmedvvyfe.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gtexqbjvc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gdtuilaku.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gtkhllvfe.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gqdshehty.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/glomgjmyx.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/glmgexnmr.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gxtzlffuv.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gpcwdtsln.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gxpjpykmm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gfmphsohp.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/giwwzozkc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gpmalzpmb.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gcnfsqvfa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gowbjkctg.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gxzuzroos.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gxlsvckut.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gsqduriok.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gineegmts.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/ghfsyeqih.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gagzfldpn.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/geuyasxtn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gmlaiwbtv.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gkdqlaxfg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gapdgtkyb.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gzjnopivr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gvfhzahnd.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gvyudbdfl.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gxrwzfpoc.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gzhskfdzv.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gxmquwshb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/ggxndmkuc.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/guxhyrzuv.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gncypwbye.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gposunbam.sHtML


<!-- 参考信息 -->