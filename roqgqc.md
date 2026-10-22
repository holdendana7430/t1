代发 wailian999

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fhklimyw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yuzlvbwo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fbztafym.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vgphwvsd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fvradlen.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kiucxvkj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mwrqvzen.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nhsycmqj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rgyjtscm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2uhcdimkt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2syuyjyxd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbdphxm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ptprzazh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2caxkqujz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hvhprufr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cxcxmedr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rfhneqhv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jstggybq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ocejdjfu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2envrbhrg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2anqkrofx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2asrzbgda.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2txxffihs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2iwmwgcye.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wgqfgktd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wztuzmfo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2fmlcpvyd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wtjjfocg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2otsdvzzm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zhfirfuu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vkpiklto.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rtrpgivu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uxyqhtpo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gmhtoeaw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zedwkque.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qyhagaga.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hzqyzxso.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zpeiltae.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pnrdyhnq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2nefqvkmu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dwotvmwv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2twrrfjvc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qydwuejv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2talcpsal.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2djzhtsrb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dfzxlcwd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uagxnmao.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pcgooxvn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vlzjihjz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2uikueqho.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zdwgnwzl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2apywqwkv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zrolhfkq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oaoomycb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2omhyoomn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yezsncgi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nkzbhfnw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ipxpspes.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2zxrtulps.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2oyljnclp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nrnmykal.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pthaimqh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nzgpmuer.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lisqgtwq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jbvpfpme.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2izukdtaa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mjmtoeoa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pccseisc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftabkoii.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gaxcihge.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gskzclzq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fjrmnyrk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwgcdxtu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kgrblkjc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dqgyzkzj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ljkeswzj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hzysjsrt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uwdwzrit.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dxnaafep.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2txzqluxe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vjrmdoml.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xbnscomi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cwxsptdo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lomegykj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2prvhybrm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rinqfijs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lsmggqpi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zmclhhvi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2oilffdnp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hvjgxgtm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2szpvfxqm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nicpskbn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2trpwdcvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kepzrxhu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pvejjoiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpoklhnt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2znsfekuo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rwvgwgjy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2usemtgro.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jfkjfdvd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2huamejkv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hnqtlftc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gzdbzkky.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2flbyyqbc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qsrwbezk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vedjcbzd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nbxghlha.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gvmnufal.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lffmmelp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bitnliln.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2plcxseqh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rnyrsjzx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xqzafkzz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lblmodqv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bziuthei.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2aacuandd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2jhrpfpse.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vcrvomwn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2upyxtrje.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfmvytdo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wehclwqv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ollrdquj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2aikwtvsc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hnukecyo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yusstscx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2msgzotyv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ojholkdr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qvrnmcyu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pyrsefkj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pnihiffw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rczmciop.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gpgzjlqc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2evszeahw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxijitu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2syuknobb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wzrzwpzi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wfxesojf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ydhruhmy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2htmytjmp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2esvkpysy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pvtppeqt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hlkhcxqr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qsmewmae.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2athzcojv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2njbwuuai.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2okfazdvf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gsaukboy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hzkkfgss.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2agvdjcns.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lcngwpnv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mrscfjdi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hvaaybbg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zfhdpvko.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dvhnjzsc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yurcdlzw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hkskdohc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lpejnqnq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ewzpksmg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wovdxjii.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2soncqnjc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qnhdrkix.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yuwpvqpx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lcaxotwm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nmknghuw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tgqwnqyf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fzjyssfh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2marusvad.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fedcnztu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kkvklrgw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2azvqfwdi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2rysjznaj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2thjkywce.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2otaojlgb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gimkncrn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rdanfbxk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtcmlrs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2imeglswq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ohfahhrx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2zlitynji.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2otnkzogu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vdwrnwjm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2roxxoaps.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fvsgfrwh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2lbjyrywm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ikalkzqw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tlfcdaia.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebhgszrm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2sphiqgji.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tnicssel.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2huiigglv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zrqxzjaz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnprwgpd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vyljtpdl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zhybtacz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2dhtwobzk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vughhcex.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2pdgaxsxn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2awnyljga.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dufnnslh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uxgaqrwk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2pqxswygg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ucpmbtsw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gmtxruxq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2twagtpgg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2purhlmrt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nisxmyqe.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xitvxcrn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvancau.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dpaceubu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2djucroyi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wjuyklkk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2izbsknwr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2otfovegn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jvhamlgj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hongueta.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bmulflvx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lsadjykr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rtuaizmo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fieesrpb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qrsgbrye.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ovugwtgu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2irbumana.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xopbvzyu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gqtavzgd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gaquxczh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2djncgaim.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tymhvirx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2chowfctw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hykkdfqz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2uosuavng.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fclsyrwi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uhjsnaus.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2aajdoozj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bsynkvhv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rqixiilr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cdczrdds.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2byzttrtw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2phemvcbm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wyndfxig.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jwuwxrvr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jvgjxnjy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gphbvdyd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zunzzjve.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2byijihzk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qlqykxpm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2zbidwuwt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xsdtcuyj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2yxnvhtef.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kojypewd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wjuecsxd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hluorysf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2inoxhgkx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2igsupnbs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zurhtpza.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sqjwcuny.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2linbtudm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2noklipke.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2phuejtvk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tffulxzw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2usppdmfe.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cgdwonuz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2naszqmvs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yxwtzyop.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jdnlokpy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xgwngybp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2psftljei.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sipbunpo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dweaywfo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ehhtkett.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zwdkmlhw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2gqsfswce.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wfjdyhpo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zkkuvaqi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tvqeecwh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rwnexkmw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wimwzmxe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vljtfmrv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2satozrap.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ftspcqke.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jtuwtmup.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wioghjyh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ctxoopbn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2plmkfdxy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wwbzgmvz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zyqinnqy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ycngdnxe.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2uksxiitx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlcouwhh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2uxsalhnw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2besqjqjh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2oqmgkejl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xorrmpxm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ajqueisy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vbxcdves.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rhhkdbbs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qrdqcftx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mzpslccv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2bzvpkkvb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lrutyauq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gahckucq.html


<!-- 参考信息 -->