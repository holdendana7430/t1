代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqprfqum.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3avkepalh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yrspqyhp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dfaqchid.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sonbcbui.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvoqzjgt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ubudszoj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ytuthvdx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rntlpyfb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3waogtcvm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xhuiyszb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fufeqxsx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjxbcozl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tdbwnaak.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3chxtgivv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pvwvklol.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pvmqmcre.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3stlnkwtq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wvqiwbof.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lyzyqbut.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zymtskty.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wfvxxpsl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xwaivrjp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kbsrfjqr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jzfzpotp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jaekzffk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ozdxgeki.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kktpnkrh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uvljcgoc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3amrleflq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ksbrtpck.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ockcgesq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jjpuaarm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3znijsgfv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wdjffvni.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3krejznzy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lgursmsx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zvpvqfsc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxczgtog.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mjfyzlgp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rmlgpkfm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gfxsehno.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vvqwkets.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3eekovtoq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3enioqlqf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jymtaxtg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3igrtyqfm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3drdqgndd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3owoaxrie.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dwqdirop.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jgjkmgpi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zxaesswo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3phpjijwh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hidzwajy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bcyvstjs.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fovmtpfl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fkjlvnuj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sjzzxonp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3npwzklil.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pccfghim.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xdeqtvqb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gxodpqfv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3adfkxltx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3sntxyhag.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wuuywvbm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kcykdder.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3chztrskg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fpwwwkoy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jvvbqokq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pncdtljd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ibxmnzgh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xncsxdsz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fhegdqzl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wsbqkoxj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vlxycbpy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wskvampc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3geodpehp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3coffajtl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hwomtxjh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ltcnjyxv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hunduazi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ydthylor.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3khtfuyrm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cvgqmnfd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3frlabryy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vedffhbx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eibwohzk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3txywkgql.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wiuibhia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gekvdmsa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qavucgxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siohqjau.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xwvtaknb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ijsrmoie.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wucwukny.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dfrhcbvl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fudhbrqi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mjfzufri.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wollotka.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xcybprzo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3iltdsmcw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eayomazt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ghbwykmt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fynzawqb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rrllgagh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3llmdbnfc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xbfoschh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vewnxrtw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3eqjxeirl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hrdnjbrk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uvlaelqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ycacvaow.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kfntuoso.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlpbnevz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lecmyzin.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wgienhzb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hsivkmou.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ndfiusth.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3meophosa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3iuuhgqza.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3czvefjvz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3laartezj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cdnqhmqo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lbxpbscz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hnftzwqj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmjwzvl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3pocvcjkd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3obxgcxrq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3luhveaie.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwctgxpm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ucimfpar.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3amqzktlm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gqfurjlm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jqzunjzy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3iraeyqhp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3chbgbvdi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jaippimg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ujcedbyy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tbtmdnca.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3efzyerrl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3abtszntc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3omiudeem.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3elptojcw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3cmqmruyg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3kyoicxeo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zfyzispf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3owcobugb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ihyecavj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zsxaidlw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gbnlljyc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hmyukywo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eprjgfyg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rckafnfx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bdcrbwga.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hpqkbtqc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fatgcdld.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jmznegxx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ucsjaeql.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qivezskg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3pgjejmqv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3phbtkzma.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vfugsjua.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3sysqcwpc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vckybhlw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dubgauhp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gsycmkvx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ndaaxcmi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tznodgox.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ccevuaml.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qhtsvspw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3sphavlla.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3luiqevih.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3usxeulbl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dxzmfrsr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lxftabxb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3agcojkqi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3htdvixrq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3vwagokkq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nyxidzdz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3qendthpq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3juimaduq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3llgsyzof.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3stfpjbvo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vcwymxcq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wquvxnwi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rpwltfnf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vtnibypc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsgligtc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3sporbpyt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ryslygeh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lducmzgf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgdonyip.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tqjdgruj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vkkqebui.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3crykwtgk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tpwjixyj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3eiklwcvr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wuskwnrg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ppgdahdn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3iaenosrz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hlzhfkpd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3odzxaxhe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pqygzgsx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wxomubjn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3etlhunia.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qhsfqthe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qtsggzog.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3prbhdtfj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3srywhlen.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3knctgoaz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rwdiknci.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xndyadta.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3kumaqdki.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lnmitdbq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qmajfkoo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3etvboqcb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fcihppgb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3aklouztl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nhhygogh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3sipysylt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rdyipfik.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3icjwdgsj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3lsysdwpf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gshgfcyp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zqttbzwl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lpxzincs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mfyojjvv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ryrqukxw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3pjwvsahg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3glhtsppm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ekdimlzr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vylhddhu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hdgivmlg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jqrownmj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ucejneqe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3sdcwkpka.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cjqvxwku.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lgbcafpe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3khgdzvue.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gpfgekoj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ghdofppb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3foislxxt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ytpasqwm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fzwvysaq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3sfzpvqjk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3llectjnx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cwkbxpku.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ikxbdfvw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3omfctrsh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3iybhbvti.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mluditgv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3obqjxueh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jqugkibt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fdfkevxx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rchoejok.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3aawxhqid.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ngocopfy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cttrfxpo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3evchlwvz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gbrerhtk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cifoewxy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3cxckciin.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gznhfofj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3udwocuvm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xljjemtl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3occvttxx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xtqraxuh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rjfrjqdq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3oikanafp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iqbranvw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3saclhnly.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjphczxy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cedodbhi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3veotyzbu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3myzlsuoq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogigtcfj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ycwwltlk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3gekjaptb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wavfcars.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nqblnflh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3erpicgea.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3blqcwjjz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cqsdnlqz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqapzfju.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3uzxvpvcy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3blgflmhg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zdncebwk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kjkjljsk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3lnwdunsb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mhsgjmzr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ypruyumd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3iupluvba.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mggtxkmo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3jesdvrmv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ohosnywl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3oeqhsdao.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ohvlllri.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jhikdpts.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3utjimmjb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uymbclhc.html


<!-- 参考信息 -->