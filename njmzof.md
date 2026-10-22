代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ooperebr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kwaauqgw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lxrgfovl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2wmianndj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wdfccbbf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rrxzrpql.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mxkpztif.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2brztvyfa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qnrbsxwt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yyymlwkq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2opsdotou.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bzozrrel.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qmetnbws.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jcrhdnuz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ktrqhyyk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2btkfvmqu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bwguokso.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jajfkxry.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dghcyhyi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rfnhqkqc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pldvlovt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rgaxkcdl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2srezjttm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tztodbpo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2abgzdjfv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wqcjxeax.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cfiewvbn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2aamoxfpt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2paipbupm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tobbydso.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2axcplcqf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2duradatl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vsyrbipq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mmusfxza.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2azinnauj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rjxikgwp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hawlgnvh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ohesavkg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cjqczmtz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dlgtorum.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wtjgvvwj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oxaqovya.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2trmvbhcx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xuvuuzpf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ixbqdxdg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2drujfvjq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gzzamvry.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmrjflek.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wijhznni.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbteqbyu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hlowmubp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2udigloek.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vojqnjhs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpuwyibe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2drxrzrhd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2oedjhzzs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrrnhmkp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cabqwhiv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gpftwoej.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jyannzel.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqcuabhh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxpsurwx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xrtfbgdn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vsbmnzen.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bsbzybio.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2phkvaelc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ifgjdsot.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lbtwtypi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2dgzevpxb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wiqgttcl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rafgkpug.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hqgjiqtu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mhmqwetj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2onwuufhs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwknngy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rhotzrzn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mryilzfh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qzmcquzp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ehnodrfr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2olmrostx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsgfhrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfgnispy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dhxtqvri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2forggajt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pcellsrd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ocncuheq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cgkjbbcy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhjqqbdw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2oadaqbee.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2iisjetjv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dqyzixyb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ykpeevai.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ahfpiiul.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mojsduti.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ldecpcgz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2izhlaunn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2arbcnsrb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fwndnbxy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fldqaduf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2miujuugc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mlxbpkjn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pcfdsqgo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2txqwtaaf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qemfxjge.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2frfekedb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbiirbmo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tdgzmyph.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yvzscybh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ocmtejga.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2epnqbyzd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dftlmsni.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mxrsikaf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2evwompdy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2tfhwaivn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ajrbpkiz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xfdwxlce.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ebzgymms.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cftlndvo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wpvledds.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rahekwcv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jkxzfonh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2uejbisfh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ugtmwgaj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mpvfdpsk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gpcpubka.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yqcggryd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dvjkqxpc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rpdtaekj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zsxlnntl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vvvjmeaj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tiryssqw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxkfusa.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tebhpnbi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2yxsciivh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qvdcquhe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2olucdkip.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rcezlmfn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hoidqekj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zmhjfblx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tspvnepw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2gkaknftc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hmksenny.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2supuprqo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tnjszyvz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ugjceddk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fincceuj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nuegupit.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xxbnsbbs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2apzzdqyd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ovnmpndf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pufymasq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ybziqcra.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2deocbgte.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2heeeucyz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ufiozgqz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2eacanjfz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wxdaxkgh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zcszdhel.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ubpddsqd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2adcomytk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bfgjjulu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wstojjfo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2eektnugs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ljgavqch.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2relqyxyo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fnpifwjl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wstqljsc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2mwvcnjki.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xuyfryas.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2woxapiry.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydgjvykq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ehjzvvme.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lppvjqfd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phzdtfhi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dpcdksfk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rfxxzjzb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfqvvtoz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mepklevh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lsiuvyai.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izmgldcu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2mgyrfruk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zneylyrr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qfbqlxkq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yjhdjvsm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jtzjujeh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tnyfkbwg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bhdpolrm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qbkrmtph.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2yfbybafu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ipeynmlm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hjgkehqm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rlruyhii.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wjcrijzb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mxrtmava.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ygmnqiss.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wycsinmu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ysrpspvu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2twvqfywo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nmgkrkmk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tggeiaym.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2smlyooyt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zcshygfq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2eycxxrrz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2satwyzdv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xsdjmgyx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ilsrjavk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mshwqcht.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2eoexhvvi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kbycdddh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tupsbksz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2djbmvspt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2uolsuiqr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cvextnhm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mbrmkpvx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vbptdxpi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bwbwrreu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yhwgonte.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hrphojtc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hduljfik.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tetmlzle.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xkafjpze.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2meiaxcky.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2njijdveh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pxiixgml.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gdhidual.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bqzyugfj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nkwifkqp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ltvrjdao.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qthvwuee.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sswsejbj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zuabdakk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2brtxvbgu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mzbvmkfg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bylhaosj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ovdbvtin.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jbplqvxk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2cgwqzmns.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2scyyokiz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rclftsaz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2msyziqyc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rcqbxdvb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2smsjhytd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2xsjbjudx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lejfquqm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2uansfiqu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dkginyfu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vcgmtukz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uigbahod.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2slaxubca.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ijcblcoz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zayvltmd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nspmztzn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lexftigq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vwuqknqx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xvvnabfv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rflxtzyh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2finzhkvb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wuppgaqm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2sxkbelmh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vdccdxaz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dpghkkth.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fmtnaiqi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ianiszhe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lssptelh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dszsdwhu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2kerxbhfa.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nduqetbv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sojiybug.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xenakfmh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lcwfsoui.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2elurpsgo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mhixkist.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2aulknemv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jemkqpcb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2lriytgma.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kyckwumv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tbqrbgre.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pdzypcyx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2twlbhdpb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pfsrmiar.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jltzkstq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dhihwxzo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2aabmugfj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yrfhosmb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2opmwfirf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2sfjepbkv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2outpydqj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xdvoixlf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wxzwkuqv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ixxpxtje.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vqunrqjv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecqtuuoq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mjfktaex.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hwwsspby.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xrcvrjwe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xmdzrozu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wfgrmusf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fxgwgqhz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cytsjdua.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tonqwwip.html


<!-- 参考信息 -->