代发 wailian999

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xvkopxvs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ossiuoqd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rbggfksq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxvfuzs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zjjytggt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3toqykitg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nhhvvbrn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zjegsseo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bcgtzdib.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3daxnwzru.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rjmzzrrv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vlagfeuh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qekqhljf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nsfsmyoi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ssqhuxop.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rrydokge.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mytsmhcr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qpduigcm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wrkotdxk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zcjejblx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uawrfsvz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nxhotuwh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3txfpjdew.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdiechrj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ydkzvcrj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3enbqddrz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3cxebcdwv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3leozxrgt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ayymqjma.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yhywlyhc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fgdhbmmq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ailgbvzh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yravmymy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lartijjg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zssypjuz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zayvzxmm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xecveyld.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lrbvepou.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3evfdxyfs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3icetklbb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mjeailnd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3prryinil.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ptqxekwp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3sazrwtyp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sfjiuspy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ibohsybc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bozqailk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3prbebnbx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3siuesovg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rqqoncse.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qsdjeadk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zhtjfeem.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qzvcbftq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fomzfafj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3liwvkrux.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fikrtmbb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ffkaanbr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gfwllztp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltvtujmm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zjkxorpc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bponrqgx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3iuguljqv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wxiypyin.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jwtuwllw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jiofssdm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pzdpazeu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3laxwktnc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxlfllqc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zlmajjkr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3coemuvtl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3krndmios.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xkspkbav.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3anlaqswv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqisavyc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cdlslepv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ccqrpbvd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhaqgnfz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwpynvvu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xgborlrc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fcxybwhh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zubxiach.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3udxcvfqh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3abajeynx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xzpzausy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lohkolxl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ifkhxtys.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3osdexmjc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ayvtnyww.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rdhofpqc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3inluyewx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3klontjht.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gpjxtodt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3elkzsyjb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rzcccghh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3luntxesx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3futlihwm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ogqxjjxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udfeufcs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xnzoudeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaqdqxli.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nqxfsxni.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kvnxvrek.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mfletukc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qrkmhhif.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ecghpfbw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bofaxvto.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xrlwulct.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uurrwehp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sxqzyhmz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wvggxpii.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mlkkhncu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tipwhvuu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3dkrragau.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fqwvmeic.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3uuhtogrb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ujulklmu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qjqihxdt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dcydjthk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ttyvcbmo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fadbftxe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eavkbjbi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jqexpryd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3anwsigra.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dmtdugta.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3yndhqjvs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3eujymaoz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3frkffwby.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3syjyagfs.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mbmfavub.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ujqqddwd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hlnyidln.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nrqehevw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bzebfncu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3turewjzg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hipuomtp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ycwuoibg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3itewrbjl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywyqkqwk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3emwocvfz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ztbewcdk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3yrtfsefm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3obbxtwgh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qcdiyppd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fcfwwdim.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibuleakm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kcgmlhwi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3eewbhglw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jyrlqejr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3utppbrac.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3iytjlijr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vovbatlr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xlvtuecq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wboinjjm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3scvaxyyg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3buumlbba.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3onytqhzx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tsydmgci.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nixgdrxk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dakyiggu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yypokykd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gouxqkdh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ftpguzli.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ohntsryr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hqbzynix.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3urpdznwb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ndabdjvh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mmwzxxvc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uigostnx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3goisuqds.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3drvlhype.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pzfwpytb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3etbkvjvy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fhfmzjvc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vylhzbks.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3uhuohjdi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nypussob.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3uvjdcfjq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3srmhlvsd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kdjkwdwn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xojqlipa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3etiyqyut.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3olhqtftp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3brlvinzx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvoymdfb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wkbzqvbc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xynexkds.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gzwtkhwg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3quqsrfov.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jjepfwsi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3upoanchi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3utpzazcv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gyhasynp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mwuvdarl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3uzoolcwa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vgkhobpr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npmkuwcd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ewyykphc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rkjffylu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3oqeijgay.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otofkbep.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3cxdzhyxw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wmhzufqp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rtuqyvym.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zfwciupf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kufrqukc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gminocht.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ujvryldn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3uqgnuvue.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kxefjxww.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3iourqtjh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kgfvdovp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zeoqevev.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dcwywbtv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vnfvcqzq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jfcxgwgz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ujegfimf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3plzfkoir.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mmknweqj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nbeygdpr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbzrzbzj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3obawcaka.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xlidddkz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3orwehiza.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mbamgghx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pizofysi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rsnqvizu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wxsroups.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jdexgzoh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ejxodnri.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3msoxbofw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3dkdtxuxx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmzjmxss.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wuxlmmms.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tjxpeftx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3uyfavmdo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kwhirope.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xocmmrmh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxhrysab.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rbefcmdp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hkxelpjl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jrhxxzfx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kltsxvxb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jpkmkfxo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3puxzecdi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3olfsldcn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jjzjopsk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kcymafxt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3phjabzfw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hakezlvt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ehkhpnqo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xipbwqvv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3usjhjgkc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vkhvfbmt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tvbesxtv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dumymcic.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3dzijvlar.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bmeriopz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3yojjqqaw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3okoxdubl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hpapogvr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vxyakhtn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3cgishzuo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ddhsnyku.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pqiiywmk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xkzsnfdq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xmmwtvuk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xhionxtt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tggyexuo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pjlvniec.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3znttzgps.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hkpjvyli.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3prhofdri.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bubpdrqm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gztvorbk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hegfiiwf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fffhuzqk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xlvezjrg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wgczmagl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rbwsvzdb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fckfxlwg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ptheieio.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vorurfnq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wrrwjgqi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ehntpffo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xztaxfxo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3egujzltz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pvfqqskf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ufpzkznz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nlqfejcj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fruylgng.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jwxeplph.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3attygpxe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fgahhznd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mlkqfggc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wgoltemq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3akxystwz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fvjqxwax.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pxcmbsum.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3oafbmavc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wrkkvdsf.html


<!-- 参考信息 -->