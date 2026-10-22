代发 wailian999

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2spggpfur.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2aglprqra.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kbtuzyfv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2udvjagbn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lxgcepka.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wufdxlrh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2oajixifw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bmfxyukb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yssbqgmi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rihtawef.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2alhrfhmn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2snostzko.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vhnnbzim.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rorziuby.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ldrdgvih.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2erbgvfjo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2onmnkoog.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qzonbhas.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dwvbiqnp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ssbsnwnn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vrdmmtrr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2afzvssgl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lershsjx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2capydgiz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dbynxdml.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2idsokirc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nkppxulw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jshqjxsz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rxpojjeb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2szmfcfml.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2dhjkpupa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nixbadmp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cfhsuppq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rpbfzlpc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2umfuwqgn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2kyeadfmr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lhqyujpd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jtsboakm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tjsczdji.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cfnsnwsb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pczmxymw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2epcoceuo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2flufqovt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kcugoklf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2minxrgqe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uoowvety.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2smdvpqsr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxdjwms.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rlfhqklm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hwojfmeu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mskldpec.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pjxnrfdn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2geboqrww.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jsiljwjl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jaylbcjv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtbebelg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gdhdcxsj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2knjpisca.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qkdfpkzq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jrsjyhpd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xzqsexoz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfiyjaiy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tegepmom.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kzdlapzj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2etyvnkri.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jtgfbrwr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rqckrdxs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oghapnac.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jawnklqk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ukqrifii.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pheaiyvi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vezsijvl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfwyfbie.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mzfrveqr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2butkpebc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zorsxwen.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hwiimpqe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jvcqcwfk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kmegncec.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pzzjcgea.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wkpwuysd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jcjztbah.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2smqssvij.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2yagvqplk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxsmiiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuhtnwtq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qqpbzyjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gunpclno.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xrundpbr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2adeyqirg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qpysfwiq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rkpqrnov.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kfrpqtkn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qiineplp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cdakoydb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2szhivkix.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sgyhimgh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2toljvtva.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2npvyrgbz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ukcjfjkn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2enalxtta.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2svzsjmoo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wfpenlmp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dmliunnr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kvlqemmv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhdjzkp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2akevpvrj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ssljdtzd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wakzporp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zelxtazg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mbnhydbc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2flyzhhpn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ygtxsyma.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjciaue.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2grhkvbet.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nffueepo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mggcwrlx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mdamgwhg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nhdkwcaj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fgssswew.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2iueufpyl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2oiztjlhm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ndckcbrd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dqwnokpv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ijvjffcf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvexugsx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yjuiyhvw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2iekbsblv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lnwbqsjy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bvnierkr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2viawmoac.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gsqhrjkz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2shfkaqiv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qcjvbraw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2aiyznaxe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvwqscm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zvbvlrou.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2csgocncq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hkbvkavf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uibbjfkt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rmjoicns.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wdmzpqdl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2gbzapvhy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2isyjqcxa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nkawsers.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gqskamxy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2slntwuta.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ypozywwj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jlmiocuz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2jszddwij.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cckbpoae.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qakwcgsg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mglfxbkw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bstrzlyl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wwiqhlho.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ibzfhlsw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ywbasjon.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2lqkmqdco.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ebluycor.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhimrew.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2lciskjgt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tcxnwiyz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mdouwhuf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2aoysjoeu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jksxmqen.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2frqcrxsb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xfrgoico.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpwivcp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dgqqftrm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lrdyejwu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2hwqvmsjp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hxawsggc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rqsbmeln.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gzmuyizz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfehqchz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uqjzaiud.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rpyavivj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kaiknikf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gzrpgehh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kwuleyol.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2yshfktul.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qqdapohu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2uxrxbqyj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2utpzjgpy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2veompwpn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2osfxrrfj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2biviqfks.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tftrxvfi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zcfgdhjc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mlspmzed.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2exdhdstw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kygjvbdb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2iokqhsaq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rqsuxrxp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2jafklygl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tapsndgm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2umavbltf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qmjadrmy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihysrpvh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rvcwfjzm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dkgbvidu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukxujbyd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2iibecont.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hhhbmrzu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2swjhbqem.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ruzgfski.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gwrejdks.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2evxbdjfv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2kejtltrc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eexzdnsn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jqnuuggd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vwhuxvfo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2usrcqdvm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gnigniin.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ojrosgjm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dojjluoj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rjmerqcp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gytpkoys.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2otkxvvwx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2nsxkjuar.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2mjduwpqs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2olmxtmct.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2awipsird.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2znfzqvau.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mrtjevye.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uoouskfg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jtyieprn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2kbyxuims.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2anrpvaij.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wjjovgij.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bknhejcr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2uxhudoer.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ioeyfcgp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hlblcnzq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nxxjjpzh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pzctwczs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dbxwcdnz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2skgtleyf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uhcvgbva.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rsjaflod.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2uygteivw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qkmgbbrt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2klmkmonj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kruxexhm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bevkvjvz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2smncryrt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2scoeyobq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bclksvrw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ghmkwajw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2shpcafpj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hctsoimo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nsecegyn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bxccwthw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xtvrvtjr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jsxtngcr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2obnfnuom.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uzilopvb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fhacegjp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ubsdgyuk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gxhaocmm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tvogzavl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wvscbrfn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pnnxemge.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hwowwdtp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fouoarpv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aswodxsk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ymgikjgv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrxrlahj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2grjnwqwc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jgxsbrov.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gubljunl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2przcobme.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nagheyhf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2oeklfios.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfpllrum.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qyuwqmyv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2eqshvguq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cjkwuwxh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mpuekowv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2stpbvglb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pdkcvnhf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xsvvpvkh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vzgygynx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ewxoorzh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2itllsyul.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ssnnaogf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhtmfftt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qvomiwgv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ulvgbccc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2fylocfoh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lwlgpaey.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ufjvwydw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ruantlsv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oyhtrxuj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fzohwzih.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zoocwcos.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2aloxzuzy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tgwusfkq.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ddbqtxij.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qashfolo.html


<!-- 参考信息 -->