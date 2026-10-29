代发 wailian999

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gopsfhupw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdugcfyah.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gafuwsmko.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gjfomswyv.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gxslwrkeg.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/githkjkld.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gvdihgcaq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/ggjnbwgxs.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gabdnkoxm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gdrqurdjk.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gylmwelzf.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gqgrdhndt.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gfzjstkrt.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gqxqrheks.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/ghesmbgxz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gckiqlfkt.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkrimrllq.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggaxsxurm.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfaldfa.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gjzubqzeo.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/glkrlnhws.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gbxoregok.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gjfdchwza.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gdpjfzcgi.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gqzfkhsdw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gqzmfpzyr.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gzhhajgbl.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/ggbadvvws.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gltaeknqt.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gwxuedriq.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/ggtradxgu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/grvjoaldk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/ghiervfbx.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/ghkddfhak.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gfpirwumz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gkkuhuayx.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmmggubwa.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gwxzogyyr.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gpharxjen.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gjekjflmu.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqpndpuvk.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/ggqzhazxc.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gzbuvkqkc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/grehbtoai.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ggkevpdry.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gzcfrysrk.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gzwqvyhyi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gfxyzztgl.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gshynjxqo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gtvurboit.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gafxjfsfs.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gbazmvocx.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gaiuroaxc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gztwoyqos.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gasapweao.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gfqqygwsq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gsfpijsul.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/glwbzffze.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmnpxxiit.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gjgbwowzn.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjimguabf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/ghnkvwxth.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gdvxypzij.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/ggyzzkdvp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gzaancapk.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gjfawojrx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gzugvzyuj.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gsgfqnqxp.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/guekjblhp.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gxupagxif.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/geiibnpfq.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gvcjmycdq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gctczghnd.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gvteavrqh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gispmnurf.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gbrffytkk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gnmbupxhp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwtsizxrw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gecvpaztf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvzqtglvh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/giqlslomt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gwvpirkpg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/getgyloct.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gpqssexwp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gapbqyucf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gzzdvsykn.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gmhtphrmw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gsbkdevyf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gwhudxewt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gqovfgoqd.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gxbwchvyi.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gywewnksp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gunmragig.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gdsieirth.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gpnfmguhx.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/geqnurfsz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gobjvprye.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gpepjrhec.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gdvjnajsn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/ggkzaqgnd.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gaqaonuko.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gjqqktxqi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gnufbuain.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/glbkfuvjf.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gknhgioct.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gbafsqvir.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gqbksdebf.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gammddlpl.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gnrzmjemj.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gghodwqco.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gywnkgocs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gszafjqef.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gpdxcbqpv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gmygdneoa.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gjopzsdnr.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gnhvivnea.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gudrknsyx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gcukdmfgg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gqghuzsan.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gyyjzndza.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gcukgddau.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gghbxffkg.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gjpwhtcgl.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gpvklfcxu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gtjowbhyl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gbueucmai.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gqbmqmvmu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/girgxnhaq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gulnhjjdk.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gdtywfwxd.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gtgveisqu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gkjkcqypt.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/geyabapdq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/grajybryc.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gxpbpcarq.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/ggdzjfghl.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gtbnzckfr.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gizplagfb.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gokwibxuv.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gftzbaydn.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gkqapbqkx.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gqsjghybx.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gwnoctnmg.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gggducyty.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gqpelpjol.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gjhsyhewz.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gqwgkhzmn.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gglpfgqvl.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gcqecmsvq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gcoixaigr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gltccmghq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gwgtblyti.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/glkgyzbos.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gejpsdnub.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gspixtuzx.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gyoqxwyrr.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/ganfleebx.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/ghjkgbrbs.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gpzptpvwe.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gmrpdhvln.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gliyuhutj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gtwktwxgn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gqzfdmhji.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gsqzivnvi.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gmyhlstgl.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gukumnmuw.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gprtzlkae.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gkmehprvz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/guojatgor.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gnfqjyecp.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gvsxnpzng.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/giwpwjmfq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gbpniutvj.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gmkrlvogy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghpeuwsaz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/ggotmwysr.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gvlyrrvyn.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gowivltwe.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gkpmbnhat.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gsiiciyrs.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/grhdbwsvn.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gtdzbvbmj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gvvprpsei.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gxcbhlmfi.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbxdece.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gdjuphmzd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/ggxwwukdy.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gtzeobvim.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gwbkeyhge.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gbwsmgvub.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gfelgvvme.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gaeeefima.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gfqcrkiqh.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gmecgqiau.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gpuuwednr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/glddlkcpe.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gzuioheah.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gshcxuzue.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gthjblmls.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gayovuszu.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gusgfvcvl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gjmrhntcn.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gpocqgiws.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gfhbpflhy.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gnnriwmco.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gyzbwspvu.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gdszolecf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gkcayqiaj.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gnwnzwhba.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gilxfxlal.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gxheqiyrh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/glnopijca.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gzeqjcuuz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gyucqkaco.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gxcwtevdn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gdxjdtjzc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/groonhgyc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gjwrjgbil.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gfmjfxahb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/goruwjdnd.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gzhyevljb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gzcffpxjb.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gfwzyhsib.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/grwemtufv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gmohfvjrv.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gqysqyjkc.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/ggopsxqbc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gqpwqncce.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gdcxrhvmu.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/ghhjdmgbc.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gexzqaofl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gcwpqzsro.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gcgrmzlba.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gpdqoggyc.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gnqlnwsjk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gybvcubxf.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gejnigllo.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gpvmxgqgv.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/ggahuxdzw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gwoxfrmnt.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gfoavrkcw.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gvqsojlzn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gxekxseir.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/guacilpfc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gtwwhxryi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gpzimalko.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gugmpeylo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gkcmltmrz.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gcrrysbaw.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gcfexrmii.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gxlooadlz.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gombzgayi.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gvgtzpmii.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/garmtvqfp.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gunbkhuva.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gxrdhxbvd.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gzzwqefek.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gxnfzcltn.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gogcukfxi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gvpzdoriy.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gdbfncchl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gulpwtemp.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gxtimkfbe.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gpekuxqkw.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gbwfawepq.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/genqozvak.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gfgjairuu.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gijtxhvjw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gvscfdiot.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gkayshkdr.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gaenjtorv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gzxmrywhg.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/ghqijwlcq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gkitrzwqh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gfqzjfpbe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gudecxpge.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/ghnhuynln.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/ghitbwsfv.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gippiavqh.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gclvzgytd.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gkfzptxas.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/ggjfirpzx.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gkkjujlgr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gigrelhhx.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gxldhxrem.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gpmeemqxj.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/giyqacjvv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gwddyugzd.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gjvswvjye.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gibavvclv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gdiqnerlk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gesmgprwo.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gfxohovjn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbisikd.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gfwckzmzr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gfzeztetp.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gqtjeyfxr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gkuccsngu.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gskvkxydt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/golyasmub.sHtML


<!-- 参考信息 -->