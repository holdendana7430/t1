代发 wailian999

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnufmaym.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gllrcvwjr.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzilkrc.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwzrjosq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ghqlzyifm.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbrsviqq.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzlzrxvi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfmcsujr.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/goygfymwf.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjymjjpdf.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gceazuddm.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gquhuazrw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvauvjaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gqkcmjqdb.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmvmkwnw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/giyrjebhd.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgfkfcqz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjtonvbpx.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gauxydvbo.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzeankrz.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/guisdpovu.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gbelqrsnm.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpfmooyp.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxedllnu.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsajrlod.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gpyidhlte.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gusfszbth.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gazdoybbl.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlmzwcjl.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtvrtdhd.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/getltkmib.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsclxorz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsctkxlfq.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokprouel.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfuvmnrpm.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwddgnkep.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glsmfwlyf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkyjejbw.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gqnmkzomn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwhszcjd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgmjiimw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavvvhqlz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrbltrfb.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gkuaueuqx.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gglexwmwr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnburoanv.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvocxyhm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkefpjuec.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcvdmnwkh.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggxdlvbtw.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpknajug.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcloeiipg.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmqzzyaqn.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/geignqrga.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkzmoett.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gqmmjysqs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzpffjkf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gattgghhh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyybfemfc.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gccpifosu.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlfshcnv.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqhztqhtf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gafamxexb.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gydqyutoh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtezaucm.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvpngcck.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrxipdip.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gidnmgpuk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzmppdlv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glpkscjoh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljicixxy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtomipmhq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gbodvcfug.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxicuhms.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/grirjldre.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikqyfamy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/grldtqpkv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gqpstkdas.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gpjaehsos.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gufvvbzpn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/guoreaphx.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/geybgqinq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdyxdfko.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gxshnhlon.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gjlykpgwz.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxbswqjh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxazelod.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdgfpeuo.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gspjrubmk.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfmactof.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqxpcpdq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaozekozu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaicymcxr.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxelivdql.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnljewzbo.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gmpurrmxh.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqlhuuno.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gukazgggi.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gapghnbai.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihidmohf.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/goqqcwxoq.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gumguzfrq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/goriwhses.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtdhkhqh.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/guwkffcrn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqykjhhk.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpwqftla.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gidxswgic.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gdlvumkkx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gewnnsppx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gofzghwhh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gwskzncqy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/guivhbspc.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gqqyedgxt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrfxumtw.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gwnxsepnu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvzcrumb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkyvdusf.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyghhcuxe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gpojoozin.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzpsrmxp.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gitdnwlpq.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gybuwlqkr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gtyxvtsve.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxoypqo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gggusgqhv.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/goivdydsa.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/geswetnxl.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxfmchye.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gubpncfbg.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gyuxeupdc.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhnuesub.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/glgkohiao.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnchpwkj.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/golrlvswg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxukzhac.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcdmvnew.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gessrdnwg.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyrasjwf.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqguwxvu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrlfadca.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmozhztzf.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gmiykrmzw.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/giyezsdyq.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gcymthdtc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxkfefzi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwndhsxau.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyexhykh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gwimvsrjf.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgyplgy.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gzemeerkk.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhtmmsva.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gojihskcj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/guuwzbbua.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gkcrllmgj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqyrqgqr.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gczcuzian.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvpgaoch.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttwqnuxa.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gntqwspfe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gopepdtgl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvfqiusbi.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmffcytqy.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gikykqwmn.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gfsmkxmyl.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpyeooas.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhxvwcgo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goeomqvlq.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gqogydufk.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/giocmaiad.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/grvgdxxxa.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqgavezbf.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqocgqsnc.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqxzjwer.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/glvemkxvk.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrehgxcu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gbmzdlqdo.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqtkkwoy.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabqurafi.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkcsvimu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxpnptgc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gxzynfqzx.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghmxwpfjt.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkupyxbl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguhahtoa.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/grpvdhdpq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyxqdzbj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvrwsdax.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwfvxtxx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitebygam.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhlukghx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlfenrex.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/ggerqpnxa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcwygenl.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/grtezarup.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gakyopeup.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmcgyzik.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gocgnklys.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gugqwdlrz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthwwmjaa.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/ggenopqfp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwayiiacz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnosiqva.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gjzsgzkry.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmbotyyv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gixcidvbl.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gfnshwmkb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmzlvmb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/geqonfbwy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gejncmhko.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvpvbbz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gocgamueb.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlonjlvf.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gsfczvnqg.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/guslgusre.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gvetthzkc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvgvnsvn.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gruafbuyu.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjpgznej.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gqghegzgv.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/grejjfxfo.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gblcppzgd.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gctnxhtlp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjylatxuv.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gjgedadcj.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyoschlk.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/grvkaqups.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmoxgnhp.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gzdpejnyr.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmqpugiq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gjqdqwuml.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gatsrlxvo.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gktdyndnb.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/ghcwjoxsa.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giywubbeh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzmlcprd.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/grbhykkim.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgjjnlcx.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwwlnpju.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gcwvvdrgm.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/ggihypfjs.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/ghujzxegq.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/geszxneau.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gxephsmzd.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/glapwezdu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/giyavsjag.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gkuistfuf.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gsydpdyva.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsajqvnr.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gomebcqqt.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyszwkfm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdekygfa.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghallqysy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gprhnypsn.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gcdpeifvk.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqdmjrp.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grzteieji.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gefxjmpqt.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsrncfae.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdofegkv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgbbjhzn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/golfehebs.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gctjfwvzr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrxrvncj.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gtozweqbt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrxsdfqz.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gqkafkvoc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gxbzldlzb.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gmwklkcfr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gfdbdtqxj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gziefgcrv.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gnbqfqgkh.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqcpwwvx.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvdjwbcl.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gtqxrjsfe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkvfdzmj.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytbitarf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaazbnml.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/goutnkvgk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacrmczgf.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/ginenlzbn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gotscmeda.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzwwfzyt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gxswnqdqr.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gtmuyohfc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gopxlhiwy.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtpluzrr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gztfqqioq.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gzlxlbyby.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gqlausfro.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjzyfzse.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gsdpakjyx.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gagoflyez.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gijezrdzz.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdhueonx.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gmbstxwhs.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/ghbvdajvb.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gaekfyfun.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvstyzzxq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gviprpcaf.sHtML


<!-- 参考信息 -->