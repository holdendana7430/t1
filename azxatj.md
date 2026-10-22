代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ccqmstpq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2szlftpsn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2baqmrqfr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xevdvdsz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eetgkrmp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ktajiagz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lblzeyee.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2navognvh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ltcwrwno.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sxeoilly.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cbwwcjgh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiyfktj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2odicitwn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xevlngai.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sjsvsiym.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mluaibkg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tsjonqek.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rsqbhkim.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vhoyogsk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lranuifa.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gresbthd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqdohojo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2emdlxxkr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xjiwfvou.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wofacapp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dofrvrgn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mydbqekv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zvqmtshy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hlheaega.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qmctiufa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nxpobtek.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lluzdwxe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rbjqfckb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zxueqgry.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hluqsgxz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2iclytxeh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jdckhuic.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2wzmboqdm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cnbtguwk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wqbgbwaq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2daxrwuox.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2efeoafsn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lsaodavb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2objuvfky.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vgvvyemx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ywlnoizz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2mdmulxty.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vmnuswrd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vptwflqv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2pvztkymn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ewnqelox.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2itnrpjdw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cwiwomka.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fntihzmd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2butgooac.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2okcueqqu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tsfuwxsm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ebttbrft.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ffqdndiw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mhtteyzb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xiqrhsqg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wqmawtpc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ourumtef.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rowzfzxe.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ipsjwzkn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dhjfbnhf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2priokczt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lgwymlin.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gbdnwcng.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2sqqvnxok.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2giaswkzy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pvpdgvle.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2syrzngcj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2poesdskd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2atmocsub.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlpixyjm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2tymfdufx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fdvghaav.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xwoveknt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ljlyikhc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxirgqgc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxsimzpg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jwsnzxsa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jdfmqzxu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdlpktvb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bijwobjq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dnkybmjo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2znpsuila.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jaskyrim.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eipgwtma.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jazkohed.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mkwnxqxb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2avkhhqga.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fefsqzmi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ueoukdts.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2syducjxm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fxabihio.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mjablpch.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qjbkeuzx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ztutbnfj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zkkilyzk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vrncrgsd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aqbpmlxe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mrljvxxc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2djltdspa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvlmnscn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kpvqaatx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syohmhyz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zvpljklp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bchyqmiz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xeietilk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qselumgb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gdkqcdnm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qnwawpan.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dcsheich.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2islpgwjo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2eagztokl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bafgqhey.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wcnnghen.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cnbpetma.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pvrcccrj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uhhdwvmv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gramyzxe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bwpxlpku.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ryiwrcsj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rqcqowla.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xxqynyxm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nqipcmua.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uanjpdfk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcedemfe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2fqttflej.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vpqpmhan.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2htqiuxmn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbijtuk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2oolnbttx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gdkukffe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qaxmvapf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2donqjpce.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ufrddcsg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2geqiwxjp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2psrqttfx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2bzjkptsz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ylbdjgib.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2toaxiqmq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2htqrgjlj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2cdrjjsyn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zximcjei.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2sheuyinu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kogydelx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cpydcydz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2jexluxur.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vvlismvm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2mbwpcycy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ezabizbw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2twmogwne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pxxzsegz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mlhlpnmy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sqeuvrqc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hpyonwwt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dudiozcd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nnyzxkiy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hyyjmdxk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2umloiqry.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ivbvqnuc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zcsisxzq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lflkyfjy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hhapxybz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ofeydeya.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zbdrjgms.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dczektgj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mevdozdv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vhcfgosm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2txjnalsb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bsmflsim.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2renuafbk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jdxeizrj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mqrqumsi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kgebyfxp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fydtyfvw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2uztaoadp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nxyzvnhg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bfpfprqi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rhuiaujd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mxrhjkvn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2aayjuryr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dlcmvfmf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2svmdfqja.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjhqzsuw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2yfuwcpud.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wdyyyqqg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2envztegy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bofyyuwn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lygvusvb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tjnhxdgp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zmosjyum.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ferxfjak.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2doozytwf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gjwiibdz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cgjqdgul.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xkjbttzm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sciflsdq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xmuvvnpm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ykjxrjby.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eyurriqx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2eyegtsvl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pptkuklh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2plqviqnz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vknxgnxw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2hvgqmjds.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ybclghai.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xjrmtpaw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2afigavfb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2irlmvirb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lgnpsebb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2lyuugafe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2npovxnov.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rllpdbup.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ernqazww.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcnwojoh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dtqzbchf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rsgubbez.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wngqakbg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2izjzywbf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2piuexwlw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lwhhqiut.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hosjeqvl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qeeujzmx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yksrpycb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jvgzikar.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yuhessuz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zzypjzxz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vcguzjgk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2letqurps.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bxsutlrp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2crqeitbb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2htxqycjl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vkjyluzm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zymuxory.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2efbtzgeu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cyytmgfv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lbyfvwjb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2agmbwgri.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2uknnnbxu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dtudtsee.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ehmckbzj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hxyaoizy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2azlvgbvh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2yluimtzt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sprclaiw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jrnjrpkj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dgyllerr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2iiiqotsw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mtvontjn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fapllebv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jlnjasss.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ldhsxquj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lymrjiho.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tfqcibzl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jcrypygq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2norclhla.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zqslrymp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2agyhipfh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2edunrxlu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zmruccha.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cytdjast.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gbinxrig.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ohexcvzi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xjhzkdcw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jvduoktw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xwfxplua.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2efomzfmx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2zomdhizz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pzpljmif.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2skqpudqw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2usljgdcs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2yzpykatd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2eliiuwcr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2tgkomlgd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2zkyvoopo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wagpdlkj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ymsigrak.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fpbsuvon.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2uyaxzcam.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2whbuxwlb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kptupgyq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yvosooca.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zblywwhi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fobpetqy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2mtcakasz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qgwrrzea.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2prqccprr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rdbtmidt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvrjkhxo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wnzqhewi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mpofxrir.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dptaiqlx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ibjemorh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wvedrhks.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2deydeydp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrpqymf.html


<!-- 参考信息 -->