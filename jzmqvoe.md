代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://pg.bjjhwx.cn

[S23] C：随机数
来源：http://zi.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cl.shtwfgs.cn

[S24] C：获取本地时间
来源：http://xd.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rz.shtwfgs.cn

[S25] C：内存拷贝
来源：http://qj.muxihuayi.cn

memcpy(dst, src, n);
来源：http://ti.shxzukj.cn

[S26] C：内存清零
来源：http://xk.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://vs.huanxung.cn

[S27] C：定义常量
来源：http://xi.panjiajie.cn

const double PI = 3.14159;
来源：http://jy.szsharing.cn

[S28] C：静态变量
来源：http://dn.asd995.cn

static int counter = 0;
来源：http://jc.jctech888.com.cn

[S29] C：变参函数
来源：http://yd.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ll.521024.cn

[S30] C：头文件保护
来源：http://fa.jctech888.com.cn

#ifndef X_H
来源：http://cg.nicolike.cn

#define X_H
来源：http://pw.shxzskj.cn

#endif
来源：http://yt.lnxyls.cn

[S31] C++：Hello World
来源：http://jq.yuntaijiaju.cn

#include <iostream>
来源：http://lj.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://eg.yuexingan06.cn

[S32] C++：字符串
来源：http://rc.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://ic.colortex.cn

[S33] C++：vector 增删
来源：http://pg.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ks.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://dz.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://xh.hahajie.cn

[S35] C++：map
来源：http://tc.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yd.bjjhwx.cn

[S36] C++：unordered_map
来源：http://af.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://br.haigaiapp.cn

[S37] C++：set
来源：http://hz.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zg.shxzskj.cn

[S38] C++：排序
来源：http://bx.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://xa.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://xa.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kb.9csxet.cn

[S40] C++：查找元素
来源：http://tv.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vp.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://jm.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rk.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://od.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://jd.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://ji.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://op.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://np.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://vz.nszjky.cn

[S45] C++：lambda
来源：http://xx.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zd.panjiajie.cn

[S46] C++：函数模板
来源：http://nj.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zr.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://kx.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://da.shxzukj.cn

[S48] C++：逐行读文件
来源：http://zg.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xq.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://mo.bookmarksfly.cn

[S49] C++：写文件
来源：http://wm.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jv.szsharing.cn

[S50] C++：格式化数字
来源：http://xc.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://en.newstarts.cn

[S51] C++：显式类型转换
来源：http://zd.yuexingan06.cn

static_cast<double>(a) / b
来源：http://oc.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://wj.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://hi.huixiangedu.cn

[S53] C++：移动语义
来源：http://nn.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://qb.szsharing.cn

[S54] C++：异常处理
来源：http://wa.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eg.colortex.cn

[S55] C++：结构化绑定
来源：http://yb.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hq.huanxung.cn

[S56] C++：optional
来源：http://dg.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fq.9csxet.cn

[S57] C++：编译期常量
来源：http://ap.shxzskj.cn

constexpr int N = 10;
来源：http://bl.yuexingan06.cn

[S58] C++：命名空间
来源：http://vm.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://ky.colortex.cn

[S59] C++：静态断言
来源：http://nc.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tg.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://yj.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lz.bookmarksfly.cn

================================================================================
来源：http://ju.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kg.gzmigu.cn

================================================================================
来源：http://ju.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://xh.9csxet.cn

println("Hello")
来源：http://xf.muxihuayi.cn

[T02] Kotlin：变量
来源：http://py.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://om.asd995.cn

[T03] Kotlin：字符串模板
来源：http://pk.haigaiapp.cn

"值: $b"
来源：http://hw.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://el.gzmigu.cn

val n: String? = null;  n?.length
来源：http://ey.521024.cn

[T05] Kotlin：when 表达式
来源：http://il.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mc.hahajie.cn

[T06] Kotlin：集合映射
来源：http://oi.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yh.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://pa.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vr.szsharing.cn

[T08] Kotlin：数据类
来源：http://ft.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://lw.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://iw.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://vt.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://nf.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cr.muxihuayi.cn

[T11] Kotlin：协程
来源：http://px.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cj.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://lw.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://kr.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://xi.asd995.cn

val m = mapOf("a" to 1)
来源：http://oi.521024.cn

[T14] Kotlin：循环
来源：http://tu.9csxet.cn

for (i in 1..10) println(i)
来源：http://dq.wgjwhj.cn

[T15] Kotlin：接口
来源：http://bb.newstarts.cn

interface Shape { fun area(): Double }
来源：http://kl.huanxung.cn

[T16] Swift：Hello World
来源：http://of.shxzukj.cn

print("Hello")
来源：http://al.newstarts.cn

[T17] Swift：变量与常量
来源：http://qn.hnjuh.cn

var a = 1;  let b = 2
来源：http://ur.szxytkj.cn

[T18] Swift：字符串插值
来源：http://cj.huanxung.cn

"值: \(b)"
来源：http://mv.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://kv.huixiangedu.cn

if let n = opt { print(n) }
来源：http://yp.haigaiapp.cn

[T20] Swift：数组操作
来源：http://ym.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xn.nszjky.cn

[T21] Swift：遍历
来源：http://jv.yuexingan06.cn

for x in a { print(x) }
来源：http://sl.shxzukj.cn

[T22] Swift：字典
来源：http://kp.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ar.colortex.cn

[T23] Swift：函数
来源：http://pi.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mc.szxytkj.cn

[T24] Swift：闭包
来源：http://gj.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://op.chemitech.net.cn

[T25] Swift：结构体
来源：http://it.huixinmuqiang.cn

struct P { var x: Int }
来源：http://dd.9csxet.cn

[T26] Swift：类与重写
来源：http://fl.szxytkj.cn

class A: Base { override func f() {} }
来源：http://cs.muxihuayi.cn

[T27] Swift：错误处理
来源：http://wt.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://ri.nszjky.cn

[T28] Swift：枚举
来源：http://ci.shxzskj.cn

enum Color { case red, green }
来源：http://gb.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://vn.yuexingan06.cn

guard let x = opt else { return }
来源：http://tv.huixinmuqiang.cn

[T30] Swift：协议
来源：http://su.colortex.cn

protocol Shape { func area() -> Double }
来源：http://rc.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://xm.newstarts.cn

print("Hello")
来源：http://hu.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://px.lnxyls.cn

local a = 1
来源：http://bp.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://ek.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ta.colortex.cn

[T34] Lua：遍历表
来源：http://gl.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dc.nicolike.cn

[T35] Lua：字典表
来源：http://xk.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://of.panjiajie.cn

[T36] Lua：函数
来源：http://xv.shxzskj.cn

function add(a, b) return a + b end
来源：http://be.9csxet.cn

[T37] Lua：字符串拼接
来源：http://xy.gzmigu.cn

"a" .. "b"
来源：http://rr.shxzskj.cn

[T38] Lua：条件
来源：http://ad.colortex.cn

if x > 0 then print("正") end
来源：http://zp.hnjuh.cn

[T39] Lua：模式匹配
来源：http://yo.muxihuayi.cn

string.find(s, "%d+")
来源：http://ni.huanxung.cn

[T40] Lua：元表
来源：http://vl.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://eu.huanxung.cn

[T41] Perl：Hello World
来源：http://bt.lnxyls.cn

print "Hello\n";
来源：http://sh.hnjuh.cn

[T42] Perl：变量类型
来源：http://vh.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nb.lnxyls.cn

[T43] Perl：字符串插值
来源：http://pg.shxzukj.cn

"值: $a"
来源：http://rv.nicolike.cn

[T44] Perl：条件
来源：http://xd.asd995.cn

if ($a > 0) { print "正"; }
来源：http://rt.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://dg.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://zx.asd995.cn

[T46] Perl：哈希操作
来源：http://qx.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bi.huanxung.cn

[T47] Perl：正则捕获
来源：http://cf.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ky.shxzskj.cn

[T48] Perl：正则替换
来源：http://tu.szsharing.cn

$s =~ s/old/new/g;
来源：http://vb.521024.cn

[T49] Perl：函数
来源：http://hw.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pm.szsharing.cn

[T50] Perl：逐行读文件
来源：http://qc.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://po.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://dw.panjiajie.cn

[T51] Scala：Hello World
来源：http://ed.shxzukj.cn

println("Hello")
来源：http://tq.chemitech.net.cn

[T52] Scala：变量
来源：http://pa.haigaiapp.cn

val a = 1;  var b = 2
来源：http://lm.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://px.szsharing.cn

s"值: $b"
来源：http://pt.szxytkj.cn

[T54] Scala：集合映射
来源：http://dg.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://te.panjiajie.cn

[T55] Scala：集合过滤
来源：http://bm.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://az.panjiajie.cn

[T56] Scala：样例类
来源：http://jm.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://cp.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://ml.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dh.huixiangedu.cn

[T58] Scala：函数定义
来源：http://di.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://su.jianghongdianzi.cn

[T59] Scala：循环
来源：http://tl.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://yq.shxzskj.cn

[T60] Scala：折叠
来源：http://oc.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xy.yuexingan06.cn

================================================================================
来源：http://pq.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://go.9csxet.cn

================================================================================
来源：http://ar.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://sh.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hx.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://xu.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aa.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://tp.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ow.hahajie.cn

[U04] Py：变量调试打印
来源：http://ni.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iz.521024.cn

[U05] Py：列表去重且保序
来源：http://ul.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://lb.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://kl.hahajie.cn

{**a, **b}
来源：http://ar.nszjky.cn

[U07] Py：反转字典键值
来源：http://gz.9csxet.cn

{v: k for k, v in d.items()}
来源：http://gb.szxytkj.cn

[U08] Py：展平二维列表
来源：http://kb.huixiangedu.cn

[y for x in nested for y in x]
来源：http://yn.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://wz.wgjwhj.cn

max(d, key=d.get)
来源：http://os.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://da.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nv.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://fl.shtwfgs.cn

(x * 2 for x in arr)
来源：http://yi.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zr.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://cz.nszjky.cn

[U13] Py：固定长度队列
来源：http://wt.nicolike.cn

deque(maxlen=10)
来源：http://rx.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://ic.newstarts.cn

defaultdict(list)
来源：http://wo.huixiangedu.cn

[U15] Py：高精度计时
来源：http://mv.lnxyls.cn

t = time.perf_counter()
来源：http://sx.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://ko.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mp.lnxyls.cn

[U17] Py：初始化日志
来源：http://vc.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://mw.szsharing.cn

[U18] Py：预编译正则
来源：http://eu.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://xt.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://jr.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://az.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://nr.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://nu.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://gj.lnxyls.cn

@contextlib.contextmanager
来源：http://hr.szsharing.cn

[U22] Py：矩阵转置
来源：http://ju.nicolike.cn

list(zip(*m))
来源：http://ph.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://tg.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ts.nszjky.cn

[U24] Py：路径操作
来源：http://tm.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xp.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://tp.chemitech.net.cn

csv.DictReader(f)
来源：http://xg.hnjuh.cn

[U26] Py：并发下载
来源：http://gd.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ns.panjiajie.cn

[U27] Py：异步 HTTP
来源：http://ok.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://kj.huanxung.cn

[U28] Py：类型别名
来源：http://gy.asd995.cn

UserId = int
来源：http://re.szxytkj.cn

[U29] Py：属性校验
来源：http://vy.gzmigu.cn

@property 与 @x.setter 配合
来源：http://br.shtwfgs.cn

[U30] Py：数据类
来源：http://wk.colortex.cn

@dataclass(slots=True)
来源：http://ea.szxytkj.cn

[U31] Py：单测
来源：http://ax.haigaiapp.cn

python -m pytest -q
来源：http://en.panjiajie.cn

[U32] Py：代码格式化
来源：http://ni.huixiangedu.cn

ruff format . && ruff check --fix .
来源：http://tg.9csxet.cn

[U33] Py：打包发布
来源：http://vu.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ol.jctech888.com.cn

[U34] Py：判断编码
来源：http://kt.huanxung.cn

chardet.detect(raw)
来源：http://eu.521024.cn

[U35] Py：发送邮件
来源：http://rh.jianghongdianzi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qv.jctech888.com.cn

[U36] Py：定时任务
来源：http://jt.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://yv.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://ak.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fe.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://ph.521024.cn

Path(__file__).resolve().parent
来源：http://oq.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://jt.nszjky.cn

sys.stdout.isatty()
来源：http://en.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://ap.newstarts.cn

print("err", file=sys.stderr)
来源：http://at.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://rj.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vo.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://cs.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uv.asd995.cn

[U43] PHP：声明命名空间
来源：http://kv.muxihuayi.cn

namespace App\Http;
来源：http://rv.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://kx.yuntaijiaju.cn

declare(strict_types=1);
来源：http://zp.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://tp.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pn.nszjky.cn

[U46] PHP：可空类型
来源：http://kw.nszjky.cn

?string $name = null
来源：http://dc.bjjhwx.cn


<!-- 参考信息 -->