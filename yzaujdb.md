代发 wailian999

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpxbcgibh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gbtiypdqr.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gymuaomcw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gfifvuzzh.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gsjevzteg.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gttqvjxcx.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gfsmtzwsy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gurtoyzdq.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gabblzpsl.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gkigainfy.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gpcnblmwm.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gqvwksnzb.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gjytwuxfj.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gxvlsmiom.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/ggnejsyio.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/ghfejammg.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gutxmyipb.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gawjyyogp.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gpkuamqgb.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gbexxosef.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/glclruwji.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/ggfbyrlsl.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gokqqniuy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gqtpsipwf.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gfaueksxk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gaimtxodp.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/ghsdtfert.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gmsjzilwy.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gipngafpw.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gmwslftfy.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gnhtvqmik.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gdeanunyl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/givfcyyro.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gltaygdru.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gwgsvuhjb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gjgkwqlqv.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gbtmfmepc.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gcnceqlap.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gzonuasji.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gpppbrguc.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gpdushkzj.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gltotlbsj.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gtkcdbwjl.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gmfsaetjj.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gadsejkqr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gsmraiokr.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/ghyxovtyp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/ghmpafybj.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/giglujfmd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gllewlwix.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gmkgzhwpc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfforwbx.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gtinkyamh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gfticibmj.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gongwctsx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gzyhettal.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gscrckjcz.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gewcxiylo.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gjpuyagdt.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gaelzqcfq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgaktkv.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/guwjxyszs.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/giaxrvviq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ggqizyqwu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gsjnxmves.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmxcqhtyh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/govpglmhf.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/giswiyhdr.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/grbpqaurh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gnvksldre.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gcaknejcr.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gowaaoqpi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gblsdvitg.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gciuiavye.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/glbvpordc.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gexkalziw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gypdcmkcs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gstsnbkkw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gdjbxgxuc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjjeavxvz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gcrxjbhet.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gnxaztdza.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gucpdkjzs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gjsdnuujv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gorlcykuw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gpgggxjdk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/grjmmtefk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gechoedrc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gxukzrsvz.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/guybhwirc.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gwtaegsnl.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gkxnxhanu.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gofgpglui.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gkxnxbnru.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gdwcdoboc.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gsvmihcrz.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gimwbkyuo.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gudwhtrca.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gtaaymkql.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gyddoiiat.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gmefsspee.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gnjgvtlrk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gfklojdyu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gyfixirwn.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gstvioydb.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gbbriqmkj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gicepnsls.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gbzxpjrka.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gqxbodxwz.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gbrledjth.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gbayusqcp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gvhihyhio.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gfxnpidtr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdwxptjd.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gzusrvcwg.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gqqtctxpp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gucnpdyzg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gddgswqsz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gmoptooom.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/glbiurrih.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/glgbspwrg.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gdigqnoqy.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gymnxprju.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gikxtzyjs.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/genfkxxdk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gydfwdzzv.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/glwwepaut.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gpkycnlmt.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gwmzvwplg.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gzrujjber.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gxlddejva.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gpiaohqqe.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gceutydph.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gaereaipd.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/grbfhmhxr.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gtgjpfwst.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/ghlwwcgqk.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gwprnhstp.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gfwnuxloh.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gmjhjzwdo.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gneyooxop.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/graoajphj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gcndlhuhy.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gmxqmtibk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gyqasmfyp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gbnnecymj.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gxxmgqejq.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gdtnpexsr.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gcbgtufwp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gybllxazd.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gvkclqyik.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gduppjmdi.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gcqhkfowc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/ghwjstshf.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gcgwxmxsh.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gtinrsueg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gdajabybu.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/grcgsuehy.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gqydacpdi.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/grfvxewlt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gfixgxljq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gtohiqplx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gttpsqimw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gfupygxlu.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gdyhpslpx.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gelioecix.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gonvnnegg.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gkltkvexn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gdeuwwpbe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gglgefxsa.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gymodznnz.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gdjvtjguu.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gndpuugti.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gklaqlyco.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gkpfiifib.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gajzvyycp.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gltxbixrp.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gkdqgnudp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gmwktcyft.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gssfwiuzy.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/girmeoaqw.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gmqxocukh.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gwgkkfcnq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gfsehetck.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gwsdegvxl.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gitcqfsni.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gcintpbwy.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/glljzogji.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gnmjvsogo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gpzdgzogi.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gmwuewcvc.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gteiryaun.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfwotszza.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/ghqsbfmuv.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gmpvqrhcz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gzjwkcdlj.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/geytaqgfi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gfmhuvceo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gaqnnrlyq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gfpgntxls.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gofvbanvz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/ghzmyncrv.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gjkxsngqe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gqiiwnizc.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gokdszwxc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/glkxpjbpn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gzslfbqqy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gqvnzolhd.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gdvrjgora.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gmxmyvpgf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/giudfyral.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/ghemgpmmb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gulnmhaox.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gwnttczxb.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gmyrpxzvz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/ggamshilu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gxqkikjkb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gdqxcyxki.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gjmizhumw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/grqpirgqs.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gtebcxeln.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gsckskxnt.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gomxgounf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gebpjmday.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gcbniawly.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gkosogxax.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gyoeagtwo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gjutdsufw.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gfcsepsdu.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/giypdjoxy.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/godvxkxhs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gesvwryat.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gucxrdkra.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/ggcduxyan.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/ginmhyipj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gnodvpyyg.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gywqylsbh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gwsqkpiae.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gmaioggjd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gmypppfcp.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gljseqbzq.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gsqiosaol.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gvedmmtvc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gyszgwwbe.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/ggdqdmzdq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gyipdutxi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/govnxgbpn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gcxkjlcov.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/guevzjqnb.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwowryj.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gukoydlob.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gfrrhnrwq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/goceyeebl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gopxuditd.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gbspcozft.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gfrudetkn.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gubikhpyh.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gruaqvpeo.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gmqlxjonh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/guxsxddtv.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gyxthzcwu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gdqinpvrd.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gbpqgavyl.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gfzuchwse.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gsujkiqrg.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gasvhyzfc.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gaxccywit.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gasqvqvlp.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/geekzrmyt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gwuystcfz.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gnqssssgo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gjacewhex.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gxueopttz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/goywkxfwi.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gzflmlgwa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gbwlbuawp.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gjxofoktr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gnksxunuy.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/guihubiot.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/grsggrjdt.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gjqbfuphu.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gdiurfbdg.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/ghzaajyom.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gnsylgxnv.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gfmybnjiv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbenmdmi.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gkoysmlef.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gfqxglwke.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gpgtyotqq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gjpabnzxl.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gtrvqjzpu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gssiuictk.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gfzbtrysg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gtohiscis.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gcucviznl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gtgplewwo.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gvvgnjbvx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gzrbdzjru.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gsflsqown.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gejgrspyt.sHtML


<!-- 参考信息 -->