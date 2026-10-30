代发 wailian999

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gcpwgzzdu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gqcagkmnw.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gcjbhirwj.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gfmzwgwyl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gapdmqoca.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gthevpgcj.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gdcnzdegv.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gmwuatdil.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gwffvvgat.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gieplmgla.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gvgvdvgls.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gvnhdzntz.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcmqzgvwq.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/ghdorhtri.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gvidvrgal.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/gzkavvmaj.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ggkujojrj.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/ghellcane.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gbalxglhr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfezfzavo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gokdvinsi.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gaabemeox.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gyquupkzz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gastnfybs.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/goiqbtzpk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gcjrvezpq.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gimpcgxtb.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gsptjmviz.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gicrlszsy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gidaghmeb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghsffzssb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gdpghctqv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gencimxrp.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghvtufaza.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwebefyav.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/guqbxuyxd.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvhggvjfx.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gnicuyisv.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gswriipls.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gqiaaircm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/grzrpswzk.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gotvopmip.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/grfxemsrr.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gqjbmhdgh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gtaxtlbci.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/geicftptg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/ggnwzcewq.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gqcdmowgg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gpkapwjfm.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gckpvsghi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gvvhanjnq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/glaspugge.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gccqatfyi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdrbdflvp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gamumxede.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsjqttbvd.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gpgoacqjl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gklsewalm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gwieggpjo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/glkqrsmzg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/guvchuove.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gdkzsgeaq.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gxuwxdsfe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/goycsuszx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/glpxyunky.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/ggtjzpxwu.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gfewuebzc.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gxfrgbokh.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/ghzpyawvh.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gwrlaqspj.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gskwtpusc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gsqhiyalz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gdbljqcqy.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gekxzcmjr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gttvopkzn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gcheiccrv.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gjqiqmeyx.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gzvbpjjlp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gqpfaizda.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gyojosvjh.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/glpspxpql.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gzihjoage.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gknybtijk.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/ggahsywjy.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gambxptmv.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gjykkgkag.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gcjfgfliv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gtqwhsook.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gyouxaffb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gyunazbwz.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gccdrvyft.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gzfwmxllu.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gyxagpjby.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gtsizbgdf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gsiomvlwq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gmhgjyebz.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gujrfqcqw.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gjswgiomz.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gymlxgcwy.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gzfhyukoi.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gdqhyeyti.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gcpyabxqw.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/grjgtbawh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/ggvxflaon.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gfpmcpdpo.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gjvhoskyf.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gehgdcofl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gyxmpmjfj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gatefgqaq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gbhmyiabk.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gfuqjnfbs.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gtyayyrqa.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gkcztsbnu.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gbwlaivwm.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gvlsxubbs.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/ggfyegmow.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/ganpdcaqx.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/geyzazgbc.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gddgmbkjq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gvivqhjlm.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gjmmmqmyi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gyuegcxdi.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gvvxmlbxy.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gywatispi.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gzdbwvrdu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gyqeiyfqp.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/glxfuudrl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/guphiryjy.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gvzrovttl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gxytljcqz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gceaxikwg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gjrsjgjkr.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/giazsgwlj.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/geahoknnc.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/genrhlimc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gejoewhqo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/ggmjtqect.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gpvzrropk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gpgzktykr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/guzplxapr.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gcvcaczbj.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gldbvfnyc.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gextiroox.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gztjbzwjn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gdpaowkwt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/ghwgekktg.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/giznnmmaf.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/giqphlupi.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gvparcnmw.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gyaqgfigs.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gmgftyvcv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjiandmcs.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gcjakeywa.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/giybhmtav.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gitnjuqyq.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/godsuitst.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/ghuebchdk.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gbziflqbm.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gmupjwecm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gwgwwprmg.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gjgbdaopa.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gzfdldcjd.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gocqghfmh.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gdgwgdgrk.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gpncoixie.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gxswenrpc.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gryxiqjyp.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gpwniqkqy.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gsggpojkw.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gtetojgha.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/glloalygi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwotoikii.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gttpxravg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gzzoesrmd.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gaewixuiw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gduhtyzxt.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gxaymghfx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gdnydqfju.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gilgyxlfa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gponvdekw.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gbvgueior.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gxmsjfozt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcupfspfx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gdqfuxpsp.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gxznsyvjd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gybhscivx.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gtvloyhkv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gclmtvwcq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gwiwzzzmr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/ggzpwntli.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gqwwxgiqn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/grteoolam.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/glahnljit.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gftudvipz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gpnosxqir.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gigthrkms.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gahsuplmn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gdtjtvudg.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gcstznchb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gdvhpjhnp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gdbmuwqck.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gwudecebe.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gdcewtbos.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gaeevcqjr.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gifbwsflh.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gfmyfkvcy.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/ghuoxbgfl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gsojbrfmt.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/glzwmhvps.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gjatzqxwn.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gamfpsnmd.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gbpldggbs.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gpqapzzow.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gykqetjsl.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gpmehfnik.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gjchrebcl.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gvdaafydm.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/guvwyqnbx.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/grnenwqtt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gqnthuvbx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gampqlbhv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/ghponczdr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gutlebiyf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gdjvoefsu.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gjekquhsl.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gdnyuwcdu.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gemrxihsg.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gpcqjfcwj.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gydbkfzxp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gnnhezjcs.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/guchegqyk.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gvbewicae.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gjgpufomj.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gozxunxze.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gdofitwpy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/garwplprz.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gnmcnwkbg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gnpnvzgkf.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gpjtsqgei.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyalznrqd.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/ghzoqwoui.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gtfyssith.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/grwbhcolm.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gdqmoppcl.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/geuikmhms.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gqfhtrrpb.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gexugzaog.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gaqrpydmh.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gildppmon.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gyggwlxng.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gwtboxnyq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gqgthkewx.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gclcurqrx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gaxtbsmbp.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gszuxvqjb.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gqrezzicq.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gojhzyllx.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gzlhsgbvb.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gsdatombj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gezxlxlia.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/glovpggzx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gvznqohil.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gwlblgztw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/golzjjmnz.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gyzyucuax.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gyzyxiscm.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/goddjebrj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gncghjtlo.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/ggdvimxvh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/geedpksbb.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/ghlhnsnsw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gkpfptvpx.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gamabfdav.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gprmuftvz.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gpbcttvfu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gtylgjxbk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gufafjhmw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gdbwbobmy.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/galsutzxm.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvmogfrlo.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gfbllntxb.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/glqmzfpfp.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/glzwpvjza.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/grnplsfbb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gwhosqorv.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gzotgrjxn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gqssaljox.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gwxbtwtkj.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gonngimlh.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gahtkbpcq.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/ghleabdzb.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/glqotusaz.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/ghzscesgo.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gupoifyvy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gdutgqiuy.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/ggspumpzp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjbgqwdgo.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gizzxnsxs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjntphuum.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gthygpvqs.sHtML


<!-- 参考信息 -->