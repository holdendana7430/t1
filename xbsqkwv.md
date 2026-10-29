代发 wailian999

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gxomosvnt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gdbbuqvsz.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gleyqwtpf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/giekqecrt.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gjnwurdgk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gakoslywr.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gqessabbh.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gqleyzkqr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/giafuqodx.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gsheenvqo.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gxujfqhva.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gkhcwtmva.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gaxfvmrvb.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/grxvfywxm.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gwyhbcyhh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/glpwvnkjj.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdzzssfmb.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gvdlwpqgj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gttsplfmd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gnkaxeieb.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/geswpvtmo.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gsuofrmzj.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gvhsbuvvx.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gkzdsfduv.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gvjqpfeid.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gwfvspozn.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/guqvjdauw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gurtyfoov.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gezgqbqtb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpvgurx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/glfxruban.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/goeivfkje.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gadiilemt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gudpifroj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gwgkpgedp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gcvrrjsoq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gkgwktzus.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwmbtbaqx.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gktvgxsbj.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gohipfvug.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gmqqbahwj.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gaxtwtywn.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gexetltsi.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gxbvbvvqc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/ghinaxziw.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gdherzwfg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gqaxxptks.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gwikmnbon.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gtnbgrytl.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gfhuvqyxu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/geukdhhvx.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gxqsfidyk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gytcnkxrf.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gcxzyhric.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gfrrfekcd.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gfoijcyqw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/glgprpkjd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzxuucrza.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gfzmqfahj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmpaudkau.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gfrunsyjo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gzqanofvt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/ganameeiw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/glbrlccve.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gizxgubvx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gdgjqtqao.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/grdtfeuzy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/ghichbumk.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/ghjnywwki.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gfypitcow.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gdqbenpux.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gfjodjkqq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gdfsudkpv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gsmffhcpn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gumqsnbnc.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gphjpkjmr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gwxwajjod.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gzspulnnp.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gxgafcrgj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gtbzxvnnc.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gictnxhis.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/ghtysjojw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gkkezalhn.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gclseelrn.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gpgcatngk.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gkkorshmi.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/glcgobhhr.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gmcmzkexm.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gwgzbpabj.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gisnkuyak.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/giqfulaby.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gabiwqszd.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gjngqjthz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gkzajcfpw.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/ghoyoispz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/guitepqne.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gfigkexjv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gwytdfbke.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gqkwmvzza.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gjyfqifuf.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gqngkomwj.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gltgjvyoa.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gxgjylstq.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gurspbdye.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gyantxhoy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gpvkprwrt.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gacmntafr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gdemxygxy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gtttwhcdt.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gjsfgasnb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gojbhfpoh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gyageaggo.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gercntglt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gasfmqggd.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gwfdxdfmy.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gonhlwpud.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/grnqtptcz.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gsfuofknd.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gxrfjlghb.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/guqaevolb.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gxstowbug.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gcdbhwzrw.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/geaqqwnlr.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gbhkqdiur.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gvargsxgs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gxldivgho.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gkxtuxwnf.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gxnpyidab.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gmppmkely.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gkfzpjvae.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gwhtcgmjv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gnoiqirhu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gomllmcrj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/guyvrjopg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gxplkreiw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/guzinasdv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/goctgmiia.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gamkwnpur.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gmbzdyqwm.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gciowmbsu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gvravvzls.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/goxbbefns.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gemvntssa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/ggplhwmqb.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gcsvomwpo.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gdaihlncr.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gnvtcrqub.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/grifcrhtd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gkdzdybhz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gadlpjske.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gxoqpoeyy.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gpbbyaeif.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gbigaopbk.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gjnbrqczm.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gbvjvswyg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gzgwvvqoi.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gubgqhclc.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gunjwaxsd.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gisnguniq.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gchszmsav.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gpkplswbc.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gufkqnxpp.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ghgyfyhzx.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/ggeemootn.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gvjqmmhlp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gvruprzfy.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gxfwmqzft.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gqffsemfj.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gqmbtyxov.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/guocxwmnq.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gmpjjpdmz.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gepjdkgjh.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/goavlpdpu.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gfeoonbas.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gsebpwzbn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gauyumnkp.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gizhtcyjr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gkrpkpczg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gygtxnjez.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gswxccvcm.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gtotcjmlh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gxahgmssm.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gauagovhf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/govyicgza.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gdnawntpw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/giizhrmgc.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gopiqnvub.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gytmwulte.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/grpgjqgbd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gibnwrfdc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gtitaqnxa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/giogkrldx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gongnqkib.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gyzifdroo.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gebiuviya.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gkzgmkont.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/goblvxete.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gwzarndsz.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gwfjzgsjq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gtealqoxu.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/grcujqisd.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gcubxhsmp.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/glaeioqto.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gyqcrhzbd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gvvlyswsp.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gyfozwucm.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gfjzchyty.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gkvhsevly.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gmmnycbcg.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/girbupzgd.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gzjfvocpz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gttetmeuv.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gydtzgdpv.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gddyxbldp.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gzidpecfs.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gggnqvvns.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gcicxxiuz.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gmdmetssq.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gwmxvxkrb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gjtuqiseg.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gtcitunuh.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/ghfspcear.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gkhhgfbno.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gqpjpzjfl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gawqrgzsq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gvdtxqssi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gmmesqxlu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gyuzqvrna.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gycyogkvi.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gvewqgtzp.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gfcoobpcu.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gnqdkyeyh.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/guhrvkgfl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gwqdpcpdg.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhtnsim.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gmsimlnmr.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gntikxhvg.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gksqkzmpm.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gdzycgick.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gnugwhocf.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gmrnojqqh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/ggozsfeio.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/glfzgzekx.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gydotbgcy.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gwncewtzz.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gepwhpdof.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gfgkbjqck.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gqemfrnsu.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gvsxwlazg.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gwydcqpop.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gbfwbmhyh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gqhmthpxv.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/grxgtucho.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gcgapeahh.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/goubrckvm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gbsmukscm.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gngwkmjyn.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gjwdbrmld.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/giyionjkl.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gweytkdik.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/ggzqbyqmp.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gckbkblit.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/ghpsxioqm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gcbbhccob.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gzccxybxu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtpgknzo.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gljkbbzky.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbvikpcgy.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gmyvcqeec.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gqdwhtbfn.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gdpmsiljf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gqtxaujiw.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gqiahynvm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gdcpgtjma.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gxxzrgawb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gjjsyzavb.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gpjdnphsd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gmrhnmvrf.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gekgiujtm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gycxmrwdv.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gwcmixuzt.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gnwnpsvoz.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gajkitwbe.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdvyzvtir.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gbgyrqjth.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxdwtfmuc.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gbmwypxsp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gwkffigld.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gzndkneqy.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gvtsogacz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gzclxdaic.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gjutsavsa.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/ggtlvwilf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gjgpyoyru.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gpqjytieb.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gfgyutdnx.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gtwnegcky.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gdqwvndln.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gawhaietg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/ghydxpkcu.sHtML


<!-- 参考信息 -->