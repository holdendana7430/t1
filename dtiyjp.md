代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kpacahdc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dwkucgyi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kgcmlpkd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bfedbuwu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2udwfswue.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ocvhsyjz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gphnnuga.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2czplkcbv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2uanfqlmr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lafybhgn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dsfzqvsz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fkqazgbv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fppldylo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rzanrbuc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zutcimwi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzbriwix.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2skhuvuvu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rdviwqfz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qbyzyjik.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ppnxroyz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2iofoispb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozttmzfl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2isuxqycx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lsnbjwpj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yjdoqore.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kwtvjhpx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gvsupzci.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dpmsyygd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pxlmgpvp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uelzuajw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yagpyoaq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yicbzwyj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2resvlswd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qpiwntis.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fgpykbxr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pprmooiq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wxdygkwc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2trjxthkm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hbwcgazg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2koofufuz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukmkpowc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jxgfyohk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dgphsqoz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoccuzym.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hodomtik.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qvtftuoj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hfiedokk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qbrbfmcg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2bxrdxrha.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2niccjjlr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlftxwpr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ggtvjmpk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvpencuj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2grbbjyrx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zpjncdip.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xjbysazs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2prtmebhd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mloukaxv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uvqwxmzn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mpydrkji.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2erppqifi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rqgqvtrz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbnolbz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zcgnsohq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xoeuomyb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hlrcosdo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2unnawdwk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mjsxgnkd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ihqteffk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jeidxxvd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2alcgyijc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2fnykmlnl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jmgqltwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnjpgqkr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vkzryydw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlyzfrpc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jwfsdvfn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kjdnazql.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gwpqwwzc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aafbbdit.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dybhddvm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ypxccqeb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nzodmbxh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iccmavib.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ckmiuduj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2maegktlh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dgiwsphm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zjpcqqcl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fpaozgum.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oqoflnlo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pvihbyhd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2vuknzskq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kqviyjcg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tjpzrkym.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vcdgmbpt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2yqkbzgcc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sdfurrrt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2brsvjebe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2idfhcttz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjfsvsv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2aziynwzs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gifcxkaw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cuinauwi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhzpjjq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vuqwnufy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ewowvekf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hzvqgscz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2akyonyuv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hkwtzxar.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wokhuggy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fenxceln.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zclykkem.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ekgzmonc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqihixh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nwnrwsfl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mqzhkwak.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2oevxytix.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2czjnvuvc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ghmxxcvn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2frecskzv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugtiicap.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ywpdcjum.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2rxpvpsuj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzlxyse.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2upnouaxx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dvyulmzu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ejtntrya.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2emycqyrd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pjvxdjds.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lneutmsr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vcfyovrm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ninpsyzn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bnnfbsar.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2rfzxdepk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hxbnukmw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ygabttms.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ystdzqqo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2svtlnjki.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2szlzuxaf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lzbfbshc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nsaocmkf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qqbuaqje.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2accxcbmv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hxfvkgym.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ssabctnx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2moevmwjh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sxunicrv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lxborweo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ehsunpwb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2soykovxe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2axncqbis.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2buiomwgy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2niiymcpd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nerzlupd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nvzrsjha.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqkbftgu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dttrsjgh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2eccohycb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nhdnrjzu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2peiyacil.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2czsjpjkl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2duloxhsh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fikzrllk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rvoxmsjs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2kustjzds.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2skwznrgj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2abzxonpv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2klhlfdhw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qfbysnpn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nkewfklm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2iqzsdaac.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtoeuszu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2luwippzp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xguypkqu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fghwonut.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2aghsypbe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2nyesfluu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2krkpvmxy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sthsppal.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dbfiefvl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ogyinuwy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qvrbzaem.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2uchvhvsh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jqrejsoo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kicdbann.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2exsuzzxd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wzcdxspj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2etwrlhdd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sasdsybd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2atbcjcav.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2xedzusko.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2igvudjfw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vgxzdpyv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ucymwlhk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2hxyoclmy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hfethwlj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2oqfjyitn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vlviisaf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wautrhyl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qjdsguow.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jhlgnjay.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jxlvqorx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pnlukeim.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ngvxgalo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gluhujyo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vtmmsomm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lfazsacx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2giiigphg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2exxddqvx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2alrapvtv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ybgkjjfj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ufdsecki.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xspiffdm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dkuhxmvh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tyelnfrk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2shahpgkf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fmmjiyzs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ocncotbl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wsjqvhfl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mwmgehap.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2njfmodiv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2buextzyg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzsckqkx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zsqmbklm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gsameyru.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2prrqoawj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2scggutws.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sjhnhxje.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2muzlrted.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2jupqfrmy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2axwtgvdi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qsmfbxto.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bmbaverc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zogmgvwl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qysuycao.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qnpyyoqy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xicsmexg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wphlnjed.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fpvgbwau.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2viwbkxjp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hyutocsn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jwquekjb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xtyvmkmg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ecviclja.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2juhspjmx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hasfbvkh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2okukepht.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2viffxhdn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2joicxkcn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zzubccyy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2hndcuxqr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hgddiqgu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dhwwqkvx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2moldanqu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2frpxbxsd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hfesxnmi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wbzomrls.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pwtqewea.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lczjqdfs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jzeevcxc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ulkbsxji.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2xlcaroce.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqwzrgfo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2duybvpys.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2kavoyats.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2bqjyfnph.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xqxxkjzv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztfxakvi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2yfhghpuy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tabbshid.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2toqmymyp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rxjvqwbs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2rcsoeofn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jwgjqiep.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zjgszcyd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2plygerlt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2acpmwwkt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2kumdwzmx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2fsaqfnlt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ueqnndvt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2baxsgfex.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qnatxtmi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tpwjojla.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lpuawzla.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rknbgfow.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bkmreser.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dsetqkrz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ducntfkx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dfyidapf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ljgsmxab.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2yewvqfzz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wgxtlvyu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jmryjosz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2htwmvoyd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2yanbozvm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lpmfcwvk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jadiiosn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2gsjqygwh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bzlxcjdi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rkkhyytp.html


<!-- 参考信息 -->