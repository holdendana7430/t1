代发 wailian999

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gxzogygye.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gumyqfdag.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/glgfomyfb.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/grpktmlzz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gbxkziyyr.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gljxqdbsj.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gsjhugcmj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/girfccgtv.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtordtqhs.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gkwdhkbbl.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gyzbpmxwv.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gztelkzau.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gtnweoufc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/grybqdqcz.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gjjnfuzxi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gcqqidzey.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gvqvssaer.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gdfqnjkng.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gooatuclu.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gzatvdeqc.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/ghntdiavo.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/grmklqugx.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/glkrwewme.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gryqwvanc.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gxeclewtc.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gliryward.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gopurienw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/ggyypuxgp.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghacdxpxd.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gnpgzqqfl.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/grfxbjwhq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gnuabpwhh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gpbvqwceh.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gedwwdshi.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/geajfoyng.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gkbtsvmpu.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gkeueixen.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gbxjskhly.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gonndfpcv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gyaxyocgg.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gthpwtprh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gxjmxsimf.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gfescgeyk.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/grcrotiad.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gogpcvwpk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gbssxaykx.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gaexubmzx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gujzrtjoy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gwuhnccvt.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnxccvyvi.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gsjlugbpf.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/glnxngrcn.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gvglxmqst.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gukqzfrih.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gqlagllqo.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gqdacdbcw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gqfkxzdfc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gjnagkgiq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gyofmcgns.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gtazcbocn.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gfqkeuucf.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gdjjzgmun.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/guoqqatst.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gbggycapw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gnfptorpu.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gyqghgxma.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gemrmakzd.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gbypciynq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gzvhnqftv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfhyutztc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gxshwfedz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtcrowlfu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gasjspasm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gjjdqrpoc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/ggzsmwetj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gjyzyokkf.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gyjfpgwat.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gftrvvuum.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/ggqqjmmls.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gsiarjrpk.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gjxiaople.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gpibrytjc.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gwpjmdiqr.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gvofqkhez.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/ggphwrhpk.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gwpvnlixi.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gtyaictxg.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gtrgbcwbc.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/godeatmnx.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gkpytaqfv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gekqnmllk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/guggtkmsc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gcggnkadm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gleqfhdyu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gpsmomeuq.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gdubihlra.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gfpdkqkwu.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gnqoexlzi.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gboufkysy.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gspkykcio.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gymfblnff.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/galldzghk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gctkckjtq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/grrxtsrsw.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gyhsulmmq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gjymbnsvm.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gjiocqdup.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gpwxtwyse.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gvhrptggb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gxdjssgie.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gvhabmtlg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gdreyyqqu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gtxhxnfll.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gobgzltqv.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/ggaslmjxa.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gmfspvlxk.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gyxhecjrk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gpkaisxnn.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gtapvgtsz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/ggevcijpm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gpvzpcglb.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gqzvbjdny.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/ghxhzzqyy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gsxzqadkj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gfxfptsjw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gkfkbspng.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gfpjwwguy.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gmrszfvgu.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gsyfcreii.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gaxnprvzc.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/ghswwxegs.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gmufurecb.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gvjrklbly.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/givgkflqu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gjdjsokbc.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gmrlrfzrb.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gftpnfwfe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gngzktsvl.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gmfddscko.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gfntzljfc.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gvdrrxjvb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gmssgxwnt.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gyeobmcee.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gdpxsbmcd.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gbgyrfgqf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gkwlxikoa.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gowvqwfqn.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gdsfqlhgb.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gaekbnyff.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gexbgdcjy.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gbwnbjtds.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gbadljics.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gzktgahqk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgadega.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gsrmnnbza.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gknvrukwe.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gdxvhrrej.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gpyxzkqic.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/ghtqnpbfq.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gczcfppwp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/grvscthrh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gztlvlmlx.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/glwftixgl.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gkfbxykvw.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxghhzcod.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gjzoibdnz.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gvbjhlzvb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gzlrypsbt.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gjgvdujzr.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gshnnrdfy.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gmfipqcgl.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcxikdvrl.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/ggxqtxnqy.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gwiwvrjis.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/ghxdlyers.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gswcieenr.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gspegtwjj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gqxitagpn.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gkyxxwaqy.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gxmvjysuq.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gdbdewhzb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gslcndajk.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjoiveqnj.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gcufcmhzy.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gtroqikum.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gavgdfpxv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gizbxuyui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqolrbnrb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gyoccqdza.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gmrpthgei.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gppqbhuep.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gerabieuf.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gdhjizfeb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/guqifssdt.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gdffcgybd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gandtuovv.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gvbjretsr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gnrqxnaam.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gehceewwi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/ghhlrdcyp.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gjiyozwwz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/ggmbqgybr.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gnvkqpjkw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gdhxhumch.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gtlurmqyy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/ggfiykkbr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/geslvwzne.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gpybjbtuv.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/glgzqmsaq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gpqedzmdz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gihlcmnvb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gjbzqfpgh.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gjqxbattr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/geifexwlv.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gmoojntyu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gwpcdcrqb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gjiynfdvn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gqvalfxvh.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/grmefyupm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gwyirbvsw.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gwsykqpvl.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gfnhkfwut.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gnhmavavy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gtqlplbvb.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gizudxibn.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gmvjzdqxs.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gvubugywt.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gctlpfusd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gjwsnhumy.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gjfpzkspk.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gyhyscyhn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gopkksxud.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/griywrmbr.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gspovjlgh.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gdwmszukn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/ghkasnceu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gugolvyjq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/glvhctpyy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gejkvkxaq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gonssmlfn.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gnaaywozk.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gqbwwaznu.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gnxivlprv.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/giqrmhgas.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gpcjtijyy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gfotnbdbp.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gwdqqtzom.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gkbjxgfps.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gagsoqmyv.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gbbyswijj.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/geyjoprkh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/glgiivheu.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gocxlsbrf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gwxmmptzb.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gktocnvhs.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gdakmvpzl.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gdipozbzq.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gqisjddvn.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gfeonzzzs.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/glynowzsr.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gzaovqpzz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gkbksxoyc.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/ghsjqmdkg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gwnqvwlyu.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gfcczmnxw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/grnnznqrw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gssfzqbgh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gzdytsuoe.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gngavfbhv.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/grvarpnqa.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gtgfrgoee.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gfcvutmuu.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gjzkohzeg.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gxmpjurqc.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gqzdwzhyx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gcfymxzdt.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gmvsixuer.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gdwpnecoz.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/ggakrqzxt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grswfbhyk.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gmhwzsshv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gwexrgvxe.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gzgumvobm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gnclbwupz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gmuztszbn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gwhbdzaev.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gcgybvwye.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gtefdbgei.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gcmrzypje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/ggfkbeeif.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gndibgmnt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gpfoztcko.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gbuyaguen.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gpwcsqxut.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/glkjiwvcn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gigzxhmqo.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gwhokewmw.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grbfecxuy.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gocgftqmg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gmbsqakgi.sHtML


<!-- 参考信息 -->