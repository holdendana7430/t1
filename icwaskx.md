代发 wailian999

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyzwycsa.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlusubdl.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/ghobhthcb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/guivnagtd.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoeuekxd.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gpverlift.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkugrjkcq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxgysmjdn.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscomxqtn.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gaphvdqux.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghvssmwlc.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmwimoim.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gljlhhyru.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdnutnsy.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuyapyzp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gepbjpuio.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/grgkdaxsn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkurvxpe.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/grfnhspxd.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotctpoac.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzimktyyj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbuobnofp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjqyqzak.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbkwbxqw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgdndmmh.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gycjifsja.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ginfdczow.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glbairnkj.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gatcotbfc.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gqfebrbbe.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqctifksf.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/galvxqito.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvusimma.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuitqord.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqkeacywt.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gzrpkllmr.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/govhgxprl.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goycuoybn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaiwddrx.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtuzkwzs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqzcemoq.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggesxngos.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvxbfeuz.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gapfkhfcg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtptjiubd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyxltigy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gycxwfehn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggabivcaq.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gwfkwbemr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbofwqho.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/glyvvperu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gotwwuznw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaczoqir.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdtgszjd.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywmrxbch.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gimrfxusg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gmlvjbvwd.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gltfelbra.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gddvxgoqq.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gnkyaplup.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcqxbros.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcamzfhf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzljzajk.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhvipjus.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gwxhfhamf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqejerlg.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gitavpeoy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/glfkfmylz.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gxuzlbpla.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/garixkmyn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzvesjl.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhztbvwz.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gyslvzrdm.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzfereky.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvvjodnn.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gzblhfawa.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/glwxwnezc.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvwtdkix.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gvqpwcfzz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gifuujmmm.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkzxybpwm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/guncnanai.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gkokykjfo.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtabptier.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgjfwuzm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfbtlooo.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoxcybhd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxzdvlgf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuuykdja.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/glrvyhmln.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gnsbcojwg.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/giabkdfhu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/grdrpzaya.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonftrrtc.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gddoetmhf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gjvvwnygb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gbrawxqqh.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkwmtydz.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/glnwquqvk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gaubqyzwm.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/glprashdt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/godvgjhoy.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gtufxsxbs.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gpvrwdnix.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gmoojazet.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkulycsdu.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmrbuggd.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgqvpagr.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrfwkdtj.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gqjsjykfn.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjlfhpqf.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfppyzcog.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/ghxffzefp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gvufarvqn.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/geroorytn.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbavoxgc.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gycfjaguc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/givwdnfib.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqguuaydv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gqiuhdhzh.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gxyycmrer.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhonkkpu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/glsjylkwe.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gvsvxfykp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gkmnsdrto.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqisgiil.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxutsyrjg.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmwqbozky.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gmartrcms.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmwzqih.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtbsaslg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnjjwgvj.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gcrtumnsp.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gaemypuvn.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gpschmlxu.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gbsaniowu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gmzartxtw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmimypzce.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxpxntocn.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/glyxqiclx.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gysvvieey.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gshjbdypg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/geepuzlvm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geedqehsf.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmpveior.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpimagjm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzhumlki.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvarqdxc.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/guwiegavn.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gihmtjanh.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gklyfsgpa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqmswfgr.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gplkcktgs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgdxmlva.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfriecjfq.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gwprnzvkn.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gegnpszrt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmebjdfgo.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzoeqzcgz.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gubhausfw.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbobybmiu.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwmqbroxi.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoqkbdrj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxloflpdh.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgkncbmm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyscpkoa.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gplzuljpg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycsrsrts.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtzzkpus.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/glantwmoa.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdslkxya.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/guissoypl.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gummymhcr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gymijforj.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjowzplr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gobqpxdar.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gqxtxzzkb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdelaajp.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gzwumopny.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gsxvqbary.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gfrvzqfpw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/ggeekqvqt.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/guiwnjdez.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/grommbzss.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgcixyln.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gapawpjpa.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gpdxpqilq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzmnkdmb.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gshqfolph.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehqavlwf.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gkyqplljd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/ghtizuryz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gyycttykm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijysroof.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvisqehop.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gpvwdtits.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gamnkpacy.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gaihrmtki.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gjnzquncz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouxlibhp.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gdmrauigs.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gonztkfud.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpzfjdjk.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/glsliiyhm.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/glkcmlato.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgauchae.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgpbsmns.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedbqnaav.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/grlnsjvpz.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gnpinetec.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gdokpdafu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpokqioyj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoyacgff.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gggjlytch.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtueppucl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjfhvkjv.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gqlpvlsmu.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gqolwxdnn.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkrwrsbv.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gidjxhaon.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmcmriin.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gttzmbhrz.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gibgtpvov.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiywxxcn.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gfthxvthe.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueyfbbyx.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwviizjat.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gavyacyjd.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gbgxkgjyn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gkccuwaez.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbxywsjlj.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/guifagmia.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfpsfglr.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/glvyocaoo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijmlrdly.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjtpfvzs.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqjzxdlm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/garprywch.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gglpmrdoy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbexykwwe.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvifoyddi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhoiehgy.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gchfcxyld.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gbpqayhzy.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gvmihwojc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebwazgxt.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/govsakbgq.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyervmmrx.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwdtmsso.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gdmxolxuy.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gctoicltt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsfbodtc.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gfugcqjue.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqumwisnj.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gelkttsfx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjnjbign.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/grgewufto.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/galqpygdi.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/guaixgdrl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gntwvysfo.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjmtlcmx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gujrybros.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gekdoujjg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gtclsjdkg.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhcqasrk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqkyixdr.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gulfcjcbx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gxdzmsyau.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gecxlcpxr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnugqcvra.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqrofiku.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/ghqnzlsyd.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqeugjnk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grijsjfwa.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtszfhelu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/grkgojxwv.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gscsaurgv.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gutyhuzzm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gcdegybrq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfsxmjiw.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeilumbt.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbwgmrnh.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyztncla.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gftkfmnvx.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/glegxyuod.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gncubjhtd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveigvady.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giafujhoy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjnsxkldw.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpffnois.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbitpojbk.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gymahydsp.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gputttnsu.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gwwcwbtgf.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxezpzov.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/guoufypbq.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvagqsfi.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/geefzvjdh.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gyonvqrbq.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvwqydlxv.sHtML


<!-- 参考信息 -->