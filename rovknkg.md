代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://oh.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://od.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://sf.szsharing.cn

[S03] C：读入整数
来源：http://uq.panjiajie.cn

int x; scanf("%d", &x);
来源：http://nj.hahajie.cn

[S04] C：字符串复制
来源：http://zd.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lo.jctech888.com.cn

[S05] C：字符串长度
来源：http://ql.bjjhwx.cn

strlen(s)
来源：http://fm.jctech888.com.cn

[S06] C：字符串比较
来源：http://ak.yuexingan06.cn

strcmp(a, b) == 0
来源：http://wp.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://nj.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nx.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://lf.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ct.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://mx.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lx.yuexingan06.cn

[S10] C：指针与解引用
来源：http://nw.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ao.wgjwhj.cn

[S11] C：逐行读文件
来源：http://ar.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://rp.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zd.wgjwhj.cn

fclose(f);
来源：http://yl.lnxyls.cn

[S12] C：写文件
来源：http://vq.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ao.panjiajie.cn

[S13] C：宏定义
来源：http://ux.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tr.wgjwhj.cn

[S14] C：枚举
来源：http://wn.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://gd.huixiangedu.cn

[S15] C：类型转换
来源：http://gw.jctech888.com.cn

(double) a / b
来源：http://sp.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://xt.shxzukj.cn

x |= (1 << 3);
来源：http://ey.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://pa.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pv.bjjhwx.cn

[S18] C：命令行参数
来源：http://gm.newstarts.cn

int main(int argc, char **argv)
来源：http://sr.newstarts.cn

[S19] C：快速排序
来源：http://be.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ge.asd995.cn

[S20] C：二分查找
来源：http://mt.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dq.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://hz.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://je.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://nd.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vs.huanxung.cn

[S23] C：随机数
来源：http://pf.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://st.asd995.cn

[S24] C：获取本地时间
来源：http://ay.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://za.szxytkj.cn

[S25] C：内存拷贝
来源：http://qy.huixiangedu.cn

memcpy(dst, src, n);
来源：http://dc.bookmarksfly.cn

[S26] C：内存清零
来源：http://dm.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://ow.521024.cn

[S27] C：定义常量
来源：http://ah.9csxet.cn

const double PI = 3.14159;
来源：http://tn.521024.cn

[S28] C：静态变量
来源：http://pr.521024.cn

static int counter = 0;
来源：http://eh.521024.cn

[S29] C：变参函数
来源：http://df.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eb.hnjuh.cn

[S30] C：头文件保护
来源：http://mn.panjiajie.cn

#ifndef X_H
来源：http://rt.shtwfgs.cn

#define X_H
来源：http://gs.lnxyls.cn

#endif
来源：http://xw.huanxung.cn

[S31] C++：Hello World
来源：http://zu.nszjky.cn

#include <iostream>
来源：http://je.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ml.lnxyls.cn

[S32] C++：字符串
来源：http://cb.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://sq.gzmigu.cn

[S33] C++：vector 增删
来源：http://mp.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ht.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://gl.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://vh.szxytkj.cn

[S35] C++：map
来源：http://xc.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ho.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://po.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jk.lnxyls.cn

[S37] C++：set
来源：http://ck.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cy.yuntaijiaju.cn

[S38] C++：排序
来源：http://op.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://la.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://vl.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://du.haigaiapp.cn

[S40] C++：查找元素
来源：http://jy.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qk.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://ll.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dw.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://si.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://yv.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://il.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://rt.gzmigu.cn

[S44] C++：引用传参
来源：http://ka.9csxet.cn

void inc(int &x) { ++x; }
来源：http://bj.haigaiapp.cn

[S45] C++：lambda
来源：http://nw.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xc.asd995.cn

[S46] C++：函数模板
来源：http://xj.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uh.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://an.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bw.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://fn.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ue.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://dp.szxytkj.cn

[S49] C++：写文件
来源：http://an.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sb.9csxet.cn

[S50] C++：格式化数字
来源：http://rh.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eb.shxzskj.cn

[S51] C++：显式类型转换
来源：http://ov.szsharing.cn

static_cast<double>(a) / b
来源：http://yb.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://kz.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://yj.panjiajie.cn

[S53] C++：移动语义
来源：http://aq.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://zp.gzmigu.cn

[S54] C++：异常处理
来源：http://oq.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ou.9csxet.cn

[S55] C++：结构化绑定
来源：http://ac.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uu.jianghongdianzi.cn

[S56] C++：optional
来源：http://tb.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ez.huixiangedu.cn

[S57] C++：编译期常量
来源：http://xd.szxytkj.cn

constexpr int N = 10;
来源：http://xi.9csxet.cn

[S58] C++：命名空间
来源：http://ko.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://ny.colortex.cn

[S59] C++：静态断言
来源：http://kr.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rp.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://hb.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qn.huixinmuqiang.cn

================================================================================
来源：http://hc.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://et.szsharing.cn

================================================================================
来源：http://zb.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://uj.newstarts.cn

println("Hello")
来源：http://dy.muxihuayi.cn

[T02] Kotlin：变量
来源：http://xa.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ui.asd995.cn

[T03] Kotlin：字符串模板
来源：http://wf.panjiajie.cn

"值: $b"
来源：http://jm.shxzskj.cn

[T04] Kotlin：空安全
来源：http://mi.huanxung.cn

val n: String? = null;  n?.length
来源：http://mz.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://qx.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zc.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://wa.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lp.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://ep.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dm.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://ih.colortex.cn

data class User(val name: String, val age: Int)
来源：http://hq.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://ga.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://dq.asd995.cn

[T10] Kotlin：默认参数
来源：http://cc.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tk.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ho.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ea.colortex.cn

[T12] Kotlin：解构声明
来源：http://wo.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://zn.asd995.cn

[T13] Kotlin：只读 Map
来源：http://ib.nicolike.cn

val m = mapOf("a" to 1)
来源：http://oy.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://kb.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://sy.shtwfgs.cn

[T15] Kotlin：接口
来源：http://bf.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://yi.shxzukj.cn

[T16] Swift：Hello World
来源：http://nd.newstarts.cn

print("Hello")
来源：http://ag.colortex.cn

[T17] Swift：变量与常量
来源：http://jf.521024.cn

var a = 1;  let b = 2
来源：http://vr.panjiajie.cn

[T18] Swift：字符串插值
来源：http://de.huixiangedu.cn

"值: \(b)"
来源：http://su.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://xk.nszjky.cn

if let n = opt { print(n) }
来源：http://ia.panjiajie.cn

[T20] Swift：数组操作
来源：http://qq.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ff.huanxung.cn

[T21] Swift：遍历
来源：http://hc.szsharing.cn

for x in a { print(x) }
来源：http://gp.521024.cn

[T22] Swift：字典
来源：http://kd.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ty.hnjuh.cn

[T23] Swift：函数
来源：http://ap.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://we.muxihuayi.cn

[T24] Swift：闭包
来源：http://rs.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ab.huanxung.cn

[T25] Swift：结构体
来源：http://aj.colortex.cn

struct P { var x: Int }
来源：http://vi.jctech888.com.cn

[T26] Swift：类与重写
来源：http://ny.hnjuh.cn

class A: Base { override func f() {} }
来源：http://vw.huanxung.cn

[T27] Swift：错误处理
来源：http://qs.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://ef.wgjwhj.cn

[T28] Swift：枚举
来源：http://yu.lnxyls.cn

enum Color { case red, green }
来源：http://mu.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://hr.lnxyls.cn

guard let x = opt else { return }
来源：http://zi.gzmigu.cn

[T30] Swift：协议
来源：http://ry.521024.cn

protocol Shape { func area() -> Double }
来源：http://za.haigaiapp.cn

[T31] Lua：Hello World
来源：http://qd.colortex.cn

print("Hello")
来源：http://yy.shtwfgs.cn

[T32] Lua：局部变量
来源：http://vq.shxzukj.cn

local a = 1
来源：http://rp.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://sv.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ys.nszjky.cn

[T34] Lua：遍历表
来源：http://kc.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sq.bookmarksfly.cn

[T35] Lua：字典表
来源：http://ws.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://ma.haigaiapp.cn

[T36] Lua：函数
来源：http://qx.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://wu.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://ca.hahajie.cn

"a" .. "b"
来源：http://if.newstarts.cn

[T38] Lua：条件
来源：http://xb.szxytkj.cn

if x > 0 then print("正") end
来源：http://uy.gzmigu.cn

[T39] Lua：模式匹配
来源：http://di.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://aq.jianghongdianzi.cn

[T40] Lua：元表
来源：http://pn.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://nv.shtwfgs.cn

[T41] Perl：Hello World
来源：http://gw.asd995.cn

print "Hello\n";
来源：http://gc.asd995.cn

[T42] Perl：变量类型
来源：http://db.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ot.szxytkj.cn

[T43] Perl：字符串插值
来源：http://mi.shxzukj.cn

"值: $a"
来源：http://ox.szxytkj.cn

[T44] Perl：条件
来源：http://kk.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://jy.szxytkj.cn

[T45] Perl：数组遍历
来源：http://vi.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://fm.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://mt.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qi.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ba.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vz.gzmigu.cn

[T48] Perl：正则替换
来源：http://pg.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://xw.huixinmuqiang.cn

[T49] Perl：函数
来源：http://bh.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fc.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://xi.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hc.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://zw.jctech888.com.cn

[T51] Scala：Hello World
来源：http://ly.muxihuayi.cn

println("Hello")
来源：http://el.newstarts.cn

[T52] Scala：变量
来源：http://ta.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://wl.panjiajie.cn

[T53] Scala：字符串插值
来源：http://dx.shtwfgs.cn

s"值: $b"
来源：http://so.yuexingan06.cn

[T54] Scala：集合映射
来源：http://mg.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://nh.lnxyls.cn

[T55] Scala：集合过滤
来源：http://fz.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uf.shtwfgs.cn

[T56] Scala：样例类
来源：http://xd.panjiajie.cn

case class User(name: String, age: Int)
来源：http://hk.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://dx.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://np.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://yd.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cw.huanxung.cn

[T59] Scala：循环
来源：http://fn.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://ie.panjiajie.cn

[T60] Scala：折叠
来源：http://hk.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uq.chemitech.net.cn

================================================================================
来源：http://ht.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://if.szsharing.cn

================================================================================
来源：http://bv.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://cj.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gx.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://ps.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ws.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://pl.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gc.newstarts.cn

[U04] Py：变量调试打印
来源：http://fc.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qc.huanxung.cn

[U05] Py：列表去重且保序
来源：http://mt.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://at.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://kl.lnxyls.cn

{**a, **b}
来源：http://xf.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://rq.colortex.cn

{v: k for k, v in d.items()}
来源：http://qi.9csxet.cn

[U08] Py：展平二维列表
来源：http://iv.chemitech.net.cn

[y for x in nested for y in x]
来源：http://yk.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://kx.lnxyls.cn

max(d, key=d.get)
来源：http://yu.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://wp.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tf.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://ar.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://pn.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pq.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://rd.shxzskj.cn

[U13] Py：固定长度队列
来源：http://uw.newstarts.cn

deque(maxlen=10)
来源：http://sm.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://cp.panjiajie.cn

defaultdict(list)
来源：http://nz.shxzukj.cn

[U15] Py：高精度计时
来源：http://ma.shxzukj.cn

t = time.perf_counter()
来源：http://ij.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://uw.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://re.shxzukj.cn

[U17] Py：初始化日志
来源：http://ee.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://ki.shtwfgs.cn

[U18] Py：预编译正则
来源：http://gt.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://ca.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://du.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ai.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://gx.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://lo.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://bx.wgjwhj.cn

@contextlib.contextmanager
来源：http://hm.szsharing.cn

[U22] Py：矩阵转置
来源：http://nm.shxzukj.cn

list(zip(*m))
来源：http://cs.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://fj.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jl.hahajie.cn

[U24] Py：路径操作
来源：http://gw.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ky.colortex.cn


<!-- 参考信息 -->