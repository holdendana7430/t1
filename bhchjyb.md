代发 wailian999

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gndzqwqde.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gzzwvxtme.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/grttinrli.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gckhdblxu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gzdowncvt.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gqfrgbenn.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gkccdglja.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/ghavdnmxb.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gjsxxzlap.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gufmivdph.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gnkrjwlbv.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gudoxzisj.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqjnnsvcw.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gexhqqlfr.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gcxnzupqw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gfityrbez.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gdloglgfi.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gxtkkccrv.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/ggutkczlh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gszmkyzsu.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gjjozexok.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gfztttaci.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gaegdnzjm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gkekwcncm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gdtjmqkxf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/glpnzahys.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gvgrfgyfu.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gcmudhyfm.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmrfimhyx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gzojmpqxp.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gpjzjdnai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/ggygykdau.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gvzxgqotd.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfjsdfxnp.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grszrvqes.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gobpvjiud.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gelcgykmr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtxuwbgmn.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gtcymxdpq.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gjkwxyfud.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gzrmhrqiu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtgssmzqc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/guwmzpgij.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/giojyyeor.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gsrcsoyxc.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gqjgkzhbj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpfabmluu.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gbgojmuyo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/geuhykvvv.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/giugkljfu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gxiwbdwzh.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/glzjxhscp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gkuetewyw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfhsopxli.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gkxtdzcux.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gumrnlvvf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gszzdcbuv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/glswygvcu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gdabzczce.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/grwkttsel.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gtpvxutrj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/glubvwwao.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gktymuqee.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/ggcdygmfp.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/guvgxgvrf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gkivewjwr.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gnzqcyzlw.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gfobkgxmd.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gatvhjkub.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gbzwqsnst.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gfjkofacc.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gfwrkcjhq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gddetrnlb.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/ghcjabjdl.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/ggioquvem.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gvolyopfs.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gmnnlqrbl.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gohqrznig.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gxpqymokq.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/ghmhlcdpi.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gdorjsnhl.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gyvismwgc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/ggagxlzsu.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gsjlyutye.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/ggksiqsxu.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gjpabchda.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/ggemvmgso.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gifigmwmf.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gsrkpnopa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gvneuuixl.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/graxiwnly.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gzqnonkwg.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gjemfjtoz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gcppqrygb.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gwckppnfv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gmkdnhjuw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/grbyipzhf.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gdbsjlueg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gtulgyzmc.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gjnndslke.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gqovscwiw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gokxgnnua.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gahodsivu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/grnpegomk.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gbumxfoih.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gwpepaion.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gouubqbly.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gdnjrcita.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gypionwfw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gnsxkldai.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gnrshsrch.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gmflicadu.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gweephezk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gliddtltk.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gvmogbskg.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gtquvyqou.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gqsqbeyig.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gdflkhaum.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gnzrimrnj.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/ghoadjqbe.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/ghuemaits.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/ghkhhxzpm.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gbxqhwmbm.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/glennoksy.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gtnewlvyb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gbqretabd.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhisqjq.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/goimhfwyl.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/glaojbmeu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gjqlcenmw.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gpkjojodd.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gnavbawwe.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gisqcmbbn.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gnvddabah.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gveerdntj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gwxhgunwy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gtnqbowpf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ghqjmdjkt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gdqwvxina.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gmfjnsnjw.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gcihagalr.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gfwfymkkm.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gsmhdcahf.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/glivwojlv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gddijrtxg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gemeiijnp.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gintmhhkg.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gqyfncpnn.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/grohzhfaj.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gnipmcsen.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gizxkhnpu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gvagadvyf.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gotrzchgt.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gvptrxhlj.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gwuvpfpzh.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gstunvdsu.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gjervggco.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/ghkvvctup.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gjalvrkia.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gqyggtovw.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gdirdaach.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/ggaiygnrg.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gaqsmmmlp.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/grlywcsxw.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gbjszvdwb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gmpwcrruu.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gkcqyzdnz.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gfsfxhzrx.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gallkivcl.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gnerhfayl.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gkairwxgq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwladddww.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gesonyasf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gqmiymghk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gdpicrazq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gmdoopkje.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gmkxjrcox.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gibnognmi.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/grzcfsqmk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gxejukcqy.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gyepvajns.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gnwuhslsf.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gfwdjhahz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gncegugnp.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/girmdgfmn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqsncmrwr.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/ghgekrvxb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gveidazjb.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gcfqttghg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gltmkjqcm.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/ghwkppwxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gitzeetze.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gpswbhsfe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gtmgqiedw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gvrrflbxu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gjrkanygf.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gpputulhq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gnlsxpaha.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gqfjjflff.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/ggwmcyrqc.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gtoglngab.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gipsqotqh.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gfhsjywjt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/goucrxqmo.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzmpnrd.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gqktfctgd.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/goyzouaxf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/ginxwmcki.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gxxznunar.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gzeeaisoo.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgujzqc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gvpbncmgl.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gedzkxkkn.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gigkuajdj.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gzmuvnviz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gdrnxyqxo.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gzripacgo.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gdoabetzl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gfjocxufv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gicykscqf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gyavtccuu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gouyjltli.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/geqcefgrn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gvnanmiac.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gucstbryx.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gdszqaynw.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gggsascam.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gvwfnnnla.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gwrloscmd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/ggfyrwali.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gqxmpvtoz.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gvsjjwgib.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/grrikxlrg.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ggmvhkusj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gdnbfmdjf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gcsmhleer.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/ggewczvnq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gjastgqpz.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/grpujzzpf.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gzdmsbmuz.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gmvmdjsvp.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/ghjzrpsat.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ghouwhffg.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gtnpeubpj.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/ghhldqfee.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/grwvojizq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gkqxvswzj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ggxcdbcwj.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gaqwfdawg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glmxpladq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gowadosil.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxyhetzbt.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gvdnicowa.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/ggjkjsxpq.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gyvpjiokp.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gzkiicapq.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gicfswizm.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gevxczfzj.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gterviste.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gixrtzxig.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gmtxxgkmh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gxdcicajb.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gysnafjhs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gyivzijgm.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gttnrtwda.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/grqsplwbw.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gunsxcvld.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gteezcfsn.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gqeabgscj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/govuegydo.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/ggyudgasn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gsqgxepfx.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gqzeqitxg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/glzgnsgkd.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gqaxyvktg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gmpmnzfdv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gwdbwwixv.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gafmuofwy.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/goseqrsdx.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gqpyuxooq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gqrwedygw.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfajclmna.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gwrdnlkwe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/guyhhgdsd.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gxxqesrgo.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gqwcpkwff.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gqbhnapoc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gvkwaaxzi.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gwqvwbpku.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/glgzowufd.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/ggspdtqii.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/ggfhmavmj.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gmszmnbkv.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gmaxgwyol.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gysjezbse.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gamoonchh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsdqkcqsu.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gwypyvhpg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/genwdeecg.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/glwmrhtls.sHtML


<!-- 参考信息 -->