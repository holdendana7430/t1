代发 wailian999

read -rp "请输入: " ans
来源：http://tp.yuexingan06.cn

[R78] 交互式菜单
来源：http://jt.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nh.9csxet.cn

[R79] 解析命令行选项
来源：http://bv.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pn.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ap.hahajie.cn

time ./run.sh
来源：http://fi.shxzskj.cn

================================================================================
来源：http://by.hnjuh.cn

S. C / C++ 专题
来源：http://vv.szsharing.cn

================================================================================
来源：http://zq.jctech888.com.cn

[S01] C：Hello World
来源：http://pb.haigaiapp.cn

#include <stdio.h>
来源：http://vd.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ik.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://kh.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://cm.panjiajie.cn

[S03] C：读入整数
来源：http://xb.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://fi.hnjuh.cn

[S04] C：字符串复制
来源：http://fp.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bo.nicolike.cn

[S05] C：字符串长度
来源：http://ip.9csxet.cn

strlen(s)
来源：http://ft.shtwfgs.cn

[S06] C：字符串比较
来源：http://rm.521024.cn

strcmp(a, b) == 0
来源：http://td.9csxet.cn

[S07] C：数组遍历求和
来源：http://bj.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sb.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://tc.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pd.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://hl.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yo.shxzskj.cn

[S10] C：指针与解引用
来源：http://ng.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://mw.huanxung.cn

[S11] C：逐行读文件
来源：http://pl.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ir.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jg.panjiajie.cn

fclose(f);
来源：http://yc.bookmarksfly.cn

[S12] C：写文件
来源：http://rl.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qs.muxihuayi.cn

[S13] C：宏定义
来源：http://mg.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vl.colortex.cn

[S14] C：枚举
来源：http://yb.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ov.huixiangedu.cn

[S15] C：类型转换
来源：http://qw.huixinmuqiang.cn

(double) a / b
来源：http://mm.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://ko.gzmigu.cn

x |= (1 << 3);
来源：http://jr.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://mb.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sp.shxzukj.cn

[S18] C：命令行参数
来源：http://fp.chemitech.net.cn

int main(int argc, char **argv)
来源：http://ez.9csxet.cn

[S19] C：快速排序
来源：http://us.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oo.bjjhwx.cn

[S20] C：二分查找
来源：http://tk.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ys.szxytkj.cn

[S21] C：字符类别判断
来源：http://dg.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://or.newstarts.cn

[S22] C：字符串转数字
来源：http://sw.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oc.hnjuh.cn

[S23] C：随机数
来源：http://ge.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.asd995.cn

[S24] C：获取本地时间
来源：http://wt.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qm.yuexingan06.cn

[S25] C：内存拷贝
来源：http://ey.muxihuayi.cn

memcpy(dst, src, n);
来源：http://zs.9csxet.cn

[S26] C：内存清零
来源：http://sy.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://og.hahajie.cn

[S27] C：定义常量
来源：http://hu.muxihuayi.cn

const double PI = 3.14159;
来源：http://fl.huanxung.cn

[S28] C：静态变量
来源：http://if.521024.cn

static int counter = 0;
来源：http://um.szxytkj.cn

[S29] C：变参函数
来源：http://qj.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mi.yuexingan06.cn

[S30] C：头文件保护
来源：http://mz.yuexingan06.cn

#ifndef X_H
来源：http://ae.szxytkj.cn

#define X_H
来源：http://bz.haigaiapp.cn

#endif
来源：http://ic.9csxet.cn

[S31] C++：Hello World
来源：http://qm.newstarts.cn

#include <iostream>
来源：http://pa.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://be.shxzskj.cn

[S32] C++：字符串
来源：http://cy.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://mt.huixiangedu.cn

[S33] C++：vector 增删
来源：http://mw.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ex.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://tt.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://kb.haigaiapp.cn

[S35] C++：map
来源：http://xr.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yk.521024.cn

[S36] C++：unordered_map
来源：http://gb.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mm.haigaiapp.cn

[S37] C++：set
来源：http://bb.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pl.colortex.cn

[S38] C++：排序
来源：http://sk.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://cp.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ki.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bd.9csxet.cn

[S40] C++：查找元素
来源：http://jo.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jk.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://rd.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sb.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://gv.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://wb.shtwfgs.cn

[S43] C++：智能指针
来源：http://mk.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://sg.bjjhwx.cn

[S44] C++：引用传参
来源：http://ug.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://cc.jianghongdianzi.cn

[S45] C++：lambda
来源：http://iy.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wi.lnxyls.cn

[S46] C++：函数模板
来源：http://co.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gy.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://xv.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ui.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://gh.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qe.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://jx.yuntaijiaju.cn

[S49] C++：写文件
来源：http://bi.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ew.haigaiapp.cn

[S50] C++：格式化数字
来源：http://hq.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jx.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://ew.huixiangedu.cn

static_cast<double>(a) / b
来源：http://xt.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://vs.nicolike.cn

int size() const noexcept { return n_; }
来源：http://be.hahajie.cn

[S53] C++：移动语义
来源：http://ms.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://gi.jctech888.com.cn

[S54] C++：异常处理
来源：http://gb.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bw.hnjuh.cn

[S55] C++：结构化绑定
来源：http://tc.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xh.hnjuh.cn

[S56] C++：optional
来源：http://ey.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tt.shtwfgs.cn

[S57] C++：编译期常量
来源：http://cc.huixinmuqiang.cn

constexpr int N = 10;
来源：http://nb.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://zh.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://kr.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ol.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jd.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://pr.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ty.chemitech.net.cn

================================================================================
来源：http://pv.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qc.shxzukj.cn

================================================================================
来源：http://oi.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://lc.gzmigu.cn

println("Hello")
来源：http://vz.chemitech.net.cn

[T02] Kotlin：变量
来源：http://js.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ss.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://iw.newstarts.cn

"值: $b"
来源：http://rj.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://dk.gzmigu.cn

val n: String? = null;  n?.length
来源：http://ax.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://bj.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jq.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://xk.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yc.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://dj.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uf.nszjky.cn

[T08] Kotlin：数据类
来源：http://nm.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://ly.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://cq.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://as.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://hd.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zz.lnxyls.cn

[T11] Kotlin：协程
来源：http://jm.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nu.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://jg.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://tk.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://kh.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://mc.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://wz.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://np.haigaiapp.cn

[T15] Kotlin：接口
来源：http://ke.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://ra.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://kc.newstarts.cn

print("Hello")
来源：http://dt.huanxung.cn

[T17] Swift：变量与常量
来源：http://lp.bjjhwx.cn

var a = 1;  let b = 2
来源：http://nh.asd995.cn

[T18] Swift：字符串插值
来源：http://ji.shxzskj.cn

"值: \(b)"
来源：http://il.shxzukj.cn

[T19] Swift：可选绑定
来源：http://ob.haigaiapp.cn

if let n = opt { print(n) }
来源：http://qb.huanxung.cn

[T20] Swift：数组操作
来源：http://ts.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ja.jctech888.com.cn

[T21] Swift：遍历
来源：http://an.shxzskj.cn

for x in a { print(x) }
来源：http://cf.nszjky.cn

[T22] Swift：字典
来源：http://uc.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yi.shxzukj.cn

[T23] Swift：函数
来源：http://po.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kj.jctech888.com.cn

[T24] Swift：闭包
来源：http://ij.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dr.shxzukj.cn

[T25] Swift：结构体
来源：http://tk.shtwfgs.cn

struct P { var x: Int }
来源：http://up.shxzukj.cn

[T26] Swift：类与重写
来源：http://vm.gzmigu.cn

class A: Base { override func f() {} }
来源：http://bp.newstarts.cn

[T27] Swift：错误处理
来源：http://py.hahajie.cn

do { try f() } catch { print(error) }
来源：http://gv.gzmigu.cn

[T28] Swift：枚举
来源：http://ta.lnxyls.cn

enum Color { case red, green }
来源：http://xy.colortex.cn

[T29] Swift：guard 提前返回
来源：http://zl.nszjky.cn

guard let x = opt else { return }
来源：http://pi.asd995.cn

[T30] Swift：协议
来源：http://ak.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://ju.shxzukj.cn

[T31] Lua：Hello World
来源：http://gm.gzmigu.cn

print("Hello")
来源：http://il.nicolike.cn

[T32] Lua：局部变量
来源：http://ye.newstarts.cn

local a = 1
来源：http://vl.szxytkj.cn

[T33] Lua：表（数组）
来源：http://ls.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://as.colortex.cn

[T34] Lua：遍历表
来源：http://kx.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://st.521024.cn

[T35] Lua：字典表
来源：http://dn.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ks.huixinmuqiang.cn

[T36] Lua：函数
来源：http://an.gzmigu.cn

function add(a, b) return a + b end
来源：http://ff.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://js.panjiajie.cn

"a" .. "b"
来源：http://zu.shtwfgs.cn

[T38] Lua：条件
来源：http://ef.nszjky.cn

if x > 0 then print("正") end
来源：http://uc.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://dn.muxihuayi.cn

string.find(s, "%d+")
来源：http://yg.huixinmuqiang.cn

[T40] Lua：元表
来源：http://dv.huanxung.cn

setmetatable({}, { __index = base })
来源：http://vf.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://dw.bjjhwx.cn

print "Hello\n";
来源：http://ij.shxzskj.cn

[T42] Perl：变量类型
来源：http://my.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ri.szsharing.cn

[T43] Perl：字符串插值
来源：http://bb.szsharing.cn

"值: $a"
来源：http://qb.huanxung.cn

[T44] Perl：条件
来源：http://xk.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://nf.shxzskj.cn

[T45] Perl：数组遍历
来源：http://nv.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://qh.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://he.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yl.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://vi.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vl.shxzukj.cn

[T48] Perl：正则替换
来源：http://pj.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://vg.9csxet.cn

[T49] Perl：函数
来源：http://ob.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iu.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://dg.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uh.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://ad.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://ad.gzmigu.cn

println("Hello")
来源：http://dk.huixiangedu.cn

[T52] Scala：变量
来源：http://ca.9csxet.cn

val a = 1;  var b = 2
来源：http://cg.9csxet.cn

[T53] Scala：字符串插值
来源：http://qm.yuntaijiaju.cn

s"值: $b"
来源：http://of.szxytkj.cn

[T54] Scala：集合映射
来源：http://ut.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://us.9csxet.cn

[T55] Scala：集合过滤
来源：http://po.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://la.hahajie.cn

[T56] Scala：样例类
来源：http://kj.hnjuh.cn

case class User(name: String, age: Int)
来源：http://ox.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://ao.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mb.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://lc.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://th.521024.cn

[T59] Scala：循环
来源：http://my.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://bq.chemitech.net.cn

[T60] Scala：折叠
来源：http://ro.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gm.jctech888.com.cn

================================================================================
来源：http://fq.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mv.szxytkj.cn

================================================================================
来源：http://rw.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://yq.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qn.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://xo.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kj.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://mj.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kp.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://qr.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ta.9csxet.cn

[U05] Py：列表去重且保序
来源：http://bn.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://ve.521024.cn

[U06] Py：合并两个字典
来源：http://fd.huixinmuqiang.cn

{**a, **b}
来源：http://zu.szsharing.cn

[U07] Py：反转字典键值
来源：http://wg.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://da.szxytkj.cn

[U08] Py：展平二维列表
来源：http://il.nicolike.cn

[y for x in nested for y in x]
来源：http://vy.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://ah.gzmigu.cn

max(d, key=d.get)
来源：http://py.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://zx.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wl.panjiajie.cn

[U11] Py：生成器表达式
来源：http://kh.huixiangedu.cn

(x * 2 for x in arr)
来源：http://sn.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ao.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://jy.shxzskj.cn

[U13] Py：固定长度队列
来源：http://fx.bjjhwx.cn

deque(maxlen=10)
来源：http://hc.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://zn.yuntaijiaju.cn

defaultdict(list)
来源：http://qu.huanxung.cn

[U15] Py：高精度计时
来源：http://cv.szsharing.cn

t = time.perf_counter()
来源：http://it.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://kk.szsharing.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://do.nicolike.cn

[U17] Py：初始化日志
来源：http://zi.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://xi.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://ny.nszjky.cn

pat = re.compile(r"\d+")
来源：http://vp.wgjwhj.cn


<!-- 参考信息 -->