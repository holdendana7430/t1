代发 wailian999

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rrmsbxpu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wctyztha.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vgkhbcyf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwpqqqv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nyggumkj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3etihzuuh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pqfmuniy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ffimrgus.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3grylkjli.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzxhqius.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pxafztfa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mfiaedkb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gryuzvoo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3wazdavwk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dptahwss.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3muekkvvy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cgvsmzzc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ofgsvqdt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3igrlashy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qgkwwgtp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mracgcxa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3medxunyt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3psotojdy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qjglfwss.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kmgzfymp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tcpdygxa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3eaunwurj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3njmfpadd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ilkxevtu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3yqqiowyg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fddgvgdq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3efvkljjk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wqbewvdi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3palpeost.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ndhaabkj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3srkhysuj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mrpragyx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jwntbxml.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fgvielcm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wejciuwg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tlutjcxb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fyxterru.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uuhfrqct.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3setpupar.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zquyybeg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bnbpdtsq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3roqbrqow.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nxjxpvql.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lvnurqke.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ydcorjwn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3spouhnvh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3fxbjmtmw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bsbxwnme.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3culnaulz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aecuwpfc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ulpzypae.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hexhmtqe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pdgqurhp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vjnqmfqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3bhtavcho.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3voonlvcn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gxyajjav.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3odsfhvfn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaokzfnc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3huokbxjh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ngqhvbuu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3nhpscmtq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqrldeqt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dqezfvfq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3goqprkgp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jkwwxhhh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xbcpspon.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwsdmtfs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxryekhi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ecelqomy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ubmbdwqm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3btjyvbtp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bdhyqhmo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uhswjckm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wdxuuoha.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bzqalqot.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ontfeudh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3boxtnkac.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3icxmytfq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qmoupxiy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aysaznfq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3whakwvqe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zdsustor.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jutictdv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nvyzpjfl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3srqgqdbu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sjsvsziv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3untyahxl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yxmjulvf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xslukewr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gsqdhjuu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fcryhxvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrwxpqfi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yeqepfrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ietpjkji.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3godobspv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3filqtbhb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3dtkdljhl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3arivilaq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tfbfxnhw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xinlfzmn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vxnxgqua.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3oncmuiio.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zpizwmpw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hzslkxzl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3altdemdg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jgwdyhiz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xigrjkxk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rleigzob.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3eawguzts.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zfzzlmme.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kldgsdir.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3aydhqbet.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nlvqvhqq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jmwxfjuc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yrkrbmoz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nsgqndfn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qzxcrzbd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jdgejzvi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3njzajydq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ygndwcqn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3nptojuit.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqdfvfb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3woefkvxc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3papnbwie.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hrobgyvg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dswixddh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3skabuemt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vnfxxalj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kxxqxccq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iirairut.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mvtdcrwb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qysrtvul.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ldydsqyv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3phgyofbs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3troqrton.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cbcjykrn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hjrwbesn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yfovpysd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zrqbwjjm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3rfsfmmlo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3yqxxxxec.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cvebddcx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qeaopovg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3uohnvanz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ylqfznjz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rdxbtnyi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3leyxxufy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3bpfmypqj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3azkpriqw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kaxfyfxv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3unowazwi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vqhfjzrx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ejfnalpm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lapktqsr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xddgbesv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3phxkfjqi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3apsmvxms.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fnayiuoy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gaeckgno.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3swolrutf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3upthrqpf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jebfxudu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hliciixh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vwznqiop.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qfhaturl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3oehlrghh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tepxxrvm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ezhaltpy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kcdapltm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ymonmvvs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pjbafmvd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3tsoollwk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3adveyhui.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tzjhhtbx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3uirspkkl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3cabxzatd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3keusnnfk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xavjxzsm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lapirimi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nzjfidvh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uwsqlicn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mysqcvzf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vtlpuniy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dqshcpjo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gtjkfjeb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3oljqujws.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vrxgqjqn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3clsqobjn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ixkgaweh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ttpscgrg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3auxqwhkj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3acuzafxz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rqzmtvhy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcfppmpo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3unzbqisp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3sekjnelp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvquudlv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kalhirqh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3plokdxsg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3bbtgwdcr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gpuoorqr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xvzteakw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pmobxkhb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qpapmtdb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ilejwljg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eioghlgv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wmjxhbrr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3awevewfo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kxvcyadr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gngczckj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kafidldu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ocphdwsv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kwphofno.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3unxqaniy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3bhifznwr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3apysenqg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3fdpimrhq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wdyqmchl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3oavunfqo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3yburwnnn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cuqomedv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ikfavorr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gudhsvgc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xnlzzqyx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ajlfxkyf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jkfnivpw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gcjevopq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wdzdjplo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3kynmwzzp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ffsqnbqi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3hhxurihd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ocznpxdp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nmrmxwih.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dwfvqwan.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oiacdqxk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dhnqaiiq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ejwvhmro.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qqykycco.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3birscqnm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fcusajfg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3coeyvzxz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cxkfhbep.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hnuhxbyd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fcmvevfb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3sbluxzsc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bfuvlsck.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uxwygymk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3myftndem.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cfmgqans.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nylobuql.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3iwtwohcz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3okrmwlfl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tjmnoojg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cbdutaml.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jteboqcf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jdxmrcvo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3debvkfsm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xkxdzltf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tzumicoj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vfpebqto.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tiznjvoj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3drlzjmiy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3awcvxrjb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ywfglrpv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qzhlutuj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mnejaiai.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nbojljhf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3micndvsg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3doujljjw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qflyvhog.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lsqzylcb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3omrwlzxs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3cmizfbdg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gofbkgvv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vndlbyvd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vuflxgsl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hbialpzg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zbucsryi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wackuhls.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3iitqpctz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dhhfqtol.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sgeeyomn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3djfexyct.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lgoqijhy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xpkakybk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wopgbjgx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zzrrmvyh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uucusjel.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qzjbjoch.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3evltftmb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ebqsavww.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oyaxjpxr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jzzlifse.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bitjqekx.html


<!-- 参考信息 -->