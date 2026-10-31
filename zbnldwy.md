代发 wailian999

[S33] C++：vector 增删
来源：http://po.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://th.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://pf.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://di.521024.cn

[S35] C++：map
来源：http://er.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ig.panjiajie.cn

[S36] C++：unordered_map
来源：http://ag.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mt.gzmigu.cn

[S37] C++：set
来源：http://gi.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mg.yuntaijiaju.cn

[S38] C++：排序
来源：http://vq.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://mx.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://lo.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bn.szsharing.cn

[S40] C++：查找元素
来源：http://fx.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tc.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://ee.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://st.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://wv.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://vt.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://ws.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://uh.panjiajie.cn

[S44] C++：引用传参
来源：http://bt.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://rg.chemitech.net.cn

[S45] C++：lambda
来源：http://dv.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mp.panjiajie.cn

[S46] C++：函数模板
来源：http://hy.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gq.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://di.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rg.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://hy.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ud.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://ei.huanxung.cn

[S49] C++：写文件
来源：http://wd.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sk.asd995.cn

[S50] C++：格式化数字
来源：http://gt.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nu.521024.cn

[S51] C++：显式类型转换
来源：http://no.chemitech.net.cn

static_cast<double>(a) / b
来源：http://bo.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://wi.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://sl.wgjwhj.cn

[S53] C++：移动语义
来源：http://qs.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://jm.shxzukj.cn

[S54] C++：异常处理
来源：http://in.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bn.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://cq.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ja.muxihuayi.cn

[S56] C++：optional
来源：http://ky.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ih.shtwfgs.cn

[S57] C++：编译期常量
来源：http://wg.yuntaijiaju.cn

constexpr int N = 10;
来源：http://ip.shtwfgs.cn

[S58] C++：命名空间
来源：http://rw.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://yx.huixiangedu.cn

[S59] C++：静态断言
来源：http://lt.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ul.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://km.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ve.jianghongdianzi.cn

================================================================================
来源：http://wf.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vn.huixinmuqiang.cn

================================================================================
来源：http://yq.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://pa.shxzukj.cn

println("Hello")
来源：http://hp.szsharing.cn

[T02] Kotlin：变量
来源：http://iq.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://so.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://yl.bjjhwx.cn

"值: $b"
来源：http://yq.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://za.9csxet.cn

val n: String? = null;  n?.length
来源：http://xp.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://ct.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ha.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://vd.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ly.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://uu.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fv.szsharing.cn

[T08] Kotlin：数据类
来源：http://sx.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://sp.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://zh.asd995.cn

fun String.exclaim() = this + "!"
来源：http://md.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ys.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://md.521024.cn

[T11] Kotlin：协程
来源：http://sa.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vo.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://pr.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://lm.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://vx.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://lk.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ze.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://zo.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://vj.hahajie.cn

interface Shape { fun area(): Double }
来源：http://yw.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://uu.szxytkj.cn

print("Hello")
来源：http://va.521024.cn

[T17] Swift：变量与常量
来源：http://um.szsharing.cn

var a = 1;  let b = 2
来源：http://wp.colortex.cn

[T18] Swift：字符串插值
来源：http://im.colortex.cn

"值: \(b)"
来源：http://tw.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://cn.hahajie.cn

if let n = opt { print(n) }
来源：http://du.wgjwhj.cn

[T20] Swift：数组操作
来源：http://su.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dn.521024.cn

[T21] Swift：遍历
来源：http://ri.bjjhwx.cn

for x in a { print(x) }
来源：http://zi.jctech888.com.cn

[T22] Swift：字典
来源：http://pg.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://is.hnjuh.cn

[T23] Swift：函数
来源：http://gg.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pf.lnxyls.cn

[T24] Swift：闭包
来源：http://bo.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wk.shxzukj.cn

[T25] Swift：结构体
来源：http://kg.bookmarksfly.cn

struct P { var x: Int }
来源：http://ew.yuexingan06.cn

[T26] Swift：类与重写
来源：http://od.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://ux.huixiangedu.cn

[T27] Swift：错误处理
来源：http://vn.colortex.cn

do { try f() } catch { print(error) }
来源：http://qs.wgjwhj.cn

[T28] Swift：枚举
来源：http://ss.newstarts.cn

enum Color { case red, green }
来源：http://yi.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://bl.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://hh.szsharing.cn

[T30] Swift：协议
来源：http://hy.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://pq.huanxung.cn

[T31] Lua：Hello World
来源：http://gg.chemitech.net.cn

print("Hello")
来源：http://jx.muxihuayi.cn

[T32] Lua：局部变量
来源：http://td.szxytkj.cn

local a = 1
来源：http://cw.hnjuh.cn

[T33] Lua：表（数组）
来源：http://gz.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zn.jctech888.com.cn

[T34] Lua：遍历表
来源：http://ol.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bo.shxzukj.cn

[T35] Lua：字典表
来源：http://fg.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://ae.newstarts.cn

[T36] Lua：函数
来源：http://og.wgjwhj.cn

function add(a, b) return a + b end
来源：http://bx.huanxung.cn

[T37] Lua：字符串拼接
来源：http://fy.hnjuh.cn

"a" .. "b"
来源：http://cf.colortex.cn

[T38] Lua：条件
来源：http://zl.hnjuh.cn

if x > 0 then print("正") end
来源：http://hr.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://yn.lnxyls.cn

string.find(s, "%d+")
来源：http://oh.hnjuh.cn

[T40] Lua：元表
来源：http://du.521024.cn

setmetatable({}, { __index = base })
来源：http://hk.521024.cn

[T41] Perl：Hello World
来源：http://jz.bjjhwx.cn

print "Hello\n";
来源：http://rd.asd995.cn

[T42] Perl：变量类型
来源：http://kq.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qa.9csxet.cn

[T43] Perl：字符串插值
来源：http://wv.panjiajie.cn

"值: $a"
来源：http://ji.nszjky.cn

[T44] Perl：条件
来源：http://cw.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://pa.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://yk.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://le.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://td.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hw.hahajie.cn

[T47] Perl：正则捕获
来源：http://bo.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://am.bjjhwx.cn

[T48] Perl：正则替换
来源：http://tm.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://uk.nicolike.cn

[T49] Perl：函数
来源：http://pw.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sw.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://ol.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tc.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://ph.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://me.nszjky.cn

println("Hello")
来源：http://sb.huixinmuqiang.cn

[T52] Scala：变量
来源：http://gk.gzmigu.cn

val a = 1;  var b = 2
来源：http://bb.521024.cn

[T53] Scala：字符串插值
来源：http://dv.szsharing.cn

s"值: $b"
来源：http://ko.asd995.cn

[T54] Scala：集合映射
来源：http://ac.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://hm.521024.cn

[T55] Scala：集合过滤
来源：http://zh.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ei.9csxet.cn

[T56] Scala：样例类
来源：http://uq.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://oa.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://qf.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://et.9csxet.cn

[T58] Scala：函数定义
来源：http://bd.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rv.haigaiapp.cn

[T59] Scala：循环
来源：http://ph.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://az.bjjhwx.cn

[T60] Scala：折叠
来源：http://ng.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://at.huixinmuqiang.cn

================================================================================
来源：http://ph.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ir.jctech888.com.cn

================================================================================
来源：http://be.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://vi.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cg.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://pg.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cj.521024.cn

[U03] Py：加载 .env 配置
来源：http://lr.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ab.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://rl.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xc.newstarts.cn

[U05] Py：列表去重且保序
来源：http://gl.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://bj.hnjuh.cn

[U06] Py：合并两个字典
来源：http://rs.huixiangedu.cn

{**a, **b}
来源：http://ix.521024.cn

[U07] Py：反转字典键值
来源：http://pj.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://fu.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://zh.huanxung.cn

[y for x in nested for y in x]
来源：http://hu.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://ca.nszjky.cn

max(d, key=d.get)
来源：http://yi.hnjuh.cn

[U10] Py：按值排序字典
来源：http://zb.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fw.colortex.cn

[U11] Py：生成器表达式
来源：http://it.newstarts.cn

(x * 2 for x in arr)
来源：http://jp.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://py.shxzskj.cn

Counter(arr).most_common(3)
来源：http://al.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://kx.haigaiapp.cn

deque(maxlen=10)
来源：http://wj.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://xi.9csxet.cn

defaultdict(list)
来源：http://ps.wgjwhj.cn

[U15] Py：高精度计时
来源：http://la.shxzukj.cn

t = time.perf_counter()
来源：http://jy.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://gy.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xi.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://pa.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nt.hahajie.cn

[U18] Py：预编译正则
来源：http://sh.9csxet.cn

pat = re.compile(r"\d+")
来源：http://tl.asd995.cn

[U19] Py：正则替换带回调
来源：http://zo.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gg.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://lb.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://mu.yuntaijiaju.cn

[U21] Py：自定义上下文管理器
来源：http://lo.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://vn.nicolike.cn

[U22] Py：矩阵转置
来源：http://fx.haigaiapp.cn

list(zip(*m))
来源：http://hn.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://lo.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sv.colortex.cn

[U24] Py：路径操作
来源：http://fo.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iu.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://ux.9csxet.cn

csv.DictReader(f)
来源：http://km.newstarts.cn

[U26] Py：并发下载
来源：http://nl.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oe.newstarts.cn

[U27] Py：异步 HTTP
来源：http://ba.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://gl.chemitech.net.cn

[U28] Py：类型别名
来源：http://zi.haigaiapp.cn

UserId = int
来源：http://nr.nicolike.cn

[U29] Py：属性校验
来源：http://fl.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://fa.hahajie.cn

[U30] Py：数据类
来源：http://ej.shxzskj.cn

@dataclass(slots=True)
来源：http://ec.9csxet.cn

[U31] Py：单测
来源：http://nc.nicolike.cn

python -m pytest -q
来源：http://py.shxzskj.cn

[U32] Py：代码格式化
来源：http://rn.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://no.szsharing.cn

[U33] Py：打包发布
来源：http://sc.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://qh.chemitech.net.cn

[U34] Py：判断编码
来源：http://jv.newstarts.cn

chardet.detect(raw)
来源：http://vw.shtwfgs.cn

[U35] Py：发送邮件
来源：http://xj.szxytkj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ob.hahajie.cn

[U36] Py：定时任务
来源：http://jv.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://qs.panjiajie.cn

[U37] Py：读写 Excel
来源：http://wt.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zc.gzmigu.cn

[U38] Py：获取脚本所在目录
来源：http://hr.hnjuh.cn

Path(__file__).resolve().parent
来源：http://ae.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://ru.huanxung.cn

sys.stdout.isatty()
来源：http://rs.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ju.szsharing.cn

print("err", file=sys.stderr)
来源：http://qb.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://js.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ux.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://ze.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://od.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://wa.hahajie.cn

namespace App\Http;
来源：http://ch.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://ue.521024.cn

declare(strict_types=1);
来源：http://hw.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://qe.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uq.9csxet.cn

[U46] PHP：可空类型
来源：http://ah.521024.cn

?string $name = null
来源：http://cd.lnxyls.cn

[U47] PHP：联合类型
来源：http://de.panjiajie.cn

int|string $id
来源：http://xy.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://nz.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iz.gzmigu.cn

[U49] PHP：只读属性
来源：http://qa.shxzukj.cn

public readonly string $name
来源：http://pw.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://cs.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://lz.wgjwhj.cn

[U51] PHP：数组解构
来源：http://mr.asd995.cn

[$a, $b] = $arr;
来源：http://yp.huanxung.cn

[U52] PHP：箭头函数
来源：http://av.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://mo.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://qn.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://eb.szsharing.cn

[U54] PHP：空安全调用
来源：http://ih.panjiajie.cn

$obj?->method()
来源：http://wd.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://wb.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wi.szsharing.cn

[U56] PHP：命名参数
来源：http://fh.wgjwhj.cn

f(a: 1, b: 2)
来源：http://ew.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://vp.panjiajie.cn

"值: {$a}"
来源：http://ug.newstarts.cn

[U58] PHP：数组三件套
来源：http://on.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zy.asd995.cn


<!-- 参考信息 -->