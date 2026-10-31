代发 wailian999

read -rp "请输入: " ans
来源：http://hc.huixiangedu.cn

[R78] 交互式菜单
来源：http://sb.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pa.521024.cn

[R79] 解析命令行选项
来源：http://bm.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://at.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://yv.shxzukj.cn

time ./run.sh
来源：http://ue.9csxet.cn

================================================================================
来源：http://fg.huixinmuqiang.cn

S. C / C++ 专题
来源：http://nf.huixinmuqiang.cn

================================================================================
来源：http://ye.nicolike.cn

[S01] C：Hello World
来源：http://vr.huixiangedu.cn

#include <stdio.h>
来源：http://bg.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cj.nicolike.cn

[S02] C：变量与格式化输出
来源：http://ei.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://tj.shtwfgs.cn

[S03] C：读入整数
来源：http://sx.szxytkj.cn

int x; scanf("%d", &x);
来源：http://ag.szsharing.cn

[S04] C：字符串复制
来源：http://gz.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hl.panjiajie.cn

[S05] C：字符串长度
来源：http://fz.hnjuh.cn

strlen(s)
来源：http://js.szxytkj.cn

[S06] C：字符串比较
来源：http://da.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://ur.panjiajie.cn

[S07] C：数组遍历求和
来源：http://ss.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ra.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://ym.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cw.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://ai.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qe.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://ih.nicolike.cn

int *p = &a;  *p = 5;
来源：http://gc.521024.cn

[S11] C：逐行读文件
来源：http://ed.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xn.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ck.shxzukj.cn

fclose(f);
来源：http://my.hahajie.cn

[S12] C：写文件
来源：http://wm.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qa.hahajie.cn

[S13] C：宏定义
来源：http://io.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lv.lnxyls.cn

[S14] C：枚举
来源：http://ex.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://iu.szsharing.cn

[S15] C：类型转换
来源：http://ly.nicolike.cn

(double) a / b
来源：http://nu.chemitech.net.cn

[S16] C：位操作置位
来源：http://vv.521024.cn

x |= (1 << 3);
来源：http://mb.newstarts.cn

[S17] C：安全拼接字符串
来源：http://fl.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dk.521024.cn

[S18] C：命令行参数
来源：http://rg.huixiangedu.cn

int main(int argc, char **argv)
来源：http://jr.huixinmuqiang.cn

[S19] C：快速排序
来源：http://xf.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hm.jianghongdianzi.cn

[S20] C：二分查找
来源：http://yi.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oj.9csxet.cn

[S21] C：字符类别判断
来源：http://gz.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fq.shxzskj.cn

[S22] C：字符串转数字
来源：http://mw.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sy.muxihuayi.cn

[S23] C：随机数
来源：http://mo.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://de.colortex.cn

[S24] C：获取本地时间
来源：http://wb.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hb.nicolike.cn

[S25] C：内存拷贝
来源：http://bm.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://qk.shxzskj.cn

[S26] C：内存清零
来源：http://qd.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://pa.szxytkj.cn

[S27] C：定义常量
来源：http://mk.hahajie.cn

const double PI = 3.14159;
来源：http://nk.newstarts.cn

[S28] C：静态变量
来源：http://cd.521024.cn

static int counter = 0;
来源：http://bn.9csxet.cn

[S29] C：变参函数
来源：http://zc.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dt.muxihuayi.cn

[S30] C：头文件保护
来源：http://eq.shxzskj.cn

#ifndef X_H
来源：http://yc.wgjwhj.cn

#define X_H
来源：http://da.shxzskj.cn

#endif
来源：http://sy.nszjky.cn

[S31] C++：Hello World
来源：http://je.nszjky.cn

#include <iostream>
来源：http://jv.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://vm.yuntaijiaju.cn

[S32] C++：字符串
来源：http://vo.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://ld.hahajie.cn

[S33] C++：vector 增删
来源：http://un.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ya.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://oz.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://yx.hahajie.cn

[S35] C++：map
来源：http://dn.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kc.lnxyls.cn

[S36] C++：unordered_map
来源：http://rb.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ex.hnjuh.cn

[S37] C++：set
来源：http://mh.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xw.hahajie.cn

[S38] C++：排序
来源：http://jv.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://xa.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://xe.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://el.yuexingan06.cn

[S40] C++：查找元素
来源：http://dt.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fs.nszjky.cn

[S41] C++：类与构造函数
来源：http://qj.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://em.colortex.cn

[S42] C++：继承与虚函数
来源：http://td.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://ob.hahajie.cn

[S43] C++：智能指针
来源：http://sy.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://ih.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://uz.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://fu.nicolike.cn

[S45] C++：lambda
来源：http://tw.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ii.huixiangedu.cn

[S46] C++：函数模板
来源：http://uh.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ns.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://fn.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xy.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://en.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nb.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://ml.haigaiapp.cn

[S49] C++：写文件
来源：http://vo.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ou.chemitech.net.cn

[S50] C++：格式化数字
来源：http://tk.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fp.hnjuh.cn

[S51] C++：显式类型转换
来源：http://jx.huixiangedu.cn

static_cast<double>(a) / b
来源：http://di.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://xd.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://yi.chemitech.net.cn

[S53] C++：移动语义
来源：http://nl.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://oq.colortex.cn

[S54] C++：异常处理
来源：http://vq.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vq.nszjky.cn

[S55] C++：结构化绑定
来源：http://mm.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fm.bookmarksfly.cn

[S56] C++：optional
来源：http://lm.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ym.shxzukj.cn

[S57] C++：编译期常量
来源：http://gk.chemitech.net.cn

constexpr int N = 10;
来源：http://jx.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://yk.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://sr.nicolike.cn

[S59] C++：静态断言
来源：http://vw.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vf.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://fu.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pp.shtwfgs.cn

================================================================================
来源：http://st.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rw.shtwfgs.cn

================================================================================
来源：http://bz.colortex.cn

[T01] Kotlin：Hello World
来源：http://uu.asd995.cn

println("Hello")
来源：http://mj.muxihuayi.cn

[T02] Kotlin：变量
来源：http://qb.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zs.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://ly.wgjwhj.cn

"值: $b"
来源：http://kb.panjiajie.cn

[T04] Kotlin：空安全
来源：http://gh.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://qk.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://oa.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jo.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://hb.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kc.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://lj.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gd.hnjuh.cn

[T08] Kotlin：数据类
来源：http://gd.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://om.521024.cn

[T09] Kotlin：扩展函数
来源：http://kc.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://ga.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://zd.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://px.hahajie.cn

[T11] Kotlin：协程
来源：http://ky.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vf.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://yx.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://hu.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://wr.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://uq.521024.cn

[T14] Kotlin：循环
来源：http://ez.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://pv.shtwfgs.cn

[T15] Kotlin：接口
来源：http://jp.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://rj.newstarts.cn

[T16] Swift：Hello World
来源：http://oy.shtwfgs.cn

print("Hello")
来源：http://pw.9csxet.cn

[T17] Swift：变量与常量
来源：http://ea.nicolike.cn

var a = 1;  let b = 2
来源：http://dj.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://vn.szsharing.cn

"值: \(b)"
来源：http://xz.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://fr.huanxung.cn

if let n = opt { print(n) }
来源：http://wt.huixiangedu.cn

[T20] Swift：数组操作
来源：http://mg.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ir.gzmigu.cn

[T21] Swift：遍历
来源：http://zy.shxzskj.cn

for x in a { print(x) }
来源：http://cj.hnjuh.cn

[T22] Swift：字典
来源：http://yf.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fa.szsharing.cn

[T23] Swift：函数
来源：http://qj.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gk.asd995.cn

[T24] Swift：闭包
来源：http://ae.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ce.shxzukj.cn

[T25] Swift：结构体
来源：http://kh.shxzukj.cn

struct P { var x: Int }
来源：http://ss.colortex.cn

[T26] Swift：类与重写
来源：http://eh.szxytkj.cn

class A: Base { override func f() {} }
来源：http://wp.hnjuh.cn

[T27] Swift：错误处理
来源：http://fp.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://vd.yuexingan06.cn

[T28] Swift：枚举
来源：http://ze.jctech888.com.cn

enum Color { case red, green }
来源：http://ss.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://ig.jctech888.com.cn

guard let x = opt else { return }
来源：http://zo.huixiangedu.cn

[T30] Swift：协议
来源：http://by.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://hv.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://oo.521024.cn

print("Hello")
来源：http://td.muxihuayi.cn

[T32] Lua：局部变量
来源：http://he.muxihuayi.cn

local a = 1
来源：http://dy.9csxet.cn

[T33] Lua：表（数组）
来源：http://ue.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://he.colortex.cn

[T34] Lua：遍历表
来源：http://sq.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wj.gzmigu.cn

[T35] Lua：字典表
来源：http://tj.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://cx.panjiajie.cn

[T36] Lua：函数
来源：http://mg.newstarts.cn

function add(a, b) return a + b end
来源：http://fp.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://xh.wgjwhj.cn

"a" .. "b"
来源：http://bo.nszjky.cn

[T38] Lua：条件
来源：http://nu.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://mf.521024.cn

[T39] Lua：模式匹配
来源：http://sy.szxytkj.cn

string.find(s, "%d+")
来源：http://ci.bjjhwx.cn

[T40] Lua：元表
来源：http://on.colortex.cn

setmetatable({}, { __index = base })
来源：http://ev.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://po.huanxung.cn

print "Hello\n";
来源：http://jc.wgjwhj.cn

[T42] Perl：变量类型
来源：http://ds.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vq.9csxet.cn

[T43] Perl：字符串插值
来源：http://ms.panjiajie.cn

"值: $a"
来源：http://jb.bookmarksfly.cn

[T44] Perl：条件
来源：http://ym.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://ne.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://dp.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://gz.szsharing.cn

[T46] Perl：哈希操作
来源：http://hr.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fv.huanxung.cn

[T47] Perl：正则捕获
来源：http://dd.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lg.lnxyls.cn

[T48] Perl：正则替换
来源：http://mc.asd995.cn

$s =~ s/old/new/g;
来源：http://qn.jianghongdianzi.cn

[T49] Perl：函数
来源：http://if.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hk.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://am.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cg.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://ch.lnxyls.cn

[T51] Scala：Hello World
来源：http://av.nicolike.cn

println("Hello")
来源：http://aw.yuexingan06.cn

[T52] Scala：变量
来源：http://vr.nicolike.cn

val a = 1;  var b = 2
来源：http://bd.szxytkj.cn

[T53] Scala：字符串插值
来源：http://nh.9csxet.cn

s"值: $b"
来源：http://lk.huixiangedu.cn

[T54] Scala：集合映射
来源：http://iv.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://kd.colortex.cn

[T55] Scala：集合过滤
来源：http://dw.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ir.nicolike.cn

[T56] Scala：样例类
来源：http://dp.shxzukj.cn

case class User(name: String, age: Int)
来源：http://ed.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://cp.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pr.nszjky.cn

[T58] Scala：函数定义
来源：http://wn.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wq.huanxung.cn

[T59] Scala：循环
来源：http://yj.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://cw.shxzskj.cn

[T60] Scala：折叠
来源：http://vk.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ra.jctech888.com.cn

================================================================================
来源：http://nl.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fi.asd995.cn

================================================================================
来源：http://za.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://yu.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qb.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://ac.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gp.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://lr.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wf.newstarts.cn

[U04] Py：变量调试打印
来源：http://nk.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hh.9csxet.cn

[U05] Py：列表去重且保序
来源：http://vw.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://fl.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://oh.521024.cn

{**a, **b}
来源：http://oy.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://vs.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://gy.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://zc.chemitech.net.cn

[y for x in nested for y in x]
来源：http://tf.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://bb.asd995.cn

max(d, key=d.get)
来源：http://bi.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://ks.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wl.521024.cn

[U11] Py：生成器表达式
来源：http://vx.hahajie.cn

(x * 2 for x in arr)
来源：http://ad.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kk.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://di.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://fp.muxihuayi.cn

deque(maxlen=10)
来源：http://ev.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://uo.hahajie.cn

defaultdict(list)
来源：http://et.huixiangedu.cn

[U15] Py：高精度计时
来源：http://av.szsharing.cn

t = time.perf_counter()
来源：http://po.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://hq.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qo.wgjwhj.cn

[U17] Py：初始化日志
来源：http://oy.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://bh.wgjwhj.cn

[U18] Py：预编译正则
来源：http://qw.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://vj.wgjwhj.cn


<!-- 参考信息 -->