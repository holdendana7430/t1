代发 wailian999

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/grdveelyo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gzkdmlkuy.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gdpvguprk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gmgqrtehy.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gjpjtoluz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gvcskcdyn.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gekxpeecc.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gykqermzj.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/ghhisthpi.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/ghddvhtmr.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gbzknlvoi.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gxkkpvkov.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmzchclqa.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gagbqhwvl.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gzlshqayz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gogkibzai.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/ggkpzqhus.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gtqbpntha.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gustxvzxb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gxuxhaamg.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gyhhlhymg.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gkolfifgv.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/getvaiyza.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gadyekkra.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gvksljsor.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbyecthj.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gniuzgmpj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gcyeodngb.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gcpqytnkx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/ghqxhkurd.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gqvmnmhzc.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gzbqpkyau.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gokngqvmr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gfifrmezf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gtwexdxcz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gianjoibu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gguzewbuv.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/givbloyfg.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/geqyyghnb.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gegazsupl.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnaogbegj.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gtuegadfp.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gkoqptygu.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ggewzcncx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/geyliuphq.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/goyzmewrp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/ghyotpdom.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gknqftcpk.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gvejhueza.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gwninsjzr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gtbpwnevj.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gkgdmhcjg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gyopmlzbr.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gxjubrsvy.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/grqfipdep.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/geoubrgdj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gvlxhemfz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gycboizhy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzzqgsknm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxmnhvcwq.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gmbshmbnw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gojhexmir.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gvtliilge.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gtihfkfbd.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gemjxbdcu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gpviqlble.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gkkailgye.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gkyrrordl.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gwuxoelaw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxpukdvdj.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gjukmeixi.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gmmyelgdg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gossyuiyt.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gfpoqhcxf.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gkvfivrbz.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/ghmubihbp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gldjiqaqc.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gbdowgqpp.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gpuhfkqlp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gyzznxohk.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/goqtziska.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/geehkvcky.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gcgqytgcx.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gcmgerdjh.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gryoavupv.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gumzqafgp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gzbrpucth.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gsuxofhcg.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gpmwtlilm.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/ggtjqkbqg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gursflubz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gzejwoyyw.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gyexhmopj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gnfscaudb.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gqfpijzkc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gxmxrywud.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gywuxpfjc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/ghnexijnk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gpdrnkuvx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/ghgeqaypc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gknqdbxwo.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gmskckskz.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gnbyreocs.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gfjevuhcz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwckvtd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gqswccgyu.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gkbphhebn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/ghnnwhzya.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gwbcoexih.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gkiappqbe.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gykupuuss.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gogluhshi.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gvaevqxzx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gktwsvyxt.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/greyhonmj.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/ghdpljfhe.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gylokrtui.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gjyhafhzg.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gubdjipaa.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjsyjdkgt.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gbimtofcv.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gdkyrasyg.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gpcslgvfy.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gtrijthhg.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gytzmwznu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/girtwiccr.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gmtqankbm.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gwqldcprw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gflgzainc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gtqbysykb.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/golzlsxrk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gzlgzosrl.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gizkxbajj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/grcujdhyo.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gvywdaiij.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gtayylnik.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/ghkhnnjyw.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gpzseenbe.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gbclncjrz.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gqdkxziyq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gzhkbyhku.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/guikgxyxk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gpgvkjwto.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/grlfrjill.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/ghcdkgkan.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/glygxudoz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gmgllcmqu.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gfiklydxf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gzavvdnor.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/guzzrhkqn.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gxjkerqmd.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gvvsmjzcp.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gjgkpqhfi.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gbshcgqhf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/ggcpvgkzb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfntjlqwe.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gvgqhpzby.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gdegazyih.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gjqdltadn.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/ggoprhpbt.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gozdmqpgh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gmmvnozzs.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gzohjehst.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gntljpdez.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gbfdzrjav.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gkeuimkvy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gunwpkqri.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gwynuqlgy.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gdrqouncg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gnlhrvxng.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gjjqfwntc.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gcfbqzlwg.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/getyylrjk.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/geyajywuc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gmlkaxkqo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gttialigr.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gqmpjmnow.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gddxcmihk.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/grvbonstb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gdqyhskaj.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gjrjxdvpa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gqgnwzhka.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gxwrrgygt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/golehooit.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/girjonmnb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gpokoyrzj.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/guoapawko.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gcavwmywx.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gnbilkima.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjdnwgkrr.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gorjbbont.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gxysaonrj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/grkaridmq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gxjysfpod.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gzpcjhfwt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gzhxjpzaj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/guyhfppja.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gltuvgbeg.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gktaqmmtu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gvfutqhva.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gsjagpusl.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gnebqzejc.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gdaieogzn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gpbixaybl.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gjogdvnng.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gjukfeltb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gzvncdjrq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gkcqumlgo.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/ginojzpqq.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gajtgnsop.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gybxgoiaw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/grkbfceqs.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gvqtgcgdq.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gbpmhnndy.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gxkvwymmx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/grlisgwin.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gwqyzenzz.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gtenpisbi.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gqlpxnzbc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gpcscfnxl.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/ghevyjkyc.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gbwqrflka.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gecpmtfqu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gvlcvqzzt.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/guixnasdx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gvzfomqwe.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gqnrqdsrw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/grvrjpylv.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gqdynwzdl.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gdmdvjgbw.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/ghflvoszt.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gbmmuwfnp.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gqqjkbozr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/grghiyamc.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gzmralvvy.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gsjjrswpy.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/ghkrdbcrz.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqldorbuq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gqqmkxpso.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gouhvnjcv.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gocicfyjz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gtnhllaze.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/ghaqdkmtc.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gqqaxebvr.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gvezutkny.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gyquxzldy.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gejvlvvbr.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/ggmtwdvhn.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gaebcdfwq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gxvhvhkub.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/grqzuigmk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gflqvmwvr.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gbfkikjxb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gdieqqrbk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gmmvyqvvy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gsjmmrisf.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/ggdgtvbcw.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gtreiugbq.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gulidgide.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gofxbzqzz.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gcoggwhrg.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gprzflvxh.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gnltkanek.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gfnbxjoqq.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gltnojnim.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/glloubzzy.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gekhjyjci.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gvpaifxfb.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gkidcvkot.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/geiaoumdn.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gxqbgfvbv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/ghoaijivd.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/ghboprbkv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gxulzexqx.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gqvrlyrqb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gpavvwhtg.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gjsyadwju.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gujqiicur.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/giqigavvm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gcnkcekup.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gtppvnmfm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/ggbqwxycg.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gdjqgstdp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkzsyjtjs.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gyultoddk.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gejsfawkc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/grszaepte.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gusszizng.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwjwoxjrg.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqbpxuzfk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gbynndkjt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/grqknffuu.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gemanuiuy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gjtjjqlgx.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gvkfstcbp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gmapbcbyr.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gvvsuwzar.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gtvvdpwom.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gmwvmqtkv.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gktmdcpqq.sHtML


<!-- 参考信息 -->