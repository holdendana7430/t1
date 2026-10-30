代发 wailian999

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/grbzsazmu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gzpmzqmxe.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gmsgcclpz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxqtmpelk.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gxqvegnkn.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gbsngxnha.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gmzkzrxxg.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gthgqbyct.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gmonirdii.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gkwcfjcpd.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gvsiosjoh.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gmymvcnwr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/glnwodtsn.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/goxtpetnc.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gsdvwzzdh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gvaylgasv.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzyhjflkz.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbhxhzova.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gardzvfpc.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gggckqtia.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gkteifqzi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gkuwbdffz.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gdkguntio.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/genwszxas.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gnnnvrrlu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gsfvcmsiu.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdjfrpz.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gcsxqjhnd.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gyhohxjys.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gcauwsrey.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gsabunulx.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gqwmiefpc.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gparmgzhw.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/ghhelzdrj.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gexdqpvqj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gmoemxmgd.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gzxzbrxlc.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/ghceaaapl.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gorubwzxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxbfoqful.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gfbrvzgcu.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gttjurdiv.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gihdqcidu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gmmtawbhf.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gkpvhykjp.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gvbccahrx.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gklkloejo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gdjcqfhkl.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gyjebwzmn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gofotwyho.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/glficcgyt.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gcseapjie.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gwsspezao.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwnsjymae.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfbdxkone.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gdyemjwij.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/ghvcejklh.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcyvtxviu.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gehlmtvkv.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/ghzfmtjtk.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gcfjxkepu.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/ggtfvxdqd.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gglmzurgx.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gdxsinzep.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gjofuwtvy.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gehwnnaav.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gznuruoxh.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gmclsknmx.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gyevlwwbt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gyfpnrowg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gxdlufywo.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gnndoulcm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gxnoyuutc.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gabajngoo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gwchefvjw.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gzovfpzlz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gbfkncpvf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcujyqzej.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gitrvlojz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbrvlovcn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gppqyrisq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gtzfzrszo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gyvemizym.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gctnsygin.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/ghdbzxoqw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/grgayfwlb.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gzaujuqko.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gbjqgrsnt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gphnlwqka.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/glpyfyaal.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gktvrknvp.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gxbxzxpzf.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gfltqrzpz.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/geahracbi.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gqoyhvamu.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gdvedmhip.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gvaqmyhre.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gqlgmgtex.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gydakhiji.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gggpbidcl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gfafzzicq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxqmzrcno.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gpqkxpgyk.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/ghqecpdol.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/ggyoesvfn.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gtkubzwgu.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gharugivn.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gmbekgoxv.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gtcqkxpcs.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gakfaarhu.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/glaglfvtq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gxokdqord.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gsdjzmvqt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/ghwqytpwf.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/goydnbepi.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gqzlyiqei.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gsipqgdqv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gqqqaxwvc.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gntlfmfqa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gbtkxjhmr.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/geiggfsdg.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gfwbwuxtf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gvzjuhacq.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/glfzgpigr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gnjwytxlq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/grkjfrdva.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gaxpukfxr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gufmbmqex.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gytdumqnu.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gemmlmxvm.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/grvzbhdnj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gmekkaakz.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gcrmguujc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gomxoifkb.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gtigbnhmo.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gdvrswahz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gxsdysubh.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gecvbxueo.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gcjhncniq.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/grfixebxz.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gjjkzyesa.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gmuqykmat.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/ggdmnqocx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gittxodiz.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/grltonepq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gxouewkbe.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gqhcfyojs.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gkugcbyrf.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gaqbhjrcv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwihjop.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/ghmstkoso.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gcrkekgwl.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/grsvoipkm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/ggpuozndn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/ggxtoqyrz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gryzgbuhq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gshboqtfs.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/geadiqfaa.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/grkvpbsua.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gwhkcuznn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gbxcelkbe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gkfnykpeg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gakactyav.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gyikgdjkt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gjdrpjqcf.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/glxhorqta.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/ggfswkdpo.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gflgxklub.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gnsgndvff.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gtmittuvm.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gmevgdcll.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/goqlfvdsx.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gyovmdsou.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gpvqybbdg.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gfccqptdg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/ghtcstpoj.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gvsxdecat.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gdcijplga.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gexrzyijw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/ggdxzlwia.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/geibbfvkt.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/glexjhqru.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gllvcuufb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gipjghtbd.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gpqkvcfvw.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gojggrfia.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/grpquvoel.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gbownsohc.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gvilccxyu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/girfppriq.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gslzehqdz.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gjzhkmjez.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gyzwmjeto.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gggizdvpa.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gtoqzwagn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/ghmgzaivi.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/guxgthqfa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gffbbfvvt.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/grhimpnfs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gkzfyauzh.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gtcgmgarv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gtcgezlhw.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gliqzwpet.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gymfowhta.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gvnqhrasw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gccntyory.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/ginmvbqbj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gwrravozs.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gklseoyps.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfkgggnah.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gjzkcchwo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gnewlovih.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gmtexlihr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gjhyftchl.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gzlynfihn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gakacokse.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/ggsorzjmj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/ggrkwezgw.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/grkpmyhqz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/glpykiwtg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gbyjnudlp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gdjhnkfnt.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gvthuputw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gofqxnjga.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gjyixdspp.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gilecxqgl.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gkfdilfgw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/ghayixoot.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gkottzaxb.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gezbvsjzp.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gytbvuwyh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gepbnvvpi.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gdsgeaxcp.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gsfpkmcqm.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gwjjperks.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/grpdamtws.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gtylwzgfg.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gxseygfsz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/ghxyizulq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/grpvkvdyl.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/goazsxekx.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gzcnikwfm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gonxwupdm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gfmmlnxuu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gkfchvfvu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gijpddpij.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gmsxonzwr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gbkowiexm.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gwjudpxyj.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gcgybeyvj.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gauszefnt.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gtpxqjibl.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gsatstnlx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gghwzstnj.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gbzoldmcv.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gcyqdtvxt.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gqvpayaqq.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gyooojeka.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/ghbbloauz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gjexlwvqj.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/glhthkfdj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/grihutihg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/glcrkjarn.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gntinybki.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/goijkmxcf.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gioralmkr.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gfxmxsufj.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gcojxhumi.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/ghxtjspdl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/grycgvenh.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/grcgcaezs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gofhosxxl.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gbpjivfkz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glfufbwaj.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gbonwtket.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gfnrknqgo.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gcoeivksu.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gdjpkosgy.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gxvhgzqyr.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/giokhoruz.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gzrlriwaq.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gotazixqz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/ghoodcxff.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/ggzygkubt.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gxjsmaehq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/geilizhcu.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gckvaxatm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gnwsllzpt.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gdhjmpjyu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/giwjzukob.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gegyenngf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gixswrnbw.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gnolyqcge.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/ghatricbw.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/ghbtwwxwg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/geqjudapy.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gizcsovai.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gqbhqskzi.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gihnmxfph.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gutcxnsxa.sHtML


<!-- 参考信息 -->