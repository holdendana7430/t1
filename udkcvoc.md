代发 wailian999

[S45] C++：lambda
来源：http://lf.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bb.yuexingan06.cn

[S46] C++：函数模板
来源：http://zo.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aw.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://ws.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kl.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://xr.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bz.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://qk.huixiangedu.cn

[S49] C++：写文件
来源：http://cn.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xh.lnxyls.cn

[S50] C++：格式化数字
来源：http://fb.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nx.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://ct.shtwfgs.cn

static_cast<double>(a) / b
来源：http://lp.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://fa.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://hv.lnxyls.cn

[S53] C++：移动语义
来源：http://ps.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://hx.newstarts.cn

[S54] C++：异常处理
来源：http://ms.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kk.panjiajie.cn

[S55] C++：结构化绑定
来源：http://gt.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wi.nszjky.cn

[S56] C++：optional
来源：http://wn.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pn.asd995.cn

[S57] C++：编译期常量
来源：http://ru.panjiajie.cn

constexpr int N = 10;
来源：http://np.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://dd.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://kr.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://dg.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rj.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://hz.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tp.huixiangedu.cn

================================================================================
来源：http://ll.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oe.colortex.cn

================================================================================
来源：http://ez.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://eq.nszjky.cn

println("Hello")
来源：http://np.521024.cn

[T02] Kotlin：变量
来源：http://bt.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mn.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://vo.yuexingan06.cn

"值: $b"
来源：http://hk.szsharing.cn

[T04] Kotlin：空安全
来源：http://rq.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ze.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://cj.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tw.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://vo.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fy.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://we.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gw.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://by.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://av.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://zi.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://zx.szsharing.cn

[T10] Kotlin：默认参数
来源：http://nl.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ko.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://kb.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jg.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://pk.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://cs.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://vi.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://wo.521024.cn

[T14] Kotlin：循环
来源：http://js.nszjky.cn

for (i in 1..10) println(i)
来源：http://az.szsharing.cn

[T15] Kotlin：接口
来源：http://vg.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://er.szsharing.cn

[T16] Swift：Hello World
来源：http://hf.gzmigu.cn

print("Hello")
来源：http://yk.nszjky.cn

[T17] Swift：变量与常量
来源：http://ma.nicolike.cn

var a = 1;  let b = 2
来源：http://se.521024.cn

[T18] Swift：字符串插值
来源：http://ag.asd995.cn

"值: \(b)"
来源：http://oq.huanxung.cn

[T19] Swift：可选绑定
来源：http://fx.shtwfgs.cn

if let n = opt { print(n) }
来源：http://ws.gzmigu.cn

[T20] Swift：数组操作
来源：http://xm.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wg.huixiangedu.cn

[T21] Swift：遍历
来源：http://ot.wgjwhj.cn

for x in a { print(x) }
来源：http://rs.jianghongdianzi.cn

[T22] Swift：字典
来源：http://ra.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vc.szxytkj.cn

[T23] Swift：函数
来源：http://mh.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zj.newstarts.cn

[T24] Swift：闭包
来源：http://jk.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://al.asd995.cn

[T25] Swift：结构体
来源：http://yq.haigaiapp.cn

struct P { var x: Int }
来源：http://dd.bjjhwx.cn

[T26] Swift：类与重写
来源：http://tz.lnxyls.cn

class A: Base { override func f() {} }
来源：http://yx.muxihuayi.cn

[T27] Swift：错误处理
来源：http://xh.521024.cn

do { try f() } catch { print(error) }
来源：http://er.huixiangedu.cn

[T28] Swift：枚举
来源：http://bj.bookmarksfly.cn

enum Color { case red, green }
来源：http://aw.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://fi.bjjhwx.cn

guard let x = opt else { return }
来源：http://bn.bookmarksfly.cn

[T30] Swift：协议
来源：http://bk.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://ht.gzmigu.cn

[T31] Lua：Hello World
来源：http://xt.nszjky.cn

print("Hello")
来源：http://au.shxzskj.cn

[T32] Lua：局部变量
来源：http://ow.shxzukj.cn

local a = 1
来源：http://cj.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://bg.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ml.colortex.cn

[T34] Lua：遍历表
来源：http://ss.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xn.huixiangedu.cn

[T35] Lua：字典表
来源：http://gu.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://wc.shtwfgs.cn

[T36] Lua：函数
来源：http://kh.colortex.cn

function add(a, b) return a + b end
来源：http://yj.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://wo.9csxet.cn

"a" .. "b"
来源：http://kh.gzmigu.cn

[T38] Lua：条件
来源：http://zm.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://sm.colortex.cn

[T39] Lua：模式匹配
来源：http://uu.shxzskj.cn

string.find(s, "%d+")
来源：http://gn.haigaiapp.cn

[T40] Lua：元表
来源：http://ah.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://hb.chemitech.net.cn

[T41] Perl：Hello World
来源：http://mo.huixiangedu.cn

print "Hello\n";
来源：http://dm.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://sq.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nf.521024.cn

[T43] Perl：字符串插值
来源：http://uo.lnxyls.cn

"值: $a"
来源：http://fv.yuexingan06.cn

[T44] Perl：条件
来源：http://ro.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://uu.szxytkj.cn

[T45] Perl：数组遍历
来源：http://bf.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://lb.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://vr.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uh.gzmigu.cn

[T47] Perl：正则捕获
来源：http://rv.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qs.gzmigu.cn

[T48] Perl：正则替换
来源：http://xf.gzmigu.cn

$s =~ s/old/new/g;
来源：http://go.nicolike.cn

[T49] Perl：函数
来源：http://ow.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bq.asd995.cn

[T50] Perl：逐行读文件
来源：http://ko.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bm.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://jr.newstarts.cn

[T51] Scala：Hello World
来源：http://gv.huanxung.cn

println("Hello")
来源：http://xx.hahajie.cn

[T52] Scala：变量
来源：http://ry.shxzukj.cn

val a = 1;  var b = 2
来源：http://ih.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://mb.bookmarksfly.cn

s"值: $b"
来源：http://qx.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://cd.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://nd.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://ia.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dj.haigaiapp.cn

[T56] Scala：样例类
来源：http://dz.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://em.gzmigu.cn

[T57] Scala：模式匹配
来源：http://mb.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nb.521024.cn

[T58] Scala：函数定义
来源：http://bz.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ol.szxytkj.cn

[T59] Scala：循环
来源：http://pt.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://rz.huixiangedu.cn

[T60] Scala：折叠
来源：http://ud.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kk.nicolike.cn

================================================================================
来源：http://dm.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qk.muxihuayi.cn

================================================================================
来源：http://gx.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://mu.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ad.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://ye.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wy.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://nx.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oq.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://wv.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dz.hahajie.cn

[U05] Py：列表去重且保序
来源：http://ik.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://cq.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://wo.hahajie.cn

{**a, **b}
来源：http://zn.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://qe.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://we.lnxyls.cn

[U08] Py：展平二维列表
来源：http://ru.jctech888.com.cn

[y for x in nested for y in x]
来源：http://sr.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://le.chemitech.net.cn

max(d, key=d.get)
来源：http://mr.hahajie.cn

[U10] Py：按值排序字典
来源：http://zn.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iw.nicolike.cn

[U11] Py：生成器表达式
来源：http://ok.yuexingan06.cn

(x * 2 for x in arr)
来源：http://sa.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ur.huanxung.cn

Counter(arr).most_common(3)
来源：http://vm.shxzukj.cn

[U13] Py：固定长度队列
来源：http://kx.521024.cn

deque(maxlen=10)
来源：http://sm.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://oy.shtwfgs.cn

defaultdict(list)
来源：http://fr.chemitech.net.cn

[U15] Py：高精度计时
来源：http://sg.9csxet.cn

t = time.perf_counter()
来源：http://eg.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://uv.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zc.shtwfgs.cn

[U17] Py：初始化日志
来源：http://he.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://li.nszjky.cn

[U18] Py：预编译正则
来源：http://vd.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://hw.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://yf.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://md.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://qx.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://gx.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ih.chemitech.net.cn

@contextlib.contextmanager
来源：http://ru.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://cu.muxihuayi.cn

list(zip(*m))
来源：http://ip.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://ly.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mo.bookmarksfly.cn

[U24] Py：路径操作
来源：http://mr.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xm.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://sz.haigaiapp.cn

csv.DictReader(f)
来源：http://ba.muxihuayi.cn

[U26] Py：并发下载
来源：http://gv.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hp.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://gl.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://rs.colortex.cn

[U28] Py：类型别名
来源：http://sk.szxytkj.cn

UserId = int
来源：http://ag.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://jg.huanxung.cn

@property 与 @x.setter 配合
来源：http://cc.huixiangedu.cn

[U30] Py：数据类
来源：http://np.nicolike.cn

@dataclass(slots=True)
来源：http://gx.hahajie.cn

[U31] Py：单测
来源：http://yb.nicolike.cn

python -m pytest -q
来源：http://km.muxihuayi.cn

[U32] Py：代码格式化
来源：http://cw.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://hd.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://nh.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ft.lnxyls.cn

[U34] Py：判断编码
来源：http://mp.szsharing.cn

chardet.detect(raw)
来源：http://du.bjjhwx.cn

[U35] Py：发送邮件
来源：http://zu.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jf.shtwfgs.cn

[U36] Py：定时任务
来源：http://mq.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://zn.shxzukj.cn

[U37] Py：读写 Excel
来源：http://xh.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mw.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://kq.gzmigu.cn

Path(__file__).resolve().parent
来源：http://ma.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://gw.shtwfgs.cn

sys.stdout.isatty()
来源：http://mz.521024.cn

[U40] Py：打印到标准错误
来源：http://vo.asd995.cn

print("err", file=sys.stderr)
来源：http://xz.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://uj.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gc.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://lb.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hg.nszjky.cn

[U43] PHP：声明命名空间
来源：http://oj.wgjwhj.cn

namespace App\Http;
来源：http://nx.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://eq.yuntaijiaju.cn

declare(strict_types=1);
来源：http://st.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://js.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.colortex.cn

[U46] PHP：可空类型
来源：http://zv.nszjky.cn

?string $name = null
来源：http://vj.bjjhwx.cn

[U47] PHP：联合类型
来源：http://hx.newstarts.cn

int|string $id
来源：http://pc.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://ru.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fk.nicolike.cn

[U49] PHP：只读属性
来源：http://xy.chemitech.net.cn

public readonly string $name
来源：http://pa.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://yh.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://zf.shxzukj.cn

[U51] PHP：数组解构
来源：http://dr.yuexingan06.cn

[$a, $b] = $arr;
来源：http://ca.521024.cn

[U52] PHP：箭头函数
来源：http://ho.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://je.newstarts.cn

[U53] PHP：空合并运算符
来源：http://eg.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://gz.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://bq.szxytkj.cn

$obj?->method()
来源：http://lh.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://bd.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://am.hahajie.cn

[U56] PHP：命名参数
来源：http://ig.szxytkj.cn

f(a: 1, b: 2)
来源：http://lq.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://oa.huanxung.cn

"值: {$a}"
来源：http://io.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://xe.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cs.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://nu.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bs.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://ih.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xc.muxihuayi.cn

[U61] PHP：正则
来源：http://wy.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ke.hnjuh.cn

[U62] PHP：日期对象
来源：http://mv.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nn.szxytkj.cn

[U63] PHP：文件读写
来源：http://pq.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ly.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://lt.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://zq.jctech888.com.cn

[U65] PHP：会话
来源：http://qp.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ld.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://cj.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cx.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://tt.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rp.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://ez.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vs.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://fz.yuexingan06.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xm.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://od.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bb.bookmarksfly.cn


<!-- 参考信息 -->