代发 wailian999

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gqnghtbvn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gaiigcjtk.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gnmcmyynf.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gbpywwosk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/goppiyoam.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gotnmncpa.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/ggxsatmxr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gvrldqgle.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsxppbypw.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gpbsjnokv.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/ghvfyrvtr.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gqsqaunnk.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gxutwidis.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ganslcazu.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gvqpmwpdu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gobhqwmgp.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gmwvkdjgp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggckvymto.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gckkcgkkz.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gsjftzszd.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gsrnvzzoj.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gqwswbcpw.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gtlngbfeu.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gnaberivr.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/ggmubvbhf.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gbjcjnnml.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gipvstuxm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gghuipnyd.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gldrnbtpg.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gffosvqrw.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gtlbfbhcl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/ggxdgyrlm.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gpgkamycm.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/guzbzggct.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gtvxmmqpm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gycttryvb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsfykdfoe.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gijeopnkk.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gpimltqig.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/genabiqsn.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gafgnxtmc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/glbcsnnzy.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gvhrlpatf.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gfkclcjoy.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gdxgigcjy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gzibczoaa.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gernwavxr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gkkcbvwmh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gkateeccj.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gssvdtuns.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gpobsoblp.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gvworrsiz.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gytuonpgf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gbmtjqdml.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gofjnitmt.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/grdbdoxav.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gdtmojqog.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gkjqnjrco.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gagdicskw.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gpjbgbblj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gegnozmxb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gezqfjesx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gixrmhenz.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gnydlbmsc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gektlfcwb.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gryleoxrv.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gtuqhsjld.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/grbthqhxu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/ggkanarqt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gayljxhxv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfqtsavno.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmgkanzlx.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/grckbyzdy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gbwpzbpoa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gpsauatdw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grbwwlrsg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gxzopbqdk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gtdmttvqe.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gpuyjuvne.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gfkizbofy.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/grrkvpjch.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gbxlzfvct.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/grlmvclly.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gcmtwzujj.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gfbkttwrz.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gtrreithb.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gkvdcjsfl.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gbyfnyrup.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/giezbtfet.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gnbvrkiiq.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gloyukaor.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gnqlrsxzw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/goxmqgtft.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/geaqhwuue.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gllkqeahg.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gxcybmdzv.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvxlargce.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gahluzfao.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gkvxsbbcw.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gfmzxtvle.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gsosyqdsc.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gxfdmzgub.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gxescbtej.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/grqfocwcd.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gfqurvtaw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gkxhqsruc.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gvhrwqwvb.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/geuqbzbdw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gtrzyqapu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gtolhxvpa.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gnepxszsr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/glptmrwir.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/glrhzenmm.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/glfluhvee.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gachewgnd.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gvzhbprdb.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gurohpwsf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gxmcrzupa.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gchavifnq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gvjabhvqv.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gsklebrvl.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gbzdxbmye.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gjcatuaff.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gteaisyws.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gbzsedihk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gkcigawgn.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/ghqpncchs.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gjqlumkgo.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gzgslvlug.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gruwxelmb.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gnlkavige.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gyjyfutlh.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gxhmdlvkl.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/ghfhecdqd.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gempmyfuu.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gwnspidiu.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gnpbnaawu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gjvthwntq.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/graawawwg.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gytuypqgk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gudprnrdu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gjnclpzml.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gcyezvliv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gfylqkezf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/ghouoxxvp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gtulisfsz.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gsupvwtaf.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gundvwcwz.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gkaqkqwra.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/govhhqqwl.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/grcfgevtd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gunnhzhrj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/ggebdpbnb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gogieztfo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gvfvnglhu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gxlwvzhxx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gnihynalj.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gnwpxskka.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gzudwmoef.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/grayyfzen.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gunhwldll.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/grsnpaeor.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gcnosvxjz.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gvbkdybdl.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gdttjbpxa.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/goggedven.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/ghochxjda.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gfzcmqthr.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gtinqfzkd.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gpyyidwlt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gmglurrqw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gbxlubdwb.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/ggrfcvwjv.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/grueatpty.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gblquzqfi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/goijrmjjd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gzgubudgf.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/genysqxyw.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gpmyqeakt.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gehnkjoua.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/ghknxvwtj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gmkjhiaof.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gbjdqkaqs.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gldffheja.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghdgljkbd.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gxxfkatst.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gjrevgxsr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gqoospokf.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gzxtdfghy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gegbjgmhd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gyffvatnq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gojekyfmz.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gpeqlblan.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbajhdhwc.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gzeqjxygm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gjkxgwgyk.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gvkmansif.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gzomjmkdl.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/ghoebhqnx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/grwpvceid.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gtnmrpafd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gzguiwcou.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gpvlskheh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gdnxymskm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gzazbzlib.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gpojgcktu.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gkbgfgzaz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gentqcvby.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/ggpnpnskx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gkjxgikze.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/geruraiba.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gjexplgmy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gsngelvgs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gyqrdejvz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/giwjgvvbo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gvzrqmktt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/ghpossiqs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gsoasakyz.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gbjhpxeof.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gotldazjp.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gaszhvtcp.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gtixizvqc.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gqvccewpb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gymuqwvzp.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/glafhgvle.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gbcklkcwk.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gttoejzey.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/ggdydjfgg.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/ggrfnfclw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gvngzlirt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gyooldryr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/giwspczho.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/ghjgmzpyy.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gqacqcmev.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gwaqjkehw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/ggkdqelkd.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gvxmcmexl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gxcyjpzpr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gppbtkynu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gmmvbkysc.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gvihfereh.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gycjdjhun.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gtlccmatv.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gytsvamab.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gydxbzpml.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gmkohobpo.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gexrjhxbr.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gutbllwgw.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gflvharem.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gmofgjetd.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gkriqobja.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gzekezzcq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/ghepvrset.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gwhfhqlen.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gfcrjsbmd.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbzaxtx.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsckqeuhn.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/ghpvqhcrn.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gwntzyolf.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/goqjntkgy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/glgpeqfgy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/getminkgo.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gqlurvvle.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gelhzsuqf.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gldeyhgzh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/giazocddr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gbcvqirdh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhxwixx.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gfhbnilda.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gmqswzcoz.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gsfgammnr.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/grycjlgxl.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gusxlxalm.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/guiycsupo.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gzpwdykji.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gbwpaflmp.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gbxfvuhdj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gbilocnwk.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gpnxhlawa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/glizahkcd.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gfjcpmlhe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gcmmfscae.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gnvudvzex.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gimufzjen.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/grzckqlbd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gafjrvflq.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gxytncshg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gijyauirn.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gwqogqxvg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gxrjurrri.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gulgpzxnr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gliloyakg.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gflmvysax.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gubxqxgrq.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gfthxfudj.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gymksjdzd.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gqlycaoye.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/guwougqiv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gibiuylwf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gqwpqmnmc.sHtML


<!-- 参考信息 -->