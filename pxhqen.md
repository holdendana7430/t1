代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zhgjokiq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3taonoogo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3norhdgon.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zyzoqqwv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zzjzmdvi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jpbwvtqo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jrosqnwg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mctexlbq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hlmxzfru.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mzvatypn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ullbltea.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ioiieimj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3pxvkpovm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3baoukavk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qghdjvai.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lgxhprms.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jouxlxmz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3azkngqfh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kwpzgngs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jvtqqmop.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wqxlddpj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ahgpyrcj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ysbmtabg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3azznjagi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3inzgvodh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qzmuznsk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rlqjmnmx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmvwph.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ssdfxgjr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uzsqaixd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ldjwsbnr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsoqzxcp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cmazoieg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lcwwpbgs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tauivioo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rmbywyds.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dgqabkej.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bnraymyu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ticgrlri.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xokwfvrh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qpvhtmmp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kbrjazao.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gagbhybx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wwjlruke.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3osfmttsd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ukctfubi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yopkbffm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3axfmzzek.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3izzccanl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jnfaenky.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3leigigml.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3efqqnvma.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3byzqhsdu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xeuyejoi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zdjibprc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hegnfsjk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qntutdwa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vesljljy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gmcyqvjs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjothwmb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qrmvsdgm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cjqofibh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pniwaeys.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zztkxgsp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jthwjydm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wmntoqaa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lczmodwx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jgkcdpfg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngzjovgj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3youguxgw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3alkkbncg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ebqigszu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3urkflwqj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ebqoeger.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bwwalrcu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3prudqgaw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zskknqrq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dsosjlvf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfuidni.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nrfzyfea.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wlbebylz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dzyhdpwm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqlqnfb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uimydpuv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mgwtjbjh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3otkeaphz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3myiqrjof.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fdbmpces.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkzvydo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzgphchn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3sfdeqyxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdcuigyl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ckwaesvu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3empvqzoc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gmyyczhz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oymqgvqh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3fpkidsfm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hihbhbkm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kdpwchol.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bxmdvbdl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sblcrrlv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3osysqecf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3kwskxdzu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fbaufnct.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3dbymxvyy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3apmriaft.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3eyseavjd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mratvofe.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jfykkfxe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vldpyree.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dseitgzx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uhtivupt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hrmlzvxx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ronzmtbn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3siijnutq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3twjvuind.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ndjeyjvu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3eilydrxb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ahejxqyj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rgibaanw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3yrfgagay.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3oykbjnek.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ipjcujvj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rvgqnuce.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3eqoyvnbm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcvrzqv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fqlpcxay.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rhuvvenh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gvfpimkn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwthcqwu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jsuoctth.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qdmvcmpw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ykndfzsp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ftfgsnua.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ycyihuka.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hmfwhaqs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fpwjkyfd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3pijmvzoy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vreuflxu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3haclnxxu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3knvqktmb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lgusxhub.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3crzkvqzn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3okpujezj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3awrvadhb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vjbwmlvw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hazmdvqw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oekhmvge.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gipnrzgz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hknmudcw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3okjarrvd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3dqcnlick.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ywqtsmxn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3znrljhrg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cwpevajz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uguoyqak.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rjgqgapz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ntbnripr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3dcbqtsmt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jivzckmr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wlcamtdt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mmundrkg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tiuqbvbe.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmqpwta.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3flqbqsdg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3eyruhfzt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vmnljnnt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gydubrbg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wkrksifc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qafmrydg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vskmdcvj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3soyulwtw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ytjdbnob.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rfdnotjt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pxjamvuo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gafloedy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ovxdzqie.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bakcfwpt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kfyyghrt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cjnmxsaf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zubbizgb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xgquudhf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rmwlaflm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3iucxsyyq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3raonybbf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lkgslcgy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xylffhyc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrvrspgq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cxwqwzaq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zgjemyuh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3klcpeevo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yogsyysf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dsobuymu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fjkdfgww.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wzsqexmq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kxsejuwd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qjdezbyo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zajffcpy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3btsclocf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xrbjhhmi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vlbcyrtv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ztuutrpl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3nsobkyeg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3grebxase.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ffqrcddm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltfaisok.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rnggbaxt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gotxmuri.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nywzyyky.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jmqcohun.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lsvslzho.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tmybktzo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mytlyvxm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cabsnmeu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3kgumvtoh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3syyzhpzk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bypazncb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3jqslzztv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3omkrzjcw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xpanniqu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uvezbqqn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3joogycly.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ujhcblhc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3eucbkdpd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ttzkxzgy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ywzkkzbw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mpmxqagx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vyvqgwgd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3uecxyixi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3gdpyfvwm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3artwbklp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3aifuicoe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3spgiwrwg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pbojrfdv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ylzuyflu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pqintzbc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3byrsotyh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ohoskwud.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kghfdxaz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dsmsvxze.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3dusvfzug.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tpuafcac.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fpzsvjoj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ujxxceqg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dcimjlgw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3yhqcfopt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ebakmzuf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qtotlawf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3yrsgkiaj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3isiiqvjr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jkwbjwyy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nkjjtzao.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jiaqqfxc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bupcsmha.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yavkqhgk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3blcfdios.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ksbxssys.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ssgtykps.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xhrddttc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wsvxuyuq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mmqzvmvw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ymobeyuw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jusvqubv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ghzymtqm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kkjlwjqj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ovhnopqh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ckhzyjgo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uosmaglt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lgerexvg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lzzaugmf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uatnxnxe.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhkydko.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iypgdiuq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wwibuuzu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jszehyjs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qrapurlb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ykazokrb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3njbthrgw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ryepomzk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lvsfacjg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pgcmxrky.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3udfrceod.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qafupdpw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3puvdaaij.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mydeotsi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3evxgcncp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jiekzbie.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hdkvktws.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3neshlmpf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3djymlxgv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sqskwbez.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3flrgldky.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rlwpcjnz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3waefbydd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3rwbddkbb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mqxruoqq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bvhhrdak.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yfeveuuv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3yoiupxsu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fixfhybd.html


<!-- 参考信息 -->