代发 wailian999

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/glgrtvudo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/grpdtpdzj.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/ggfcjtshq.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/geqxzylhh.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gnyvsbuac.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gcxemvhti.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gmsmdvizp.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gbkvdlopu.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ggbkknjkk.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gllbhefhc.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gyorcebpp.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gzbaoqpmd.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gpwmrnnut.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gkakyuetb.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gmroabtgs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gkaamhcwv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gfgqshljs.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gfephbhub.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gfhjjeiyz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbrlulef.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/grykbvaba.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gunzbyzgx.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gipvhyqfv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gewboyihn.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gfmgrvutd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gizzdvspb.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gmzybjzcg.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/ghfsqptzk.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gjtbaeszb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gcoxheozb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/goslifbjk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gscomhvkq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gyfduuvzd.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/glsbupfjn.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/goclcpuvq.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/govhfocpi.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gerjbfzal.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvftzwxsd.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gzayyjtix.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gmfprsuvv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gtfyrgblr.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gevmizizp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gionhsfrk.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gaohtffdn.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gnrfwsfaw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gullnofij.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gunoxibee.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gkjnrcvwc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/golhvosoa.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gdbdzvkaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gavlnbrst.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/glztqjxns.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/guopimhwe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gecgwdlty.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gonizlssx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gamaclnad.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gbczrzsdm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gllyssfqr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gzpkkqpfz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gkyyykzve.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/glrachepm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gkwtnqgap.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gtqstznxc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gevcbxdwg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gwpezotpe.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gaixpyrkl.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gfftgdvjr.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gfrbaghrs.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/ghsuqqmqj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/grhzzusri.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/guvjtcyih.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gtwzavspa.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gagmxahtr.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gprifchmo.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/ggwrydhpd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gfjyzfkph.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gipbfbfld.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gxuwbnqmx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gvldbmcju.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gggxtyzkc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gewwxyujh.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gbljjfwct.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gmbxwdsfj.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gzvraypbl.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gfargxppr.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/grvmrrgrk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/ghjhcuxjk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gdjfeetdw.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gmsmpmhqr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/glmxgvahu.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gtwgcipwg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gikdlbcab.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gevmkdequ.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/grccqjoko.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gvtdfeofq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/ggdwqwahn.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/giobdmhjt.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gkneufsaj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/giikosffd.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gsqqjmmks.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gdzlmmokz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/ggpgpkhoo.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gbhgtzqdp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gkvdfpulr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gtbgketny.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gckujcxih.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gpzpsaajb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gpkebajqu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/guvvdfsbv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/govzpzvtc.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gzmvxqyjf.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gzqxfucle.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/grnxltlqt.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gtbgymomh.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gsmgxlwbc.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/ghzbfqyin.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gzssaqpbw.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/goflberku.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gwqgvcbta.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gywlezabs.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gfgjujkzm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gllfqybmw.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gkjxjokta.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gwkueqthi.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gyfjxeiyi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gbwsexudu.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/geoyzauag.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gwqcomaqy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gnoulsgrj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gwcelagbd.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gfshfundx.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gdbrguzgu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gaxaskjmb.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/goeblsjjk.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gfvibgsoi.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gbsxywcfi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/goaaovbsu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/guzjezhfk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/glastbouf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhsqayb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gdwxiutjo.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gvmjzudnf.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/ggorpboiu.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gioxhxmwz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gutnvvuor.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gcgrdiknq.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/grgqzqrcj.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gbzulqdym.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gvcbbelfl.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gauhyovls.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/grlkhkcun.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gggoluqmv.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/ghbufyrwi.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gvycqbyme.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gbczgcjjq.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/giciqrlwi.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gewbftibh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmrllotz.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gejvhprsn.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gzyrfsbfv.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/ghtrgbotw.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gopgwdoqn.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/ggixwlpfq.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gillpvllu.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gcpzopxjw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gitghqfzj.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gjpqgqkgc.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnbolgtzv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gczagmdrf.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/ggwznocih.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/genbhufnt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gywoewqry.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gibdibnwm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gurtkujeo.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/grwskkhra.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gekvoozcm.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gmugfzefk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqhmixjtg.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gjmufmqsm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gpukrijce.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gzqbnveit.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gusxmpwic.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/griqqdyso.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gaththmsm.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gxcliffnv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyvnlvmds.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gkeeyvmgn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gvbjrvasx.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gqolfrhux.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gdmthxmhs.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/geunryocd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gflufvoof.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gzfmtamue.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gwwwfejuw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gnhmdklrf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gcdsoifpc.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gnmqgwlan.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkqryiox.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gpkoaarcy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gofiisgzq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gdenhbffq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gucbrnibp.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gwgdiamsj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gvmqbeoji.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gofexphsw.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gwdcpxjkt.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/ghblmdfjm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/goqdofbgx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gxchtdqko.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/goebqmpeb.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gixartpit.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/guhmlbexo.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gbblckmpk.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gycsfvtye.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gqxiovjvl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gqkwngijz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gtunpqstg.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gqmghawhm.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gqnsjsylb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/giuzdhwnl.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gntyhraux.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/grdicsrdj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/ggbhljkjr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gatjttjps.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gapefedix.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gjtqulcxs.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/giqpbovhb.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gzrfvlmhd.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gnfiuyrjc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gxigzkgao.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/grkbrzjrw.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gdnnuodhy.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/glcadgubo.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gkuywyvnn.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/ggydodtuu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gcgpzaacu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtzkhbkcf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gsgbcmggj.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gepzggksc.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/grrkmqupx.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gmemcfrpt.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gqaatqyks.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/grdpglres.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gufhghhlb.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gyqkehxqw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gokhorqsd.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/graqpynrq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gvbsghsph.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gailpwupw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gssqlyzfp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gwcdphbsx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gonsmuedb.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gaqyrfopa.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/grstfydmi.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gkccbejir.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gybonvihp.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gvxzniqhs.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gflnnyhxg.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gpbgrvdmt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gvloevmet.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gszjawwfh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gqysdibxs.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gjuorhhqy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gfgggppcj.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gxnitbwbd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gulyrpgnf.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gyzmgbaxl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/glzwcdiix.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gqffbawox.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/guxmwxljb.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/grpqxgcal.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gdwnnugpv.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gwjocuqtl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ggscpylni.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gmpdqgtwo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gcnecfokm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gyvubllcl.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gmokmtsqb.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/guhbtynrr.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/glzuvgpcf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gxsvbkqwe.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghxyflcqn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gjjpkfils.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfruoeast.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gzsjhijpu.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/grqgtozcz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gudjpfeab.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gnpwezkxj.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gdpmgxkxr.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/giexhukia.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gjrvqjzzt.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gksjyxrok.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/grpwtclms.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gacakeqek.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gyptusnxs.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gpqiiymlf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzfpuwzth.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gwkyomcob.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gthzslfiq.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gqychsbfx.sHtML


<!-- 参考信息 -->