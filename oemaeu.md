代发 wailian999

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bvuuziec.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cdydrrkm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lfqdznen.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lfvihzxc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ibuwlrpv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lwusnkej.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bmvuesrc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kkybfpkr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rloghqmi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zqvajyss.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nbsunnwp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fpiluoke.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2agbqmmzi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rljmsino.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vjgytzia.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mlgblutx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rakhwvrf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sgxahoxe.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bxzcrdua.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wivhxyfj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2anoqoitv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2yqjdzyxy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bycdmgrx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zckzlsnx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gvwuopoy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2cpdjxcuu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bhkseqyo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vloykwan.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pvmapofg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sebfdfge.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kqzxqsiw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bmhyencq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ikhhjulh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2imamlcvw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bevkfege.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgnfjvyv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hezfyjuj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wrrianxe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2znwihlwo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dcrrgvmy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2imgtipwt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2igayqwyn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ellupbpg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2znpjwljr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gwtxwjti.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tdkjlzfb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wlbmmcdj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zsjlkngo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zmagxrge.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2chazhots.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hyirkuad.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xhdioklj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ajeyghle.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nstaoitx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkvbwvud.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wzdgaenr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gxrlgfxs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zvjbrzia.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wloajlgt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vcviwkom.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycgkgomg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aikkzczp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rvqpuchz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2geesozzh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xaoymmni.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bfbhkbgt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rnwpcipf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2anayhpwm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2bimbcdyf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zftiuvrf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pslneamv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pgiagqkg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mefbbrgb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2phtlrodf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vpdonocd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rgmaebsj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ivrzihfx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qyxjrqbl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bsytfcru.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oyoawykw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxaldgba.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fanckvay.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2osekkdvt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2plsyspee.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnvnwkq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pavewfhn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hpceqfvl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2oqgypbhe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2grheofxj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2phyeilej.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oinwvvpt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cbvhqgif.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rryzvlfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yluitssp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2obitunww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bruywrdg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xjwzuuls.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wnpslhwz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zwzfyfye.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2achwpjby.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sugcfmpa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rxrymkmq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hjcukqkz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ynzugiau.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2aupqtnhy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dilekwcq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wecifbiq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lnhyvbid.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xiwspars.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hgwcddpu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rpdkmctt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mskukcjh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2chpeuvrx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpwyhus.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zkljzjac.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rufigavh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rtmpazcl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2datebxgz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2resqjwlf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hjnlqabi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mmmfhyrf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yewslwxg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ewxibyym.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hvrjabto.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2iaqpsbiy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2owrovgvc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ptsmcldu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ksvtpkhq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2spzzoqjf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vbngvwyv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2irndvocz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wkaqsnuw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2epsgzcut.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqyorgxi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2bxsnycad.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2bbkozgbk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tzqgzbkt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2hsfqiqvb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kqcixrfn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rdayujjo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tffytucs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2arjlnuhu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hdvprybm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lcoarkaf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xxctxtpb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jlpohgsh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ipqgpjgg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rbgckuok.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2cduhukwf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2psuoagqu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qwkuwjdn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rmxlirbk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hknttlck.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2rmnffvha.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iqxwpotq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jsmfufdr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gawrovgr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wxifmlbx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hhwrenpb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dqtimlzu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jfzwetxn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fupccizo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2svhczbwl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rqtvpapt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pjumrwds.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ujspglwc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cxbqykfm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2scekxzvj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2iixngnjt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gbhvxtqt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zdyshtrx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2minktnzi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rlejcgls.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2occxiiya.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2sbcgvqtd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rttqoisx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xnexxbbw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vcguggvl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wbgacyak.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2suubdyze.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fzdynfun.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kuufayya.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fedtwhwi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hcvlsaty.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2oesegtza.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hthxfrby.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fjpsujvh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wzfgmeag.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnbnopfz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hzfkmfra.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2imslcnjq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewjdqmoh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ukwqraas.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2awflwgye.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jjqssvlx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hwndxhbc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2chelfwas.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2drbgsyej.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2taqdpwdk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yxswfncm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kgepevyf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2cdtqkxan.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2jbqnxhkj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2djmiumgi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sutrwzza.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wxcbojsz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qfasyvda.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtluztmg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2agcfioxh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcgiamyc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dxebtasu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2eaetwumv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2oggbhhbt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qxaekwak.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ujjgmqzp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wbozzwei.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hhmemiil.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ukktuaqo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2obqvsenc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jlzxrfxp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2goswidvg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qexebsbm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ixczbrmm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kkptrwsc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fmhyawek.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pplsruey.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xvhmpfkh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xctkmokx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vtcpwwej.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ypgdcevf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rsxxyozz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ymwagqdp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wtsfufao.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tftlamqm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2azixexdp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2jbxrjdfm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zvokbksf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xggporfa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2odkfoklg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2etlqzzwa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bpwcomix.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2izthrdnw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2stttvjlm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2datdrgna.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2iznuogax.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2quegctjp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pchmtlsn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wonirqyv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zsbjjtle.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vszgpnvk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2reqymhop.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gmifwzzf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tlzsozou.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jezjfjyk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bewlipri.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wiemrtam.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fapxntac.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bjyhurej.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2tmcnfcve.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ccdwyfff.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2jvnhkxby.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mgqqqhco.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qfybibey.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2yzvlvfod.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2muayykgz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vzxsjvbx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2yrawrsyq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fevlonoz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qqsvvtmq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zjvorevc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2awwthpzr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pammvxqs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hgavtama.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pwfkgaam.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hmmufnir.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pxomumel.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2duqorudz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2nylkbzcr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ziktsmaa.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wlwdelum.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ezctaicn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fzowards.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ljeibfgu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ydsopfxu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hhyohrtn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dyvxvnze.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kjtrmklr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gnsngaes.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lkbrjctq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2paqrxwlb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ujkhzjfb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jbokhbwm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zspzrphc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2liwnyqka.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2stsstety.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ivqqkpek.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qndmlzso.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kogzotcn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ysgablch.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dluyymjo.html


<!-- 参考信息 -->