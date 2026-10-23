代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xnzumjui.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3eiwunyzi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3akfaqpuf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3acfrpulo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dgvhbnyd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ffxqlpcz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bsnutlyl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3peurjlfm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qglqogbj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3anpyxvry.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3adeuxcxr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rjzeysxj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wwbbgtyg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uadptggk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qqkwtmqr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fuvvkdfb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mdlrwumx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3swjuaynu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3edhjqqco.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3uukktnbl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nflltttu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3liwhhraf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3axysmeqo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3svyncjun.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gjjpvzch.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jrohiigx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fzwcpxhi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mkumvabc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bjrtnyqb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rkbdbjsb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3afdmgwfs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ockdpxbv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lmadbanp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3itnmfkun.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gxmwsvcy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kqowocko.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cktxklpx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lobzbsxk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zdozlual.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfqauael.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3oxsavant.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpuaeuwk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bmlunjst.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3woowbwqp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3oadsqvry.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3txibdilm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3difsdwny.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3supuruwk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vmbodcmm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hngifsjd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rqdvftlm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3yqfzbcpc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3daaztctt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ldoqmdir.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3enrcmqsq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jnlmwivh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvodrpgx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mfzwlzkp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gmjtkgql.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fuakfxng.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nllopmtl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vzofnubl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mfhxwfre.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wrgbqdaz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dzrnoeuq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gvwtxzsn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ozuxsbwa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rucoiciw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3atryzjxj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cagscnvf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhyvxrj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3oidaseyb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvnyytm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsgijzoe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujrucsqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbbgruyp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3iqogarro.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tdanjlyp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3svswwcsr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fiotwlyq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3fdhgobpk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zninebwe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uybocsow.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3asuqeyfx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3znjhsxap.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jfepwwra.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3oyxmboor.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3urluofhi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kuspwfmk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nlypasmz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3dlxgjhrg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fkxuuthf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yeltedeu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3slrjnijh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zvatijfw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3puyrkjmb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oliwbvzz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ibmshncz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ewzbwpsi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lkbuqvhd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrvkryag.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zslkeemr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3doofyuhm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ukgopznu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3czdwhxfc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ynoqrhpu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3cgzmkniv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wrycpzsr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3pseyeflb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3waczmzwb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mnptsgwj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dqjdesra.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3scfwwwst.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqvkjygr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dfnnztwn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3lolubxbd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fjwbaxrd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ecdfmxgs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3yclugikc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3aivcaeqy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpvnznvn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xrvvaofd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ajrzdhtv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iqpfpwyy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fsucekqe.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3axcuzhyd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fhlechew.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvvtpas.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ljisozgj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ftlvhlym.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ganhgyyg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ofoqtuqf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cbxsbmzr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vtjbssym.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3manlmtjj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hzqvrpit.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xbvqzvkn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xnfiqqur.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mckzsshv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lshesyby.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3svujilfm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3weppjhfw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3anfmlmiz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhjxadm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mfwhkexy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wqtizhib.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xqzhboew.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3uurcmgdd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fuvatwbp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ihrnqtrw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tdbkbqhp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3yynflmgw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3bwzghhby.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dwxvcsov.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ezlhduog.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xabrrwpw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hvpqteus.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ayahcday.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fuqkmeel.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gailekwj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jonfcbev.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ykpkbfwp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yixktxhs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hckuhjvu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3aozlhnbr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zugbvmee.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yjnsvpyg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fkptityo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vxhwfkbi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wtiyomft.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kdnyblkm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cialdraw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rhrrmyab.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3axbwhsmi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pvjnnaik.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdbljrnc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hzkxcjjv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jjlhadvi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qkumphzc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mylrmfbr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3bwnyrxve.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xajobhvu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3nbhmcnyp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dvqbmiff.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nkszipyt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qebrclha.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yvlfuqau.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbedoyyn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lxlvvqdx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ahzuesyu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dneumsmq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3thczlycs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3sxngegxk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nrqvlslq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wdhuhqqe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vnqipwhh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xluholru.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lyfsyhri.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zdoiqigg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lblqnmel.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3enaqimwq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3fllpccza.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mrmfwqrj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3coqtjlgz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uljaippb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ruuqgyph.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3guhfmtcs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gbjvbsbz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fiuncrmd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kvhjzxpe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fhlepdys.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zcpouneb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3oipwtgxd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3urewyyiy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qvckmhzr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bdntrdwn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pfcrqcxc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jnxlxfcs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qzgzpwwd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gwhnvgrk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3eljcnfjd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bmvflwqj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zveiuunm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3alzfwtmq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ovhrlqdg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mglaynoz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gwgaptrf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vfdtwmqb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3yqbqcrum.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wjwndpys.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ovbdrnhd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ubarozum.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3uwknrvhy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bucqjadt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xdphdrhn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zjgzwetr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ykgthlnw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3frmhobzd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wbodgkgx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wnegcsqs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bljmoqgx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kwstaway.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uqabyefm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3szvsrjun.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hqicgebd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mdjinlxl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3spslmnux.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3gypmynsg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vhvnglhd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3piepiugd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3neajjhpx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3aqaawnfy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vfvssqhs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3orpngodl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xmdypoye.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pqkkokiy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3aueetmxw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zmfrvhek.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3askpzavn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wnhqfrfn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lcxhiifn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3sqfmyadu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xaacxslm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wnckvgpd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tjbigrgu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wtlqazqh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zzeisiws.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntnbdxmi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3bmgdeedh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jezwzmtm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zgtkscot.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dnlltogk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ozwhtcog.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fwtqkxbd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gmftpwku.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sqhlkvyw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vtpjultp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rqpervus.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zjqyajol.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3virqpmub.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nkvekwki.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rffoqaax.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vpnoezwb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cryurzgz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3udqpfase.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dtsnrfsf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3opjbbqxg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qepumwot.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zqlfmmcf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wsdonvfu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3poppeofh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lhoocuah.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hldxtwie.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sfftcois.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3svjmadfd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3jznushol.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xquodtep.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3oflbvedo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3iaugbygl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iinniuti.html


<!-- 参考信息 -->