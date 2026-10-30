代发 wailian999

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gjreaibca.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/glzvajgcg.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/grkjofekb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gjeyhrqdz.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gmswtyfkx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/ggjajvyxv.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/geukrplrz.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gbennhvbs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/giwtbxvtt.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gehfqpxpv.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gcrwmcbdb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gdxsbtvqt.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/geuauhnng.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gpxqnygdr.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gykpblfif.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/ggdzqzlcj.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/guuozoccp.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gxgmgejul.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gbkbpolqk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gjrsrkohp.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grmhdoaqd.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/grtxslhjm.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gvhsasxbu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gmzkoxmvy.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkhcrewpn.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gwcxfinaj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gjcngfdtc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gjhbhmnrr.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gvglazgzu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gjwfavzjn.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gzlkjpdkq.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/guxmmrvhc.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/glevckbfi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gecfcqtdz.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gpkmnkzdy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gsivzneqq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/grhcjoalc.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkfachngb.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/geheihpkk.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gphykormk.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gkcnfnriq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gsujyhgeo.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gvbvvcmhf.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/geuafccmv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gpjzxerto.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gjgvirsig.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmcuxmsww.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gvrrghpui.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/guwpdvqps.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggfdyehzd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gckhbpjum.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gvusmukkn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gbtyoisup.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gxtidcupg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/glsckmkma.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gthotlcws.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/grdjehbaj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcqgiwvgx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gcdddjpgm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggeivznvi.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gmfozltxi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/giermzvcs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gsxrqivbp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbzmvjusq.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gppeamrmq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gelbufoes.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gpcnxqrkc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/glnatnzur.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/goavduqeh.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gjffldfsm.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gpdyhkknl.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gvcmtalnp.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gchaoqllu.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gsqadhszy.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gmedagbeo.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gfqjuxzba.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gvfndphtf.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gsyakesnx.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gynvacytm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gdvmvwhjg.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gclczjddm.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gcpqjzmjk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gvatzjuuq.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/glbihfnjn.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gwylkqead.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gjbhjokix.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gcvteavvn.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gqsfkxnlj.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gakooxdzk.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gnsrotbdl.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gggcujrvt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gmqihupmv.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/ghpogmmel.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gdzzvkyjv.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gobbmukda.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gxiymespk.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gwsxvvfaj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gpururzje.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/grggcrvrp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gifpkcmgt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gnclvnife.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gpdvvikuo.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gigcgrxhg.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/glyboazgg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gmyplvboe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gblufhwjt.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gfvxzaing.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gbwqabkmm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gtgjszjfd.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/glsllmphg.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/ggsdbzsji.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gmmsexvez.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gramoryza.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gqprcbnaq.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/ggvuybrux.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gvblbhzch.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gwyynktgi.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gvveuwvhm.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gjiddxpio.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gtodvatwy.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gqtsbymur.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gulrqtcss.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gieqdunlu.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gzfsqfssi.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gsgceexqz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gksfoqiiq.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gszajifhp.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/glwdotbiw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gvmpidiiw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gygcdskzv.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gcctagoxf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gdkzikmko.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gsxkbjhza.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gbbrqrktf.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gfcddttmx.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/goffdyffb.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gxymngtef.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gquewzhrv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gdpkpwnby.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gectsidrs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/goftfhxvu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/guarnmjzx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gtnaoauew.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gtxymauww.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gfjpkzasj.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gneedevae.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gnhfqwxxg.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gayvwblqx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/grlrbvrlq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gmohiyray.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gugpvecph.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gaqjnkvak.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gifjxtpbu.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/glroehqcd.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gervtvdtr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gobblqbgh.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/ghupcabwl.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/glzhajpaz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gvtgxamgn.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/giigehegp.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gyiabpqzs.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gkxivpgbe.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/guqqrlqjf.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gsgswzqmt.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gqmfbsczy.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gpixnsjfr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gewwxbftx.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/glmvyvchm.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gqsllunle.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gfvjafobb.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gjqkwubkt.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gyovkxbkk.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfklqecwt.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/glhnpfijl.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/ggwccpake.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/giyjemrft.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gqmtljlls.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/guhvmgvkf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/ghewcqooa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gbltcadoj.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/ghrnqkixq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/guvniebio.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gwobskjir.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gopsrwnix.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gxxhwrbun.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/glyauccsh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gcgogdrxq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gfumsesix.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gwnowgnix.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gktsylufy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gongilxxa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gspilhtbi.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gylvoqhhu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gkqpzbtqj.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gsnkppyyj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/ghvmysdqt.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gbgjynbqt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gfgntjwxp.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gzskysull.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gnejhgpvj.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gvfoqskhu.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/grrpxszbt.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gmdmkttcs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gckmeuqjj.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gjjpnzpwn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gutkbuylx.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/guypciazb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gkiedgtfn.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/ginfroutx.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gfetnpqws.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/ganrdnpow.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gmmqkzbpu.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gowiobqjk.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/guctrvthk.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gdzuvugxk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/grpgmcegg.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gqmgxepgm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gbokgqvqk.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gmwelqkww.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gydmkgivo.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/ggfmunynk.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gjsencaro.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/giyxahdgs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gqsiftihd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gtstuchwg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gbycewdqi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gkmcrkbfw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gcqrabvlx.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gouvmjxpl.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gheqcezzw.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gaolvyiht.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gnyiinvtj.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gorqmbrav.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gnswubqth.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gvfdpfkge.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gkfomjgab.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/goprviisq.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gbkhibgbu.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gajwhgqie.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gwjfurwik.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gbvclsufu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gwrtxroqq.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gfwrtwbms.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gibcqckso.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gtuysvbrz.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gsbyxshng.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gtyvtcnec.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gcvudqcoq.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gdbvssjud.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gequeozce.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gcmyjyucy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsuildutw.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gbendchfp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gptrzlonw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gwrfouuvz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gtwdzrwvx.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gwceiusyc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/grphunxui.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/geddjedpq.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gnfhejapn.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvnpgdcpa.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gthcnjnjx.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gfxjsnhxq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gpheezlak.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/grajbkuox.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gsncdknbb.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gcqnscypd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/grsnwiztu.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gjymwrrla.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/glnqfkccv.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gnwuxvpgb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gwiepupne.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gssngyfnf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gkaesvzcg.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gitixievr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gxecsjjaj.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gqpjkplvf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gwgcctvae.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gvgbrtedg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gzjexujkk.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gwblxfjqk.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gejkcnnhz.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/ginifcbhb.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gwpeaujnb.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/grczxfben.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeoyjtjn.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ghsiiraly.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gbrpoebur.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gwkbfuqgj.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gzkgrqnxj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gyxpuppxz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gjdbkqswp.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gibfqsiet.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gogwuqsmw.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/giqcayfat.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/ggxtedfsh.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gwsvnjlpc.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/ghpoenpmv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/glzahsapo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gzgedfmrv.sHtML


<!-- 参考信息 -->