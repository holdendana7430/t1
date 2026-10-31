代发 wailian999

int x; scanf("%d", &x);
来源：http://sj.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://yh.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://aq.shxzskj.cn

[S05] C：字符串长度
来源：http://mv.chemitech.net.cn

strlen(s)
来源：http://kl.huanxung.cn

[S06] C：字符串比较
来源：http://on.hnjuh.cn

strcmp(a, b) == 0
来源：http://vl.panjiajie.cn

[S07] C：数组遍历求和
来源：http://aw.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ua.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://sj.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vd.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://sy.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vj.chemitech.net.cn

[S10] C：指针与解引用
来源：http://cp.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://jz.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://rs.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://wn.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nw.szxytkj.cn

fclose(f);
来源：http://kj.huixiangedu.cn

[S12] C：写文件
来源：http://kh.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ej.panjiajie.cn

[S13] C：宏定义
来源：http://si.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://by.muxihuayi.cn

[S14] C：枚举
来源：http://rn.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://mt.hnjuh.cn

[S15] C：类型转换
来源：http://zv.hahajie.cn

(double) a / b
来源：http://ho.hahajie.cn

[S16] C：位操作置位
来源：http://lg.haigaiapp.cn

x |= (1 << 3);
来源：http://ug.newstarts.cn

[S17] C：安全拼接字符串
来源：http://it.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cc.szsharing.cn

[S18] C：命令行参数
来源：http://wp.hnjuh.cn

int main(int argc, char **argv)
来源：http://ae.nszjky.cn

[S19] C：快速排序
来源：http://gp.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ot.jianghongdianzi.cn

[S20] C：二分查找
来源：http://mr.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kr.shtwfgs.cn

[S21] C：字符类别判断
来源：http://sq.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jb.panjiajie.cn

[S22] C：字符串转数字
来源：http://vy.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xy.szsharing.cn

[S23] C：随机数
来源：http://bh.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bl.newstarts.cn

[S24] C：获取本地时间
来源：http://wq.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ia.huixiangedu.cn

[S25] C：内存拷贝
来源：http://pj.huixiangedu.cn

memcpy(dst, src, n);
来源：http://zg.bookmarksfly.cn

[S26] C：内存清零
来源：http://xl.9csxet.cn

memset(a, 0, sizeof a);
来源：http://fd.jctech888.com.cn

[S27] C：定义常量
来源：http://uf.colortex.cn

const double PI = 3.14159;
来源：http://oi.huixinmuqiang.cn

[S28] C：静态变量
来源：http://bu.hahajie.cn

static int counter = 0;
来源：http://vj.nicolike.cn

[S29] C：变参函数
来源：http://tp.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lp.panjiajie.cn

[S30] C：头文件保护
来源：http://zw.nicolike.cn

#ifndef X_H
来源：http://bi.yuexingan06.cn

#define X_H
来源：http://cf.shxzskj.cn

#endif
来源：http://aj.wgjwhj.cn

[S31] C++：Hello World
来源：http://lc.asd995.cn

#include <iostream>
来源：http://hj.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://gi.newstarts.cn

[S32] C++：字符串
来源：http://mu.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://vg.shxzukj.cn

[S33] C++：vector 增删
来源：http://cy.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gc.panjiajie.cn

[S34] C++：遍历 vector
来源：http://vu.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ai.wgjwhj.cn

[S35] C++：map
来源：http://wo.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rz.nszjky.cn

[S36] C++：unordered_map
来源：http://xe.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bi.nszjky.cn

[S37] C++：set
来源：http://sv.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mp.nszjky.cn

[S38] C++：排序
来源：http://nb.asd995.cn

std::sort(v.begin(), v.end());
来源：http://dm.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://ve.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lp.haigaiapp.cn

[S40] C++：查找元素
来源：http://io.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lv.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://nq.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ck.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://bc.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://ll.szsharing.cn

[S43] C++：智能指针
来源：http://ju.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://zs.nszjky.cn

[S44] C++：引用传参
来源：http://tf.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://ia.nszjky.cn

[S45] C++：lambda
来源：http://zb.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qm.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://ko.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oy.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://dd.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ak.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://ue.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mp.szsharing.cn

while (std::getline(in, line)) { }
来源：http://rd.szxytkj.cn

[S49] C++：写文件
来源：http://js.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gg.muxihuayi.cn

[S50] C++：格式化数字
来源：http://ey.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://es.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://xw.hahajie.cn

static_cast<double>(a) / b
来源：http://kr.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://ed.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://yu.nicolike.cn

[S53] C++：移动语义
来源：http://ya.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://dr.nicolike.cn

[S54] C++：异常处理
来源：http://le.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ww.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://hy.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wk.szxytkj.cn

[S56] C++：optional
来源：http://jm.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dw.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://vg.nszjky.cn

constexpr int N = 10;
来源：http://zk.nicolike.cn

[S58] C++：命名空间
来源：http://fd.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://bd.shxzskj.cn

[S59] C++：静态断言
来源：http://ef.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ab.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://uo.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hh.colortex.cn

================================================================================
来源：http://cg.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://di.muxihuayi.cn

================================================================================
来源：http://fw.szsharing.cn

[T01] Kotlin：Hello World
来源：http://ra.shxzukj.cn

println("Hello")
来源：http://ex.nszjky.cn

[T02] Kotlin：变量
来源：http://yt.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ra.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://ao.bjjhwx.cn

"值: $b"
来源：http://op.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://zj.shxzukj.cn

val n: String? = null;  n?.length
来源：http://wr.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://nb.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ex.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://bm.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xq.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://ut.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gz.9csxet.cn

[T08] Kotlin：数据类
来源：http://rq.521024.cn

data class User(val name: String, val age: Int)
来源：http://ea.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://bg.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://dn.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://zy.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rq.wgjwhj.cn

[T11] Kotlin：协程
来源：http://ag.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jt.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://lx.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://sg.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://go.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://jj.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://nk.hnjuh.cn

for (i in 1..10) println(i)
来源：http://hf.shxzskj.cn

[T15] Kotlin：接口
来源：http://mi.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://td.newstarts.cn

[T16] Swift：Hello World
来源：http://ms.huanxung.cn

print("Hello")
来源：http://ei.gzmigu.cn

[T17] Swift：变量与常量
来源：http://ba.colortex.cn

var a = 1;  let b = 2
来源：http://wt.huanxung.cn

[T18] Swift：字符串插值
来源：http://wa.gzmigu.cn

"值: \(b)"
来源：http://pw.colortex.cn

[T19] Swift：可选绑定
来源：http://xc.shtwfgs.cn

if let n = opt { print(n) }
来源：http://eu.nszjky.cn

[T20] Swift：数组操作
来源：http://hu.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gg.newstarts.cn

[T21] Swift：遍历
来源：http://lk.hnjuh.cn

for x in a { print(x) }
来源：http://ss.huixiangedu.cn

[T22] Swift：字典
来源：http://mt.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fm.panjiajie.cn

[T23] Swift：函数
来源：http://kh.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bz.newstarts.cn

[T24] Swift：闭包
来源：http://ge.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tn.shxzukj.cn

[T25] Swift：结构体
来源：http://sm.jctech888.com.cn

struct P { var x: Int }
来源：http://bc.521024.cn

[T26] Swift：类与重写
来源：http://gn.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://ap.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://kk.nicolike.cn

do { try f() } catch { print(error) }
来源：http://kv.gzmigu.cn

[T28] Swift：枚举
来源：http://dv.huanxung.cn

enum Color { case red, green }
来源：http://um.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://fw.huanxung.cn

guard let x = opt else { return }
来源：http://hj.asd995.cn

[T30] Swift：协议
来源：http://cw.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://yr.shtwfgs.cn

[T31] Lua：Hello World
来源：http://so.jctech888.com.cn

print("Hello")
来源：http://rq.shxzskj.cn

[T32] Lua：局部变量
来源：http://gs.szxytkj.cn

local a = 1
来源：http://ov.huanxung.cn

[T33] Lua：表（数组）
来源：http://pb.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jb.hahajie.cn

[T34] Lua：遍历表
来源：http://du.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://et.yuexingan06.cn

[T35] Lua：字典表
来源：http://fq.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://ev.haigaiapp.cn

[T36] Lua：函数
来源：http://nx.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://ww.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://ey.hnjuh.cn

"a" .. "b"
来源：http://sq.hahajie.cn

[T38] Lua：条件
来源：http://xl.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://qk.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://tg.521024.cn

string.find(s, "%d+")
来源：http://cd.muxihuayi.cn

[T40] Lua：元表
来源：http://ys.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://yn.hnjuh.cn

[T41] Perl：Hello World
来源：http://ox.wgjwhj.cn

print "Hello\n";
来源：http://yh.lnxyls.cn

[T42] Perl：变量类型
来源：http://hx.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sn.lnxyls.cn

[T43] Perl：字符串插值
来源：http://fi.nszjky.cn

"值: $a"
来源：http://mu.yuexingan06.cn

[T44] Perl：条件
来源：http://sd.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://kx.nicolike.cn

[T45] Perl：数组遍历
来源：http://ic.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://sr.shxzskj.cn

[T46] Perl：哈希操作
来源：http://hs.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iw.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://qi.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zu.hahajie.cn

[T48] Perl：正则替换
来源：http://ix.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ei.szsharing.cn

[T49] Perl：函数
来源：http://uc.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://va.newstarts.cn

[T50] Perl：逐行读文件
来源：http://wn.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ui.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://an.nszjky.cn

[T51] Scala：Hello World
来源：http://zb.shxzukj.cn

println("Hello")
来源：http://vr.bjjhwx.cn

[T52] Scala：变量
来源：http://yj.bjjhwx.cn

val a = 1;  var b = 2
来源：http://fj.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://cy.newstarts.cn

s"值: $b"
来源：http://or.colortex.cn

[T54] Scala：集合映射
来源：http://vb.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://mj.shxzukj.cn

[T55] Scala：集合过滤
来源：http://ig.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hu.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://dh.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://vu.szsharing.cn

[T57] Scala：模式匹配
来源：http://ci.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ji.huanxung.cn

[T58] Scala：函数定义
来源：http://sc.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pc.521024.cn

[T59] Scala：循环
来源：http://mr.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://sa.haigaiapp.cn

[T60] Scala：折叠
来源：http://en.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dr.jianghongdianzi.cn

================================================================================
来源：http://rq.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cq.bjjhwx.cn

================================================================================
来源：http://bj.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://nm.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bh.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://sw.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://on.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://mp.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fx.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://ln.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tt.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://tx.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://nb.shxzukj.cn

[U06] Py：合并两个字典
来源：http://ej.haigaiapp.cn

{**a, **b}
来源：http://fe.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://vq.521024.cn

{v: k for k, v in d.items()}
来源：http://re.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://bf.hnjuh.cn

[y for x in nested for y in x]
来源：http://nd.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://jv.panjiajie.cn

max(d, key=d.get)
来源：http://ro.panjiajie.cn

[U10] Py：按值排序字典
来源：http://lm.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pc.newstarts.cn

[U11] Py：生成器表达式
来源：http://rf.panjiajie.cn

(x * 2 for x in arr)
来源：http://uc.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gg.szsharing.cn

Counter(arr).most_common(3)
来源：http://pf.shxzukj.cn

[U13] Py：固定长度队列
来源：http://hy.wgjwhj.cn

deque(maxlen=10)
来源：http://ab.colortex.cn

[U14] Py：分组收集到列表
来源：http://ft.shxzskj.cn

defaultdict(list)
来源：http://ra.wgjwhj.cn

[U15] Py：高精度计时
来源：http://xx.chemitech.net.cn

t = time.perf_counter()
来源：http://hz.nicolike.cn

[U16] Py：命令行参数解析
来源：http://ai.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://em.szxytkj.cn

[U17] Py：初始化日志
来源：http://fb.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://qs.huixiangedu.cn

[U18] Py：预编译正则
来源：http://zr.521024.cn

pat = re.compile(r"\d+")
来源：http://zi.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://pk.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sf.lnxyls.cn

[U20] Py：缓存函数结果
来源：http://fj.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://ps.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://rs.wgjwhj.cn

@contextlib.contextmanager
来源：http://uf.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://mz.hnjuh.cn

list(zip(*m))
来源：http://dk.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://vy.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tg.huanxung.cn

[U24] Py：路径操作
来源：http://qp.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://po.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://oy.hahajie.cn

csv.DictReader(f)
来源：http://zk.szsharing.cn

[U26] Py：并发下载
来源：http://ly.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rm.newstarts.cn


<!-- 参考信息 -->