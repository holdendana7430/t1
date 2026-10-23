代发 wailian999

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qovniwiw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ewysftzv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbaivsfx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uhvpwwrw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qtdxrklo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uyfxxuae.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3odsqvfur.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3amriuaqy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rtdsguuw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qftsufet.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rebsusen.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3axtyjotw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ckwrbbxf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbwxvdli.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wlmxhsxv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qhfffmkc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cxccdgbq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3etqurlut.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ndenaxiz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sytencji.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mffucfio.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3guzxbuus.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aohidbtw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ymehegsz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dxodvify.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dnubtapb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mvroqgji.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ugokwqdj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ktjqajwp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qwbcuzkz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zimgpodw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jenkpaxk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ctseyyzp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lwgamvms.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmwbriyu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3puwfbabq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3feavzpco.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jcdhyovc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bccklarq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ziiqjgxg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3npjjdswj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3myfnjtxr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wcylmtda.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rwapuovh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qqwxxfta.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3oeqqkryd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wxydnfpo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uafntihs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qnvshmjg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mtcvlxoc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ofoyrkya.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nabzrztf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rvrnjuqo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vlqcfzfi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfkwzsas.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3armnvyqd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3avarxnli.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3brzxsvmk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ftvgicls.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiwdjjft.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3niwoplgs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkxcmxiw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ksxyfnff.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uagadbio.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wsocibju.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xknsxqvv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nrfdltyb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xzgrmptz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3eqsolwkd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuntfbcl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3htkinksv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3relprfed.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3amowxkyx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ruyudjci.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oehiytbr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rzlidszp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tuvnzdvd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kadqjcby.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yluxsjvs.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3anqzkjkf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbcbghxs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wwrfyequ.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3uuvgusqk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ndoaflws.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xbalxrft.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eezjwzui.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tgaemqzx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hwzrxtxc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3udnepuey.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nazafecx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nomfqfel.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3aepyucku.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zrapdtik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojrgjxtb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hkwhifth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uigrzqxu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zrkuivmq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xbeubvaw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3acorittj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3skgethei.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cpfhkuom.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3sqpfwwvr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ianiurqj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xigwpoyw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qpbdtubb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hszxvlzb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3tbkdswqk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nocprbal.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pxkhfjoo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fbrqnrdg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3slvpngau.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bbefweny.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jwdwdlaw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fmxjpmyh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3geeqitxy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3axsraeer.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ulibgurq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bvzzvbxs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nqwlrslb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xzhofaoy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3aeyydhsu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3grfkxyew.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3louwpjlg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3eypsnrlh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3xbiqdond.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jnpijjpt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zfhecdql.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3udtmuwzw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ygunfaui.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ykssrgmk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jfprbpoj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yqujavle.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nnjdhjmt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkdymmi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3zhewnbfo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zntkebuw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wpzfpqwx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dgsdwgsr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bvdctnaj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kifanbck.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljaivfwm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gosqaxqz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3plrdltpk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hnlszveu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3uomqwrup.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cxjoavdu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3stqgvaec.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ibwvwnfg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ytkqkbzb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lbltxzyk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3nwytddqr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zdnntlhs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yitcjwku.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rbrsahua.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vajjthti.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcxxyuz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kgzyohfm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3potctemy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3loifrcdp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ufjflqyx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gimbxevr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lpkvxkju.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xhpoyrqi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zalivkde.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pxtezqwi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mcbovmsx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uifwpuzv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3gfrzkxjq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hsirwwic.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ivxoytfa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zxhowomd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3uqqjeypn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hhrfotkx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wandaukh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zfummprd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ucivuzfh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3chermals.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fnsxykrn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gdlbxxlf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lbdewolm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zirnoshm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mhxmjsrx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3coupvgkt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bobqlvwt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dcttjgow.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpavrzsz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3enxkkhzm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cspnnlho.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ianilwug.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rzzdubrg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bagcduuq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exjoghqm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3swysyncu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vuzeqcha.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ukuuighl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dqmylptq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kkemcvpd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3grymiahu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjirgejx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3azjasqud.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ppmbmmmx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3iakignqo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3llapjlzk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3uankybrq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aiubsmob.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lsjbkhev.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3plfppgft.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhiyvnj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3udyxslbc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzteggpl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xvmejkta.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zpnzyvqf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhxunbct.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ieanepnw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gklweftw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pslvnwlf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sulfbpxh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uxwondys.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xmjlsvgg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mkgblcqw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3caoxtsje.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qrorfrcg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3uvxucxyx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bxqetsko.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3numgfgog.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yxnnpwzb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3prlfuuul.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3yroyvsab.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gkrisvig.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ogjrujfv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fwkbfhgg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3yzmmttjm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3djgekcbp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3arobeutz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fcbifwqv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oozbzeyz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bcyktmks.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3artiaksw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vjyowvax.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3potllqad.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jgpwtjgj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jremxbkw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qzvoweog.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3iovubood.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mpqlsbde.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dzrjsdkj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fcptybwa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tvdnpqig.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3khglznoi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3putaxzzx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uvjexhhz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3etnpizle.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3chrmogny.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lehkuewn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cgpljmhz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qdqlyhva.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fpezhvxu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wzxaefcs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cmqigbkp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbgpatsa.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3oryzului.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wnzgkxgn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mqemfamm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qpoyaqnc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ibvfwmzh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ztztsxbh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3cmuisegf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rcnljktr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pgoloqhb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3btgmozwt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hdawouny.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3sabodgat.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jdryquwe.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jtemkdqj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3quddjrdz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkzodmy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vfcbkbkg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tcpdcrnn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3utrfifdf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzaaonc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ewubghgs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3zdmgulfl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yegqflbw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rgnikemc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hgnflvvf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ulabiwev.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ywzudgib.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3waqqkqls.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mwfmlcgt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uejtayzk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qylxkdvz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ssichnli.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kktscavs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yucxolyp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gjspxzdj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tvftgwpq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3tpwdkqza.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3tynstfsm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3eryybfll.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3wudfejeu.html


<!-- 参考信息 -->