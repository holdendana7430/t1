代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://dk.shtwfgs.cn

[R76] 使用临时文件
来源：http://wa.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://im.521024.cn

[R77] 读取用户输入
来源：http://ip.nszjky.cn

read -rp "请输入: " ans
来源：http://im.asd995.cn

[R78] 交互式菜单
来源：http://nh.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ta.jctech888.com.cn

[R79] 解析命令行选项
来源：http://pz.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ow.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://an.9csxet.cn

time ./run.sh
来源：http://wa.nszjky.cn

================================================================================
来源：http://xf.lnxyls.cn

S. C / C++ 专题
来源：http://gl.bjjhwx.cn

================================================================================
来源：http://wq.huixiangedu.cn

[S01] C：Hello World
来源：http://ti.huanxung.cn

#include <stdio.h>
来源：http://xl.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dz.nicolike.cn

[S02] C：变量与格式化输出
来源：http://df.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://vw.nicolike.cn

[S03] C：读入整数
来源：http://tj.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://eo.lnxyls.cn

[S04] C：字符串复制
来源：http://pd.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fa.shtwfgs.cn

[S05] C：字符串长度
来源：http://zy.muxihuayi.cn

strlen(s)
来源：http://yt.newstarts.cn

[S06] C：字符串比较
来源：http://zn.chemitech.net.cn

strcmp(a, b) == 0
来源：http://sc.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://nu.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iw.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://ck.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://st.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://jf.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://is.asd995.cn

[S10] C：指针与解引用
来源：http://fn.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://ux.yuexingan06.cn

[S11] C：逐行读文件
来源：http://yx.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://py.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dj.hnjuh.cn

fclose(f);
来源：http://pw.nszjky.cn

[S12] C：写文件
来源：http://ux.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bl.chemitech.net.cn

[S13] C：宏定义
来源：http://di.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ic.shxzukj.cn

[S14] C：枚举
来源：http://pn.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://cj.gzmigu.cn

[S15] C：类型转换
来源：http://sf.hnjuh.cn

(double) a / b
来源：http://ve.panjiajie.cn

[S16] C：位操作置位
来源：http://al.wgjwhj.cn

x |= (1 << 3);
来源：http://sk.521024.cn

[S17] C：安全拼接字符串
来源：http://xy.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xg.haigaiapp.cn

[S18] C：命令行参数
来源：http://ky.colortex.cn

int main(int argc, char **argv)
来源：http://rx.wgjwhj.cn

[S19] C：快速排序
来源：http://nc.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ee.asd995.cn

[S20] C：二分查找
来源：http://dn.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jb.wgjwhj.cn

[S21] C：字符类别判断
来源：http://mt.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yn.newstarts.cn

[S22] C：字符串转数字
来源：http://kl.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://of.panjiajie.cn

[S23] C：随机数
来源：http://ix.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jy.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ir.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bj.haigaiapp.cn

[S25] C：内存拷贝
来源：http://qz.huanxung.cn

memcpy(dst, src, n);
来源：http://uv.szsharing.cn

[S26] C：内存清零
来源：http://dc.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://us.szxytkj.cn

[S27] C：定义常量
来源：http://xq.shxzukj.cn

const double PI = 3.14159;
来源：http://ua.yuntaijiaju.cn

[S28] C：静态变量
来源：http://ax.bjjhwx.cn

static int counter = 0;
来源：http://eo.szxytkj.cn

[S29] C：变参函数
来源：http://tx.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hw.shtwfgs.cn

[S30] C：头文件保护
来源：http://ps.bjjhwx.cn

#ifndef X_H
来源：http://ri.hahajie.cn

#define X_H
来源：http://bn.gzmigu.cn

#endif
来源：http://ww.shxzskj.cn

[S31] C++：Hello World
来源：http://gs.hnjuh.cn

#include <iostream>
来源：http://ze.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://ry.jctech888.com.cn

[S32] C++：字符串
来源：http://uz.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://lb.szxytkj.cn

[S33] C++：vector 增删
来源：http://gm.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ga.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://pq.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://rk.szsharing.cn

[S35] C++：map
来源：http://qk.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ny.nicolike.cn

[S36] C++：unordered_map
来源：http://pg.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ee.9csxet.cn

[S37] C++：set
来源：http://nv.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jw.yuexingan06.cn

[S38] C++：排序
来源：http://jq.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://wy.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://ay.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://px.shxzskj.cn

[S40] C++：查找元素
来源：http://pe.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uu.newstarts.cn

[S41] C++：类与构造函数
来源：http://wt.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nc.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://ud.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://sz.panjiajie.cn

[S43] C++：智能指针
来源：http://xl.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://vo.newstarts.cn

[S44] C++：引用传参
来源：http://lr.9csxet.cn

void inc(int &x) { ++x; }
来源：http://wn.newstarts.cn

[S45] C++：lambda
来源：http://cq.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ph.yuexingan06.cn

[S46] C++：函数模板
来源：http://cu.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fk.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://ay.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ar.szsharing.cn

[S48] C++：逐行读文件
来源：http://ln.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iz.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://oa.haigaiapp.cn

[S49] C++：写文件
来源：http://mj.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wv.521024.cn

[S50] C++：格式化数字
来源：http://bn.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tg.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://xo.hnjuh.cn

static_cast<double>(a) / b
来源：http://kj.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://dz.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://iq.wgjwhj.cn

[S53] C++：移动语义
来源：http://np.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://bm.bjjhwx.cn

[S54] C++：异常处理
来源：http://dw.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vk.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://cb.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://na.521024.cn

[S56] C++：optional
来源：http://nv.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mi.haigaiapp.cn

[S57] C++：编译期常量
来源：http://mw.haigaiapp.cn

constexpr int N = 10;
来源：http://rc.lnxyls.cn

[S58] C++：命名空间
来源：http://ck.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://wb.szsharing.cn

[S59] C++：静态断言
来源：http://ju.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mf.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://up.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bn.szxytkj.cn

================================================================================
来源：http://xt.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sk.jctech888.com.cn

================================================================================
来源：http://zd.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://rh.yuntaijiaju.cn

println("Hello")
来源：http://iy.shxzskj.cn

[T02] Kotlin：变量
来源：http://ex.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://au.asd995.cn

[T03] Kotlin：字符串模板
来源：http://eh.hahajie.cn

"值: $b"
来源：http://sb.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://ve.hnjuh.cn

val n: String? = null;  n?.length
来源：http://mp.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://ag.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://na.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://wf.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vk.asd995.cn

[T07] Kotlin：集合过滤
来源：http://yy.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dj.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://mn.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://tl.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://qp.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://nl.huanxung.cn

[T10] Kotlin：默认参数
来源：http://hy.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ig.haigaiapp.cn

[T11] Kotlin：协程
来源：http://rh.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://og.colortex.cn

[T12] Kotlin：解构声明
来源：http://at.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://ts.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://kt.newstarts.cn

val m = mapOf("a" to 1)
来源：http://ph.shxzskj.cn

[T14] Kotlin：循环
来源：http://xa.nicolike.cn

for (i in 1..10) println(i)
来源：http://mh.521024.cn

[T15] Kotlin：接口
来源：http://wl.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://hg.szxytkj.cn

[T16] Swift：Hello World
来源：http://zj.shxzukj.cn

print("Hello")
来源：http://vl.panjiajie.cn

[T17] Swift：变量与常量
来源：http://eg.huanxung.cn

var a = 1;  let b = 2
来源：http://al.shxzskj.cn

[T18] Swift：字符串插值
来源：http://dr.chemitech.net.cn

"值: \(b)"
来源：http://dk.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://rm.huanxung.cn

if let n = opt { print(n) }
来源：http://ty.shxzukj.cn

[T20] Swift：数组操作
来源：http://sx.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pq.szxytkj.cn

[T21] Swift：遍历
来源：http://cz.newstarts.cn

for x in a { print(x) }
来源：http://sw.lnxyls.cn

[T22] Swift：字典
来源：http://hb.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hz.asd995.cn

[T23] Swift：函数
来源：http://wb.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://us.yuexingan06.cn

[T24] Swift：闭包
来源：http://xb.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gf.wgjwhj.cn

[T25] Swift：结构体
来源：http://za.9csxet.cn

struct P { var x: Int }
来源：http://db.lnxyls.cn

[T26] Swift：类与重写
来源：http://ea.panjiajie.cn

class A: Base { override func f() {} }
来源：http://ev.szxytkj.cn

[T27] Swift：错误处理
来源：http://fs.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://jx.bookmarksfly.cn

[T28] Swift：枚举
来源：http://bu.bookmarksfly.cn

enum Color { case red, green }
来源：http://zq.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://wi.nicolike.cn

guard let x = opt else { return }
来源：http://gn.521024.cn

[T30] Swift：协议
来源：http://dn.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://vc.shxzukj.cn

[T31] Lua：Hello World
来源：http://kq.bookmarksfly.cn

print("Hello")
来源：http://ou.haigaiapp.cn

[T32] Lua：局部变量
来源：http://uj.nszjky.cn

local a = 1
来源：http://wv.asd995.cn

[T33] Lua：表（数组）
来源：http://wy.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://es.colortex.cn

[T34] Lua：遍历表
来源：http://gr.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mo.szsharing.cn

[T35] Lua：字典表
来源：http://gr.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://df.huixiangedu.cn

[T36] Lua：函数
来源：http://ip.shxzukj.cn

function add(a, b) return a + b end
来源：http://yl.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://ml.chemitech.net.cn

"a" .. "b"
来源：http://yl.521024.cn

[T38] Lua：条件
来源：http://te.shtwfgs.cn

if x > 0 then print("正") end
来源：http://eh.newstarts.cn

[T39] Lua：模式匹配
来源：http://kn.wgjwhj.cn

string.find(s, "%d+")
来源：http://tl.szsharing.cn

[T40] Lua：元表
来源：http://er.521024.cn

setmetatable({}, { __index = base })
来源：http://eq.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://od.muxihuayi.cn

print "Hello\n";
来源：http://qg.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://ee.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gj.hahajie.cn

[T43] Perl：字符串插值
来源：http://zv.haigaiapp.cn

"值: $a"
来源：http://oi.huanxung.cn

[T44] Perl：条件
来源：http://dl.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://rt.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://zl.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://ws.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://fi.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ni.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://gc.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gr.huixiangedu.cn

[T48] Perl：正则替换
来源：http://nj.hnjuh.cn

$s =~ s/old/new/g;
来源：http://ov.huanxung.cn

[T49] Perl：函数
来源：http://ap.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://be.colortex.cn

[T50] Perl：逐行读文件
来源：http://bl.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sa.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ww.newstarts.cn

[T51] Scala：Hello World
来源：http://ej.huixiangedu.cn

println("Hello")
来源：http://sz.muxihuayi.cn

[T52] Scala：变量
来源：http://aa.nszjky.cn

val a = 1;  var b = 2
来源：http://py.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://zi.shxzukj.cn

s"值: $b"
来源：http://xs.shtwfgs.cn

[T54] Scala：集合映射
来源：http://ds.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://ii.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://qr.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wm.shtwfgs.cn

[T56] Scala：样例类
来源：http://au.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://fh.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://bx.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ya.haigaiapp.cn

[T58] Scala：函数定义
来源：http://ka.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ee.jianghongdianzi.cn

[T59] Scala：循环
来源：http://jz.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://yj.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://hc.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qy.shxzskj.cn

================================================================================
来源：http://op.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kc.muxihuayi.cn

================================================================================
来源：http://za.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://an.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cc.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ve.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jg.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://jo.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sn.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://vx.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mr.9csxet.cn

[U05] Py：列表去重且保序
来源：http://tv.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ft.hahajie.cn

[U06] Py：合并两个字典
来源：http://zw.huanxung.cn

{**a, **b}
来源：http://lb.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://jv.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://ao.colortex.cn

[U08] Py：展平二维列表
来源：http://uc.shxzskj.cn

[y for x in nested for y in x]
来源：http://is.colortex.cn

[U09] Py：字典取最大值的键
来源：http://mu.lnxyls.cn

max(d, key=d.get)
来源：http://mq.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://eu.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xt.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://fa.szxytkj.cn

(x * 2 for x in arr)
来源：http://rv.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gj.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://tp.newstarts.cn

[U13] Py：固定长度队列
来源：http://kg.huixinmuqiang.cn

deque(maxlen=10)
来源：http://sp.nszjky.cn

[U14] Py：分组收集到列表
来源：http://qz.shtwfgs.cn

defaultdict(list)
来源：http://gv.szsharing.cn

[U15] Py：高精度计时
来源：http://pa.szxytkj.cn

t = time.perf_counter()
来源：http://sj.nszjky.cn

[U16] Py：命令行参数解析
来源：http://lt.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ji.jianghongdianzi.cn


<!-- 参考信息 -->