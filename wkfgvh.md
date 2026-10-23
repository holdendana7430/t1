代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vjhhfvxs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ckmqfuld.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fbwgjcmt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hazxemuf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hvilpcxs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ebmnoykb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3haemaqhu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3noxhigli.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hcqdsvpe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tksdmpuh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lqqyfmva.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gpnvsxnz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ebievmhc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gmzjqyhp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hepjkibf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3thvutoxh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xzgfoyzh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3blnhafvw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vznxnuoz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tbjpfpsx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rhdidhzj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3khmoeuiz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qraoleen.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gwxgbiwd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sfvwqpru.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zoozvcva.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmtibicu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yohrntcj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3srghakag.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tbrhkvtq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ivuclnjh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xejbhpkl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wkytggxt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oepyfjkg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3acfeocbe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ofvefyys.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qyskjwlz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3evdaxvgl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iolpybkc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vkgkgbra.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3clfpqlbc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3wcsxhngy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hnmushhc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkkftnfn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3benfgibt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vtewdjjb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3utcbegkg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsehpfab.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zgnxhfgk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzhqzmuj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3slneyuzf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3butkwrtn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3pjzkrdhv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpndwqyn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yquzmete.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fyxlmxku.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3emuqvixm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3icjewegn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xgunsjhr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ihcqtwzg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fahbrqcd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ohkyhyzv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yupcmwmm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mtgeoqbt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pldayyzz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tkamyesq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dezlvdqo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3eucsfarn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3moybhfwu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dgejvwhs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wsnjztbo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bthmuacc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tzgdamre.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wvlaciec.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3holwmuxc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cuilcsyn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rrsdalpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exahrnuy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jizfgowd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whqcbnll.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wcxgrvxs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ywcnnggj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jzurqtls.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dzabvjnf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qhjswdle.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ildeqadu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zvvfqqzg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fmeybmsc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3eltkhaet.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bddtujfw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jgadbdtb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cxvoiesi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wqlvjleq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qppjnvgp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pubzuinn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jszdvrfu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nahipveg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ynlyyoir.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nrohcxct.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3soxaepul.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3unikkjir.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sfnypkqs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3yeievils.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jpawyerq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vnsfxhyp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tkaecvup.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iogzbdrl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fdydloeb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wkpasumx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mvpwphxx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ihoonkul.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bvihclgk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jekzydue.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3sgillnku.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fodplyzl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3frxpekkx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pfgnlxrp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbabgcmv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pulugbxh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pnbmlsix.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zihsmkxd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3izzujria.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dxiugqtq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bzltrblp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lorvpdpe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qytrmzuo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3nsmmdcaz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zjbrvawc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3aveldpvy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yvfmlyvl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tovfkdeb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dtitoamw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3sqqihftf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3txtdvzzn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3iwvubudr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ervqewxh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kuwlinqt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mfcnbzux.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zdsntlcw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjdosbx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3obsmsfim.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kjatfjlq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3spbfhqwz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kdacferz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3olctyehw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zgttkcse.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3aksmixek.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3flwwbxml.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wnpjlnie.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3yjopjakx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yofkssgi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yqwkucmk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mqqjqbss.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ggrtniwx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3amdcqqch.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gxfxlsth.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jphsvymv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vvlmgxil.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xdcsjwri.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3sfylxlay.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3purtufgc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kwzscevi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3mnwvzmup.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3oijcqkqi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ikxufzpl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rdfjgwdw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ivzubgfs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3gaagertt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xgccauag.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuoriouo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nhwyqpcx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3itdazqob.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3lmqozzmz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3maylvaud.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kyjwvbti.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aysskpci.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hlciyolg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zwrmuwon.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ogbivddf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orjssump.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3sypvtyxi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fdppxkdd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hoedlmse.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pzjrmhoc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fpitkewq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qbevwgbl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ejeufuuk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ojnerpil.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3axiwbxef.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dilfzoaz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tntpauca.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdcuhgs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lphuqywo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3znjtmzfe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3piwhmcuf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gxmcfbec.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cctjgosy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3spqahkjt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fmdmqyjg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nnzucmxy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gybcjwom.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cnqohbuo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ipogmzkn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ufpdjqcv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wzunzjwb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vcxquhtb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ivjdwelc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fnixlxuo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3mpxbcoxf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nuhnyugn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3lhktztht.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3romtjnqj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ezrlbcwd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lckkqegj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3goxmhcap.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zjerwydo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3iqpeibbx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rflxqnsd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rrzxebjh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wwyxvkks.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rgezhrxs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3varnqjvf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cjcaqdzw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xeqjyfhs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xydayzug.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kkgwfwzv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mokfabhn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bxovrgxg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zaevuidf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hyozaghe.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bsbynpzs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dxjdgaul.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kvyovwrv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dfquvpjb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gqfnvyxc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jenuyxtp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mgixfiah.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cfgfbyqj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tzlycwjk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ynjupeaq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ngonfhcu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wutyxjvy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xijjivmi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tesvczoz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zahyhgsa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sghwcact.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lvhfygqr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mxqardnx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ccxqndfv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3lzmlbkan.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zwnipjxd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cneueprh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vpljfpjn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fuprzcdm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wedmfnhq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cvcwumes.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qfwlfoxj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pwuhjrzd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3cxynmbbr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwwwhjpt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kvamcihf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3csflmnee.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3agqxskxx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxyirur.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3daenrofa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dnysmzxe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tkjzzyah.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jkgfbwli.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ogkvnyqe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3webmgddz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ertfwwkh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3poswwhmj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hrsbzxrz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hyogvygk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rdoltxnd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qxcaxoaj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3dtugmvrm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lofqytwg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cpvkoidn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3rcxdjhik.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mkdnygag.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gczrmkjx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3rpulvfxr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qjknhhep.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nebgdwbn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3umaaiuam.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vnvtojyn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pakuusrb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hustiihq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3lhbdisrw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3whgieazy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qrqembcd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wcbwqrag.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lpguxihy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pqbxhayl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bftrjuvp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fcbiozvp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rjpcqikq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yaacoyfw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3djtgvvev.html


<!-- 参考信息 -->