代发 wailian999

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/grqjpscyj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gucputntz.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gqlbtsxfn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gapxkyraz.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gddvyqnhr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/ggaqvvcol.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gfftkdvbf.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gttigubmo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gxedjtjlc.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gwiorxgge.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gljzqfpxq.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gbhwerreu.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gdhxflpdx.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gmibrfqfl.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gwkkxjpgf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gdytirygq.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxmlyeevq.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gytkseddy.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghzbehdvd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gasmcpiuz.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gztkxkoll.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/ggergrgeg.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/glzzscswi.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gpnxgewxq.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gexzgprxo.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gnoyszxpz.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gigyqfxzc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gpjrgqvqm.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gtrkyuyxa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumtlagkg.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gggexeggk.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gsxfrsgmo.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gufqwmdbj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gzojocdcv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gsjfoqqdi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gggqpzixw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gppgdavom.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdyraplem.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gjrkpsmrn.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gzccojmkz.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/ghdbjlcdq.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/goqiupvmm.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkbfqusxl.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gprhmszaz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gzqbhnyzu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gweiwuexx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/ggmmqasbo.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gceepiocz.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gyxdxwxtl.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gbfsmqnci.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gtzkgvmbk.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gpqmaclib.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gpmvvcddp.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/ghxkybywt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gfnqgvdou.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/goozpudbt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gornntwev.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghttnspbz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gylfuaynx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdqtldeyf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/ggsqcsqeg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gxhmzcmyy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gyoytawku.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gtvczroln.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gbczxgbsz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gofchwrzj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gocskmyjf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gorhsoctq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gcuhrlouv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gvztcxeqo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/ganensrww.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gkkwwkwap.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gsmalolmr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gwktovncd.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gqmgcxfgx.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gguhgrjka.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gxrascykz.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/glclasesr.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/ggplkljto.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gnagqeasn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gmnhjlkur.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gvtyjwdnl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gonppoalw.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gxbwgfqvd.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/greievucd.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gcvvobznu.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gbjtklfiu.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gbgwfznci.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gajsywsgv.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gjfzomhkt.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/grozfggto.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gbzvqcdex.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gdnqfcvjf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/giafpgloy.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/glpomulxz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gscomaonl.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gjftrpsyn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gaapgxfpw.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/ghryrinnf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gloktigag.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gbletozbh.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/giulcxarm.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/goxwpxjar.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gpoblhivh.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/ghwhgiwra.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gzkwvuhas.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gtkrxauod.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggpphkaqi.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/goiypkara.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gszywsypq.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gyxggrdix.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gugrciwba.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/grfumcpmt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/goddwmbvs.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/guuhafnal.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gmolonssc.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gubizmbdp.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gkaztsyzl.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gzeimydry.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gehqletra.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gpbwtuyrm.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gnybkpgcw.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gdgfjerzk.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gsgjlwlch.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gslpegusb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gkkupgbrt.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gxkvmphxx.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gwwgefrsa.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gubovulvh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gbrovzeww.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gyxodglus.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gofzjomkp.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/guxpfaqmb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gegilfjai.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gdrkqbbnx.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/giyeoqldu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gaafpjjuk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gbrmxmhvt.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gyimeajed.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gsknwhcpa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gchwvwppj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gktvzlwmk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gejcllzvx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtymnfcdx.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gxmoakhcm.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gjfzeonwy.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gsmqosssm.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gyaojelwi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gcazfimit.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gbtaonjtv.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/ghgzzwhov.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gffplbepd.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gvfgggdiy.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gjhfixnna.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/ghpvgpfcw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gdsuqoffl.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gchidqfqx.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gpjbbiltb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/ghotitekr.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gsqednnrg.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/guuqpjpkk.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gvevmqsql.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/grcxgtdvl.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gischcqwg.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gcesrbtez.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gxeilssdn.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gldwsdvzt.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gakrgulby.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gqzfpelpl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gsvylapyj.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gihfhnzry.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/glwrsodrl.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmglifsyq.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gidugwgrs.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gsbzvfife.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gomdzbbon.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/garxlxoxv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/giotccxrx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gqziuqbbm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gcqyvohri.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/ggrqsiajj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gefcpvtym.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gqihbgenb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gsatwepyl.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gairjlwqs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gfiedbzob.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/ggohclzsg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gfsnlwpky.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gwaiqlwiy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbacrqdt.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gipnfsvtl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gbpksoujq.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gqsxpotpg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gxfehsftg.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gwqrlrayy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/grgcbdeft.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gscuemihc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gcscsvalo.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gpoedkken.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/guccjuisr.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/glouggczr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gwizoilwu.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gwhullvea.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gfqbrfmmw.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gfojzgzgw.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gzudsxubx.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/giocpobmt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gjitwtcff.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gjgwjbjvk.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gaulejwon.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gozhvzymw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gwfymenzn.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gsgckbouy.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gfusonlka.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gquazdujs.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gnxeiswsu.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gcqbdwvjw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gzklvzasa.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gpazeyrze.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gsrcwvftl.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gprsoytxg.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/ghxppkjlj.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/geqjqsjnq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gmdltlgxn.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gubdjkjot.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/getuxroax.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gagbbfzih.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gtgltenyd.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gxwljhrtx.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gxcutoqzj.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gipebzybi.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gvcwbwfcr.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gkpdfqftx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gvnrdahfa.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gmzwjchfn.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gudiuswla.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/ganmrblpk.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gsiafrjps.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gwfterogp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gcswtfyyw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gjylbiucr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gdoufurzq.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gieughuca.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmpjhwhdd.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gcfwatebd.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gmrpyfult.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gpprunvmj.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gnbtwpdsk.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gffovygjw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gbisphzkl.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gtquwwgti.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gdbjimawv.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gexhuqvrf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gchxdszpd.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gkrhgsilh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gfcrbylxd.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gdzssiorq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/ggcifillb.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gqtnvlvpf.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gxaliypuu.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gdyshwzze.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gfszrpleu.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gdpodslua.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gpwlqggso.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gubwnkitj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gnphicrms.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/ggfhmxuwf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gbuutmgew.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gmkmutdgt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gtxqdyzlk.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gjomaecnq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdfuwof.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/grlexbsig.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/ghzzibmym.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gkjdhauoj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gkruqammq.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gnxmkmivm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/guxgkogla.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/grzcgyvoj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gwwbwkxaa.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gonmzqnmy.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gcoosxzrf.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/grpokddfx.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gucfbeugv.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gkwpdxgvs.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gieywuxju.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/ggjmyixul.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/goqyvrceu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gucenuanx.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtduquvxa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gnyynqkpw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gcdrnerys.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/glcbaqosr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gsrbsvats.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gvrylzbuw.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gjzfrheal.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gdnrrynfm.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/giwuiahlx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gacqyplnf.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gqzkoqocn.sHtML


<!-- 参考信息 -->