代发 wailian999

int x; scanf("%d", &x);
来源：http://yb.colortex.cn

[S04] C：字符串复制
来源：http://xs.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ox.hnjuh.cn

[S05] C：字符串长度
来源：http://gk.yuntaijiaju.cn

strlen(s)
来源：http://xv.521024.cn

[S06] C：字符串比较
来源：http://to.huanxung.cn

strcmp(a, b) == 0
来源：http://yv.gzmigu.cn

[S07] C：数组遍历求和
来源：http://aa.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fe.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://gq.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hy.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://ab.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nv.jctech888.com.cn

[S10] C：指针与解引用
来源：http://yn.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://rn.newstarts.cn

[S11] C：逐行读文件
来源：http://fb.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://td.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cd.szsharing.cn

fclose(f);
来源：http://pm.521024.cn

[S12] C：写文件
来源：http://nk.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vf.hahajie.cn

[S13] C：宏定义
来源：http://ap.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yt.szxytkj.cn

[S14] C：枚举
来源：http://ur.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://wm.shxzukj.cn

[S15] C：类型转换
来源：http://uj.chemitech.net.cn

(double) a / b
来源：http://at.shxzskj.cn

[S16] C：位操作置位
来源：http://nw.huixiangedu.cn

x |= (1 << 3);
来源：http://bq.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://qf.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cr.521024.cn

[S18] C：命令行参数
来源：http://jo.hnjuh.cn

int main(int argc, char **argv)
来源：http://pt.huixinmuqiang.cn

[S19] C：快速排序
来源：http://vh.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zk.panjiajie.cn

[S20] C：二分查找
来源：http://gq.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dg.panjiajie.cn

[S21] C：字符类别判断
来源：http://gi.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wu.9csxet.cn

[S22] C：字符串转数字
来源：http://ed.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qt.huixinmuqiang.cn

[S23] C：随机数
来源：http://fl.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ib.nszjky.cn

[S24] C：获取本地时间
来源：http://pk.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tq.shtwfgs.cn

[S25] C：内存拷贝
来源：http://ds.shxzukj.cn

memcpy(dst, src, n);
来源：http://sq.muxihuayi.cn

[S26] C：内存清零
来源：http://qu.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://dt.gzmigu.cn

[S27] C：定义常量
来源：http://cm.hnjuh.cn

const double PI = 3.14159;
来源：http://is.9csxet.cn

[S28] C：静态变量
来源：http://cc.shtwfgs.cn

static int counter = 0;
来源：http://qm.huixiangedu.cn

[S29] C：变参函数
来源：http://mr.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jz.shxzukj.cn

[S30] C：头文件保护
来源：http://ne.huixiangedu.cn

#ifndef X_H
来源：http://ve.shxzskj.cn

#define X_H
来源：http://mm.szxytkj.cn

#endif
来源：http://ko.lnxyls.cn

[S31] C++：Hello World
来源：http://sr.gzmigu.cn

#include <iostream>
来源：http://cn.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://rp.haigaiapp.cn

[S32] C++：字符串
来源：http://bl.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://gu.gzmigu.cn

[S33] C++：vector 增删
来源：http://sv.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aj.newstarts.cn

[S34] C++：遍历 vector
来源：http://fd.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://ae.newstarts.cn

[S35] C++：map
来源：http://ch.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xk.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://vu.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dw.bookmarksfly.cn

[S37] C++：set
来源：http://mf.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rd.muxihuayi.cn

[S38] C++：排序
来源：http://vs.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://em.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://ly.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qt.bjjhwx.cn

[S40] C++：查找元素
来源：http://dk.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://up.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://re.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bd.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://bm.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ol.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://tn.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://sm.shxzskj.cn

[S44] C++：引用传参
来源：http://ga.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://nr.asd995.cn

[S45] C++：lambda
来源：http://ad.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qa.wgjwhj.cn

[S46] C++：函数模板
来源：http://ei.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qa.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://zj.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qc.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://no.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://no.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://kl.huanxung.cn

[S49] C++：写文件
来源：http://ee.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yt.lnxyls.cn

[S50] C++：格式化数字
来源：http://yf.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nx.panjiajie.cn

[S51] C++：显式类型转换
来源：http://ka.szsharing.cn

static_cast<double>(a) / b
来源：http://mt.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://gv.colortex.cn

int size() const noexcept { return n_; }
来源：http://nr.panjiajie.cn

[S53] C++：移动语义
来源：http://bq.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://xd.szsharing.cn

[S54] C++：异常处理
来源：http://rs.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cb.newstarts.cn

[S55] C++：结构化绑定
来源：http://zs.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lj.9csxet.cn

[S56] C++：optional
来源：http://rf.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://id.nicolike.cn

[S57] C++：编译期常量
来源：http://lr.chemitech.net.cn

constexpr int N = 10;
来源：http://rb.lnxyls.cn

[S58] C++：命名空间
来源：http://yj.521024.cn

namespace ns { int f() { return 1; } }
来源：http://vr.panjiajie.cn

[S59] C++：静态断言
来源：http://lc.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ab.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://vc.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kq.newstarts.cn

================================================================================
来源：http://lu.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fj.521024.cn

================================================================================
来源：http://cq.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://nn.nszjky.cn

println("Hello")
来源：http://dd.chemitech.net.cn

[T02] Kotlin：变量
来源：http://hf.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pd.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://ts.nszjky.cn

"值: $b"
来源：http://nq.newstarts.cn

[T04] Kotlin：空安全
来源：http://iz.shxzskj.cn

val n: String? = null;  n?.length
来源：http://xn.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://ge.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fb.asd995.cn

[T06] Kotlin：集合映射
来源：http://vv.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://no.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://vw.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xo.szsharing.cn

[T08] Kotlin：数据类
来源：http://za.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://oq.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://ei.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://uf.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ri.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nu.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ae.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vq.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://dz.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://fp.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://pt.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://gi.asd995.cn

[T14] Kotlin：循环
来源：http://pu.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://sl.gzmigu.cn

[T15] Kotlin：接口
来源：http://sw.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://vt.shtwfgs.cn

[T16] Swift：Hello World
来源：http://xs.huixiangedu.cn

print("Hello")
来源：http://ev.colortex.cn

[T17] Swift：变量与常量
来源：http://os.chemitech.net.cn

var a = 1;  let b = 2
来源：http://iw.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://ln.muxihuayi.cn

"值: \(b)"
来源：http://ip.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://zz.jctech888.com.cn

if let n = opt { print(n) }
来源：http://zu.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://jj.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kx.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://bo.yuexingan06.cn

for x in a { print(x) }
来源：http://hv.colortex.cn

[T22] Swift：字典
来源：http://af.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jt.jctech888.com.cn

[T23] Swift：函数
来源：http://nx.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://si.521024.cn

[T24] Swift：闭包
来源：http://dh.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bu.huixiangedu.cn

[T25] Swift：结构体
来源：http://hq.shtwfgs.cn

struct P { var x: Int }
来源：http://gb.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://zy.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://vb.bjjhwx.cn

[T27] Swift：错误处理
来源：http://aj.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://sk.gzmigu.cn

[T28] Swift：枚举
来源：http://ip.huixiangedu.cn

enum Color { case red, green }
来源：http://ty.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://nb.huanxung.cn

guard let x = opt else { return }
来源：http://vq.bookmarksfly.cn

[T30] Swift：协议
来源：http://ku.colortex.cn

protocol Shape { func area() -> Double }
来源：http://vw.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://yz.yuntaijiaju.cn

print("Hello")
来源：http://hb.gzmigu.cn

[T32] Lua：局部变量
来源：http://bm.wgjwhj.cn

local a = 1
来源：http://ea.szsharing.cn

[T33] Lua：表（数组）
来源：http://va.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kj.asd995.cn

[T34] Lua：遍历表
来源：http://yp.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cm.haigaiapp.cn

[T35] Lua：字典表
来源：http://hl.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://kt.shxzskj.cn

[T36] Lua：函数
来源：http://qf.chemitech.net.cn

function add(a, b) return a + b end
来源：http://cr.asd995.cn

[T37] Lua：字符串拼接
来源：http://xj.shxzukj.cn

"a" .. "b"
来源：http://ea.wgjwhj.cn

[T38] Lua：条件
来源：http://yp.wgjwhj.cn

if x > 0 then print("正") end
来源：http://mo.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://bd.nicolike.cn

string.find(s, "%d+")
来源：http://bk.szxytkj.cn

[T40] Lua：元表
来源：http://fu.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ay.huanxung.cn

[T41] Perl：Hello World
来源：http://pl.yuexingan06.cn

print "Hello\n";
来源：http://yi.shxzukj.cn

[T42] Perl：变量类型
来源：http://gj.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yj.shxzskj.cn

[T43] Perl：字符串插值
来源：http://lb.gzmigu.cn

"值: $a"
来源：http://ld.hnjuh.cn

[T44] Perl：条件
来源：http://uf.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://oo.shxzskj.cn

[T45] Perl：数组遍历
来源：http://nl.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://ea.shxzukj.cn

[T46] Perl：哈希操作
来源：http://om.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ey.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://da.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tr.shtwfgs.cn

[T48] Perl：正则替换
来源：http://hu.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://lk.szxytkj.cn

[T49] Perl：函数
来源：http://ad.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ju.szsharing.cn

[T50] Perl：逐行读文件
来源：http://el.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kh.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ve.bjjhwx.cn

[T51] Scala：Hello World
来源：http://vj.huixiangedu.cn

println("Hello")
来源：http://hr.chemitech.net.cn

[T52] Scala：变量
来源：http://mh.yuexingan06.cn

val a = 1;  var b = 2
来源：http://gp.hahajie.cn

[T53] Scala：字符串插值
来源：http://jd.lnxyls.cn

s"值: $b"
来源：http://jt.gzmigu.cn

[T54] Scala：集合映射
来源：http://zs.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://zd.szxytkj.cn

[T55] Scala：集合过滤
来源：http://pw.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nf.hnjuh.cn

[T56] Scala：样例类
来源：http://ff.szsharing.cn

case class User(name: String, age: Int)
来源：http://us.newstarts.cn

[T57] Scala：模式匹配
来源：http://gd.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gk.9csxet.cn

[T58] Scala：函数定义
来源：http://mc.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mv.haigaiapp.cn

[T59] Scala：循环
来源：http://yv.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://aw.shtwfgs.cn

[T60] Scala：折叠
来源：http://hz.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bd.521024.cn

================================================================================
来源：http://li.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mc.jctech888.com.cn

================================================================================
来源：http://ox.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://ar.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wy.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://im.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yr.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://ma.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uo.huanxung.cn

[U04] Py：变量调试打印
来源：http://bu.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zl.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://kn.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://cq.szsharing.cn

[U06] Py：合并两个字典
来源：http://bh.lnxyls.cn

{**a, **b}
来源：http://fu.nicolike.cn

[U07] Py：反转字典键值
来源：http://dl.hahajie.cn

{v: k for k, v in d.items()}
来源：http://pi.gzmigu.cn

[U08] Py：展平二维列表
来源：http://ro.panjiajie.cn

[y for x in nested for y in x]
来源：http://hy.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://xm.asd995.cn

max(d, key=d.get)
来源：http://by.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://re.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://za.lnxyls.cn

[U11] Py：生成器表达式
来源：http://dh.huanxung.cn

(x * 2 for x in arr)
来源：http://bz.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eo.gzmigu.cn

Counter(arr).most_common(3)
来源：http://yh.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://tn.panjiajie.cn

deque(maxlen=10)
来源：http://nd.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://ou.hahajie.cn

defaultdict(list)
来源：http://bl.nicolike.cn

[U15] Py：高精度计时
来源：http://pe.jctech888.com.cn

t = time.perf_counter()
来源：http://rj.colortex.cn

[U16] Py：命令行参数解析
来源：http://vm.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pd.jctech888.com.cn

[U17] Py：初始化日志
来源：http://bd.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://cp.muxihuayi.cn

[U18] Py：预编译正则
来源：http://tr.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://we.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://fl.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://es.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://al.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://dw.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://ty.shxzskj.cn

@contextlib.contextmanager
来源：http://dp.nszjky.cn

[U22] Py：矩阵转置
来源：http://xv.jctech888.com.cn

list(zip(*m))
来源：http://nl.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://mq.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sg.newstarts.cn

[U24] Py：路径操作
来源：http://xh.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xo.colortex.cn

[U25] Py：CSV 按字典读
来源：http://jc.jianghongdianzi.cn

csv.DictReader(f)
来源：http://za.hahajie.cn

[U26] Py：并发下载
来源：http://bz.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tz.jianghongdianzi.cn


<!-- 参考信息 -->