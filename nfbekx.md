代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jnsqboou.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tagzfqet.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oeqmrtet.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pnmwcuyt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2debpiwox.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2igwdnjen.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jkojxqeh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2rszhpfcx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lhsfuxts.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zkiwaxyt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kqltzaru.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2azmaduqv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2atcdylcu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qynonvzf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kbpadxot.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hzpyqrrr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2uwsesvtl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yrpbnycs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2inwhfabf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ozqnqbdm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ehyprtfb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhrrkel.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qnzibfni.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2aofxecab.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cdijokcl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lywqyzts.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2btkztypa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vbjlotvn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cvykyuja.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2marnrdcg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rbowniex.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xqnjsxkb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2isfggbwh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gbjprkee.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bbmehbvg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yiehdtfg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gmpgkfgh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2easjlbtd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhvdygjy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ynliolys.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fjwyomyl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2slefnogj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2akdsvupf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pyowuiuh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2izgwypty.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hfhjsmjp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vtfgfsxq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gesqnwhm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wgscfnjy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mcgfmdmm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxzhvjtj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qzoaseav.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vkjicorb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hqolphxc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ncxhsqcz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ibbbovtn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tftujoty.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ykgvlpek.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pzngifpo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hwjlpofn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ovqbkxik.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oknlmwec.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2uiifzxml.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2masrmkea.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtgmgjgy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mwzqrugs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2apskouad.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vpydxnfc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dbsfapto.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2utxjeegs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2evpnspqs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vovgxdhx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xlznzepb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fosggjow.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pruyptrm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nqcfgggl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2eshzgnbf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fjrvyqdt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2pxtfzlvw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2isnquxtq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2adiheuta.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gpxjegmo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pggfbfxp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pwbylksb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ujxczdew.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xglfirsk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kcpezuqf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2eazjzkyr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wruwtvvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltumiart.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xfiazmqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oaqcnumy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2sylgfmyz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fcxjpwpk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dqxdhzah.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wafajjtq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2syixzmis.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ggihlssm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rvytazni.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2trbmhkco.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qkjodxhy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sdjsyxkt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2thpuezqx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lwordtsg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2koewtcez.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2czckqvzx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jplbfbbd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dcqwrcco.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2cqdxhomj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrzyszb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nsxxhoor.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2firngpss.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gyrakcrm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwqbxckr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cegndhzm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcenauo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2lmnhgpmr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xrzasxcn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2apgrthir.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pavlibdr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qsbhjisb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2uwepxzdv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fvzhsqtv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mlgdnhtp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ckdjbjgn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vuopdmmn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dlcaofce.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2utslztet.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2omflxgfr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2eoznsjzw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pofdmtfa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2njfwjdey.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ooohyaik.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xqloelpg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tzxzxuqy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qjwnezlh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2sgeknwog.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uynmnrzj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qvkqteya.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2utngdtes.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yphblsdp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gbtmdird.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hehdtawh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pinvdsbw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2skzwwevn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2czrpcvpi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mgmhpniv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ztbiuatl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lllclnkc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vmzlziwr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fczpifwv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vwueyfrr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jfzrtnld.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kefdenfl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tekwilwv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2kzwbaoyf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2vkjmzxys.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2oilzebqf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2usgzfrbo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2chpusduv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ewnrjjxm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lqrotdic.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2foldwcue.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhpxkwn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bspqmfxe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rhcnfztt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cycynqng.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ripgbjgj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ymjoedix.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2abyorcuj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ikhcuxyk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2viblexbm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wmnlrijn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fgirffhr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2trlzviac.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2crinjtvw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2txijexzu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wjtszsnj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hapgiaek.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xbkjluja.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gyyqdnse.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oayrukjn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ttkkmxfa.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2onttvcuz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2gdlnewke.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iftmhpgb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2omvurxpm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ddpwwrfa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xnwbmvvp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2fzqtbjcu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zvysjywc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcfqznno.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zazevjbg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2csqypfab.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nzgtzxaa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rxrbqbvn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2itoxndhv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2elbioyyv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2pynfurxp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2klpudxep.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2oihdmaur.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ietjpgtl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mjonqblw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tboczgqg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pcirbaxu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpvasjop.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uqardskv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2drveuinb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ikirpslw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pkzzgzji.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tcehulab.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fodbvaet.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2oghfzcmy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxouekeo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xmenssmj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2irwdxiiw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bocdhiar.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2rqlmukww.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kjhllqct.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2uqabprqk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2iaqxtxew.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fvovuilc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qsvdzdlm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fqcncocb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ddkxcgcj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pszdlduf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wkzwgbqs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ojcbauuq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjqmls.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rnskvher.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hujwxvnl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mhmkgpiq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hwxdjwwa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hcgztjgn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ndukkqcp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vhdmmfrb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2amelgniz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvcysqi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmltzmkr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ppsfdyir.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2zjxrbbwx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ynnfqqme.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2siiiapjo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dcrpjotm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2wkqvzrxu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2axbgsjdw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xxeicahw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ebihavyp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rawmemph.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mtgrxnvi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zplgnvet.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ztwfxzdz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wcivfogj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vjyhsvdy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bfpmycrg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qmpnosjg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yuwdsxoa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mmghrtft.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ijvcchzh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qebfwljl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2abgrmrif.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bjlwyais.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dcxcqwrq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2znjprznq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fjbodqdr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bkwzyucr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wapohbfc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jekofmlq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ladkzsqn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ifcgkqzq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjekmpsn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjvvkbj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ralbqrks.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tsyjxaph.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2phpbncle.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kjegtwbr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2affcddeb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2abcmbzvy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2unwklocg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qnwvicka.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2teklqvhk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2sraulfhx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2guggsblv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bilvoacr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2edoscsdo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eqtofery.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dyjcxmbm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2yvvaezeu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zgloufzx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zenrshmh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lnwpoaok.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2emyncwhx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2savpkaff.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qlrqctjt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2wpdioshs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gvgaeiat.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ibiypcxs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2akusmqbm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nfitaprf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2byocokse.html


<!-- 参考信息 -->