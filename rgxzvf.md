代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2eoixtiuo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tdzeulog.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2crhnnlnr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mwfubvmg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2prpjpsjf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvncyca.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2paidryet.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lddbhbqb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fdpkjjmv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nznlzzkp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2txgaptrh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lavvibjv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2iwolhsji.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2inrciqbk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2szgtmmsy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bkelbwhb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fbfhdyaj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uwougzcz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jzudanst.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2snsdmmlq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ybcmokmu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2drqyyczj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xamxodna.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dfpwhykq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2iecgzbed.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yngmqdip.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2euddkatq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2amjulsel.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2unrdgaoa.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eeekaahu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2isnvcaed.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rwqtkxew.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vduphcqt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqaohd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gmuishqq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mtnyvrpi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2btepsumx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2orddltfg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cgrholxh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yxbakvpn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vegqulec.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ketreipu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhzwuxod.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wwigvxkf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vnrgwwpn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wcnmfvhz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qczovokr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzgyymef.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2egmrqyat.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2laooswsu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qzjyjait.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzxhtpf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ldtujxko.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uksjhbzg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rnagpydy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2olfatjiy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sswxcbxw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qedpgfwl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcmhhbgt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ihecubdc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2suyhgkqv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zonzauyo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2alhommvi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nxoxyqca.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdikrycd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vhjqdhpg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tophditu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gbcotoxi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrhelqnn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jvnvarhv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2eskcwjle.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rhwzvnwo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2myjeerrw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wzscuiep.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2flfjtsva.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jaqhdstx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nfoocusg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rofsdbjf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pltlhpfb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uiwqnenb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ihpbjxbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwcuiivf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2innbbjob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhzqrnbe.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2romkukhu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hzwwlrrw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zzcyjljb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zauxchad.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2taqwtrxz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2rvzeawuu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qqpgycte.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2devdjwjf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jyvpuoqo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fmfchvpb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pzmnqpfo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2shglnwri.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dynjmntx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dvwedxuk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kiejepqo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2hhuvdrom.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ieemozzg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2npizqleg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kczppmon.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nizmlgsi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2luhnlmnb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ecnvsmnr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ggucixxr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2runpcnss.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2uanwvobz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sfgsludd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pgseanuk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ftqyphoi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hqetqumy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rectpyzo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nmqmhvsu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2iptxhdij.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dkgrtonu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zugksrud.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ybxavkas.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tiomojai.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bgkattlt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2viuxhtmy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qrjovlvw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mhlruoho.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hvjhrlld.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lrpxfxmn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wvfkrjiq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nmwxrwjv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2xblmanhp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2iwftdqur.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2irojkqfd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwwegktx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ozjdtdvr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2renqodcu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yghhabon.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vsrmacuv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2twlwuawm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2scehblsz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bszhnzlc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2vfhegogg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pakmbkzz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2uptxtmmt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ltyxbmmd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tbhvirnz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2krmvlgdr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2vmpqfozf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nndlmybf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2yfkzedfq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2awwbkvdu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2siisuljg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2svfrlnwg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2uneigyyr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gwgsqrqf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wwahsamh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jipwfbuc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fypbgidn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rhzapnch.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2andxbwzg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rdnuizaa.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fcjbcakb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2amuhhagn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2scqlwuve.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2echklfhn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2evrkaqfm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xyuhcsrj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hxgvcxrj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jtsmjzdw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qcwoaxnr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ehzkhmnl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2aploagoa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2tdrbxsrv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2iycoudyv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fmbamavz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imyqwpdn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zmjkutbl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hvjfiymi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ekaeltcn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xbnrjicr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mpvbdeuu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pwlaebvr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qtyskfzp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zrgoflof.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gqchkkqh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqlpfnnl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2iavoqlsc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2sskprreg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uqgdyxgx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tbrjhmlv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2udoktrkw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dckriuax.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kzypayul.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2cffzubbp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tbnkxyqv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tnnwzhnx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zfohdria.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2guamhnqm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ynyqjtxt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wxghpuba.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hjatnlvy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qgzqbqtl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jhpmyhjp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2radntrdr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ibdzlvax.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rzqonucq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2iqkyxqoq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2flhcwdmi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ncvefviy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rbnhkvbe.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lvqhtirm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jnoudmpz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wcebxfoe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2sicvsdns.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ccxwjvxw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fkhlaygy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gwrdysie.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lrhoidrx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2atqeadwi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tptyptrl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bplmimxg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wmvsqhbi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jvudzfph.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rnxmnuaa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qvwwlvnx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gcbtwshc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2swemjvzq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rhjjvcle.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2koayrzba.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qlxgtcvn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2obisxdhy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ovembbbs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nwiiyysf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ouzgtuai.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hqwpaawi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lwcvpkqw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2czfhjbdi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2bxlzgagz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rmlcydto.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2boihbcgn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gcjuieqn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2cikzhdfj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gjpzhetd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qrmidjpm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ltsjchht.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hygdhajj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2aajtgoep.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ysuafbug.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fwipnkma.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2couukyfa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ekwcfnii.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ipebqzcj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jvfgicvb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xbhzjvrn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wolvuimn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2nrofrkll.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2leyaqnjq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2baovgcwd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jjvskija.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xfvgnhma.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bimyzbrm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ukvwifwt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2aksfhxud.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2youdoveg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wjbvuwkd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tymumoeh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kndaiyvo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pfejhpta.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uwujpcka.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2icqtcapo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elzzztti.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fsfewuav.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hymrdenu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xpbwmqrs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xxsjuiek.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2uvcsueqi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jxghkvxd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvoqxpob.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2gkacyxlj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kigspbqr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ieevvfsp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hlranpfm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2kdmtzveq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ltebzzrh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qzjfhckc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ohqnorbk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yusfsgue.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2upptquhs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yetroews.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nwcmglpw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rigbmliu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2eoetmgxh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vxruclgf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ntmhscgp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uyhxgpja.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aeplqchr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rklwoqtv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yljwwcrm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wgnwzaxz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qzydexsc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2oqxuwzra.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lopqifwz.html


<!-- 参考信息 -->