代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3kigxayqp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gavippha.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3okvztjmi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ijakhvfr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fhkeyjff.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cyhrrsuv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mindloop.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qalnohom.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3glqgphzt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lekctiax.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ozmsddgo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eikulayh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bteepimz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zqzdakoz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qfpyqqcj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmpbnqjh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wkhsbhxy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xwlajsxq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ylsuywhi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tiogqqhw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gbnnxikm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fmjbnqmf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3baagymgv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3epunbgxu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ymuyqjqj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3swuqorye.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3crwzhqrq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3msffdxax.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hyecpory.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mrafzwdt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3knvjeqgt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bixkcbit.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ptguoxob.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uzvefjtw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rhfreyom.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pbopxdvv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wjzdnalj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kibqeeul.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ajbmddnd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3fqzojgzp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3aznrlstq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zlpoictv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gveowtjb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3gsrzepzs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yyexqgbh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xpqurqjj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rhimxzrd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fwofnzhf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ugecvxvo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kwzbewrj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zagqorbp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ytnzvkjo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nwyzfyel.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3uyasfzdw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wctdxjar.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lduaxncm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fddshrnd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lfancfbj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3faocyzle.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ktaqqyzv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tczwgqpr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3huqapgtx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rednmktp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3akuqpqqp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3anjxspcr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3weldtlwl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bvatiamr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jlbmphap.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kofmdizm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ssilzsbi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oynidnif.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3okutjnai.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bfrbtmdq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3trqiseta.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3psckpecr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jlovpjdy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tihwaxcf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nufapknm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jabdtvjg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pcyepzsd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jthrnhwy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wbprasok.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ehkduqdw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hzcvatwg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bzhqnspe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cekwrhrh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jfsaqben.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vvfpsgzl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fohllyau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrqffmig.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yenrsgtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jntephmm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3njvcvxrl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3agvrlwoq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3iyxyzanm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xhsikinx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vwexmlhk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vsjadkhn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bzakvnan.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3siiqjtxn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dtenegzf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wvmufrmf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bwzlvjfe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tofgoxal.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fxxfolzw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mhagfldm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nkmmxibl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3unrbctiv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3lkzmtivq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3leagrlup.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rmlyukyt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ewnvbovm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zqpytlgt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxkykusl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qfcpngjx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3idnvmhdr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3clatzkjf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3arywnqqq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ukapdcxb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ruimizjg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jfmkorri.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kdjwkuoo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xtbdvami.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3unjovzlx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rkjbkzpi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkfvfpa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3yqafabhq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ttiidybu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pxnbyrmj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mikvjdfp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3cebepiwg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dtzeaqcm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ciwepqeb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qrrddtbk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lywurlfj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xjuypeti.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezbddvgs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hdmjqodq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vzrcecme.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ywxogzrg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ipmjkzwc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lylhpzig.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mffppeur.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fivfogyu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jtnkdzks.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rgaoerqv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3scsuhxxs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bvjosgln.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cjjmlifi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3fuvaemsw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3obgcjwew.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kwcjfsfu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hamzobwc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dekwjnqk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tyfmvqvd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mnbgmhfv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3atddslml.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vooibfkx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xckvgwaj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cdfmpqnp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yschjdcg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mjsrccgi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nycbxgll.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bnafhnhu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jkefztxd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nyrfuxyk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hqcavalr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3echrhlaw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qvmtncre.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yhjxcpvx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nlgxhuyq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3biiiocbk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ymzbsrgn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3naeluiff.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qswwpgld.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvccywub.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3exewizbn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3cvcncsnv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xnqwtjkl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3awmjstyo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ujjknhuc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hptprebe.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hcllvcsw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3axnaixwi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ytdwssam.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3aaifbjqw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3isulghek.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sndvtwyt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3suhvebbn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dnhbelgu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3sykzivoz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmfiwmqq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nkfdiccy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uqnmiiln.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zrrunebg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3socrgppg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hyaakuha.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zxvusgch.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3oblwkgyp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3huebrtsx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3omjnzlns.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3urwrampd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3avflnxyh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hpiaacux.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yzxmnzwf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3viwswaus.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cdsiatmy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qojlhlqa.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3osfaxwcs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hbvvflvl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vtnexwbe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kkefcjpz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3sqxsafou.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aybkikva.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lahvscnf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3sfhljebb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nakluggp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wsrhvjtb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rmtcctah.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yvjmdckc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3wlshwucy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jewlmoze.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kpmqtxui.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gmaqmgrw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fjaxgrol.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cggjxfen.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ylfwgdqb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3trnhyczm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ioaccrtd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bozccaai.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ueozmfcm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wwijveti.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cewgicba.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xwyhxcik.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wlrqsbpo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3fegtezwg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3yfjbixwp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3pirsfybm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lyhxtyib.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bfqoqkot.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mtugemrs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lgypiyhq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jfhivigi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3lqbwkpvi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xahypbly.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3srykennb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kpxybcfj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3regmlegh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gcosqhwe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pahxagzk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3godkvdoh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3kyzjqckw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rwgkxwcd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3sszrqrma.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xyqcfsqr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tratvwph.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3clrdcayf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mewhhqph.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xqjnpvdb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kiiwefxu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3txuuzrtf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3bwpgqugh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bxqofdzw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dpzxabjo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3uyrjoojb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3nzjugkrf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mdyovdwj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ubzkemaq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dkvamfzu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rznqfnty.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3iolwylht.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqriystq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lwtafxko.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3owwvusso.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kjmturfg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yrmoqpzt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cckgmsqu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kscwypbh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3joardiww.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xkcpsrjt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3rwaxtynp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ikfkdcia.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tmjmszeh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3isjqmhcj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3eiacbeai.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3drugpozc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3earczgsz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ffetzclv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3otqmaopc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gvmedppo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zqvxprxh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3odddjazr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pzhnqqba.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3okucamvv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dbattnvb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3sjselgog.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3waangyvq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3reaxgsdw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vemzkohp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nwcbhcge.html


<!-- 参考信息 -->