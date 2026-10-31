代发 wailian999

[S43] C++：智能指针
来源：http://kq.521024.cn

auto p = std::make_unique<int>(5);
来源：http://ec.haigaiapp.cn

[S44] C++：引用传参
来源：http://eb.szsharing.cn

void inc(int &x) { ++x; }
来源：http://ks.szxytkj.cn

[S45] C++：lambda
来源：http://el.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zd.nicolike.cn

[S46] C++：函数模板
来源：http://zq.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dm.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://wf.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bs.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://vh.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zb.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://ur.bookmarksfly.cn

[S49] C++：写文件
来源：http://pr.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qh.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://vp.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xb.huanxung.cn

[S51] C++：显式类型转换
来源：http://wd.haigaiapp.cn

static_cast<double>(a) / b
来源：http://on.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ix.9csxet.cn

int size() const noexcept { return n_; }
来源：http://rj.szxytkj.cn

[S53] C++：移动语义
来源：http://cb.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://tb.haigaiapp.cn

[S54] C++：异常处理
来源：http://nr.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cx.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://sg.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uk.nicolike.cn

[S56] C++：optional
来源：http://xa.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nk.wgjwhj.cn

[S57] C++：编译期常量
来源：http://cc.wgjwhj.cn

constexpr int N = 10;
来源：http://cs.yuexingan06.cn

[S58] C++：命名空间
来源：http://od.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://mu.huanxung.cn

[S59] C++：静态断言
来源：http://hy.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ax.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://pi.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jo.chemitech.net.cn

================================================================================
来源：http://yz.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jz.panjiajie.cn

================================================================================
来源：http://pr.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://rq.hnjuh.cn

println("Hello")
来源：http://ph.nicolike.cn

[T02] Kotlin：变量
来源：http://ac.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gm.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://gd.bookmarksfly.cn

"值: $b"
来源：http://ft.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://om.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://lr.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://uz.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nn.huanxung.cn

[T06] Kotlin：集合映射
来源：http://uh.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vl.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ie.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ey.shxzskj.cn

[T08] Kotlin：数据类
来源：http://st.asd995.cn

data class User(val name: String, val age: Int)
来源：http://nc.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://zn.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://hh.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://ft.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fn.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://wz.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vo.hahajie.cn

[T12] Kotlin：解构声明
来源：http://ur.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://uv.asd995.cn

[T13] Kotlin：只读 Map
来源：http://bf.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://yk.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://bq.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://yt.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://ah.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://np.panjiajie.cn

[T16] Swift：Hello World
来源：http://ob.jctech888.com.cn

print("Hello")
来源：http://zw.gzmigu.cn

[T17] Swift：变量与常量
来源：http://ru.gzmigu.cn

var a = 1;  let b = 2
来源：http://xh.hahajie.cn

[T18] Swift：字符串插值
来源：http://tb.hnjuh.cn

"值: \(b)"
来源：http://jh.9csxet.cn

[T19] Swift：可选绑定
来源：http://uk.hahajie.cn

if let n = opt { print(n) }
来源：http://lo.chemitech.net.cn

[T20] Swift：数组操作
来源：http://ca.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cd.panjiajie.cn

[T21] Swift：遍历
来源：http://wh.jctech888.com.cn

for x in a { print(x) }
来源：http://cc.huanxung.cn

[T22] Swift：字典
来源：http://jn.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ib.shxzskj.cn

[T23] Swift：函数
来源：http://lm.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://my.huixiangedu.cn

[T24] Swift：闭包
来源：http://yc.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xn.colortex.cn

[T25] Swift：结构体
来源：http://rc.521024.cn

struct P { var x: Int }
来源：http://xi.huixiangedu.cn

[T26] Swift：类与重写
来源：http://br.gzmigu.cn

class A: Base { override func f() {} }
来源：http://mj.szsharing.cn

[T27] Swift：错误处理
来源：http://qt.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://en.szxytkj.cn

[T28] Swift：枚举
来源：http://bv.huanxung.cn

enum Color { case red, green }
来源：http://lt.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://uy.lnxyls.cn

guard let x = opt else { return }
来源：http://zb.huixiangedu.cn

[T30] Swift：协议
来源：http://rj.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://as.panjiajie.cn

[T31] Lua：Hello World
来源：http://ah.haigaiapp.cn

print("Hello")
来源：http://zd.lnxyls.cn

[T32] Lua：局部变量
来源：http://aa.shxzskj.cn

local a = 1
来源：http://hn.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://pq.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oi.huanxung.cn

[T34] Lua：遍历表
来源：http://ms.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hu.huixiangedu.cn

[T35] Lua：字典表
来源：http://cy.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://bk.nicolike.cn

[T36] Lua：函数
来源：http://eg.9csxet.cn

function add(a, b) return a + b end
来源：http://vd.huanxung.cn

[T37] Lua：字符串拼接
来源：http://qj.szxytkj.cn

"a" .. "b"
来源：http://hn.wgjwhj.cn

[T38] Lua：条件
来源：http://nh.wgjwhj.cn

if x > 0 then print("正") end
来源：http://yb.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://pt.9csxet.cn

string.find(s, "%d+")
来源：http://lk.yuexingan06.cn

[T40] Lua：元表
来源：http://fh.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://ox.szxytkj.cn

[T41] Perl：Hello World
来源：http://as.nszjky.cn

print "Hello\n";
来源：http://fi.jctech888.com.cn

[T42] Perl：变量类型
来源：http://fb.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ab.szsharing.cn

[T43] Perl：字符串插值
来源：http://fe.newstarts.cn

"值: $a"
来源：http://ir.huanxung.cn

[T44] Perl：条件
来源：http://yz.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://mj.colortex.cn

[T45] Perl：数组遍历
来源：http://cd.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://lv.hnjuh.cn

[T46] Perl：哈希操作
来源：http://ii.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cd.szxytkj.cn

[T47] Perl：正则捕获
来源：http://jh.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sm.chemitech.net.cn

[T48] Perl：正则替换
来源：http://pe.gzmigu.cn

$s =~ s/old/new/g;
来源：http://ly.huixinmuqiang.cn

[T49] Perl：函数
来源：http://fh.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ic.asd995.cn

[T50] Perl：逐行读文件
来源：http://ii.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qu.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://yq.shxzskj.cn

[T51] Scala：Hello World
来源：http://jz.nicolike.cn

println("Hello")
来源：http://vm.yuexingan06.cn

[T52] Scala：变量
来源：http://yq.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://sh.nszjky.cn

[T53] Scala：字符串插值
来源：http://yo.szsharing.cn

s"值: $b"
来源：http://zj.nicolike.cn

[T54] Scala：集合映射
来源：http://oh.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://ju.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://md.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gs.muxihuayi.cn

[T56] Scala：样例类
来源：http://xm.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://tx.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://bu.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://za.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://xg.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gv.jctech888.com.cn

[T59] Scala：循环
来源：http://dn.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://oh.shxzskj.cn

[T60] Scala：折叠
来源：http://fc.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cl.wgjwhj.cn

================================================================================
来源：http://jz.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qd.colortex.cn

================================================================================
来源：http://kt.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://hd.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://de.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://zf.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vp.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://ub.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wg.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://pz.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zs.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://jg.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://hn.panjiajie.cn

[U06] Py：合并两个字典
来源：http://fa.yuexingan06.cn

{**a, **b}
来源：http://ow.huanxung.cn

[U07] Py：反转字典键值
来源：http://ck.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://qv.colortex.cn

[U08] Py：展平二维列表
来源：http://vm.9csxet.cn

[y for x in nested for y in x]
来源：http://pf.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ec.chemitech.net.cn

max(d, key=d.get)
来源：http://kc.szsharing.cn

[U10] Py：按值排序字典
来源：http://me.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ye.nszjky.cn

[U11] Py：生成器表达式
来源：http://rn.newstarts.cn

(x * 2 for x in arr)
来源：http://kw.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qx.colortex.cn

Counter(arr).most_common(3)
来源：http://zg.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://vj.jctech888.com.cn

deque(maxlen=10)
来源：http://pf.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://dl.lnxyls.cn

defaultdict(list)
来源：http://mh.yuexingan06.cn

[U15] Py：高精度计时
来源：http://zh.muxihuayi.cn

t = time.perf_counter()
来源：http://wa.nszjky.cn

[U16] Py：命令行参数解析
来源：http://mu.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gm.newstarts.cn

[U17] Py：初始化日志
来源：http://as.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://um.shxzukj.cn

[U18] Py：预编译正则
来源：http://ar.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://ye.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://mc.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ve.nicolike.cn

[U20] Py：缓存函数结果
来源：http://kt.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ke.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://xg.jianghongdianzi.cn

@contextlib.contextmanager
来源：http://dq.9csxet.cn

[U22] Py：矩阵转置
来源：http://cp.wgjwhj.cn

list(zip(*m))
来源：http://hh.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://ic.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://at.panjiajie.cn

[U24] Py：路径操作
来源：http://hx.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ah.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://do.panjiajie.cn

csv.DictReader(f)
来源：http://na.asd995.cn

[U26] Py：并发下载
来源：http://cd.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cx.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://uu.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://jo.yuexingan06.cn

[U28] Py：类型别名
来源：http://es.bookmarksfly.cn

UserId = int
来源：http://mt.hahajie.cn

[U29] Py：属性校验
来源：http://up.gzmigu.cn

@property 与 @x.setter 配合
来源：http://hk.panjiajie.cn

[U30] Py：数据类
来源：http://ws.shxzukj.cn

@dataclass(slots=True)
来源：http://lo.huanxung.cn

[U31] Py：单测
来源：http://tm.9csxet.cn

python -m pytest -q
来源：http://cq.hahajie.cn

[U32] Py：代码格式化
来源：http://ol.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://ua.9csxet.cn

[U33] Py：打包发布
来源：http://or.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://zn.lnxyls.cn

[U34] Py：判断编码
来源：http://xq.huixiangedu.cn

chardet.detect(raw)
来源：http://na.521024.cn

[U35] Py：发送邮件
来源：http://bn.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://av.huixiangedu.cn

[U36] Py：定时任务
来源：http://aw.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://yr.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://oi.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wb.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://ox.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://ew.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://lg.shxzukj.cn

sys.stdout.isatty()
来源：http://jc.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://xd.newstarts.cn

print("err", file=sys.stderr)
来源：http://rw.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://dk.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wl.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vl.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jx.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://df.9csxet.cn

namespace App\Http;
来源：http://rv.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://vu.haigaiapp.cn

declare(strict_types=1);
来源：http://iv.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://uu.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yf.yuexingan06.cn

[U46] PHP：可空类型
来源：http://ft.muxihuayi.cn

?string $name = null
来源：http://qu.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://np.huixinmuqiang.cn

int|string $id
来源：http://ps.lnxyls.cn

[U48] PHP：纯枚举
来源：http://ww.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ey.wgjwhj.cn

[U49] PHP：只读属性
来源：http://dt.huanxung.cn

public readonly string $name
来源：http://yh.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://we.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://ig.gzmigu.cn

[U51] PHP：数组解构
来源：http://kj.lnxyls.cn

[$a, $b] = $arr;
来源：http://mv.asd995.cn

[U52] PHP：箭头函数
来源：http://pk.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://hx.colortex.cn

[U53] PHP：空合并运算符
来源：http://sm.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://xa.lnxyls.cn

[U54] PHP：空安全调用
来源：http://hc.shxzukj.cn

$obj?->method()
来源：http://tq.shxzskj.cn

[U55] PHP：match 表达式
来源：http://sy.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rr.wgjwhj.cn

[U56] PHP：命名参数
来源：http://kc.wgjwhj.cn

f(a: 1, b: 2)
来源：http://zo.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://xw.521024.cn

"值: {$a}"
来源：http://kj.gzmigu.cn

[U58] PHP：数组三件套
来源：http://zh.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://go.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://vd.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ad.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://cj.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://em.haigaiapp.cn

[U61] PHP：正则
来源：http://km.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zu.asd995.cn

[U62] PHP：日期对象
来源：http://pq.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zn.shxzskj.cn

[U63] PHP：文件读写
来源：http://kq.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sq.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://xc.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://ob.huixinmuqiang.cn

[U65] PHP：会话
来源：http://xv.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ds.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://iy.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nf.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://xf.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vl.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://mj.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zh.shxzukj.cn


<!-- 参考信息 -->