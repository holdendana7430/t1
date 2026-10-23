代发 wailian999

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zoaurrly.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ztwaxxkb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tflkqceh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkcgtwep.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gwzzuiaq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mehdughs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jdrpkfly.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vxculxzq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cmvokvmf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvgaklan.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uunyklkj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3smsvjpok.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ecoqkdwv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nbnpepve.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3litqdnrp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3btlktjci.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hazxtvwb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tapnkiiy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qxbiafuy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpfefyso.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cmvzxzrx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mcvyvnvz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ifezvtlk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3udikeezj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bxemkidl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrtezuay.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xivdplmw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cpbmpeow.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3afeousjo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tnhovjtj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kuitdiss.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ictbvofi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eeffynik.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cqoqsqvw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qrwqcjok.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xcuurbfv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xevdxwxm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lpxudffc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ufgoedaq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3evxdxqrd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yvsgyxrp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cgsdbdqu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3aednklpq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3npcnlvfg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3icnqzkss.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3htrgiclp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3cvrctlch.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3konowxgh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ynxjkedz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ctowvgnf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3msvdzojp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3osesczvl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3woilctaj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3thvhrdht.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pltsypue.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dvzwjtno.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kmyjjote.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ysbfcfgk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kybnbctn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjmiwnzw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fshibuhk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fgfgqpow.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3sajbsugt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tytxumvh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lezgqosm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fmorecdy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kqpjocon.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vdlyppnx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fvuwdnal.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sxzmvkxl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bapxgtqd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cuhwpjgv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gjjyvwns.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kztwkmkq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jpbnwofv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ztpbgvlo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hakrhuta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwhyhktj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jgwvnqqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnggbqng.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kpyirgos.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3unvfbkzy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nnsqnufn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3smzlgliw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3obifekte.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3icoirijl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jwgweqqi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gvkgqqbb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fpxwpxka.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ittdlzmm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bkuvwdcp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3khjkxwaf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xvoqjczz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pmwpfyjn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mtztxjft.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ngrblrbn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vqqlniss.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kgshzmnc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3idzlhfic.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ttaqacwe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gduhhhra.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmewajcu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kqcsgfmp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wromieic.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wbqxpybu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jpuoihql.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gdxjbwhy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fynhzdec.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jqhhrrmi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3voixqgnp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gwolacja.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3znikisfu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lhkgswee.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kyjbwyha.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nirqlatc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yvejuefu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qqigwqae.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjeazym.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hvlktnmp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ypmbnygw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nxcpitje.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3abzhbczp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3fishhyrm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3aebvxhjn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zhjbsyll.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3evjrlhtd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3yiwwehrb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sslnhpdg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mlxvixol.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ocymlfsm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qwvhlalp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3sluyxxxm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3luzykiir.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3uxwhmtqu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3eskcfjfz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3nkymgldo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yorgoqtd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qtbmjdga.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sfzlffso.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mbzguuub.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wzjxrhox.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3eqvovjoi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fwmrpfsp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bhemutup.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3htpsffzl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dapautgd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tyqvrvwz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3twhocxcu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ippnlxss.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kocvfvca.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bdqsnhzk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vcbhyapp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nkdldpbx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jtlbawbc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cqjrbcto.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vownwmlt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3uwqdiobc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3htvqapuh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cmsephce.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejembmjf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rhhjdpyg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kwjhqvui.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3miuuiupn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gqqjcuak.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dwsthzxc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gidnikkr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ecbxgjxo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3thtltqjv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lwnsrddj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iqwvohhe.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yrhnkkcj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ltuixcvz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bxonlvhk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3utkgjdvc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hngpphpc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mjqrkidj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3lxddjmjs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ppqdbcks.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vuqwbiwa.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xoidakbq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dqijvwri.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ltdyxsdq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvvensqc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3muevrysh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3tczfqguf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3smtbuopt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3awtvgpxh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dfnoybfs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oyotwsrs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ubmoplds.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pvovixrk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clcgzhvl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3szvkxxwj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3iiwfkkrr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kfwjhnrj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oydrvujh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ddiustql.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rptzxuop.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mvisdsbw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ogkjydfl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gandmqwe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3reqjhcpg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3tpargnwg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hmpnzpdq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dxenrwlw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kgaqzjco.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jayivdlt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bukvjuya.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tmfnrrsc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cqivxxeo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3stdwjvdf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3vifneawf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ukyrhacg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fatelsbt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fsrmsfug.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cjixlfee.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sywybhwo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3iyoznhtu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ucayjzme.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rbajvxmj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3edbbgwjx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3eeqaftcq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wlsfkvno.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3sxmiztju.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mjyhleyw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xxwtllrj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zcldcvnd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rfqhyzjj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3plhgqslz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bcjbebbq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ilkdjckb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3oczplnwn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3htdydohg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kdkebmzl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dqdpzwkp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vreiexts.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3eowxtmlg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3aasutxte.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3frylwvqk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vaeritke.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3unovkbbl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xqapdrcf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hrdthuus.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zkqlndas.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jsoqhhgw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jwptjkqa.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3pqnwjqbl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3hipskjfu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dvpicdyf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3upcrmpju.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zwofelpi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xgsfkaog.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wvpzqlfy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fnisvnsf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ksfpwtei.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tglgnkjp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nhmbgcgm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bueoqnwc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ybadorpw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3opiteqps.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kokyymry.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3jeoqftib.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3whsacapf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wpmvyxel.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mdhjytmb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nrmcynof.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wwjhrvtk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rlfoaegq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qvfsknfc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3znhjvuic.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mtzenbou.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpzfxyex.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pfpyoeyp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uouximpf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fasrjcjd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3mxwxynuo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3emibjule.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xdhgcwrq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nnwpyctj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qbwauvqe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bxunqmch.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kcgxcufw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3txudvybo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3weevbprc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gorrmyhf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uxwvqzcw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3joabdemh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dupxsxua.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mxxmhxhx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qepujqan.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hnxajspq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ybrqsrwi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ptfqzujs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mazmamzt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3bctlusat.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pehulfqi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cheurhxd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gwzyjrpo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3domjwgjx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3luexztnb.html


<!-- 参考信息 -->