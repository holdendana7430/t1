代发 wailian999

int x; scanf("%d", &x);
来源：http://tr.newstarts.cn

[S04] C：字符串复制
来源：http://sj.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://od.nicolike.cn

[S05] C：字符串长度
来源：http://xo.jianghongdianzi.cn

strlen(s)
来源：http://od.9csxet.cn

[S06] C：字符串比较
来源：http://ku.muxihuayi.cn

strcmp(a, b) == 0
来源：http://ai.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ag.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lc.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://xm.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fn.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://oc.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hi.asd995.cn

[S10] C：指针与解引用
来源：http://mw.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ku.colortex.cn

[S11] C：逐行读文件
来源：http://gu.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://kj.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://up.lnxyls.cn

fclose(f);
来源：http://ke.huixiangedu.cn

[S12] C：写文件
来源：http://cg.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vl.huixiangedu.cn

[S13] C：宏定义
来源：http://lf.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nm.huanxung.cn

[S14] C：枚举
来源：http://po.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://zi.shtwfgs.cn

[S15] C：类型转换
来源：http://pa.jianghongdianzi.cn

(double) a / b
来源：http://np.bookmarksfly.cn

[S16] C：位操作置位
来源：http://jz.nszjky.cn

x |= (1 << 3);
来源：http://qz.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://yz.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gy.huixiangedu.cn

[S18] C：命令行参数
来源：http://wo.521024.cn

int main(int argc, char **argv)
来源：http://na.hnjuh.cn

[S19] C：快速排序
来源：http://pj.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://if.newstarts.cn

[S20] C：二分查找
来源：http://xh.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://py.gzmigu.cn

[S21] C：字符类别判断
来源：http://xl.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ay.9csxet.cn

[S22] C：字符串转数字
来源：http://gm.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bi.newstarts.cn

[S23] C：随机数
来源：http://tn.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uf.shtwfgs.cn

[S24] C：获取本地时间
来源：http://jx.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sb.bjjhwx.cn

[S25] C：内存拷贝
来源：http://ii.szxytkj.cn

memcpy(dst, src, n);
来源：http://yi.shxzskj.cn

[S26] C：内存清零
来源：http://vg.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://la.huanxung.cn

[S27] C：定义常量
来源：http://nc.lnxyls.cn

const double PI = 3.14159;
来源：http://mr.9csxet.cn

[S28] C：静态变量
来源：http://cv.gzmigu.cn

static int counter = 0;
来源：http://gp.huixiangedu.cn

[S29] C：变参函数
来源：http://xf.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bp.szxytkj.cn

[S30] C：头文件保护
来源：http://as.panjiajie.cn

#ifndef X_H
来源：http://tn.panjiajie.cn

#define X_H
来源：http://gc.nicolike.cn

#endif
来源：http://jl.chemitech.net.cn

[S31] C++：Hello World
来源：http://zz.muxihuayi.cn

#include <iostream>
来源：http://dq.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://cy.shxzukj.cn

[S32] C++：字符串
来源：http://sn.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://ee.szxytkj.cn

[S33] C++：vector 增删
来源：http://xl.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hj.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://vt.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://lw.colortex.cn

[S35] C++：map
来源：http://hc.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lm.szsharing.cn

[S36] C++：unordered_map
来源：http://tk.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pq.gzmigu.cn

[S37] C++：set
来源：http://md.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pt.shxzskj.cn

[S38] C++：排序
来源：http://qe.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://ob.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://if.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kh.shtwfgs.cn

[S40] C++：查找元素
来源：http://eh.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pj.nszjky.cn

[S41] C++：类与构造函数
来源：http://fv.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rw.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://cs.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://nq.wgjwhj.cn

[S43] C++：智能指针
来源：http://fp.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://mx.huixiangedu.cn

[S44] C++：引用传参
来源：http://lh.szsharing.cn

void inc(int &x) { ++x; }
来源：http://py.chemitech.net.cn

[S45] C++：lambda
来源：http://kj.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gy.bjjhwx.cn

[S46] C++：函数模板
来源：http://ai.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hj.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://rg.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cf.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://gu.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pz.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://rf.shxzukj.cn

[S49] C++：写文件
来源：http://bz.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ds.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://jv.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ga.lnxyls.cn

[S51] C++：显式类型转换
来源：http://ew.shtwfgs.cn

static_cast<double>(a) / b
来源：http://vy.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://ze.newstarts.cn

int size() const noexcept { return n_; }
来源：http://tl.huixiangedu.cn

[S53] C++：移动语义
来源：http://sr.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://gm.9csxet.cn

[S54] C++：异常处理
来源：http://eb.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ev.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://va.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jk.haigaiapp.cn

[S56] C++：optional
来源：http://ga.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cw.huanxung.cn

[S57] C++：编译期常量
来源：http://cp.shxzskj.cn

constexpr int N = 10;
来源：http://yl.jctech888.com.cn

[S58] C++：命名空间
来源：http://dw.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://zn.colortex.cn

[S59] C++：静态断言
来源：http://wg.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://my.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://kl.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ia.asd995.cn

================================================================================
来源：http://bt.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kq.haigaiapp.cn

================================================================================
来源：http://sp.colortex.cn

[T01] Kotlin：Hello World
来源：http://oj.huixiangedu.cn

println("Hello")
来源：http://by.asd995.cn

[T02] Kotlin：变量
来源：http://zn.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cy.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://sx.shxzskj.cn

"值: $b"
来源：http://re.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://cg.lnxyls.cn

val n: String? = null;  n?.length
来源：http://xw.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://tn.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rq.newstarts.cn

[T06] Kotlin：集合映射
来源：http://ir.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rp.asd995.cn

[T07] Kotlin：集合过滤
来源：http://ni.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gb.nszjky.cn

[T08] Kotlin：数据类
来源：http://qf.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://sj.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://yi.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://ks.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://vu.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jv.9csxet.cn

[T11] Kotlin：协程
来源：http://rn.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yw.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://gv.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://ke.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://jw.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://dz.nicolike.cn

[T14] Kotlin：循环
来源：http://nf.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://mf.haigaiapp.cn

[T15] Kotlin：接口
来源：http://ir.newstarts.cn

interface Shape { fun area(): Double }
来源：http://uy.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://sy.wgjwhj.cn

print("Hello")
来源：http://tv.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://lw.521024.cn

var a = 1;  let b = 2
来源：http://qu.shxzskj.cn

[T18] Swift：字符串插值
来源：http://jt.jianghongdianzi.cn

"值: \(b)"
来源：http://bk.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://bg.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://fd.nicolike.cn

[T20] Swift：数组操作
来源：http://hd.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bg.bjjhwx.cn

[T21] Swift：遍历
来源：http://rt.yuexingan06.cn

for x in a { print(x) }
来源：http://kx.hnjuh.cn

[T22] Swift：字典
来源：http://zc.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sm.hahajie.cn

[T23] Swift：函数
来源：http://md.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cp.muxihuayi.cn

[T24] Swift：闭包
来源：http://pd.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mo.huixiangedu.cn

[T25] Swift：结构体
来源：http://ac.chemitech.net.cn

struct P { var x: Int }
来源：http://fd.huanxung.cn

[T26] Swift：类与重写
来源：http://uu.panjiajie.cn

class A: Base { override func f() {} }
来源：http://he.9csxet.cn

[T27] Swift：错误处理
来源：http://ic.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://wj.hahajie.cn

[T28] Swift：枚举
来源：http://vu.panjiajie.cn

enum Color { case red, green }
来源：http://ya.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://yg.nicolike.cn

guard let x = opt else { return }
来源：http://tf.newstarts.cn

[T30] Swift：协议
来源：http://qi.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://cd.lnxyls.cn

[T31] Lua：Hello World
来源：http://iz.szsharing.cn

print("Hello")
来源：http://ax.bjjhwx.cn

[T32] Lua：局部变量
来源：http://cl.newstarts.cn

local a = 1
来源：http://dc.huanxung.cn

[T33] Lua：表（数组）
来源：http://mr.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sz.bjjhwx.cn

[T34] Lua：遍历表
来源：http://cw.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iv.shxzskj.cn

[T35] Lua：字典表
来源：http://pg.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://qu.9csxet.cn

[T36] Lua：函数
来源：http://ie.wgjwhj.cn

function add(a, b) return a + b end
来源：http://cd.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://vd.9csxet.cn

"a" .. "b"
来源：http://dx.bookmarksfly.cn

[T38] Lua：条件
来源：http://ey.jctech888.com.cn

if x > 0 then print("正") end
来源：http://tg.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://mc.asd995.cn

string.find(s, "%d+")
来源：http://xy.panjiajie.cn

[T40] Lua：元表
来源：http://mo.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://pj.panjiajie.cn

[T41] Perl：Hello World
来源：http://je.bjjhwx.cn

print "Hello\n";
来源：http://sr.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://ab.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mi.colortex.cn

[T43] Perl：字符串插值
来源：http://sa.huixinmuqiang.cn

"值: $a"
来源：http://tk.huanxung.cn

[T44] Perl：条件
来源：http://yn.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://uj.521024.cn

[T45] Perl：数组遍历
来源：http://ed.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://hw.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://zk.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oy.9csxet.cn

[T47] Perl：正则捕获
来源：http://it.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pp.nicolike.cn

[T48] Perl：正则替换
来源：http://sg.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://tw.muxihuayi.cn

[T49] Perl：函数
来源：http://vn.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://us.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://vo.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ks.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://my.huixiangedu.cn

[T51] Scala：Hello World
来源：http://wd.wgjwhj.cn

println("Hello")
来源：http://me.jctech888.com.cn

[T52] Scala：变量
来源：http://rm.chemitech.net.cn

val a = 1;  var b = 2
来源：http://ae.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://ck.huixiangedu.cn

s"值: $b"
来源：http://yb.panjiajie.cn

[T54] Scala：集合映射
来源：http://pd.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://bf.shxzskj.cn

[T55] Scala：集合过滤
来源：http://nf.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mf.nszjky.cn

[T56] Scala：样例类
来源：http://dh.colortex.cn

case class User(name: String, age: Int)
来源：http://vd.shxzskj.cn

[T57] Scala：模式匹配
来源：http://ym.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xk.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://qi.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://li.asd995.cn

[T59] Scala：循环
来源：http://kk.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://an.haigaiapp.cn

[T60] Scala：折叠
来源：http://ff.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ml.521024.cn

================================================================================
来源：http://hp.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lk.shxzukj.cn

================================================================================
来源：http://bn.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://tw.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://os.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://pa.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uv.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://vs.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iu.panjiajie.cn

[U04] Py：变量调试打印
来源：http://kn.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lp.9csxet.cn

[U05] Py：列表去重且保序
来源：http://ai.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://ag.newstarts.cn

[U06] Py：合并两个字典
来源：http://rx.lnxyls.cn

{**a, **b}
来源：http://oo.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://tk.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://yw.nicolike.cn

[U08] Py：展平二维列表
来源：http://tr.muxihuayi.cn

[y for x in nested for y in x]
来源：http://em.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ub.newstarts.cn

max(d, key=d.get)
来源：http://mh.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://fw.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rn.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://uw.shxzskj.cn

(x * 2 for x in arr)
来源：http://tl.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kf.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://op.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://dz.huanxung.cn

deque(maxlen=10)
来源：http://on.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://zv.huanxung.cn

defaultdict(list)
来源：http://qy.shxzukj.cn

[U15] Py：高精度计时
来源：http://bl.9csxet.cn

t = time.perf_counter()
来源：http://mf.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://dp.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hq.521024.cn

[U17] Py：初始化日志
来源：http://hr.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ak.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://ob.huanxung.cn

pat = re.compile(r"\d+")
来源：http://qq.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://ke.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jo.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://wt.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://jt.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://jp.gzmigu.cn

@contextlib.contextmanager
来源：http://pr.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://nx.haigaiapp.cn

list(zip(*m))
来源：http://wt.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://ok.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://de.shxzukj.cn

[U24] Py：路径操作
来源：http://vr.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nl.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://pp.asd995.cn

csv.DictReader(f)
来源：http://kj.colortex.cn

[U26] Py：并发下载
来源：http://zc.shtwfgs.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ix.9csxet.cn


<!-- 参考信息 -->