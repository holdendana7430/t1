代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://cp.hahajie.cn

[S02] C：变量与格式化输出
来源：http://ek.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://qc.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ll.colortex.cn

int x; scanf("%d", &x);
来源：http://qe.asd995.cn

[S04] C：字符串复制
来源：http://vh.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cd.lnxyls.cn

[S05] C：字符串长度
来源：http://dh.huixiangedu.cn

strlen(s)
来源：http://ez.huanxung.cn

[S06] C：字符串比较
来源：http://at.lnxyls.cn

strcmp(a, b) == 0
来源：http://au.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://dl.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ek.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://jf.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ym.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://xv.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aa.gzmigu.cn

[S10] C：指针与解引用
来源：http://jv.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://yv.lnxyls.cn

[S11] C：逐行读文件
来源：http://jl.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://ow.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bw.szsharing.cn

fclose(f);
来源：http://pu.521024.cn

[S12] C：写文件
来源：http://zy.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ft.9csxet.cn

[S13] C：宏定义
来源：http://se.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gk.521024.cn

[S14] C：枚举
来源：http://zw.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://yd.nicolike.cn

[S15] C：类型转换
来源：http://cc.yuexingan06.cn

(double) a / b
来源：http://df.wgjwhj.cn

[S16] C：位操作置位
来源：http://dl.9csxet.cn

x |= (1 << 3);
来源：http://as.nszjky.cn

[S17] C：安全拼接字符串
来源：http://zc.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cp.lnxyls.cn

[S18] C：命令行参数
来源：http://fr.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://cb.gzmigu.cn

[S19] C：快速排序
来源：http://hl.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qg.hahajie.cn

[S20] C：二分查找
来源：http://fn.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qi.yuexingan06.cn

[S21] C：字符类别判断
来源：http://uj.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ch.szsharing.cn

[S22] C：字符串转数字
来源：http://qd.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ek.lnxyls.cn

[S23] C：随机数
来源：http://ya.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rb.panjiajie.cn

[S24] C：获取本地时间
来源：http://tl.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://an.bjjhwx.cn

[S25] C：内存拷贝
来源：http://wo.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ky.9csxet.cn

[S26] C：内存清零
来源：http://sd.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://jk.chemitech.net.cn

[S27] C：定义常量
来源：http://sb.haigaiapp.cn

const double PI = 3.14159;
来源：http://xg.bookmarksfly.cn

[S28] C：静态变量
来源：http://cg.521024.cn

static int counter = 0;
来源：http://yf.muxihuayi.cn

[S29] C：变参函数
来源：http://rh.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ov.shxzukj.cn

[S30] C：头文件保护
来源：http://iy.huixiangedu.cn

#ifndef X_H
来源：http://of.521024.cn

#define X_H
来源：http://qq.szsharing.cn

#endif
来源：http://cg.szsharing.cn

[S31] C++：Hello World
来源：http://ji.bookmarksfly.cn

#include <iostream>
来源：http://mo.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://oz.haigaiapp.cn

[S32] C++：字符串
来源：http://bz.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://xi.hnjuh.cn

[S33] C++：vector 增删
来源：http://sy.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hr.hahajie.cn

[S34] C++：遍历 vector
来源：http://mm.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://fq.jctech888.com.cn

[S35] C++：map
来源：http://eg.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vq.hnjuh.cn

[S36] C++：unordered_map
来源：http://ch.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jk.nicolike.cn

[S37] C++：set
来源：http://ks.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ha.newstarts.cn

[S38] C++：排序
来源：http://bh.521024.cn

std::sort(v.begin(), v.end());
来源：http://ec.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://bg.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ri.panjiajie.cn

[S40] C++：查找元素
来源：http://sy.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cj.panjiajie.cn

[S41] C++：类与构造函数
来源：http://jd.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ob.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://ae.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://oc.nszjky.cn

[S43] C++：智能指针
来源：http://yi.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://vw.asd995.cn

[S44] C++：引用传参
来源：http://js.newstarts.cn

void inc(int &x) { ++x; }
来源：http://lm.jctech888.com.cn

[S45] C++：lambda
来源：http://cc.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://on.asd995.cn

[S46] C++：函数模板
来源：http://uc.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nd.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://rq.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ij.szsharing.cn

[S48] C++：逐行读文件
来源：http://pg.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qj.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://dz.huanxung.cn

[S49] C++：写文件
来源：http://ln.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.szxytkj.cn

[S50] C++：格式化数字
来源：http://al.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zq.9csxet.cn

[S51] C++：显式类型转换
来源：http://gz.asd995.cn

static_cast<double>(a) / b
来源：http://bc.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://px.hahajie.cn

int size() const noexcept { return n_; }
来源：http://qj.bjjhwx.cn

[S53] C++：移动语义
来源：http://xz.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://rl.9csxet.cn

[S54] C++：异常处理
来源：http://cj.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sy.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://cj.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://es.chemitech.net.cn

[S56] C++：optional
来源：http://tb.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://re.muxihuayi.cn

[S57] C++：编译期常量
来源：http://hj.huanxung.cn

constexpr int N = 10;
来源：http://nr.bookmarksfly.cn

[S58] C++：命名空间
来源：http://wa.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://no.bjjhwx.cn

[S59] C++：静态断言
来源：http://ol.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ua.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ww.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pa.wgjwhj.cn

================================================================================
来源：http://pm.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ws.bookmarksfly.cn

================================================================================
来源：http://gm.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://hj.yuntaijiaju.cn

println("Hello")
来源：http://xg.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://ba.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yr.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://pn.hnjuh.cn

"值: $b"
来源：http://fy.shxzukj.cn

[T04] Kotlin：空安全
来源：http://gv.nicolike.cn

val n: String? = null;  n?.length
来源：http://li.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://am.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sd.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://db.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jw.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://kn.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ht.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://qa.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://ny.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://zp.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://zz.szsharing.cn

[T10] Kotlin：默认参数
来源：http://om.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sm.nszjky.cn

[T11] Kotlin：协程
来源：http://vo.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://al.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://wb.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://td.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://it.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://hc.lnxyls.cn

[T14] Kotlin：循环
来源：http://np.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://zq.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://wb.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://bq.521024.cn

[T16] Swift：Hello World
来源：http://ie.shxzskj.cn

print("Hello")
来源：http://df.521024.cn

[T17] Swift：变量与常量
来源：http://ki.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://uq.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://pw.huixiangedu.cn

"值: \(b)"
来源：http://yk.nicolike.cn

[T19] Swift：可选绑定
来源：http://ne.muxihuayi.cn

if let n = opt { print(n) }
来源：http://vo.wgjwhj.cn

[T20] Swift：数组操作
来源：http://tt.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zu.wgjwhj.cn

[T21] Swift：遍历
来源：http://bv.shxzukj.cn

for x in a { print(x) }
来源：http://jx.hahajie.cn

[T22] Swift：字典
来源：http://sb.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bz.shxzukj.cn

[T23] Swift：函数
来源：http://fr.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jr.newstarts.cn

[T24] Swift：闭包
来源：http://nx.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dv.colortex.cn

[T25] Swift：结构体
来源：http://oa.yuntaijiaju.cn

struct P { var x: Int }
来源：http://gf.colortex.cn

[T26] Swift：类与重写
来源：http://yh.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://tp.gzmigu.cn

[T27] Swift：错误处理
来源：http://xp.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://qk.shtwfgs.cn

[T28] Swift：枚举
来源：http://fz.nicolike.cn

enum Color { case red, green }
来源：http://nf.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://ol.szsharing.cn

guard let x = opt else { return }
来源：http://eh.hahajie.cn

[T30] Swift：协议
来源：http://xx.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://mo.jctech888.com.cn

[T31] Lua：Hello World
来源：http://ga.bookmarksfly.cn

print("Hello")
来源：http://xt.asd995.cn

[T32] Lua：局部变量
来源：http://me.bjjhwx.cn

local a = 1
来源：http://cr.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://xj.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pb.haigaiapp.cn

[T34] Lua：遍历表
来源：http://nq.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://de.szsharing.cn

[T35] Lua：字典表
来源：http://xo.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://fs.9csxet.cn

[T36] Lua：函数
来源：http://yk.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://df.hahajie.cn

[T37] Lua：字符串拼接
来源：http://md.yuexingan06.cn

"a" .. "b"
来源：http://gg.521024.cn

[T38] Lua：条件
来源：http://iy.nicolike.cn

if x > 0 then print("正") end
来源：http://iy.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://wq.bookmarksfly.cn

string.find(s, "%d+")
来源：http://dn.newstarts.cn

[T40] Lua：元表
来源：http://pj.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://ly.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://qn.asd995.cn

print "Hello\n";
来源：http://ij.nicolike.cn

[T42] Perl：变量类型
来源：http://ho.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mj.lnxyls.cn

[T43] Perl：字符串插值
来源：http://cz.nicolike.cn

"值: $a"
来源：http://bp.hahajie.cn

[T44] Perl：条件
来源：http://ta.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://ji.nicolike.cn

[T45] Perl：数组遍历
来源：http://sv.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://ub.hnjuh.cn

[T46] Perl：哈希操作
来源：http://ph.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ej.521024.cn

[T47] Perl：正则捕获
来源：http://pg.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ge.panjiajie.cn

[T48] Perl：正则替换
来源：http://kx.lnxyls.cn

$s =~ s/old/new/g;
来源：http://un.nszjky.cn

[T49] Perl：函数
来源：http://sn.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ke.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://vc.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hl.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://tr.yuexingan06.cn

[T51] Scala：Hello World
来源：http://hb.gzmigu.cn

println("Hello")
来源：http://kh.jianghongdianzi.cn

[T52] Scala：变量
来源：http://oe.szsharing.cn

val a = 1;  var b = 2
来源：http://qm.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://ul.newstarts.cn

s"值: $b"
来源：http://bv.wgjwhj.cn

[T54] Scala：集合映射
来源：http://uv.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://aj.nszjky.cn

[T55] Scala：集合过滤
来源：http://re.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kv.bjjhwx.cn

[T56] Scala：样例类
来源：http://je.panjiajie.cn

case class User(name: String, age: Int)
来源：http://eo.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://qb.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rc.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://yy.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rk.jianghongdianzi.cn

[T59] Scala：循环
来源：http://rc.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://gr.chemitech.net.cn

[T60] Scala：折叠
来源：http://hc.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bm.521024.cn

================================================================================
来源：http://fc.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wx.szxytkj.cn

================================================================================
来源：http://ix.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://jg.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qx.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ke.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pw.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://pm.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://od.lnxyls.cn

[U04] Py：变量调试打印
来源：http://ph.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://je.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://mr.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://ee.huanxung.cn

[U06] Py：合并两个字典
来源：http://pb.gzmigu.cn

{**a, **b}
来源：http://zf.shxzukj.cn

[U07] Py：反转字典键值
来源：http://qf.newstarts.cn

{v: k for k, v in d.items()}
来源：http://py.colortex.cn

[U08] Py：展平二维列表
来源：http://fk.muxihuayi.cn

[y for x in nested for y in x]
来源：http://fw.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://en.jianghongdianzi.cn

max(d, key=d.get)
来源：http://zw.shxzskj.cn

[U10] Py：按值排序字典
来源：http://zs.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qu.huanxung.cn

[U11] Py：生成器表达式
来源：http://ub.colortex.cn

(x * 2 for x in arr)
来源：http://hw.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nh.9csxet.cn

Counter(arr).most_common(3)
来源：http://ty.nicolike.cn

[U13] Py：固定长度队列
来源：http://zv.gzmigu.cn

deque(maxlen=10)
来源：http://yf.9csxet.cn

[U14] Py：分组收集到列表
来源：http://tx.bjjhwx.cn

defaultdict(list)
来源：http://ua.yuexingan06.cn

[U15] Py：高精度计时
来源：http://gm.muxihuayi.cn

t = time.perf_counter()
来源：http://wt.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://uj.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ci.gzmigu.cn

[U17] Py：初始化日志
来源：http://os.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://vn.shtwfgs.cn

[U18] Py：预编译正则
来源：http://yl.9csxet.cn

pat = re.compile(r"\d+")
来源：http://vh.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://sm.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ay.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://lj.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://zb.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://if.521024.cn

@contextlib.contextmanager
来源：http://qz.hahajie.cn

[U22] Py：矩阵转置
来源：http://sa.bjjhwx.cn

list(zip(*m))
来源：http://kj.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://cx.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ez.shxzukj.cn

[U24] Py：路径操作
来源：http://my.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ge.newstarts.cn


<!-- 参考信息 -->