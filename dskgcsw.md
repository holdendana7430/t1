代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://or.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://qe.szxytkj.cn

time ./run.sh
来源：http://ju.wgjwhj.cn

================================================================================
来源：http://pi.huanxung.cn

S. C / C++ 专题
来源：http://kw.yuexingan06.cn

================================================================================
来源：http://ky.yuntaijiaju.cn

[S01] C：Hello World
来源：http://ub.bjjhwx.cn

#include <stdio.h>
来源：http://rd.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vd.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://nm.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://ju.wgjwhj.cn

[S03] C：读入整数
来源：http://zc.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://tx.jctech888.com.cn

[S04] C：字符串复制
来源：http://is.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yq.jctech888.com.cn

[S05] C：字符串长度
来源：http://hj.asd995.cn

strlen(s)
来源：http://je.haigaiapp.cn

[S06] C：字符串比较
来源：http://fb.chemitech.net.cn

strcmp(a, b) == 0
来源：http://fl.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://zh.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lf.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://gf.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vh.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://ag.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qo.yuexingan06.cn

[S10] C：指针与解引用
来源：http://nw.colortex.cn

int *p = &a;  *p = 5;
来源：http://ph.lnxyls.cn

[S11] C：逐行读文件
来源：http://wf.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://qm.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dh.hahajie.cn

fclose(f);
来源：http://jv.521024.cn

[S12] C：写文件
来源：http://od.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://md.bjjhwx.cn

[S13] C：宏定义
来源：http://fs.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oa.yuntaijiaju.cn

[S14] C：枚举
来源：http://xv.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://va.huixinmuqiang.cn

[S15] C：类型转换
来源：http://zw.newstarts.cn

(double) a / b
来源：http://eg.lnxyls.cn

[S16] C：位操作置位
来源：http://nb.asd995.cn

x |= (1 << 3);
来源：http://kt.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://he.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xu.bjjhwx.cn

[S18] C：命令行参数
来源：http://vi.asd995.cn

int main(int argc, char **argv)
来源：http://wt.yuexingan06.cn

[S19] C：快速排序
来源：http://yd.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dw.9csxet.cn

[S20] C：二分查找
来源：http://nk.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vo.huixiangedu.cn

[S21] C：字符类别判断
来源：http://py.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sv.colortex.cn

[S22] C：字符串转数字
来源：http://bk.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lp.asd995.cn

[S23] C：随机数
来源：http://mx.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ft.lnxyls.cn

[S24] C：获取本地时间
来源：http://ga.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xe.hahajie.cn

[S25] C：内存拷贝
来源：http://sq.newstarts.cn

memcpy(dst, src, n);
来源：http://vo.shxzukj.cn

[S26] C：内存清零
来源：http://zw.huanxung.cn

memset(a, 0, sizeof a);
来源：http://xu.huixiangedu.cn

[S27] C：定义常量
来源：http://je.shtwfgs.cn

const double PI = 3.14159;
来源：http://hd.lnxyls.cn

[S28] C：静态变量
来源：http://eo.shxzukj.cn

static int counter = 0;
来源：http://ni.hnjuh.cn

[S29] C：变参函数
来源：http://vh.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cy.shtwfgs.cn

[S30] C：头文件保护
来源：http://gt.yuntaijiaju.cn

#ifndef X_H
来源：http://vl.bookmarksfly.cn

#define X_H
来源：http://ft.newstarts.cn

#endif
来源：http://pb.muxihuayi.cn

[S31] C++：Hello World
来源：http://sg.colortex.cn

#include <iostream>
来源：http://wg.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ml.nicolike.cn

[S32] C++：字符串
来源：http://hg.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://fl.panjiajie.cn

[S33] C++：vector 增删
来源：http://ri.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sg.gzmigu.cn

[S34] C++：遍历 vector
来源：http://lb.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://nj.muxihuayi.cn

[S35] C++：map
来源：http://zj.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oh.szsharing.cn

[S36] C++：unordered_map
来源：http://id.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://do.9csxet.cn

[S37] C++：set
来源：http://aw.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xn.yuexingan06.cn

[S38] C++：排序
来源：http://sx.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://ms.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://db.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ww.newstarts.cn

[S40] C++：查找元素
来源：http://ig.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kp.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://tg.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ib.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://mz.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://rb.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://gd.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://xz.haigaiapp.cn

[S44] C++：引用传参
来源：http://pd.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://sm.newstarts.cn

[S45] C++：lambda
来源：http://xn.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dl.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://ah.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xf.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://vh.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cx.colortex.cn

[S48] C++：逐行读文件
来源：http://qc.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wk.szsharing.cn

while (std::getline(in, line)) { }
来源：http://dd.haigaiapp.cn

[S49] C++：写文件
来源：http://ns.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kr.hnjuh.cn

[S50] C++：格式化数字
来源：http://fs.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eg.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://uj.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://es.521024.cn

[S52] C++：const 与 noexcept
来源：http://so.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://ed.asd995.cn

[S53] C++：移动语义
来源：http://jk.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://xy.jctech888.com.cn

[S54] C++：异常处理
来源：http://sy.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tc.szsharing.cn

[S55] C++：结构化绑定
来源：http://fh.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vs.shtwfgs.cn

[S56] C++：optional
来源：http://nd.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hn.shxzukj.cn

[S57] C++：编译期常量
来源：http://gy.bjjhwx.cn

constexpr int N = 10;
来源：http://qn.yuexingan06.cn

[S58] C++：命名空间
来源：http://mm.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://br.shxzskj.cn

[S59] C++：静态断言
来源：http://lg.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gp.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://na.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mg.szxytkj.cn

================================================================================
来源：http://xj.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kq.jianghongdianzi.cn

================================================================================
来源：http://fy.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://um.szxytkj.cn

println("Hello")
来源：http://um.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://sn.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gx.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://pb.panjiajie.cn

"值: $b"
来源：http://bw.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://vk.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://zi.colortex.cn

[T05] Kotlin：when 表达式
来源：http://rf.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bu.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://em.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sn.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://dn.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jz.hnjuh.cn

[T08] Kotlin：数据类
来源：http://px.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://ea.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://qr.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://md.9csxet.cn

[T10] Kotlin：默认参数
来源：http://zq.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sa.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://fy.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vx.szsharing.cn

[T12] Kotlin：解构声明
来源：http://uq.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://mj.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://cz.521024.cn

val m = mapOf("a" to 1)
来源：http://xi.newstarts.cn

[T14] Kotlin：循环
来源：http://ms.colortex.cn

for (i in 1..10) println(i)
来源：http://av.hnjuh.cn

[T15] Kotlin：接口
来源：http://im.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://ya.newstarts.cn

[T16] Swift：Hello World
来源：http://vk.gzmigu.cn

print("Hello")
来源：http://pk.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://yh.muxihuayi.cn

var a = 1;  let b = 2
来源：http://wa.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://vd.colortex.cn

"值: \(b)"
来源：http://tb.huanxung.cn

[T19] Swift：可选绑定
来源：http://uw.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://kc.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://tj.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://an.huanxung.cn

[T21] Swift：遍历
来源：http://jw.wgjwhj.cn

for x in a { print(x) }
来源：http://pr.newstarts.cn

[T22] Swift：字典
来源：http://hx.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gg.huanxung.cn

[T23] Swift：函数
来源：http://tv.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ax.shtwfgs.cn

[T24] Swift：闭包
来源：http://pk.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uu.lnxyls.cn

[T25] Swift：结构体
来源：http://ng.huixiangedu.cn

struct P { var x: Int }
来源：http://sn.yuexingan06.cn

[T26] Swift：类与重写
来源：http://cx.shxzukj.cn

class A: Base { override func f() {} }
来源：http://fm.hnjuh.cn

[T27] Swift：错误处理
来源：http://ne.colortex.cn

do { try f() } catch { print(error) }
来源：http://wk.shtwfgs.cn

[T28] Swift：枚举
来源：http://ea.nszjky.cn

enum Color { case red, green }
来源：http://lg.colortex.cn

[T29] Swift：guard 提前返回
来源：http://zf.wgjwhj.cn

guard let x = opt else { return }
来源：http://bb.shxzukj.cn

[T30] Swift：协议
来源：http://xj.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://gj.hnjuh.cn

[T31] Lua：Hello World
来源：http://ub.huixinmuqiang.cn

print("Hello")
来源：http://yw.nicolike.cn

[T32] Lua：局部变量
来源：http://ee.muxihuayi.cn

local a = 1
来源：http://xb.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://rs.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nq.lnxyls.cn

[T34] Lua：遍历表
来源：http://ds.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ni.asd995.cn

[T35] Lua：字典表
来源：http://eu.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://gd.bookmarksfly.cn

[T36] Lua：函数
来源：http://xh.521024.cn

function add(a, b) return a + b end
来源：http://wu.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://pq.yuntaijiaju.cn

"a" .. "b"
来源：http://tq.yuexingan06.cn

[T38] Lua：条件
来源：http://wt.panjiajie.cn

if x > 0 then print("正") end
来源：http://xl.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://gb.bjjhwx.cn

string.find(s, "%d+")
来源：http://mf.newstarts.cn

[T40] Lua：元表
来源：http://ee.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://og.colortex.cn

[T41] Perl：Hello World
来源：http://hu.hnjuh.cn

print "Hello\n";
来源：http://mb.haigaiapp.cn

[T42] Perl：变量类型
来源：http://ud.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ab.szsharing.cn

[T43] Perl：字符串插值
来源：http://fx.chemitech.net.cn

"值: $a"
来源：http://ub.gzmigu.cn

[T44] Perl：条件
来源：http://gd.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://ft.gzmigu.cn

[T45] Perl：数组遍历
来源：http://nr.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://vu.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://lv.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ll.nicolike.cn

[T47] Perl：正则捕获
来源：http://zk.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fd.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://bq.newstarts.cn

$s =~ s/old/new/g;
来源：http://dm.muxihuayi.cn

[T49] Perl：函数
来源：http://ee.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sc.szsharing.cn

[T50] Perl：逐行读文件
来源：http://nh.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://st.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://bc.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://tw.bjjhwx.cn

println("Hello")
来源：http://ib.szxytkj.cn

[T52] Scala：变量
来源：http://af.9csxet.cn

val a = 1;  var b = 2
来源：http://mi.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://zp.bjjhwx.cn

s"值: $b"
来源：http://fk.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://cp.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://fu.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://mx.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gx.bjjhwx.cn

[T56] Scala：样例类
来源：http://wr.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://km.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://wx.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ik.hnjuh.cn

[T58] Scala：函数定义
来源：http://ah.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xm.gzmigu.cn

[T59] Scala：循环
来源：http://wj.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://ty.shxzukj.cn

[T60] Scala：折叠
来源：http://pq.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fg.bjjhwx.cn

================================================================================
来源：http://wc.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gr.bookmarksfly.cn

================================================================================
来源：http://zq.521024.cn

[U01] Py：创建虚拟环境
来源：http://tf.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mf.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://jk.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ev.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://go.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uf.hnjuh.cn

[U04] Py：变量调试打印
来源：http://yp.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gr.nicolike.cn

[U05] Py：列表去重且保序
来源：http://en.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ax.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://jx.nszjky.cn

{**a, **b}
来源：http://ac.asd995.cn

[U07] Py：反转字典键值
来源：http://jd.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://kr.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://vw.hahajie.cn

[y for x in nested for y in x]
来源：http://dy.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://md.shtwfgs.cn

max(d, key=d.get)
来源：http://le.hahajie.cn

[U10] Py：按值排序字典
来源：http://ga.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mn.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://qi.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://xc.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://po.hahajie.cn

Counter(arr).most_common(3)
来源：http://vn.9csxet.cn

[U13] Py：固定长度队列
来源：http://rg.asd995.cn

deque(maxlen=10)
来源：http://oc.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://hs.shxzukj.cn

defaultdict(list)
来源：http://sb.haigaiapp.cn

[U15] Py：高精度计时
来源：http://qd.chemitech.net.cn

t = time.perf_counter()
来源：http://tw.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://om.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rw.asd995.cn

[U17] Py：初始化日志
来源：http://so.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://ag.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://cc.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://fq.hahajie.cn

[U19] Py：正则替换带回调
来源：http://hc.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vy.huanxung.cn

[U20] Py：缓存函数结果
来源：http://fz.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://ec.huixinmuqiang.cn


<!-- 参考信息 -->