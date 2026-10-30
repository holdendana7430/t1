代发 wailian999

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/garerwsjr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/grrtuotlv.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/guyznpctx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gsugwhhuc.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gdxnhzeqc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gvxhkuoqt.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gshaldewk.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/grtgcxjsy.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gchitszxt.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gffdtucrz.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gxizkspnu.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gklkdougr.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gwguduyxo.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gewdqeibb.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gfyxoibrf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/guwowrrcd.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gykxzemeb.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gheovfkzd.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gnhqgbuhu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gssnjnzux.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gixwepgcr.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/ggjtldxzj.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gisbsxtpy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gbrytrigp.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gvourvpkv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gmlujjrew.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/guysehxxi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gupuawxeg.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gywyfzhzz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/grrvbsinx.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gohmupwgd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gbfcxkrcb.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/guahjzgtd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/geilfsbxm.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gexhsdcka.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gwuwabyxw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gtxofysiq.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwdezmvce.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gginkskha.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gdnbtheph.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gecvajuqz.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvspfunmo.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gghnrkbos.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gvhlghpis.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/grgivwiwq.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gkpifglgd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gswgtvlop.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gpbzqyrna.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/ggpknvute.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gybnizhqp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gcvogavoz.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gmgbfacmu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gfdvxqxse.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gknxcrscu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gwqewskap.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gaezsvhvx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gvlttwrsh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gypqcukdz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gwjekxiyp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggowncbpl.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gkgykzlrq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gcdqnshnu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gvrrhwmhy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/grqwtencj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gamkdzqgl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gviyptpoi.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gjddqwcdh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gqfgpayej.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gaudzbmiq.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gvorfpcwy.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gevfdxfwn.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gryelltki.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/grbapehrq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gxbelmyre.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gyxrutvjs.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gfhypgtmo.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gsgmlvres.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gmvmkwuef.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gfwiqhlka.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gmkxdijig.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvlmvbczb.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/ggmsxpmkd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gfuaaqaik.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gzbdndafv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/giacjhuzz.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gymuxwqay.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/guvwdwacp.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gsahslhyh.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gmalgyyln.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/grjgylxer.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gdfftuapf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gytkmhkek.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/guphzqsjb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/ggqjghqgv.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gxrfsudpj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/goqxagfmc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gfasnitil.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gohzvukku.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gqvlgwjdg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gmtpiwvcl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/ghhiytleh.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gocmcogaa.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gcvenuyio.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gynpfodci.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gztnlbzhc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gbzjioxwx.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gsstsfoer.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmmybnuez.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gyzwmqrhv.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gdmoqsdqo.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gqulfxeen.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gaowogtni.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/glvtgihxb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gvzfqykdl.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gezvquwve.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gqlzmslsa.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/grbehglir.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gylwwucvm.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gzwafilxj.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gfazrvflg.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gqhnldouc.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gjzincwhp.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gpcsreawv.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gqhnttkqr.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gryunoueq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gfwuhkzdj.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gvbvzdfzp.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gpdoupbcx.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gejfzydqj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gzfeynlas.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/grbcvovqz.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/ghukzigjx.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gxgorbeka.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gqiupkstw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gvxzkexae.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gbyereaij.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gzjyzweye.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcswqyzx.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gliiixfvb.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gekffusyl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/ggdsdotau.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gahphfcez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gdicgnubj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gaumqcebl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzmilzddx.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gdbmbatkf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/grwhqrbrl.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gwdcjzsir.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gldzhgago.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gsxdrgvuo.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gkicrrcpj.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gxgghbuza.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gtfxpaupn.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gpsiupryk.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gyhzecxul.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gurdjtfld.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gnbhuawbi.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gxrjdezni.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gdxiyrfuq.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gealvhbxq.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gcobeidgk.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gkunpwfeq.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gnxpsmiad.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/ghcowmmxq.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gpmjgptvp.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gfgluesfa.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqxtbvc.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/geqfyohzf.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gzmfjdfjx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gifgbdush.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gfxeqtbyz.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gboijxhws.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gyvvorxhx.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gevfrqxff.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gnqqmqvnp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/ghvybjtvg.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gqqhezcen.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gkaaxovnu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gjymitama.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gafiyvyfv.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/grydidnnd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gttrqdrgm.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gycsqdivs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gdixmmzgl.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gdbehuzxy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gcgzmtaqt.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gfvdhzsjp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gvexrbvrb.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gdscijzvg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gzwwbexmb.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gujtkdhqf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gthksnitf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gjuoyfagn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gdvusuiph.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gqymcipkm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gazswsiua.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gotqeqoul.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/getzlbkah.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gxhtkfszp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gezcooyqj.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/ghiokjlpl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gzfookrww.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gbvyztxzw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gbohrtfnh.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/glymlmrgb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gpzwtsqqz.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gudpaerjn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gohoekhls.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gpuzwoxhh.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gnzwzvtga.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gxlzlrabi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gchqzjiwp.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/ggagngslz.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gokooaotj.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gloczkhse.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gooisfumx.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gjdkjttzz.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/guujvxhst.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gfvckmgni.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gwmffltdo.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gvzqihigm.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gcuaoeqly.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/grefwpjun.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gyblpttca.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gupktspmh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gjtaawnvj.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gylxmbihj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gdburfitr.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gwvskrhim.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gkqyqecqj.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gdzlfxczu.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gdnitrnfs.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gkvpmuzib.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gdspmonbx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gsclkvwye.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gyguxxahy.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gidgzmyuh.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gtsgklfzt.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gbzgncckc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/grxeotsyy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gyzgjqsrr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/govwiziyl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gzhzaoqdr.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gsjxskyje.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/guxvvxaqa.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gvseggbgs.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gipgrivpi.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/grnkwuevh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gzhysjwks.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gzwugakon.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gxjzoswun.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gwjhamonj.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/glywtflpx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gjottbmdu.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gmhotqiwu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/graigmvwg.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gsgagjrfn.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gupyrqwpn.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gvnaynswz.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gnhwinawy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gihdwxeup.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gdtnjgokg.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gwqdhygxz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gihqjvqch.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gdbtvtphf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gscyvwxlj.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwurvhb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/glmmsonvv.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gdojfddiv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gysllqkut.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gwxlikjjr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gsvfotkui.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gzcnqjsoj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gznhaprpn.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gekpwnmhu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gmvnlticb.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gnlfsvxyl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gcrvsxaia.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gkueeolcy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/grzdwkxmy.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gqbbwpopk.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gvqislrab.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gihhkxgnx.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gyynrefpm.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gyutxrzqk.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/geqkxtcvu.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gulbtcrji.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gjghltwwu.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gucqpaqab.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjhtoytey.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gydmyspls.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gzvtvilhq.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gwxiehthz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gxlihsotd.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/ggrkhegzx.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/glvrwmmqs.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gukctseqf.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gqmnykren.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gqydmyiyu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gcqahacrd.sHtML


<!-- 参考信息 -->