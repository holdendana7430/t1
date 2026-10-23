代发 wailian999

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zczttvsy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gtddjdbt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3equmwzbg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojrzoegp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pqkdutgt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwldhcd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hoyktegu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qxmeeana.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nuzqadst.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vhvimuof.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pvrlfxsi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3drbwnqei.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3aygulpbz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qmfgmtqh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wqcxrhnc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3eholsyjz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cdwimiac.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tiufpqni.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vaeklret.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pnlzrxeb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mqlsrddh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3sfqvluwa.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kondadsk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gxqkeear.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mivefqrv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uloszeec.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jmssgqrf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lamemubw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3stwrcqnp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jnsqfotc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kjzjhuwb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vangxruf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ocphonka.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3stjwgumn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3sgafjrta.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yrecevlv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tpvvpaje.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pjzwjidh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3myuvcfxm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cogtejef.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3judjvoxl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rsodbsjn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nxhresss.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yothwwge.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jksmcoit.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3epqqmuno.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kwfkysxf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvgodorz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3slfhqhwp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3twhdyskk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tjpspwsk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ziqpfukz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qbmlcdpn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rehjwvzm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aycheopf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rsyuaepl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3agodrjft.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iidlcwjh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jzvlsofp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fupechnz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nowwjqob.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pkdqvweg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dywsaaac.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3doqyrhaj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nydxqzql.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qkzjreyp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lifeawwy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bpzvbtpr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qnipoepi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3frwkqlez.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dzwggkmf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zovcsvei.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bexziyta.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgzycqbg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3atfpvaty.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bzmnqgid.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zzvmurdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roscbpem.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3svdljwre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbjochay.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gpfptmxy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wxkkkjxt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qwcbyhfh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3szdwvpqz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xirqzsne.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yyjhtrsh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3cpqlbily.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3buhwpapz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xlvbrvrf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lzkjxmei.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gzamhqbl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3uyvgeudc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3cfixzjyk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nxxolswk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3azokvggq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cakonyfc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jkdocwjc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3luolnmwi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bkzpmuyt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ntbgyott.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ywcukmim.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sppumgoo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3tilgorif.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwxwtix.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3axdnduvz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbqjpmf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ivifbasl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zqkqvkpk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3iqctlejk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nimgxxlk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3irpoumyl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3oitxmhak.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kotwumax.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ffocodbl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3defpuqeo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ocawtrrh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3lkjamcaw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqgrfijv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nkrobtah.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3phjggnao.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hjrkkeyc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3adxbwflc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cxclwmmw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ougvgrmw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrxcsyal.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3uvpbyscy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wkqtyykl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ravqdvnk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3aofmghbq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3tmtwfniy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dxcrlczn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uzybufwo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tommmhsb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3evqgjjeo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oppkwidh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kvaxtwph.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gtsetmcf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lgiisknn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wiwdewyl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xecbdzoa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dvhiylgd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wwqbxrac.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sdsqlugl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qkizntbl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3akorclnk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3smgobuiw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3axwgxhll.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hgihquqt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3psmewmfb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bihpyfkn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nsdnpkms.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bmjxdmup.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wnzzgfgn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kgpsklnk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ttdvlhoj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3cezifvzr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qvrmvrbm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3tvvnxrov.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rkxcogcd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3veplzlnd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3buiioixf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nbfvmwna.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uxpjkhee.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xpidbccu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nkyheefl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3djtsvcrl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kcdcqipj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wgssbwzn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dolswrda.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfwcewk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rkjixyow.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zhcizbad.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3agbqghwv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qscdvwpf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hcamawkc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgoqjnfm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gfjhkmom.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pzyfickx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xxcpwgde.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqdxjtgo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hzynrasa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hecuopiv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hmxvimrd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cqrgkywa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3psbsrona.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lmvasjtc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3iefqptje.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3mksgdtzj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ozomfeuh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yzkvgkhj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3drepetzo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ryvmtrfo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hjnexmzb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3yuuokyqj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3senqbclu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3reuywbuc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ufmypsfz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewthggjs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zsyakldu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ijuyohrp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gbenxhvn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rfeettxg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zwstsbjy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3shxdaokl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vcwlqffh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3oeddbwzx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qevvnmni.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tiazymbc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gzmejdgn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pekvkhuu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mvolqjlc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivqjjnoq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ubgedkhn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3outovlur.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qgboxkrr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cfdeuqds.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3njvahybr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zuiesccl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ntzaxmqe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3crhtwqhr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wicldlbd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ttdlfqrd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3etrqpaih.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3llltzqme.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3shgplgij.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zkwodped.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3awuadjnz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xkvpiybg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fikaltgh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3eunagath.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tptnjwxz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nveahvch.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rftfaemh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3inmmkjpv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kcibswwh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3waappyop.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kfblbwjg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3slylxkat.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fyurusvq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3hnekcdzs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lgswgujk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jdiernqq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pbhjkfyk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3medikucm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3eskuaiya.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fjumhizq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ymguhymf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3idnsyxcz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wurxavoj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hwjbbusv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kuidwgfb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jzytueuv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3rpxxgssm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fswipwcr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bmvxuqrn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3asxzhcxk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bggbtbnj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yuqkyzaq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3olcgwkma.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ziiygjwy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vqcfapef.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3prhenrtw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tcuxatcl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgdjncdu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcpmddac.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fqdvchth.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3enaajupy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qkxdtyhb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wyqgltqh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ymyqsmow.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3uiohcyku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jqjwbbuw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ttbcghqk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mumlzdca.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3eqdmwdwf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3owlexwew.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qxvowihq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pzfiogfp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ibgvlgch.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bivtwhik.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3iuzysiey.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qltxlvon.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3cadauzyi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3idkaevpa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ashjgnhb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xkhplcli.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wqfhtwmi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sijnrxgh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qjoxjglk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3csrjgnzt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zfqenhvt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3tcbonboc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fcdqiorv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qvdvjpfv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3dsukmypd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3glaycaae.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3blmfjsvs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rspmcrem.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tnbdfnad.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3brvijwmr.html


<!-- 参考信息 -->