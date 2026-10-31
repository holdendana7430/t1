代发 wailian999

[S45] C++：lambda
来源：http://rj.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ll.szxytkj.cn

[S46] C++：函数模板
来源：http://ac.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cc.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://rj.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mi.nszjky.cn

[S48] C++：逐行读文件
来源：http://tt.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://co.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://ea.yuexingan06.cn

[S49] C++：写文件
来源：http://az.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yh.hahajie.cn

[S50] C++：格式化数字
来源：http://oh.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ha.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://fu.jctech888.com.cn

static_cast<double>(a) / b
来源：http://za.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://ri.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://qn.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://xh.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://dy.9csxet.cn

[S54] C++：异常处理
来源：http://xl.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pp.shxzukj.cn

[S55] C++：结构化绑定
来源：http://wm.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zf.521024.cn

[S56] C++：optional
来源：http://av.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ok.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://de.yuexingan06.cn

constexpr int N = 10;
来源：http://uq.panjiajie.cn

[S58] C++：命名空间
来源：http://js.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://ac.nicolike.cn

[S59] C++：静态断言
来源：http://rb.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jz.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://ex.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lr.huanxung.cn

================================================================================
来源：http://du.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ro.nszjky.cn

================================================================================
来源：http://hz.szsharing.cn

[T01] Kotlin：Hello World
来源：http://os.521024.cn

println("Hello")
来源：http://qc.hahajie.cn

[T02] Kotlin：变量
来源：http://wd.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ya.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://il.521024.cn

"值: $b"
来源：http://lz.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://xm.shxzukj.cn

val n: String? = null;  n?.length
来源：http://bk.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://cd.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fa.szsharing.cn

[T06] Kotlin：集合映射
来源：http://lg.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jv.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://yq.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tr.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://wz.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://cn.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://qe.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://wr.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://ao.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wa.wgjwhj.cn

[T11] Kotlin：协程
来源：http://sj.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vb.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://hz.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://rr.colortex.cn

[T13] Kotlin：只读 Map
来源：http://zk.nicolike.cn

val m = mapOf("a" to 1)
来源：http://qa.shxzukj.cn

[T14] Kotlin：循环
来源：http://et.huanxung.cn

for (i in 1..10) println(i)
来源：http://mn.yuexingan06.cn

[T15] Kotlin：接口
来源：http://ri.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://nu.asd995.cn

[T16] Swift：Hello World
来源：http://kx.wgjwhj.cn

print("Hello")
来源：http://dy.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://tm.shtwfgs.cn

var a = 1;  let b = 2
来源：http://zs.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://aj.haigaiapp.cn

"值: \(b)"
来源：http://if.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://ng.hnjuh.cn

if let n = opt { print(n) }
来源：http://ih.huixiangedu.cn

[T20] Swift：数组操作
来源：http://ah.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vs.chemitech.net.cn

[T21] Swift：遍历
来源：http://kx.9csxet.cn

for x in a { print(x) }
来源：http://iq.jianghongdianzi.cn

[T22] Swift：字典
来源：http://ve.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xd.hnjuh.cn

[T23] Swift：函数
来源：http://rk.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uu.wgjwhj.cn

[T24] Swift：闭包
来源：http://gu.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ij.9csxet.cn

[T25] Swift：结构体
来源：http://np.hahajie.cn

struct P { var x: Int }
来源：http://te.hnjuh.cn

[T26] Swift：类与重写
来源：http://by.panjiajie.cn

class A: Base { override func f() {} }
来源：http://qx.szsharing.cn

[T27] Swift：错误处理
来源：http://wy.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://tx.hnjuh.cn

[T28] Swift：枚举
来源：http://ti.shtwfgs.cn

enum Color { case red, green }
来源：http://ce.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://nv.bjjhwx.cn

guard let x = opt else { return }
来源：http://kk.9csxet.cn

[T30] Swift：协议
来源：http://rw.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://yk.nicolike.cn

[T31] Lua：Hello World
来源：http://le.jianghongdianzi.cn

print("Hello")
来源：http://xg.gzmigu.cn

[T32] Lua：局部变量
来源：http://at.shxzukj.cn

local a = 1
来源：http://gh.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://jk.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://es.asd995.cn

[T34] Lua：遍历表
来源：http://pi.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yi.asd995.cn

[T35] Lua：字典表
来源：http://wv.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://fg.shtwfgs.cn

[T36] Lua：函数
来源：http://gf.hnjuh.cn

function add(a, b) return a + b end
来源：http://ck.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://xr.colortex.cn

"a" .. "b"
来源：http://bh.hnjuh.cn

[T38] Lua：条件
来源：http://fd.hahajie.cn

if x > 0 then print("正") end
来源：http://ba.9csxet.cn

[T39] Lua：模式匹配
来源：http://sv.panjiajie.cn

string.find(s, "%d+")
来源：http://px.jianghongdianzi.cn

[T40] Lua：元表
来源：http://ee.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://ol.wgjwhj.cn

[T41] Perl：Hello World
来源：http://gn.yuntaijiaju.cn

print "Hello\n";
来源：http://nj.521024.cn

[T42] Perl：变量类型
来源：http://ku.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rj.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://kh.521024.cn

"值: $a"
来源：http://cw.muxihuayi.cn

[T44] Perl：条件
来源：http://ho.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://fu.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://gw.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://dj.gzmigu.cn

[T46] Perl：哈希操作
来源：http://li.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qq.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://qk.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qw.panjiajie.cn

[T48] Perl：正则替换
来源：http://lz.hnjuh.cn

$s =~ s/old/new/g;
来源：http://ck.colortex.cn

[T49] Perl：函数
来源：http://gx.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pw.521024.cn

[T50] Perl：逐行读文件
来源：http://rj.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ag.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://iz.hahajie.cn

[T51] Scala：Hello World
来源：http://na.521024.cn

println("Hello")
来源：http://jk.hnjuh.cn

[T52] Scala：变量
来源：http://qj.shtwfgs.cn

val a = 1;  var b = 2
来源：http://lj.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://us.bookmarksfly.cn

s"值: $b"
来源：http://cg.521024.cn

[T54] Scala：集合映射
来源：http://sh.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://cr.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://zf.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ix.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://yn.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://zx.9csxet.cn

[T57] Scala：模式匹配
来源：http://gr.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://im.nszjky.cn

[T58] Scala：函数定义
来源：http://wl.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xh.szsharing.cn

[T59] Scala：循环
来源：http://ov.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://sz.huanxung.cn

[T60] Scala：折叠
来源：http://av.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ez.9csxet.cn

================================================================================
来源：http://df.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ug.shxzskj.cn

================================================================================
来源：http://bd.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://ax.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rv.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ed.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wx.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://pp.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ot.9csxet.cn

[U04] Py：变量调试打印
来源：http://cs.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jq.nszjky.cn

[U05] Py：列表去重且保序
来源：http://oy.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://hr.huanxung.cn

[U06] Py：合并两个字典
来源：http://re.huixiangedu.cn

{**a, **b}
来源：http://bq.szsharing.cn

[U07] Py：反转字典键值
来源：http://ih.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://ds.hnjuh.cn

[U08] Py：展平二维列表
来源：http://ve.muxihuayi.cn

[y for x in nested for y in x]
来源：http://ty.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://hm.chemitech.net.cn

max(d, key=d.get)
来源：http://pf.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://mj.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hk.colortex.cn

[U11] Py：生成器表达式
来源：http://tm.jctech888.com.cn

(x * 2 for x in arr)
来源：http://oy.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pl.asd995.cn

Counter(arr).most_common(3)
来源：http://ul.asd995.cn

[U13] Py：固定长度队列
来源：http://hn.szxytkj.cn

deque(maxlen=10)
来源：http://pk.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://sr.asd995.cn

defaultdict(list)
来源：http://ol.muxihuayi.cn

[U15] Py：高精度计时
来源：http://lk.huixiangedu.cn

t = time.perf_counter()
来源：http://ts.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://pl.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ch.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://pu.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://qn.shtwfgs.cn

[U18] Py：预编译正则
来源：http://kc.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://cv.jianghongdianzi.cn

[U19] Py：正则替换带回调
来源：http://fo.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fq.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://ro.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://om.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://yr.shxzukj.cn

@contextlib.contextmanager
来源：http://qu.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://bm.shtwfgs.cn

list(zip(*m))
来源：http://vu.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://bz.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hj.szxytkj.cn

[U24] Py：路径操作
来源：http://cx.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pk.521024.cn

[U25] Py：CSV 按字典读
来源：http://ov.wgjwhj.cn

csv.DictReader(f)
来源：http://xt.jctech888.com.cn

[U26] Py：并发下载
来源：http://kc.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hj.asd995.cn

[U27] Py：异步 HTTP
来源：http://ns.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://ui.wgjwhj.cn

[U28] Py：类型别名
来源：http://na.haigaiapp.cn

UserId = int
来源：http://ec.panjiajie.cn

[U29] Py：属性校验
来源：http://nj.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://dg.hahajie.cn

[U30] Py：数据类
来源：http://lf.shxzukj.cn

@dataclass(slots=True)
来源：http://jb.huixiangedu.cn

[U31] Py：单测
来源：http://at.nicolike.cn

python -m pytest -q
来源：http://yc.bjjhwx.cn

[U32] Py：代码格式化
来源：http://gr.newstarts.cn

ruff format . && ruff check --fix .
来源：http://to.huixiangedu.cn

[U33] Py：打包发布
来源：http://zb.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://gu.asd995.cn

[U34] Py：判断编码
来源：http://nx.nicolike.cn

chardet.detect(raw)
来源：http://hx.haigaiapp.cn

[U35] Py：发送邮件
来源：http://ns.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://os.jctech888.com.cn

[U36] Py：定时任务
来源：http://sb.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://io.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://jm.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ri.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://pm.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://wj.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://gg.hahajie.cn

sys.stdout.isatty()
来源：http://nf.szsharing.cn

[U40] Py：打印到标准错误
来源：http://cp.huanxung.cn

print("err", file=sys.stderr)
来源：http://ec.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ib.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ti.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://sw.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xc.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://gy.szxytkj.cn

namespace App\Http;
来源：http://sd.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://my.huixiangedu.cn

declare(strict_types=1);
来源：http://fn.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://ya.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fb.nicolike.cn

[U46] PHP：可空类型
来源：http://fu.szxytkj.cn

?string $name = null
来源：http://nx.shtwfgs.cn

[U47] PHP：联合类型
来源：http://gd.nicolike.cn

int|string $id
来源：http://ft.521024.cn

[U48] PHP：纯枚举
来源：http://tx.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ub.bjjhwx.cn

[U49] PHP：只读属性
来源：http://eq.shtwfgs.cn

public readonly string $name
来源：http://pw.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://cz.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://dg.nszjky.cn

[U51] PHP：数组解构
来源：http://id.huanxung.cn

[$a, $b] = $arr;
来源：http://fy.hahajie.cn

[U52] PHP：箭头函数
来源：http://ve.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://na.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://pb.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://kw.hahajie.cn

[U54] PHP：空安全调用
来源：http://xb.yuntaijiaju.cn

$obj?->method()
来源：http://lm.gzmigu.cn

[U55] PHP：match 表达式
来源：http://jd.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jm.haigaiapp.cn

[U56] PHP：命名参数
来源：http://ss.jctech888.com.cn

f(a: 1, b: 2)
来源：http://vz.asd995.cn

[U57] PHP：字符串插值
来源：http://sy.lnxyls.cn

"值: {$a}"
来源：http://ad.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://aj.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wc.newstarts.cn

[U59] PHP：自定义排序
来源：http://vr.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nn.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://as.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jm.9csxet.cn

[U61] PHP：正则
来源：http://bp.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ys.hnjuh.cn

[U62] PHP：日期对象
来源：http://hn.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://da.huixiangedu.cn

[U63] PHP：文件读写
来源：http://wv.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ua.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://fi.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://jh.bjjhwx.cn

[U65] PHP：会话
来源：http://gw.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hu.colortex.cn

[U66] PHP：设置 Cookie
来源：http://yi.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rb.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://rt.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kl.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://wx.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://il.jianghongdianzi.cn

[U69] PHP：PDO 预处理
来源：http://bt.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tg.nicolike.cn

[U70] PHP：PDO 事务
来源：http://qa.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://au.yuntaijiaju.cn


<!-- 参考信息 -->