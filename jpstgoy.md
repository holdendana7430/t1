代发 wailian999

read -rp "请输入: " ans
来源：http://sh.shxzukj.cn

[R78] 交互式菜单
来源：http://on.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mw.newstarts.cn

[R79] 解析命令行选项
来源：http://bt.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sh.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://br.szsharing.cn

time ./run.sh
来源：http://ca.newstarts.cn

================================================================================
来源：http://md.jctech888.com.cn

S. C / C++ 专题
来源：http://tl.shxzukj.cn

================================================================================
来源：http://ei.nszjky.cn

[S01] C：Hello World
来源：http://uz.huixinmuqiang.cn

#include <stdio.h>
来源：http://pq.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gw.newstarts.cn

[S02] C：变量与格式化输出
来源：http://gq.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://pt.wgjwhj.cn

[S03] C：读入整数
来源：http://rm.521024.cn

int x; scanf("%d", &x);
来源：http://sw.wgjwhj.cn

[S04] C：字符串复制
来源：http://gj.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fy.521024.cn

[S05] C：字符串长度
来源：http://yc.9csxet.cn

strlen(s)
来源：http://ta.gzmigu.cn

[S06] C：字符串比较
来源：http://su.haigaiapp.cn

strcmp(a, b) == 0
来源：http://lj.asd995.cn

[S07] C：数组遍历求和
来源：http://ed.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yc.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://dv.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qf.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://hu.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zl.gzmigu.cn

[S10] C：指针与解引用
来源：http://nc.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://en.yuexingan06.cn

[S11] C：逐行读文件
来源：http://nt.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://gk.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://co.hahajie.cn

fclose(f);
来源：http://vh.bookmarksfly.cn

[S12] C：写文件
来源：http://gc.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rk.lnxyls.cn

[S13] C：宏定义
来源：http://wj.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kd.yuexingan06.cn

[S14] C：枚举
来源：http://hf.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://lg.hahajie.cn

[S15] C：类型转换
来源：http://ht.huixiangedu.cn

(double) a / b
来源：http://bu.jctech888.com.cn

[S16] C：位操作置位
来源：http://fh.bookmarksfly.cn

x |= (1 << 3);
来源：http://ty.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://mg.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xl.colortex.cn

[S18] C：命令行参数
来源：http://fw.chemitech.net.cn

int main(int argc, char **argv)
来源：http://dv.newstarts.cn

[S19] C：快速排序
来源：http://vm.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xf.yuexingan06.cn

[S20] C：二分查找
来源：http://be.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ja.colortex.cn

[S21] C：字符类别判断
来源：http://ai.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wv.hahajie.cn

[S22] C：字符串转数字
来源：http://lb.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fc.nicolike.cn

[S23] C：随机数
来源：http://df.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gk.huixiangedu.cn

[S24] C：获取本地时间
来源：http://do.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://di.colortex.cn

[S25] C：内存拷贝
来源：http://mj.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://sv.bjjhwx.cn

[S26] C：内存清零
来源：http://re.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://sb.yuexingan06.cn

[S27] C：定义常量
来源：http://ct.muxihuayi.cn

const double PI = 3.14159;
来源：http://nk.asd995.cn

[S28] C：静态变量
来源：http://wx.yuntaijiaju.cn

static int counter = 0;
来源：http://ti.hnjuh.cn

[S29] C：变参函数
来源：http://xn.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xp.jctech888.com.cn

[S30] C：头文件保护
来源：http://ec.nicolike.cn

#ifndef X_H
来源：http://kt.asd995.cn

#define X_H
来源：http://qm.shtwfgs.cn

#endif
来源：http://pw.gzmigu.cn

[S31] C++：Hello World
来源：http://jr.9csxet.cn

#include <iostream>
来源：http://ia.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://wb.yuexingan06.cn

[S32] C++：字符串
来源：http://lb.colortex.cn

std::string s = "hi";  s += "!";
来源：http://pq.bjjhwx.cn

[S33] C++：vector 增删
来源：http://vg.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hp.lnxyls.cn

[S34] C++：遍历 vector
来源：http://go.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://zv.colortex.cn

[S35] C++：map
来源：http://zy.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bx.shxzukj.cn

[S36] C++：unordered_map
来源：http://fj.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bx.lnxyls.cn

[S37] C++：set
来源：http://uu.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xm.muxihuayi.cn

[S38] C++：排序
来源：http://tl.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://ni.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://ap.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wc.521024.cn

[S40] C++：查找元素
来源：http://yp.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://we.szsharing.cn

[S41] C++：类与构造函数
来源：http://sk.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xt.szsharing.cn

[S42] C++：继承与虚函数
来源：http://bs.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://ll.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://tr.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://od.jctech888.com.cn

[S44] C++：引用传参
来源：http://xv.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://mo.szsharing.cn

[S45] C++：lambda
来源：http://ba.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ee.hahajie.cn

[S46] C++：函数模板
来源：http://vl.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hp.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://xn.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hv.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://dz.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oq.hahajie.cn

while (std::getline(in, line)) { }
来源：http://pl.wgjwhj.cn

[S49] C++：写文件
来源：http://cl.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hn.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://xr.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tq.nszjky.cn

[S51] C++：显式类型转换
来源：http://xt.hahajie.cn

static_cast<double>(a) / b
来源：http://ty.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://eu.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ae.asd995.cn

[S53] C++：移动语义
来源：http://rk.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://pn.hnjuh.cn

[S54] C++：异常处理
来源：http://kk.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sl.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://ck.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ji.yuntaijiaju.cn

[S56] C++：optional
来源：http://pu.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://as.lnxyls.cn

[S57] C++：编译期常量
来源：http://xo.shtwfgs.cn

constexpr int N = 10;
来源：http://mc.nszjky.cn

[S58] C++：命名空间
来源：http://lc.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://bu.nszjky.cn

[S59] C++：静态断言
来源：http://br.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://og.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://nb.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jn.jctech888.com.cn

================================================================================
来源：http://sd.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iq.shtwfgs.cn

================================================================================
来源：http://wb.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://jg.hnjuh.cn

println("Hello")
来源：http://zp.muxihuayi.cn

[T02] Kotlin：变量
来源：http://vr.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jf.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://ss.lnxyls.cn

"值: $b"
来源：http://st.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://au.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://my.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://tc.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ss.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://qq.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kv.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://lk.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qm.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://wj.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://mb.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://mq.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://ka.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://gf.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hi.hahajie.cn

[T11] Kotlin：协程
来源：http://de.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jb.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://xl.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://mi.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://cy.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ku.szsharing.cn

[T14] Kotlin：循环
来源：http://rg.shxzukj.cn

for (i in 1..10) println(i)
来源：http://ru.wgjwhj.cn

[T15] Kotlin：接口
来源：http://fz.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ds.9csxet.cn

[T16] Swift：Hello World
来源：http://lk.shxzukj.cn

print("Hello")
来源：http://qt.colortex.cn

[T17] Swift：变量与常量
来源：http://sf.huanxung.cn

var a = 1;  let b = 2
来源：http://ej.gzmigu.cn

[T18] Swift：字符串插值
来源：http://nm.shxzskj.cn

"值: \(b)"
来源：http://du.lnxyls.cn

[T19] Swift：可选绑定
来源：http://da.yuexingan06.cn

if let n = opt { print(n) }
来源：http://nn.bjjhwx.cn

[T20] Swift：数组操作
来源：http://fq.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tq.panjiajie.cn

[T21] Swift：遍历
来源：http://bb.gzmigu.cn

for x in a { print(x) }
来源：http://ay.bjjhwx.cn

[T22] Swift：字典
来源：http://su.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pa.chemitech.net.cn

[T23] Swift：函数
来源：http://jz.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hr.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ez.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ql.wgjwhj.cn

[T25] Swift：结构体
来源：http://lv.hnjuh.cn

struct P { var x: Int }
来源：http://dr.hahajie.cn

[T26] Swift：类与重写
来源：http://st.lnxyls.cn

class A: Base { override func f() {} }
来源：http://ff.szsharing.cn

[T27] Swift：错误处理
来源：http://ki.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://bh.muxihuayi.cn

[T28] Swift：枚举
来源：http://dm.szsharing.cn

enum Color { case red, green }
来源：http://pf.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://eq.shtwfgs.cn

guard let x = opt else { return }
来源：http://gd.nszjky.cn

[T30] Swift：协议
来源：http://vh.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://fe.panjiajie.cn

[T31] Lua：Hello World
来源：http://sp.panjiajie.cn

print("Hello")
来源：http://oa.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://ul.shxzskj.cn

local a = 1
来源：http://ka.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://xn.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sc.yuexingan06.cn

[T34] Lua：遍历表
来源：http://oj.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yb.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://wd.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://hy.521024.cn

[T36] Lua：函数
来源：http://yo.colortex.cn

function add(a, b) return a + b end
来源：http://fg.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://zf.521024.cn

"a" .. "b"
来源：http://gd.bookmarksfly.cn

[T38] Lua：条件
来源：http://tu.huixiangedu.cn

if x > 0 then print("正") end
来源：http://rd.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://bc.shxzukj.cn

string.find(s, "%d+")
来源：http://vz.haigaiapp.cn

[T40] Lua：元表
来源：http://cf.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://ys.asd995.cn

[T41] Perl：Hello World
来源：http://tv.colortex.cn

print "Hello\n";
来源：http://fb.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://tf.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ka.shxzukj.cn

[T43] Perl：字符串插值
来源：http://ro.hahajie.cn

"值: $a"
来源：http://kt.asd995.cn

[T44] Perl：条件
来源：http://ij.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://pp.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://xa.colortex.cn

for my $x (@arr) { print $x; }
来源：http://np.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://gh.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bf.szxytkj.cn

[T47] Perl：正则捕获
来源：http://tn.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rm.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://fm.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://aq.asd995.cn

[T49] Perl：函数
来源：http://to.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hp.newstarts.cn

[T50] Perl：逐行读文件
来源：http://ix.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bn.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ec.521024.cn

[T51] Scala：Hello World
来源：http://hs.haigaiapp.cn

println("Hello")
来源：http://ej.hahajie.cn

[T52] Scala：变量
来源：http://kf.gzmigu.cn

val a = 1;  var b = 2
来源：http://ix.hahajie.cn

[T53] Scala：字符串插值
来源：http://ww.szxytkj.cn

s"值: $b"
来源：http://br.nicolike.cn

[T54] Scala：集合映射
来源：http://ae.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ys.hahajie.cn

[T55] Scala：集合过滤
来源：http://ne.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cr.chemitech.net.cn

[T56] Scala：样例类
来源：http://uz.hahajie.cn

case class User(name: String, age: Int)
来源：http://sm.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://zb.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sv.asd995.cn

[T58] Scala：函数定义
来源：http://jl.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rr.huanxung.cn

[T59] Scala：循环
来源：http://px.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://za.nicolike.cn

[T60] Scala：折叠
来源：http://ab.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wm.521024.cn

================================================================================
来源：http://ih.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uz.panjiajie.cn

================================================================================
来源：http://ci.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://tl.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hj.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://ju.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qg.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://cw.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cl.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://jt.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ht.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://pa.nszjky.cn

list(dict.fromkeys(arr))
来源：http://ph.asd995.cn

[U06] Py：合并两个字典
来源：http://pn.yuexingan06.cn

{**a, **b}
来源：http://ag.lnxyls.cn

[U07] Py：反转字典键值
来源：http://ei.521024.cn

{v: k for k, v in d.items()}
来源：http://cj.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://fd.panjiajie.cn

[y for x in nested for y in x]
来源：http://rh.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ih.lnxyls.cn

max(d, key=d.get)
来源：http://tz.colortex.cn

[U10] Py：按值排序字典
来源：http://nz.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rz.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://ev.huanxung.cn

(x * 2 for x in arr)
来源：http://nu.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dc.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://dm.newstarts.cn

[U13] Py：固定长度队列
来源：http://wo.huixiangedu.cn

deque(maxlen=10)
来源：http://yz.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://dx.hnjuh.cn

defaultdict(list)
来源：http://th.huanxung.cn

[U15] Py：高精度计时
来源：http://mr.bookmarksfly.cn

t = time.perf_counter()
来源：http://eq.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://yj.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ab.shtwfgs.cn

[U17] Py：初始化日志
来源：http://qg.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://hf.colortex.cn

[U18] Py：预编译正则
来源：http://tp.huanxung.cn

pat = re.compile(r"\d+")
来源：http://jj.huixiangedu.cn


<!-- 参考信息 -->