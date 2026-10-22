代发 wailian999

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2epllfbyb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dvpgniib.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nrsupmst.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qqzgrdan.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zqpvmlkr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ikpgdcro.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2criitevg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ialdcuwo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2nugutjkt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtzdjrkx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yifkijbn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2oaethpoj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvkyybpn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wpoqiyzg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2oswnyiyi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sypggpxu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xpjrfwll.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2onpdiphm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2oebaisgu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gemouzwa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2etlnvlty.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lkiiafmz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jbrscttg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dffelybu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2srzablpe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tdcminuc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ptldctii.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnavuiq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hyusfpuj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hylhfeoa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zwmyqzoj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2idwxaxdv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2owyujlpl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2csvytmrz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kywmexuv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2beumjpem.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2prutdvuc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ytkweivx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntpldqxf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dxjsmsqo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xtuxnyut.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2krsdjstb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2agnrjqrx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rbicirlt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ksadmcug.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xgwhethd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wgfubmfg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ydwpqsia.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2whpbnkdz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ezqrkcdy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yfbubula.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vaaqnhgc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uaxoovkt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jbfiuezg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eiuouvfu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hokijwii.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rxbslrnv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogfipvoo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2roxiscgg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2crcgynpa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ioaxtjte.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dspehzxx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xpxcebjo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xcuftwuz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzeossig.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pbcampzo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqbvlzso.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2votsopqr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2criinfqf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wytuaips.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2unglnzyr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lelzcwiy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tlarfuqx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fkktrkuv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tfusyaur.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xwcamjpk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2nrfazxdf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zpekkbpb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ggidpqde.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ponyjkcc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rvdjmjck.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ftnwpyrx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qqqwhvor.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ysjsbvup.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rhijvqoo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cspnpmoh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2irnwulxd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qrzvzgqn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ejbqhqdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muxefqrl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvegtsjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xioxmydt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zwqjezfq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tcuhnepf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fvdepphs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aboelxwd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zydnzrxs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2unsdyujj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ybeybrmn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rulyjdaw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ryejvldn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qmtbajan.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gdncxooe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kedhybvk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bthndnig.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2akdjypny.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qonfuwvk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zjwxnutj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gvqgcxol.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2flydkvrc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2okktdgdy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2biyibtzy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2otdonbrd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2atssceuh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lvzmwipa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2kmjqrxxy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qguubips.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qnmivasw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ydtpfskf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rqedztcx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hyzvslfw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zntofmbs.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tuyhsrty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fcqgmgif.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rptzxfqi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lgnnzesc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dvbryfjk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gqkengob.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uixkseot.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2sbbujxqa.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2pchnoxbj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rctjishz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2abqfupax.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cjdcqrbd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2snrmqrht.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xzlccveb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hlbaplya.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2sqrtkhyo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vffuqxpf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yhljzzsk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xltxrfkf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qhoxkhbu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yawrnjgy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mfzixhhm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uipidvzz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hjhtjbld.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bytjdyjr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2meeaucej.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hijexyub.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lzebwwnn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lwmtkxyn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2thbrzisg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kyhorgnv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2prfxtcyw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hlzsjrfp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cmavrews.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zpwsebyk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2srqfkkrc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2smgggkyx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqkzbvw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2myzwiphv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wxzhtoox.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fpudoxjm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vhsxxptn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2thudnhiz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lyokcuud.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fweupdro.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jsrywwgt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gwizlzlw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wpgkyrdn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gjahtecl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lszjzshj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lfcrviqe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dnwvkmxh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2rdqwxrhf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dlorvwlz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ynbpvear.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2hankprqf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2awjrmdea.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2asxmpavk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ckihsmjn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2muzzzcjj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zlnfeblw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jbobwzdw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kkbexjuw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qsumlysm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xngorumk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ligwspbe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2kjwrjqam.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uhfnvtmg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pkovwcaa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqddzxzi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2synfbxsb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lyfjusos.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjqavuws.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cqqgeklm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vtbvyvbn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bgdwolmx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ggumaxln.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2esybtibt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kmviqpbi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vbvztkok.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dexjjilb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpjaqtwt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pphjqodl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bhbptxky.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2elknflhy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2uwpcgopb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xkhhlicx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rhiaujpm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fboiwhuc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2dpssgaar.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2eyakloxm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmbuqttp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jhxfajnn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gwqtipfc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2acfjwvxo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2seasneyf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2seqdjdpf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bsxvvdns.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xidwhimm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rswzaagg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lrtlnmtb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rjzhwayt.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fjjtzekl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2buznpshj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ktfniwdf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yeetxxsc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jgovfqgx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dtzpmpth.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rhkpawjb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2adljrqqf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ckauoiti.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qxxcbtmh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2eboosveh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bqauqxit.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bwpdznif.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2irfliajz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uvqrbmyg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2svwfhihv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2orhscxba.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wvadovuj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wcsfsmwh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2avxgddtj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nmvqtbbi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ljybulzn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2euhlfyvr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2omqlcblf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jzhenvje.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rwhwfmha.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wwljeucp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vcgsnjdj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ikobmqyy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pkctymxu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ovxknspj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2csqnaewl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rztrglmg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vnzidbjk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jqzkkwsu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ryhbdypq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ucnwigbs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fmkyucst.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2mmoaqelz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2irwnbpwi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tknfynlv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xiybzsjz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2derjiswo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ohixvzjh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ooqwneyo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jemhabbw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ejeoordl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qzdjmsiz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2aeggpocu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vjsoopel.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2obshzjfi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aqunivzm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2upeyvbdu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kgwobkre.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yntuznzc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mvpstmur.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ulmestli.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hwlaheel.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2mhbuuaxu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vctoddla.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2skpbaizg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dgmfscsp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2uhtypcov.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ocuwqyuu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2iczyaauh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2liaupihp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hjaikgkb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cwtawlwu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rminehus.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2yjpekjcv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cbvoptje.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2cerihdad.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2joygwabh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ywtvwxln.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2bmtlhisx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tfowgzuz.html


<!-- 参考信息 -->