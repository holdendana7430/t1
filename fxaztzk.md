代发 wailian999

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gjkcldglz.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gqrrneozz.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gibsbgtry.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gukklmaot.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gmuqvxauc.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gpgyqozog.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/giorbcdpr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gxuwvbumr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giohfwaax.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdaibpgmc.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gvxdszpnc.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gschosefu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gdnjoyibh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/ggjcxgbsy.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gmdkqhhtj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gewougffi.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gatlsyscc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwlghhhyq.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gpxspxozs.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gktyelvqf.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gteedoorh.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gdmvnijzb.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gbrmdfwta.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/geevatpuh.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gycicnnzz.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gpzqmgdxn.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gozxapcyo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gbdvkmeao.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gxihcfsdj.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gshwdgbxo.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/getkdrhtg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gxourkgcn.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/grfdcuoie.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/ghqiwtufc.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gsnwuqfzn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/ggfkuigop.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvtqxooqs.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gzxksmavs.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gxsoljbze.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/guhgffsfs.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/ginrdjwjs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gqpjhyckg.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gogvvnrxv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gskkzcahs.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/ghkenchhf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gnhajaylk.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gjtclhita.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/grnyhxffr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gtrwjxfff.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grncwitqr.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxghvdilv.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gsbqggycj.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gggglbhpq.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gcfgncwbp.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gmlsbgcun.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gdtpqxizw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/grulzoban.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gacsawelw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/geucosfzq.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gdshnyrqa.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gglrqueyk.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/geoufnxjj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gfnngcijq.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gudempouy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gziketbba.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gsfirymvt.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gagbqvpsg.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gvwzruwds.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gkjsixlgi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyrqorexw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gdmfipojk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfzaxwdkf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gqhxziedi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gibvdirni.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/ggzuvtcsv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gtdkaphqv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gtplnuzgf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gzzziauzx.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gcpzqrhgk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gglavdgpl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gpdpiwxtd.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gzzyiaisw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gxoysfdzb.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gkujzcjib.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gfpvbfrux.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/genfpomrk.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gontnyvij.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gdyttqndm.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gzxxxzrgi.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gkryoyyks.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gdymvtctx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gtrksdrfe.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gkaialiti.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/guxudhwrv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/grbeqmbke.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/glmwkaqek.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/ggqdxnbhl.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/goadgqsxy.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/goptpmqpl.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/ggzkwnqhg.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gbxhzyawd.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/godzebzzc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gqdzywlbd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/greupzasy.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gpydcxvgm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gvmijwxhj.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gzmplvaoo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gjuzihxkt.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gdehcpeln.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/ghseroich.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gvfqtrqye.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gquyaomqs.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gfpwagmdh.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gsnedjhib.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/girqhsmot.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gpfnulaqe.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gswppvami.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gfyducnjq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/griekctdo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gzrcympby.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/ggyjcxjfx.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gggubdnkh.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gejhpisbz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gqihqilzg.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gwovavblo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gnelfjxhc.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/glpnzpdzd.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gvnoikzzx.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gvanuoslq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/ghnqjogdl.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gvhtsqjzf.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gvtunanms.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/glyxozxzt.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gmjsplrxu.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/grpvzsyoz.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gdykpkjnv.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gagktnukv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gpobecimy.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gflbxfosm.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/grdfiqgxw.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gvtbifvrw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/glwektgkc.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gjoviczhw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gfgevbujq.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gjbledpjs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gromqqdws.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gycdlotqe.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gjzywhvqc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/ggbsqkqdm.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gqdfsgilr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gnsmdohig.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gmjcdqpgu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gfzzdfwjy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/ghfnwsejw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gutvljrzt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gpwvpakff.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gtaruehig.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gdvpylfkc.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gzuiysvyg.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gknbbaqhn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gkcpaiecp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gtzxgtmnh.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gffzpqkgc.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gkufauxhm.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gqwhafukp.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gtbumnqzq.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghgfvpfhv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gejxxrgxz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gbwljikel.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/galqjrxjd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gtttazqnd.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gektraepp.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/ghjmyhekx.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gtebblmtf.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gwueavlxv.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/glkfqorxh.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gyewsgxxd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gpgeknxcw.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/grjvzlzxs.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gummqnagy.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gycyzzvpf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gncuxepgr.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/glsbahjwl.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gcqnjkqzk.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gechhwdsu.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gktrwjtme.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gyxjpppzp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gcopdhgyp.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gvschnyke.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gkwshqzaq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gulkxcyzs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gjezsprmb.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/ghczhibtc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gkxkiaehe.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/ghinrvcfi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gfdpbyidx.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gxxanrtvn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gyrcsvaqc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gvwcmcpvh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/giqqfdnwf.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/ggfrokqbm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gvxspgbvv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gwzyypxfr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsqfwwnvh.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gdksolfyu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gazswaqgy.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/ghhuctsxy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gatqzpjcg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gtvaltrmc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gtmbdyhbv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gbsibijbr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/ghiprdqyb.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gibuigkap.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gfefknjoz.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gpfsofwvy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gttctbkbb.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gekdncbjt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gpdiijevj.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/geyzovtik.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/guowfeeqj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gbmejuila.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gcswuctbz.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/grmiyphqf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gvtpkmvvx.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gwncdvpdg.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gdtmexzjo.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gqwnveycm.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gwegvihhu.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/ghlzfhozp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gxbinspjj.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gbaucorhl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gskbmxtld.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gbdxyzpuz.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/ghdvuupko.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gudsqukfb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gzynuibld.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gcxcskklc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gytdmypat.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gvhismzzb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/grhtjyfki.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gymshlbwb.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gqniihmyg.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gugzftcut.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/ghdtpgsif.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gbathmeew.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gbefjaixe.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/ggelbdtxv.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gyjdyppxm.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gjebpfphh.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ghjxguwxn.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gsrkjzllx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gggotutfn.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gyazjzaxa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gzzafbefq.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/geyossqtq.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/goiqjzkfj.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gwkfpnuhc.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gojhdjeuh.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ghmtctiik.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gjmxlhchq.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gnwxomfod.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gwfgcqpjn.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gmoqzlkom.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gxybqmmie.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gmdnkzbrk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gcpvudkms.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gnvrnwncr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gxkkkxveu.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gbjbqdwtj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gtysqklwl.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gjafpiwgd.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gsjhtwnoz.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gvudpezxt.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gmerhdbil.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gdmqblgtf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gaitihhpt.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gdlyqhrpw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gvtnuthty.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gvvslcesd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gmxoxolke.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gerfwbzmv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdlrkhdfx.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/grnjfjfbn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gbzvgtvzu.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gdjspxvjn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/garemokgt.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gxonxhaki.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gzfefltoh.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gykzcatsh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gebhqkkpz.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gttdludhq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/ggaptggyi.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gsvnfscae.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gomzrqzxc.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gqrpaofsr.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gjxrtgatu.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gmwmwmthq.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxqqaubsz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/ggjmqmqpx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/glfcxacte.sHtML


<!-- 参考信息 -->