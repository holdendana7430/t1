代发 wailian999

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ilmecjsl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbawdryl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3owbxcflm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xeowlebd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzpkrsen.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3owjrdgbl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zhxfftyv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pylffqkg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lbvnejan.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wycpjwqz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bjqjlwzm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vvqxiflv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ooqtczcl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vnvkanup.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bsbreaqx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nntiugoi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3shqqmmog.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nvbmppfq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fkjtlmjj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ygptchss.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lllwhqcc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pgyuzeev.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3anhdokmy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3oqcnfphs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jwyjlwjk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hjenrgdc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rmpgflff.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mhpgiroc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3alnmalzk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vasqpuey.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3niucsmbf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gearbnko.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gwvfanbg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bvewaeds.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbmzctbm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bnbumypi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ktzkguok.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kzlbftjs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zarbspki.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cuyxvwrc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rxwgaugt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xyzmugxd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nognqsyu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zrxdedxo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zenvslqf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rjuqpfjw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ikwgtvrd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jyetlknr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3whstlmqu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pqyvlafx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3enkryzff.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cdlgtfgr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3puicjkvm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3otqapxla.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gnjdbygp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaylpodt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xcyqnskp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fytshffu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bpobkcuu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wxpifupo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3elchrydi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uqapxhis.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmwixrip.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xlpminss.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ddveiucg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3imqtlyou.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tmembynk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uwtdpszz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dxbdrlcy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aibcohdg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fnfxbpvc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rjvvpehu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zafhrosw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3agbpokja.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbcnvzo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gxazphzh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vwjoggxq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kehodpdz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3aojmrgpy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3shuvpalq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sxnzdwlk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ujuyphpf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3axplglix.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3urhxruyr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yiytbyoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aijtguso.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emjoqjyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zehabhjb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zahycbmc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rhtjhbui.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hohfxqer.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yzbrjvpf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3iaqadhdr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jhqfyxvp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vebkkleg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wmbrrxuc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fvgfbefe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rmwiyopd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3thtrlcet.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dckypgld.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rglaguup.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wittmpck.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xjuupghj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3iphzkprf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rvrmiqod.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbtumth.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3obpkmtix.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3edkmavwv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kjecxcgc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3srpsutov.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kjsclorh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ixeenbbf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ejoetebw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3cnhlslmm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ildflucf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3msqhkbqn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qyxomaee.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3styxcwoe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3oluzxpqr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3srxhvpez.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nhcmtqtn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cynycnvj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fkchvame.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gzpxoyyk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3isouzrjm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3opuesomk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ofjijabj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gdbnnkdt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hqqajwlq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xfycuzpi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zycibhkz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tvbtcuqg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3govddpph.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tjfmuxyr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qlwiyics.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pcooualu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3tpegnzrf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ccytyzhf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bczxmgfy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ucnlexva.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ovtfnpnx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ctzmvsaw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wbpwbkae.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yotnumfk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lhspwcuy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xodwyfle.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ghnamdpz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qbtgnqvr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fvcahhjf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3urhhkutr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3uajclksq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3oaadrvwf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bfuielaw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3egpknfsq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ykidbwkh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ybbyyygw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bawxrlei.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbkuydo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3exljlmtc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3erlwpplp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fjjuhxla.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3yxmqxxxu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gnnjoelx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3eelcjdkk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3quzsnycx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3gvzmqehb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dczstuug.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jbvnlouq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ltvuruwm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ztdskwdd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fjcdnqti.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3lsmrnvnw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ctdjamaf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xyhagvkr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ttqfpgtr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3thiwjjso.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3edxierhw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3utnwwviw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3loksasxt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gesdfsvm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3znhpegkt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rvifidre.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cqbksjsr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xxpfwfwb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jyenwfes.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kglxfzud.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mnjtbfcz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gnlfbvqf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hwbkwuji.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3eejeqfvc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewpzkvia.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nztqbmrh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3yvddsgsu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xdrgxpmj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rvzaiwch.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ddifqeio.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gpobqxhy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uworlgse.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lgysviql.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lahjbooq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tdpacgtw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3bbpqypuf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qqfrpnxk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3eegurqrr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3eythvwjz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uunysqpq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xbdmuqlv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3orqnpaap.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3aojurexs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rglxbpbl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hzrmyfki.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jkyuofpb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3oohbopuj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qxvjjmhz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gejniyta.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jmdxdujj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3nzutxugw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ozhnfaju.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3oqvsqpix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vqpkryoq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3odynknla.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ljkkhhsy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3armlnimp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jexforhd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hcnfkiub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3roqtvfeo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wwllzsav.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ysfewohu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3svfzalgt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yakqodab.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nquqlgkn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3tpvfnwmg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ozspqpxj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3azottrup.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vacfskic.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3pxwxgrsp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3idsjnoys.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3shxbqyvm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wjfbyoth.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kkmoaizw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fnxqlocf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qucuofyq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lmssujnl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3iojhjfaz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3muamnihh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3svrbgqif.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ilvedqof.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tpohcval.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gfhewujr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ilrnndfz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rewlphmf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3odacxhdw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3twbwlftn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ohihcpuf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rdwvdlmb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fcwghjbi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3diclunzu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tjcahwvx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yekmkcjk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rfucrlzp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nkwbxeax.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ctmtakvg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kwazgeaz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3owvnnxaz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qcrevrzu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xstoyhsb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3feibvsib.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tysalntg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3sxpwvrrd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rqzevdat.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3efyzkdql.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vhjsaozm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dmkxezbz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ulozjxxa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zsenvtmq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3psrswlem.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ecojqtbe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sjnepidx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3gviqbfvo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sdybuhaz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yfbomtbk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ipfyrlbq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qdyaolzh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3eeayjsrl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3hfvyitie.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bwhqnvsl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cqjceihz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rcjnctyl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nkmciixi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qobkknka.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3amottudx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rppernkw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3stetdljj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3auymmqdk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ewtkpocd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nbcrnqkw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3pqtvzmrt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3smugqmhz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fehfbrln.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zlsyvkjv.html


<!-- 参考信息 -->