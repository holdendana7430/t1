代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://ac.bookmarksfly.cn

[R76] 使用临时文件
来源：http://xm.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mc.bookmarksfly.cn

[R77] 读取用户输入
来源：http://fh.muxihuayi.cn

read -rp "请输入: " ans
来源：http://tz.bjjhwx.cn

[R78] 交互式菜单
来源：http://kw.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://os.wgjwhj.cn

[R79] 解析命令行选项
来源：http://sa.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://no.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ri.gzmigu.cn

time ./run.sh
来源：http://gw.muxihuayi.cn

================================================================================
来源：http://zm.wgjwhj.cn

S. C / C++ 专题
来源：http://cf.wgjwhj.cn

================================================================================
来源：http://bd.shxzukj.cn

[S01] C：Hello World
来源：http://pv.huixinmuqiang.cn

#include <stdio.h>
来源：http://qg.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jj.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://hs.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://gi.szxytkj.cn

[S03] C：读入整数
来源：http://kv.szsharing.cn

int x; scanf("%d", &x);
来源：http://zk.hahajie.cn

[S04] C：字符串复制
来源：http://iy.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://od.hnjuh.cn

[S05] C：字符串长度
来源：http://wo.shxzskj.cn

strlen(s)
来源：http://ay.szxytkj.cn

[S06] C：字符串比较
来源：http://jw.hahajie.cn

strcmp(a, b) == 0
来源：http://lr.huanxung.cn

[S07] C：数组遍历求和
来源：http://ec.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vi.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://cm.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ib.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://rz.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ne.bjjhwx.cn

[S10] C：指针与解引用
来源：http://vl.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://jq.hnjuh.cn

[S11] C：逐行读文件
来源：http://oi.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://zd.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://za.jctech888.com.cn

fclose(f);
来源：http://eq.bjjhwx.cn

[S12] C：写文件
来源：http://nd.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gm.jctech888.com.cn

[S13] C：宏定义
来源：http://wv.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hh.asd995.cn

[S14] C：枚举
来源：http://zi.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://xk.huixinmuqiang.cn

[S15] C：类型转换
来源：http://mj.haigaiapp.cn

(double) a / b
来源：http://re.bookmarksfly.cn

[S16] C：位操作置位
来源：http://bz.hahajie.cn

x |= (1 << 3);
来源：http://rk.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://bc.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ob.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://dd.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://la.hnjuh.cn

[S19] C：快速排序
来源：http://ts.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bx.colortex.cn

[S20] C：二分查找
来源：http://bv.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xz.newstarts.cn

[S21] C：字符类别判断
来源：http://se.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jq.hnjuh.cn

[S22] C：字符串转数字
来源：http://yq.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uf.shxzukj.cn

[S23] C：随机数
来源：http://kp.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ir.hnjuh.cn

[S24] C：获取本地时间
来源：http://zb.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fr.huixiangedu.cn

[S25] C：内存拷贝
来源：http://ed.nicolike.cn

memcpy(dst, src, n);
来源：http://mi.jianghongdianzi.cn

[S26] C：内存清零
来源：http://lf.colortex.cn

memset(a, 0, sizeof a);
来源：http://np.panjiajie.cn

[S27] C：定义常量
来源：http://yd.hahajie.cn

const double PI = 3.14159;
来源：http://rj.jctech888.com.cn

[S28] C：静态变量
来源：http://zr.colortex.cn

static int counter = 0;
来源：http://qx.shxzskj.cn

[S29] C：变参函数
来源：http://aw.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ku.panjiajie.cn

[S30] C：头文件保护
来源：http://rz.9csxet.cn

#ifndef X_H
来源：http://co.shxzskj.cn

#define X_H
来源：http://wi.colortex.cn

#endif
来源：http://cw.colortex.cn

[S31] C++：Hello World
来源：http://ur.shtwfgs.cn

#include <iostream>
来源：http://ms.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://mf.szxytkj.cn

[S32] C++：字符串
来源：http://fa.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ne.jctech888.com.cn

[S33] C++：vector 增删
来源：http://bu.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ep.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://wu.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://db.jianghongdianzi.cn

[S35] C++：map
来源：http://pg.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wb.yuexingan06.cn

[S36] C++：unordered_map
来源：http://bi.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zp.521024.cn

[S37] C++：set
来源：http://pg.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qd.asd995.cn

[S38] C++：排序
来源：http://qu.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://wy.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://vs.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ai.bookmarksfly.cn

[S40] C++：查找元素
来源：http://ez.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nj.asd995.cn

[S41] C++：类与构造函数
来源：http://sz.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fq.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://gz.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://ll.huixiangedu.cn

[S43] C++：智能指针
来源：http://wd.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://su.gzmigu.cn

[S44] C++：引用传参
来源：http://xy.nszjky.cn

void inc(int &x) { ++x; }
来源：http://rt.nszjky.cn

[S45] C++：lambda
来源：http://ij.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oy.asd995.cn

[S46] C++：函数模板
来源：http://mm.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mn.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://uz.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ga.panjiajie.cn

[S48] C++：逐行读文件
来源：http://xo.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cb.nszjky.cn

while (std::getline(in, line)) { }
来源：http://xh.asd995.cn

[S49] C++：写文件
来源：http://xr.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://il.wgjwhj.cn

[S50] C++：格式化数字
来源：http://wl.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ea.asd995.cn

[S51] C++：显式类型转换
来源：http://sg.9csxet.cn

static_cast<double>(a) / b
来源：http://mu.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://tp.asd995.cn

int size() const noexcept { return n_; }
来源：http://vh.yuexingan06.cn

[S53] C++：移动语义
来源：http://pc.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://mp.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://gy.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ct.shxzukj.cn

[S55] C++：结构化绑定
来源：http://xa.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rs.muxihuayi.cn

[S56] C++：optional
来源：http://la.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xr.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://go.szsharing.cn

constexpr int N = 10;
来源：http://la.hahajie.cn

[S58] C++：命名空间
来源：http://ip.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://ki.bookmarksfly.cn

[S59] C++：静态断言
来源：http://hr.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gz.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://nz.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kx.huixinmuqiang.cn

================================================================================
来源：http://fj.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hb.panjiajie.cn

================================================================================
来源：http://ub.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://cg.hnjuh.cn

println("Hello")
来源：http://ey.hnjuh.cn

[T02] Kotlin：变量
来源：http://ko.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yw.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://dg.newstarts.cn

"值: $b"
来源：http://gz.szxytkj.cn

[T04] Kotlin：空安全
来源：http://mr.nszjky.cn

val n: String? = null;  n?.length
来源：http://xf.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://zy.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lm.colortex.cn

[T06] Kotlin：集合映射
来源：http://gp.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nb.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://qi.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shxzukj.cn

[T08] Kotlin：数据类
来源：http://fe.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://ve.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://yr.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://jx.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://io.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ll.bjjhwx.cn

[T11] Kotlin：协程
来源：http://rn.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://us.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://oh.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://kc.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://ah.huanxung.cn

val m = mapOf("a" to 1)
来源：http://iy.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://cg.nicolike.cn

for (i in 1..10) println(i)
来源：http://lv.lnxyls.cn

[T15] Kotlin：接口
来源：http://ki.colortex.cn

interface Shape { fun area(): Double }
来源：http://zb.chemitech.net.cn

[T16] Swift：Hello World
来源：http://sb.wgjwhj.cn

print("Hello")
来源：http://fp.shxzskj.cn

[T17] Swift：变量与常量
来源：http://qy.asd995.cn

var a = 1;  let b = 2
来源：http://gk.hnjuh.cn

[T18] Swift：字符串插值
来源：http://kf.bjjhwx.cn

"值: \(b)"
来源：http://cr.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://hh.szxytkj.cn

if let n = opt { print(n) }
来源：http://pq.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://qc.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jo.szxytkj.cn

[T21] Swift：遍历
来源：http://zr.nszjky.cn

for x in a { print(x) }
来源：http://lf.muxihuayi.cn

[T22] Swift：字典
来源：http://fg.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mo.wgjwhj.cn

[T23] Swift：函数
来源：http://jm.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://st.wgjwhj.cn

[T24] Swift：闭包
来源：http://oe.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sw.hnjuh.cn

[T25] Swift：结构体
来源：http://rp.gzmigu.cn

struct P { var x: Int }
来源：http://sv.newstarts.cn

[T26] Swift：类与重写
来源：http://uw.hahajie.cn

class A: Base { override func f() {} }
来源：http://me.chemitech.net.cn

[T27] Swift：错误处理
来源：http://do.colortex.cn

do { try f() } catch { print(error) }
来源：http://hh.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://yj.huixinmuqiang.cn

enum Color { case red, green }
来源：http://vg.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://qt.nicolike.cn

guard let x = opt else { return }
来源：http://jq.newstarts.cn

[T30] Swift：协议
来源：http://bm.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://lb.shtwfgs.cn

[T31] Lua：Hello World
来源：http://mn.jianghongdianzi.cn

print("Hello")
来源：http://kl.huanxung.cn

[T32] Lua：局部变量
来源：http://jp.haigaiapp.cn

local a = 1
来源：http://oy.asd995.cn

[T33] Lua：表（数组）
来源：http://wi.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ks.nicolike.cn

[T34] Lua：遍历表
来源：http://yh.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vh.nszjky.cn

[T35] Lua：字典表
来源：http://er.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://kv.szxytkj.cn

[T36] Lua：函数
来源：http://ft.muxihuayi.cn

function add(a, b) return a + b end
来源：http://ak.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://gm.nicolike.cn

"a" .. "b"
来源：http://gd.yuexingan06.cn

[T38] Lua：条件
来源：http://eg.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://cb.shxzskj.cn

[T39] Lua：模式匹配
来源：http://kl.szsharing.cn

string.find(s, "%d+")
来源：http://ul.jctech888.com.cn

[T40] Lua：元表
来源：http://jm.szsharing.cn

setmetatable({}, { __index = base })
来源：http://bb.bjjhwx.cn

[T41] Perl：Hello World
来源：http://sv.haigaiapp.cn

print "Hello\n";
来源：http://nc.huixiangedu.cn

[T42] Perl：变量类型
来源：http://oh.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dv.9csxet.cn

[T43] Perl：字符串插值
来源：http://ww.jctech888.com.cn

"值: $a"
来源：http://dl.lnxyls.cn

[T44] Perl：条件
来源：http://hj.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://bg.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://bv.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://nx.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://vb.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qh.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://wt.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qi.newstarts.cn

[T48] Perl：正则替换
来源：http://lm.nszjky.cn

$s =~ s/old/new/g;
来源：http://dm.newstarts.cn

[T49] Perl：函数
来源：http://og.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gv.asd995.cn

[T50] Perl：逐行读文件
来源：http://uu.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cl.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://zl.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://fg.haigaiapp.cn

println("Hello")
来源：http://ro.szxytkj.cn

[T52] Scala：变量
来源：http://qv.gzmigu.cn

val a = 1;  var b = 2
来源：http://mz.gzmigu.cn

[T53] Scala：字符串插值
来源：http://me.hnjuh.cn

s"值: $b"
来源：http://jo.haigaiapp.cn

[T54] Scala：集合映射
来源：http://ue.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://wb.newstarts.cn

[T55] Scala：集合过滤
来源：http://wv.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ns.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://cd.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://lm.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://rp.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aw.nszjky.cn

[T58] Scala：函数定义
来源：http://eq.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ki.lnxyls.cn

[T59] Scala：循环
来源：http://yd.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://zd.shxzukj.cn

[T60] Scala：折叠
来源：http://km.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ki.wgjwhj.cn

================================================================================
来源：http://gv.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://my.newstarts.cn

================================================================================
来源：http://rn.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://qj.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uf.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ow.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ej.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://as.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bc.panjiajie.cn

[U04] Py：变量调试打印
来源：http://po.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dv.nszjky.cn

[U05] Py：列表去重且保序
来源：http://gt.hahajie.cn

list(dict.fromkeys(arr))
来源：http://tl.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://gh.shtwfgs.cn

{**a, **b}
来源：http://tb.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://gq.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://rf.hnjuh.cn

[U08] Py：展平二维列表
来源：http://dk.bjjhwx.cn

[y for x in nested for y in x]
来源：http://ad.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://xg.haigaiapp.cn

max(d, key=d.get)
来源：http://uq.nszjky.cn

[U10] Py：按值排序字典
来源：http://xt.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jr.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://ts.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://ep.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tj.asd995.cn

Counter(arr).most_common(3)
来源：http://pj.hahajie.cn

[U13] Py：固定长度队列
来源：http://cw.hnjuh.cn

deque(maxlen=10)
来源：http://it.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://ai.yuexingan06.cn

defaultdict(list)
来源：http://ln.9csxet.cn

[U15] Py：高精度计时
来源：http://cj.shtwfgs.cn

t = time.perf_counter()
来源：http://rb.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://gk.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ag.shtwfgs.cn


<!-- 参考信息 -->