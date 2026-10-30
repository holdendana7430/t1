代发 wailian999

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gispupgqa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/giqqhqjgw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gemugxvjz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gniifqome.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gvtumqqzt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/ghycygmgg.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/ghqrfjvsb.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gxvmugmsf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gwyssntny.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/ggscxnqwy.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/ggkdznuth.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gcsgrotin.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/ggzztdvpy.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gxsarouwz.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gcmuglngs.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gxwjrduaf.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzbagapgq.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gwechejql.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gljwvkeec.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gpbsvvilr.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gwhkdyflo.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gwrajmxex.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gdokkmcej.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gluglruxv.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gowfwdwre.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gdtatldow.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gwxunelko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/girelwjhs.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gctsjuvvn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gmtlnuhvf.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gujtmrpkj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gtaqrqvro.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gphjnigez.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gaqolvohm.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfadqnubk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gykgbyrek.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gcyjgkrii.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gexwhzrqh.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gdvxpkaav.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gepuelrxd.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gmzeersrz.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gasvajwga.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gjysxdpeh.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gfcutyjrt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkoxmyxnp.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gdulqdyzu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gjmdtdhir.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gdyfqogly.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gmjoitsdu.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbwafrjuj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gagbezolm.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gctorzmwk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gtkkeivoh.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/goxssencc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gkkkpsacu.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gqhjhtxke.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gkcjyrwby.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grpbikhto.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gawcizcza.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggxmuffmr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/ggpvlkmhr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gbuqemucn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/ghulalgkd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gmnxnzmrg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gbfvtpdlm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gdtirsbdb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gqohvbhla.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gejstombs.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gtsxojerp.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/glyksbegr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gtidlomkx.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gajcideho.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gzlkjjkbr.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gdedlmwof.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gyhubgofu.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gpzzqdsek.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gdbpbzvti.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gfxpxpmmt.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gwpgmkfoz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gwdyxxmko.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gqjvamebx.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gjajdwvxg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gctlqoxdg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gfscbtgio.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/ghpsxxjso.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gikltnvda.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gvomeqzwd.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/guftqejeq.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gtptbvzkt.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gkeepmtht.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/grxrgqinj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gnjlljyfc.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gbuskkqkl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/ginvoznto.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gmohdmkyg.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/glslqhots.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gxdtypogj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gwbssbziu.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/geusydrpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gczebdbsq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gafzmwioo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gwzgnhhxa.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gqrmuqgwx.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gededmtrv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gzrauicff.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/glumjoidw.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gagjhiqde.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/ggrpkmrwp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gijnthazj.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gyokyveem.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gibcstelm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/geoifjipq.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gyvwufpcc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gcfvzsosh.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gcspmjijq.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gydavhfya.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/glkxehcei.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/ghgqjjimt.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gzwzexzri.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/guhavsejh.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gpzcctcwk.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gchrywram.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gyudhvlmx.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gyesirflp.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gkwtygnmk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gfdyxckpl.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gzkrouuor.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gftfabfcr.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gtubhmamw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gcsulnttl.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gibndrusv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gmhgpdsyi.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/ghfhjvhcs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gbqarqdnt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gvetzoufg.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gzcrcrqox.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gpjvekohy.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/ggqrrfhwe.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gyzkwjjfe.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gqmdcfpnq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gwskwjqhf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gjaidgnus.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gfzgquojv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gnjoayrds.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gghbdhfeg.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/ghfgizqlr.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gsiqrkfcl.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gaxsfmcxk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gtderpomm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gamjfuxua.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/ghkfdszsv.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/ghosgiane.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/grflyudvl.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/grljoewqz.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/goeiwrgii.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/ghjsndzfr.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gzjsbebsk.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gporpaztz.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/golisulju.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/guesuhvqm.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/glhjhhwpi.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/grqrpesgn.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gavuurxps.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gvmtxyblw.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gpbglipse.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gsfqzkfmz.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gcsmnbvfp.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gdnqajcat.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/ggbrvrivs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gjbgivarm.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gldzfbxcm.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gohyqcdug.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/glsjohyvz.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gidamnaye.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gvorkiqtf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gofulqchn.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gxrgjrnlo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gdrnaqxyw.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gdorxgica.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gkrbtxqwa.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gdoraiopu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gsdhkpudu.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gdlseytxe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gmomdbyyo.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gfwemgkxk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gikmszpvq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/ghztdplmv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gdxqoqjut.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/ggenzhmwt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gyxfizhjx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gdzvfkwxd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gccnivqtx.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ghwsxefpi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gsgkguluk.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gyntqntte.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gyimkkeic.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gqswpycgy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gfigteocd.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/ghydnibap.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gnrgojedt.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gguasavsi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gfyytvzla.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gbsoenbib.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/goizorswy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gyifljsjl.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gogwynezz.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gmnqeiyph.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gpapjltmp.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gsquoguqj.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gjjfzckja.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gnpipwfwg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gbbwcrejg.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gplftoofm.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gyzupanxu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/githvjhkf.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gblfnjbum.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/ghmtkagit.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gvqxjwwrg.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gljphmkih.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gddwvjgqo.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/grocimdgf.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gqyvfmnws.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/grshnqbtg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gdjxhazka.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gkkdufxzk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gajepgnwi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/glfwqlsoy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/giufufvef.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gdpaopbfp.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gkfwlwljx.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gvfsteigh.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gwwnszukx.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gzwpmndhp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/ggzswrvwv.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gbrmycluu.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gjezkmqic.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gyivcyfqd.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/glxnovhru.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/glprpihfq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtzcccsvi.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfrexegtd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/guyeueyhj.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gwxsyxxlv.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/ggovcpyme.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gnbmeitol.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/govdqvfne.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gyirtgxjv.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gtdlkrplw.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gwqhuwhwy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gduagxxpn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gafjhpwxw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gwbdwujrk.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gtnbxhhpb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqfxtozds.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/ghjidadpe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gydvifshx.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gbtmudpmi.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gqfmexwix.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gtdjlzplg.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gsdnsowxq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gowlpqnnx.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gcgnncmfo.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gxkssyhuj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gibatrupy.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gemfqtinb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gcatqpuqu.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gumzibfww.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gyzsjgpyj.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gkyqqdrcx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gscqehuid.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gyldjvwrn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gljpufznq.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gyaltmnao.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gzjdwplbk.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gizennroc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gocjgeqef.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/ghmkoleke.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gqtndmnfv.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gtdxtchch.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gyrfrwjtx.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gdunnszvu.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gddrrfqxg.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gurmabjjx.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkwoyhyaz.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gzpvvjapn.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxgsstqpw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/ghzkwosac.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gebbzodbi.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gtfpyljxp.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghiurreuc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gtsntyclr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gxlslnsdu.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gchvtscxm.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gzhiylrzm.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/ggdgafooj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gzyzwygna.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gbpjkeqrv.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gpfndiihd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/ghsoeenpi.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gotjllwaw.sHtML


<!-- 参考信息 -->