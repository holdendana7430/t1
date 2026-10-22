代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2imflteyi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mnykiynm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2casthizi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qciysjzf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ohnocgzz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xvuixeev.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2uyorezip.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eozxuwxn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uldarjls.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ueppakoa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2faplboqg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jtunwdtp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lseelgny.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qpctpgka.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ojcigfmy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tmzuvsrz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2sykxccpv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fxtsmylh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tvpczxph.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2thjbcaxy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2litcfqxr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2sfudafsi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2akahyned.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xjwgtyqg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rlkhbvkp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cquatkiv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mbipfhwa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hsxkarqv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2igrqxfxd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rbfwnznt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zsosgxhc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nqmutyyr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2enddgnyw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2iwpgipeg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cqsgfnzh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwrudnmu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rwepcpmx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vvilhnqz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zadaqvps.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lgadvvvg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yozobkwz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kphtybdg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wriqoovq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fsxbjuze.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lbppkcri.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2knmvsngu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2femlnlma.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bpmgysar.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyrxgjqt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irnhjdow.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ujcaqqgf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfnwkrai.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vxtvevnp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mlkxygcv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qndjxexr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2otevafmq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2juhbiurx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2siqkkrls.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2emejxtiw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xykmovlb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dmtcwcmo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2phjvvckx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uzwanxgx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2obdrxvun.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wixefhma.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cxlepqnb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2elktsyba.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xqvbmvey.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcqlhws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfwnydss.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qtpdmypb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slyqxefn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bkmvjmxq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pmvymlsz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2aurqsouv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xlkfbjdc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bzidvtdl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2hrbmqskk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2uldwxfvf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ayddagky.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lhbspnct.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bzfidjei.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2kcfreiet.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xqtzwsqw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qosolrcn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2figemqrq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2akhkxboi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xwtlgwja.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ybnjiraw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xgxbzisi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jtldbjmh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aznqwbyu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2omfrheoc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgyctkks.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ebggkdve.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtuqusny.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2psreoqgj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ixhmozzy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bkfbetle.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qwpbraby.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ovdhjzar.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2arntvask.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2azajdhgt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yqjrvdcx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ovxswazt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tlqrayss.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2sozkiqei.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2azpmexfx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2axcngtcb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uscojxwm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mcbdiwij.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bnrjtdhk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2uegzubxd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xnylyuox.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2egbinamd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2scrwpeav.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnmdztop.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2aozqnsvk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gdyrmedc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2demxqbqq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rsypxwuk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hodgvfcz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2asjzclvm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zgdfpaoe.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2gyrytcdu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2yyzgguht.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pzqoxgvb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2shiqkeax.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fnddvhxx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dofscoxb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xnhlqvnf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tznhrohm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2vmnwfcct.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nfaavlrb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2coqgaiyg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2fnjyvvsk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2iujvkpmy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zmmcndgh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qnovyysr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2iwhyibqb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zajsxqnf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2najmgdjw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kinuniyo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qynukqfm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qvflumya.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2woimblnc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2uowsifok.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cecsnrss.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pyjzzinb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ahdsvlic.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2epalxclk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2veoeimcy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2tdwgwoyh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tczxmlhm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2kcqoavnu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bsagwuau.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qliyolhw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hphuqhrt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hfokfqud.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kqduxosm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ktntisad.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qclojusr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kzlknznx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qxozprfc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2gyzzqnga.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mzyagwkr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ieifkxct.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dafabqzv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kpyqwbtm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bdjwzfue.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ixgqfkkp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2sqyylutt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qtfpeuqb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2quykpwax.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ancssxil.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nokjtcmo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ddqemqym.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rpuxulsj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hslibkft.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2irqyfmji.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sagpfkdm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bxbqvrfq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jbvcrunh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tkpaitwz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ovkxjzge.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnneicdn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2kgfcymuc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tebrozad.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vtljeqhn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwjncghk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cjxksynm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zzmqetkf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2veiwkeeg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzegzckl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ebszuius.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rhwzuzgn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ynytjrqy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2otlkonti.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zjdpdmnk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2aahgzkpn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bpuiaofb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2awswqhyj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lesjglbk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jbbpxobw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qunvzncj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qysplari.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wdftkgeb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jzpgbfff.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bxpbjhbp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mannpivk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ymuyftzs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2undfrfer.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rlkucfef.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2iuavlwkg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wmzusbat.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zxhwoeit.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kgtzqyhn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxwnyvt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ihyvmymv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mmblgwcv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dorbgwzb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2skxvvinp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2armpdnny.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2aezeofsc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2plutyoar.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2adslvdqr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mheightc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vchykhhx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xcbfnpjl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2tvsggkdv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lygfwnhy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qnvzjkcb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nyihwgbd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vnowdunu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2irppfogi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xysglzkm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kjqkcccf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uaxysunp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2naglbnkr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2pgqhznlr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lbesjvlt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2grzbnoiz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zlbcswap.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zqgoekiq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mpuhdspf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cvreplrl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2feghpltr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cyrvsgcq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xbrewfkx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ujkaxktu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2myoibguo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rsnsacit.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzsqmljs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gprasduy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pdbqwrbo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2etvuiwlc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dweyyrsn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lavmhtem.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kpaifeap.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mxosdpab.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2amoetish.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sjrnnibx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vzoekmmk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lyeijout.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ofilnznw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cvngewal.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cumuseqe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wshaablh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wepuyipz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2myquimoc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vptaiupq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ayqnklph.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tzhzuzhu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2usjvrrxu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2qsydqjbe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qxmgyswb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sagotsfr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xjlbkuak.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2gpvkchtb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rqgtjnii.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bkmeqkjj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bsjtdyot.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fbqfsbua.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vhbrhjmw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jdvypvqi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cqvsjcpp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ggytqatu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ahdrqzar.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2cglydwwv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zrgxurdv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yrdccoyf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cfvncizz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2asrgcqij.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2iumksnad.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hmbnxoys.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zprjoyoo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zcyzodjl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zdsgdcwj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2mfrhiubb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgzqvea.html


<!-- 参考信息 -->