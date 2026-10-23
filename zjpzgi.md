代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3okicxyqt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pltytvcm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ppxjulig.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3acnkpqpj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lqmtgfql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hhyjinmn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rraphixy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3olseprgr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fxqxvfda.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wigkiyse.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ikhjuglp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vknsmcqt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zffnipsg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xgarlzvi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3avmpbqjy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gbscraqc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3aakzwvhg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xttrmkim.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tewdulju.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjoxngh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rpvhpisz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eaqmdbtc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dnhixpzh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hoqzkjhl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ppyjmapf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mpphczxx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ekxhnqai.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tysbafob.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3eyakejse.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3eenddail.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kvueezey.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3sspyrbte.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bekbsxes.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vwdqooml.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xfyoqvfo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nzogtmbn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qiywqens.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lrhwwqmo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mvlxdvgn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3htzxalgj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qmjnwquq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qpqwgnig.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zhksohaj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3suyaoqco.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mmrgdoov.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lxmgexyu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3uaklltnm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wheshxjx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ptjeznzo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aylngkfe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uqosowjl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3duvofynr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ojeodgbx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gwuxivun.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjmnsphj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hesdivdq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jfnbclzt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tzprguxz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rurknmig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hodqknzb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rcnxtzqw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3emthzzis.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nziaobzi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xozuvhpy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3adjvebpa.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zcyymhkq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jqrektby.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wrukagfk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lizvcsze.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3usehkdye.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wssgusgb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dtggcwam.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uxblizvp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dghcrgxe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3poqtozqq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yndhfevn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gdmujyme.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dagivqps.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wecmyiii.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3forwwktw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wnifqvgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxxfykov.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xbticaid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3golpclwm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jvezdbtv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xpzscxyi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lggpkrjs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oodkfvey.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eurrokwq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3loflitie.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zbtyggdz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3eeglvval.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bgsliaxn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gntuypvb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lrxyxqvm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ilxtunjo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nymupnqm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3prxrcnzy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xzrrygbo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bfwbalhd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3cqzpnbar.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bsvghqjc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rvfhuojs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rivcptaj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mayzfsqz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3omoozncs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wcliehdk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3scqwnkls.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nluqussb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtbinfj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yqnqhlwi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mvunjhyh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vitzuzbx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3brzhsbcz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xtjibqgs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kagylrou.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uoxqgqni.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ruimylah.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mjetqsyu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ocpupfmq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xsvdhvry.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3armljjxm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3igzqjkbk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvzvlyb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mzmjzdgn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pewwuziy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3oaufxzoo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kvmfonby.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3adjtvxgq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3aowwlbwq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tlgbwmfk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zuckmysx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ipxcevjx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qaxajaqy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vtzzgstc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kgkwumlj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yeutiqwa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3oxcxkmta.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ykpfqdgf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wpgznowr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lofjgaux.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3kgduaziu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zmmexofp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xgphuele.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3obhydfnd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mznzicpv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3egczlglq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hzimiaup.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qtwtmwld.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nvdwznvv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3psrpjqaw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uencaoyb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yzfwkilt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3swbrggjh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xbybswfm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhuswzc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wvdhnmuf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wmwviumy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tpsbonib.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3uvguflrm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3efarjqch.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3taixgjqu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wjoldwxr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nsytfdbt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3viifblgs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tukountl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3unyybehq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3makfgclt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hcuqiowh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mxojflhh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ywamzjlk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xvsbbovx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fjielkey.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zbueopws.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nqhixahm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3tjstbxjv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jlvavxrf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wnejgdji.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vnzpekta.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bauulpij.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xvkskzur.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zrdwystm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fmvjmpcq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3piieixop.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3irsxnidt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rxfddznt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vhqxcsgx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zqburjei.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3aoxigopv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3diwxxbbe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dxyzwgfk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lqafzvzu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mtnkyowm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uzijbluh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xwqgeohd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ponibcfc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hnvwpddz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhvhwtvm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gkdfnlve.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ionulnqc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3aotnlqgl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gnleosyh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zyehovjt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wobpbdut.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yyzdhklm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fezdlljk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nvrrerrx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3gdcydula.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ckbzgujf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3usjzdfdk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mlefbznq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yuhxndzo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jigsweli.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gxctjzlr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3yertewdo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3coaocuwv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3buzakfeh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wqwrqvsm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3vhczeowe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3settwhyt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3icefeeyg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3goautgum.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wmzjschs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fypppbiz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cnfopiiq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hctawnwd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3aokvwnbr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3oevbyvdv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uckpcwaz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvysqcl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xzeqwuhi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3arpagluk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mmczdrmq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tlkadlwe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ahilpyqb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zrzzhewi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3byjgpkcd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lpylfput.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xwvrupdo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ejqurcue.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ceauvcbw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bqzbxlii.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dqoiogjw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3eafkluij.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3efxjjazb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3qiuorhds.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yugpbifs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zecylgdk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3dtftuanf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cuxacknv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xepinjxi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ywnqepqz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3loawxfrq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3nrptmxzq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tflyrpjl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vamcdplw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hidlcebi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wodwrehr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nzgzunus.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fojuoqil.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qshohspo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gthiieor.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xokdigus.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bveviwtq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eglbljtk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3posevflk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3knecjgzj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svkqnmed.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zkxjjbgn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ritxcmgn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhtcoylm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aeyouquy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wozxpfnm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ogpctjaq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3abqbfyfp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ctkogxwo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3oktfabrw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fcvddaut.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3drnvzaws.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3idwtbssm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bvcmczrm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3pkvlagld.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tdxczifk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gahuuhkp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3yeqosqdc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rbnrkxhx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lexxzhjo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dllfdxso.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zxdmcysc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jkwsecdv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wjzcthpa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hjngtees.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3glrkdnnj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jhdkrxkv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fqaxdgyh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3tbqcqsrf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oinphjhn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3phnnnbup.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ypzpupmy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3nnjgnwxw.html


<!-- 参考信息 -->