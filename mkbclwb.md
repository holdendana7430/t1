代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bm.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://re.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hs.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://gi.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://my.newstarts.cn

[S10] C：指针与解引用
来源：http://ha.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://fu.gzmigu.cn

[S11] C：逐行读文件
来源：http://md.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://ct.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tk.521024.cn

fclose(f);
来源：http://hz.jctech888.com.cn

[S12] C：写文件
来源：http://qy.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://la.bjjhwx.cn

[S13] C：宏定义
来源：http://up.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vv.shxzskj.cn

[S14] C：枚举
来源：http://sa.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://uz.nszjky.cn

[S15] C：类型转换
来源：http://lf.wgjwhj.cn

(double) a / b
来源：http://rl.bjjhwx.cn

[S16] C：位操作置位
来源：http://eg.huanxung.cn

x |= (1 << 3);
来源：http://vu.newstarts.cn

[S17] C：安全拼接字符串
来源：http://rd.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ue.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://jr.nszjky.cn

int main(int argc, char **argv)
来源：http://af.szxytkj.cn

[S19] C：快速排序
来源：http://ds.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eu.521024.cn

[S20] C：二分查找
来源：http://xt.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wr.asd995.cn

[S21] C：字符类别判断
来源：http://dw.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gk.asd995.cn

[S22] C：字符串转数字
来源：http://st.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yt.panjiajie.cn

[S23] C：随机数
来源：http://sk.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bu.hnjuh.cn

[S24] C：获取本地时间
来源：http://az.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cb.gzmigu.cn

[S25] C：内存拷贝
来源：http://jk.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://nj.jctech888.com.cn

[S26] C：内存清零
来源：http://na.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://tm.shtwfgs.cn

[S27] C：定义常量
来源：http://gb.hahajie.cn

const double PI = 3.14159;
来源：http://zj.yuntaijiaju.cn

[S28] C：静态变量
来源：http://rn.szsharing.cn

static int counter = 0;
来源：http://ww.szsharing.cn

[S29] C：变参函数
来源：http://iu.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ec.shxzskj.cn

[S30] C：头文件保护
来源：http://mn.haigaiapp.cn

#ifndef X_H
来源：http://qv.muxihuayi.cn

#define X_H
来源：http://hz.shtwfgs.cn

#endif
来源：http://qa.9csxet.cn

[S31] C++：Hello World
来源：http://np.521024.cn

#include <iostream>
来源：http://vb.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://rq.muxihuayi.cn

[S32] C++：字符串
来源：http://bq.asd995.cn

std::string s = "hi";  s += "!";
来源：http://ev.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://xm.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wh.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://nd.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://xr.jianghongdianzi.cn

[S35] C++：map
来源：http://og.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yy.huixiangedu.cn

[S36] C++：unordered_map
来源：http://vd.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://co.jctech888.com.cn

[S37] C++：set
来源：http://mx.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://so.bookmarksfly.cn

[S38] C++：排序
来源：http://so.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://mb.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://yo.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bt.hahajie.cn

[S40] C++：查找元素
来源：http://my.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wg.shxzukj.cn

[S41] C++：类与构造函数
来源：http://jf.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ht.colortex.cn

[S42] C++：继承与虚函数
来源：http://pt.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://hf.jctech888.com.cn

[S43] C++：智能指针
来源：http://vw.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://st.nicolike.cn

[S44] C++：引用传参
来源：http://ux.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://zw.lnxyls.cn

[S45] C++：lambda
来源：http://in.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://so.asd995.cn

[S46] C++：函数模板
来源：http://vp.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iu.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://mh.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oa.9csxet.cn

[S48] C++：逐行读文件
来源：http://yc.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vx.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://kt.chemitech.net.cn

[S49] C++：写文件
来源：http://mu.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lk.jctech888.com.cn

[S50] C++：格式化数字
来源：http://jh.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qa.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://fy.9csxet.cn

static_cast<double>(a) / b
来源：http://hc.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://fe.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://nm.lnxyls.cn

[S53] C++：移动语义
来源：http://bf.521024.cn

std::vector<int> w = std::move(v);
来源：http://vc.yuexingan06.cn

[S54] C++：异常处理
来源：http://rj.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aw.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://ku.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wi.szsharing.cn

[S56] C++：optional
来源：http://fa.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kg.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://kg.yuntaijiaju.cn

constexpr int N = 10;
来源：http://cy.huixiangedu.cn

[S58] C++：命名空间
来源：http://ep.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://se.hahajie.cn

[S59] C++：静态断言
来源：http://pr.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tr.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://fx.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qf.huixiangedu.cn

================================================================================
来源：http://ww.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rx.bjjhwx.cn

================================================================================
来源：http://ls.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://jf.nicolike.cn

println("Hello")
来源：http://mv.hahajie.cn

[T02] Kotlin：变量
来源：http://mb.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://al.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://wo.newstarts.cn

"值: $b"
来源：http://nt.lnxyls.cn

[T04] Kotlin：空安全
来源：http://xh.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://kc.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://mc.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ls.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://yo.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fh.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://yw.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xd.nicolike.cn

[T08] Kotlin：数据类
来源：http://zh.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://bi.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://hy.asd995.cn

fun String.exclaim() = this + "!"
来源：http://vs.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ku.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zt.haigaiapp.cn

[T11] Kotlin：协程
来源：http://gz.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kp.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://pr.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://sc.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://lp.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://aj.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://bl.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://ue.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://lp.huanxung.cn

interface Shape { fun area(): Double }
来源：http://lx.panjiajie.cn

[T16] Swift：Hello World
来源：http://yq.huanxung.cn

print("Hello")
来源：http://kd.asd995.cn

[T17] Swift：变量与常量
来源：http://yb.huanxung.cn

var a = 1;  let b = 2
来源：http://ps.gzmigu.cn

[T18] Swift：字符串插值
来源：http://ov.shtwfgs.cn

"值: \(b)"
来源：http://ho.gzmigu.cn

[T19] Swift：可选绑定
来源：http://zf.bjjhwx.cn

if let n = opt { print(n) }
来源：http://on.huanxung.cn

[T20] Swift：数组操作
来源：http://gg.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sv.szxytkj.cn

[T21] Swift：遍历
来源：http://hl.shtwfgs.cn

for x in a { print(x) }
来源：http://li.yuexingan06.cn

[T22] Swift：字典
来源：http://xc.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ox.lnxyls.cn

[T23] Swift：函数
来源：http://xv.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ap.chemitech.net.cn

[T24] Swift：闭包
来源：http://vu.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xg.szsharing.cn

[T25] Swift：结构体
来源：http://ws.muxihuayi.cn

struct P { var x: Int }
来源：http://dw.9csxet.cn

[T26] Swift：类与重写
来源：http://tq.9csxet.cn

class A: Base { override func f() {} }
来源：http://gm.newstarts.cn

[T27] Swift：错误处理
来源：http://mp.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://tu.shxzukj.cn

[T28] Swift：枚举
来源：http://nc.gzmigu.cn

enum Color { case red, green }
来源：http://eo.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://wf.jctech888.com.cn

guard let x = opt else { return }
来源：http://lv.gzmigu.cn

[T30] Swift：协议
来源：http://qu.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://bt.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ob.shxzskj.cn

print("Hello")
来源：http://ld.colortex.cn

[T32] Lua：局部变量
来源：http://rx.colortex.cn

local a = 1
来源：http://oe.lnxyls.cn

[T33] Lua：表（数组）
来源：http://cz.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nu.shtwfgs.cn

[T34] Lua：遍历表
来源：http://pa.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cc.muxihuayi.cn

[T35] Lua：字典表
来源：http://ib.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://wq.521024.cn

[T36] Lua：函数
来源：http://hz.colortex.cn

function add(a, b) return a + b end
来源：http://zi.9csxet.cn

[T37] Lua：字符串拼接
来源：http://gw.yuexingan06.cn

"a" .. "b"
来源：http://qy.newstarts.cn

[T38] Lua：条件
来源：http://eu.muxihuayi.cn

if x > 0 then print("正") end
来源：http://ds.szsharing.cn

[T39] Lua：模式匹配
来源：http://lj.gzmigu.cn

string.find(s, "%d+")
来源：http://mo.hnjuh.cn

[T40] Lua：元表
来源：http://tp.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://vw.muxihuayi.cn

[T41] Perl：Hello World
来源：http://cv.jctech888.com.cn

print "Hello\n";
来源：http://tq.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://is.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cr.hahajie.cn

[T43] Perl：字符串插值
来源：http://wj.panjiajie.cn

"值: $a"
来源：http://mu.szxytkj.cn

[T44] Perl：条件
来源：http://ld.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://ky.shxzskj.cn

[T45] Perl：数组遍历
来源：http://ln.asd995.cn

for my $x (@arr) { print $x; }
来源：http://ni.szsharing.cn

[T46] Perl：哈希操作
来源：http://hm.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sd.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://qz.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zx.huanxung.cn

[T48] Perl：正则替换
来源：http://si.9csxet.cn

$s =~ s/old/new/g;
来源：http://xw.jianghongdianzi.cn

[T49] Perl：函数
来源：http://ne.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xw.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://gj.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jo.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ri.shxzukj.cn

[T51] Scala：Hello World
来源：http://pb.lnxyls.cn

println("Hello")
来源：http://rr.gzmigu.cn

[T52] Scala：变量
来源：http://xw.huanxung.cn

val a = 1;  var b = 2
来源：http://il.hnjuh.cn

[T53] Scala：字符串插值
来源：http://vf.newstarts.cn

s"值: $b"
来源：http://zn.colortex.cn

[T54] Scala：集合映射
来源：http://eo.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://kd.521024.cn

[T55] Scala：集合过滤
来源：http://wf.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mg.521024.cn

[T56] Scala：样例类
来源：http://uv.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://zq.panjiajie.cn

[T57] Scala：模式匹配
来源：http://mz.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tf.9csxet.cn

[T58] Scala：函数定义
来源：http://dh.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qj.9csxet.cn

[T59] Scala：循环
来源：http://px.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://lo.wgjwhj.cn

[T60] Scala：折叠
来源：http://my.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gk.szxytkj.cn

================================================================================
来源：http://oo.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xh.asd995.cn

================================================================================
来源：http://as.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://jn.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dh.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://je.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uz.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://ko.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fj.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://hj.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://em.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://nn.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://rb.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://ve.haigaiapp.cn

{**a, **b}
来源：http://tq.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://qp.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://as.asd995.cn

[U08] Py：展平二维列表
来源：http://ev.wgjwhj.cn

[y for x in nested for y in x]
来源：http://vp.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://du.lnxyls.cn

max(d, key=d.get)
来源：http://eq.asd995.cn

[U10] Py：按值排序字典
来源：http://lf.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sb.shxzukj.cn

[U11] Py：生成器表达式
来源：http://up.chemitech.net.cn

(x * 2 for x in arr)
来源：http://zn.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pb.hahajie.cn

Counter(arr).most_common(3)
来源：http://by.panjiajie.cn

[U13] Py：固定长度队列
来源：http://tv.lnxyls.cn

deque(maxlen=10)
来源：http://iv.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://gk.panjiajie.cn

defaultdict(list)
来源：http://vu.9csxet.cn

[U15] Py：高精度计时
来源：http://xi.nicolike.cn

t = time.perf_counter()
来源：http://wd.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://gb.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qj.gzmigu.cn

[U17] Py：初始化日志
来源：http://dq.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://gm.muxihuayi.cn

[U18] Py：预编译正则
来源：http://hx.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://sz.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://ly.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qb.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://mp.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://nj.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://ls.hahajie.cn

@contextlib.contextmanager
来源：http://ay.nszjky.cn

[U22] Py：矩阵转置
来源：http://wq.lnxyls.cn

list(zip(*m))
来源：http://zm.szsharing.cn

[U23] Py：分块读取大文件
来源：http://zp.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://km.wgjwhj.cn

[U24] Py：路径操作
来源：http://bc.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fa.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://ec.nicolike.cn

csv.DictReader(f)
来源：http://gf.chemitech.net.cn

[U26] Py：并发下载
来源：http://jw.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qh.huanxung.cn

[U27] Py：异步 HTTP
来源：http://md.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://kp.9csxet.cn

[U28] Py：类型别名
来源：http://re.bookmarksfly.cn

UserId = int
来源：http://ym.9csxet.cn

[U29] Py：属性校验
来源：http://an.asd995.cn

@property 与 @x.setter 配合
来源：http://jz.huanxung.cn

[U30] Py：数据类
来源：http://vn.nicolike.cn

@dataclass(slots=True)
来源：http://oy.shtwfgs.cn


<!-- 参考信息 -->