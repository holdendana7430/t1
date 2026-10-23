代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dichfpmo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fzsnyoai.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dkpyqjaf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3khopouro.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3svokfcuk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rvaermwg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sjcxzwyp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvjpnll.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3eddroeps.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kmtsvkoj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lfsmtvjf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zoumoxfq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zmphggpw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3comitevr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vdfflyzi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zcbbfjaz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qfetzudu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3teahdsra.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rqyhhmfd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pmkbjebc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3caeqorpw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qxfsnwxt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sltunvre.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3opdwkjai.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oepsejek.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hcczgybw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mmtgrbpw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3aysirebb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gmjtmjbe.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3imuincjs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uhfxpcdm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bilymctu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uxosbxqc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qbambdjj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3anioinig.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dudhreoq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bvmyxkba.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bwcarhvs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ttdzujym.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsvjqjtu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vtzeolyq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ogbvmuea.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ybukihbs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xargmerj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sotiqdma.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3plcktsrj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ngonqgcy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nhgwupuc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jhfgvdkh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gqqpophf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xnfcmgkr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kaeyftxt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xkmrhrek.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3djyrtohw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iradxjhf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yqohavcz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3emxqlvtd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mjzwamgf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3citjfbqx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qmrmpvrk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fdghqaav.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vtnhttia.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydemxmwu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fmiytbzc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iqsqvnqm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3muazpjpk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3eszhnobd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zocurmql.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3pemzbudc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hmbpnwvo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oqrpvelq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tvuuljby.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3uumgsvmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uiktdmkq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hiyvbxae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anktxzch.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qxgcpvmk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mphiyqtx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jbkabnku.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nbjsoyna.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tgddstuh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bjbtcjiy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lngfnzpo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ihyqfbqf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gwrdddaj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3geicodot.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ztgjcbtr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3iaihftmt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bouahwai.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yjhcltzk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qqaopmxp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mmsmekpf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3cwnopwln.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rnvgwcxm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3pkatljfs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jxpsuimy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3swqpfdra.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kakvyipz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cosbikrj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ximyplmi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebxxgjtz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3juwneogc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bdtkgpqc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhfxawv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3paszfdpf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cebjyjtn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cgoubvbo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xlryugbh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xhfigqnw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpbncwz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ukavlivi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ftvwfglm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3myuinksz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hniqpzrk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wzzvnhxn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lrxxbarl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3laakbvcr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3obhtpsgb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3snccfxos.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bbhrweys.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jeptfvfw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wwjmtkms.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dsruajnn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqddxqc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pmmtuiqo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3dwddpyso.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3igmrcjef.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrsfcfs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zrovzefg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nmlkhkul.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3uohwnquk.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3smqckgks.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qjmdvnls.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xldbjvev.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xzcdorwc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpkvsoy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kcecbyvc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3phyqmduz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fgqxaddc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3msqfauwi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3aozmlgps.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tebuepai.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3unpqbogd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3oiyzelrm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wnjzgeyc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ohzkbyet.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pefsjyho.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3smkdcjap.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3suwofhnw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zoljysos.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rtpqjzcg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3pycmpfpz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3riavmnuc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rpuqwjbu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fwhdujry.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xnfegznc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ifflezdv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sgcgohsp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pyomfjsw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrhibxpf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lrcbkgtt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rzgatqrf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zuyesnuk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mabkkkok.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bfskldjo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qwcprycc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qyxqcfxg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cvskamva.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nrvcqgtx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vdvslhrz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3omhbtybp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zxvjyuva.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uurweisq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ycluxnky.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3trumsxqk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jiebquqi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3adpqbpap.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kfozonlu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3onggamwv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qqvpepyw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gdjjbqnf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rruyvsuc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3srtstweo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nxnyzmyz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ymczlczt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3chbcjkdq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbdctbms.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zopprdsu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wduxqbsa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bepjdkzl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3faovekvh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3clauqvjz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nzazufhp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nqxdmfxx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gdkjakvp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tyuehaef.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3osmulhck.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mswaxnhu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pomxmfif.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3felphqbj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3iqgmoirj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3axbltzro.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kpsbnuwp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pzjglalv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ceglamyw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3boaytaai.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3felkqbjq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gbdrtjvh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lczdjpnh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nfkamrzh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lgwhhgwk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hfhawndf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bkkhyyzo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qoxmpgjy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fhrrzyaz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lhhbphob.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mcfhjrvr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kphaqtco.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3edvuguwp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nsqpjoir.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nnyimrio.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tnnxhkpg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mfzlmtav.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3mjmfjclb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dfgdykxc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3oojyvkgt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3riioygka.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yxpcwlkw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lpfoimlq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tpaqqphq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3guwbtpfi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qoiimcqk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vxvodwni.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3rlhdzwrn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vlqvneqd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dnlmugpa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hhecmyvc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zsvplsls.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pgphxcbl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3uimbzsiy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dhvuicfm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3smzbdprq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3eoyckpit.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mksximst.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3efqvfmxj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3onijwsxw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hzbypyhi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3bouuupkh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dokyjjji.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dpucqbmb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3kqirujiv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jszzxywh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3erxmrffw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ddlouwyo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zqxfeivb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pbiyrxfi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3owlzqlnh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ndqkgimz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3arykumfw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogrgbhlz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qxyoxagx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bmumizfe.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkxuvcku.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rcnogbij.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3idkvazsr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ezfiidpx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tpnjpjgw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jsdsstpx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pwdgknih.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uzbhrmuw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pwyazmpu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uxfliaip.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3lstcwcrf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jrmqgtog.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cggposmn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fckymawx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jbpopyxn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3salcnazd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3apspdvwt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3eomfmzag.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qzalacau.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ikfcahfd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3annlhytb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3edlqiucr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sxwzpngv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3uznltyfs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fggasnph.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3eephgygj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qptkprgh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ycyjkroh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3emaslhvs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fetimugm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3onzbfogj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3coeuaret.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3cbyfbxtw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bejdbpgw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3juhmsngt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dnojotvd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jemtzivo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fxwlewaw.html


<!-- 参考信息 -->