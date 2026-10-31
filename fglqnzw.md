代发 wailian999

read -rp "请输入: " ans
来源：http://nl.9csxet.cn

[R78] 交互式菜单
来源：http://me.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kf.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ut.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qj.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://cy.szsharing.cn

time ./run.sh
来源：http://vk.szxytkj.cn

================================================================================
来源：http://yo.haigaiapp.cn

S. C / C++ 专题
来源：http://mm.szxytkj.cn

================================================================================
来源：http://ht.9csxet.cn

[S01] C：Hello World
来源：http://wc.panjiajie.cn

#include <stdio.h>
来源：http://hg.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ui.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ku.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://mb.shxzukj.cn

[S03] C：读入整数
来源：http://ao.shxzskj.cn

int x; scanf("%d", &x);
来源：http://nw.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://lc.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xv.huanxung.cn

[S05] C：字符串长度
来源：http://sa.bookmarksfly.cn

strlen(s)
来源：http://lb.haigaiapp.cn

[S06] C：字符串比较
来源：http://uc.wgjwhj.cn

strcmp(a, b) == 0
来源：http://lk.szsharing.cn

[S07] C：数组遍历求和
来源：http://bg.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ao.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://sp.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mj.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://hn.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yk.gzmigu.cn

[S10] C：指针与解引用
来源：http://qe.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://am.jctech888.com.cn

[S11] C：逐行读文件
来源：http://af.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://je.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ay.shxzskj.cn

fclose(f);
来源：http://ji.yuntaijiaju.cn

[S12] C：写文件
来源：http://dh.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kb.bjjhwx.cn

[S13] C：宏定义
来源：http://oh.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wr.huixiangedu.cn

[S14] C：枚举
来源：http://vl.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ry.hnjuh.cn

[S15] C：类型转换
来源：http://fh.hnjuh.cn

(double) a / b
来源：http://ua.asd995.cn

[S16] C：位操作置位
来源：http://nm.chemitech.net.cn

x |= (1 << 3);
来源：http://sj.hahajie.cn

[S17] C：安全拼接字符串
来源：http://di.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ds.jctech888.com.cn

[S18] C：命令行参数
来源：http://gf.lnxyls.cn

int main(int argc, char **argv)
来源：http://qt.muxihuayi.cn

[S19] C：快速排序
来源：http://xo.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://et.nicolike.cn

[S20] C：二分查找
来源：http://hh.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bg.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://nm.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yp.9csxet.cn

[S22] C：字符串转数字
来源：http://le.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://en.jianghongdianzi.cn

[S23] C：随机数
来源：http://kq.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ro.hahajie.cn

[S24] C：获取本地时间
来源：http://ay.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://at.newstarts.cn

[S25] C：内存拷贝
来源：http://pk.nszjky.cn

memcpy(dst, src, n);
来源：http://ct.hahajie.cn

[S26] C：内存清零
来源：http://hl.newstarts.cn

memset(a, 0, sizeof a);
来源：http://fa.huixinmuqiang.cn

[S27] C：定义常量
来源：http://go.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://jk.gzmigu.cn

[S28] C：静态变量
来源：http://mr.szxytkj.cn

static int counter = 0;
来源：http://qv.521024.cn

[S29] C：变参函数
来源：http://ik.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ev.bookmarksfly.cn

[S30] C：头文件保护
来源：http://ii.nicolike.cn

#ifndef X_H
来源：http://ya.colortex.cn

#define X_H
来源：http://jt.jianghongdianzi.cn

#endif
来源：http://qn.nszjky.cn

[S31] C++：Hello World
来源：http://lc.asd995.cn

#include <iostream>
来源：http://mp.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://ug.huanxung.cn

[S32] C++：字符串
来源：http://qr.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://ep.shxzskj.cn

[S33] C++：vector 增删
来源：http://nk.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yv.hnjuh.cn

[S34] C++：遍历 vector
来源：http://yr.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://br.shtwfgs.cn

[S35] C++：map
来源：http://cm.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rl.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://jz.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vf.colortex.cn

[S37] C++：set
来源：http://ms.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ud.panjiajie.cn

[S38] C++：排序
来源：http://vh.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://ul.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://tx.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zw.muxihuayi.cn

[S40] C++：查找元素
来源：http://qi.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ee.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://hv.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dy.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://ut.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://xq.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://fn.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://rp.gzmigu.cn

[S44] C++：引用传参
来源：http://xb.nicolike.cn

void inc(int &x) { ++x; }
来源：http://vz.chemitech.net.cn

[S45] C++：lambda
来源：http://hi.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mj.jctech888.com.cn

[S46] C++：函数模板
来源：http://sb.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vd.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://jv.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jp.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://iq.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bf.newstarts.cn

while (std::getline(in, line)) { }
来源：http://lm.szxytkj.cn

[S49] C++：写文件
来源：http://vb.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zn.szxytkj.cn

[S50] C++：格式化数字
来源：http://cb.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ga.lnxyls.cn

[S51] C++：显式类型转换
来源：http://zj.bjjhwx.cn

static_cast<double>(a) / b
来源：http://bu.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://rv.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://ly.jctech888.com.cn

[S53] C++：移动语义
来源：http://aa.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://qb.haigaiapp.cn

[S54] C++：异常处理
来源：http://fo.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bj.colortex.cn

[S55] C++：结构化绑定
来源：http://ez.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nf.yuexingan06.cn

[S56] C++：optional
来源：http://xg.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ka.panjiajie.cn

[S57] C++：编译期常量
来源：http://tn.szxytkj.cn

constexpr int N = 10;
来源：http://nx.hahajie.cn

[S58] C++：命名空间
来源：http://nm.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://is.muxihuayi.cn

[S59] C++：静态断言
来源：http://vv.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lz.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://aq.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fi.hahajie.cn

================================================================================
来源：http://ca.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ts.521024.cn

================================================================================
来源：http://ni.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ls.jianghongdianzi.cn

println("Hello")
来源：http://nc.muxihuayi.cn

[T02] Kotlin：变量
来源：http://jx.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vp.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://qs.muxihuayi.cn

"值: $b"
来源：http://up.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://sk.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://fh.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://dx.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ng.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://ta.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://se.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://da.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dw.nszjky.cn

[T08] Kotlin：数据类
来源：http://mp.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://kz.asd995.cn

[T09] Kotlin：扩展函数
来源：http://yr.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://yb.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://bc.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wb.hnjuh.cn

[T11] Kotlin：协程
来源：http://wp.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sr.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://tt.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://ab.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://hl.newstarts.cn

val m = mapOf("a" to 1)
来源：http://qf.shxzskj.cn

[T14] Kotlin：循环
来源：http://ws.shxzskj.cn

for (i in 1..10) println(i)
来源：http://sc.asd995.cn

[T15] Kotlin：接口
来源：http://lg.huanxung.cn

interface Shape { fun area(): Double }
来源：http://jj.wgjwhj.cn

[T16] Swift：Hello World
来源：http://gh.panjiajie.cn

print("Hello")
来源：http://ud.lnxyls.cn

[T17] Swift：变量与常量
来源：http://wp.lnxyls.cn

var a = 1;  let b = 2
来源：http://ss.szxytkj.cn

[T18] Swift：字符串插值
来源：http://gz.nszjky.cn

"值: \(b)"
来源：http://aw.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://hg.colortex.cn

if let n = opt { print(n) }
来源：http://zu.szsharing.cn

[T20] Swift：数组操作
来源：http://hv.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hn.haigaiapp.cn

[T21] Swift：遍历
来源：http://rk.hahajie.cn

for x in a { print(x) }
来源：http://oc.wgjwhj.cn

[T22] Swift：字典
来源：http://az.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ot.nicolike.cn

[T23] Swift：函数
来源：http://qb.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yn.newstarts.cn

[T24] Swift：闭包
来源：http://vl.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rf.haigaiapp.cn

[T25] Swift：结构体
来源：http://zi.newstarts.cn

struct P { var x: Int }
来源：http://xo.nicolike.cn

[T26] Swift：类与重写
来源：http://jk.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://le.shxzukj.cn

[T27] Swift：错误处理
来源：http://jc.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://uw.nszjky.cn

[T28] Swift：枚举
来源：http://le.gzmigu.cn

enum Color { case red, green }
来源：http://sy.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://ru.jctech888.com.cn

guard let x = opt else { return }
来源：http://me.huanxung.cn

[T30] Swift：协议
来源：http://pq.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://lb.jctech888.com.cn

[T31] Lua：Hello World
来源：http://af.9csxet.cn

print("Hello")
来源：http://jp.lnxyls.cn

[T32] Lua：局部变量
来源：http://or.panjiajie.cn

local a = 1
来源：http://mf.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://ds.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pt.shtwfgs.cn

[T34] Lua：遍历表
来源：http://wz.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xj.9csxet.cn

[T35] Lua：字典表
来源：http://pw.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://uo.9csxet.cn

[T36] Lua：函数
来源：http://rh.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://ar.huanxung.cn

[T37] Lua：字符串拼接
来源：http://ku.gzmigu.cn

"a" .. "b"
来源：http://hg.szsharing.cn

[T38] Lua：条件
来源：http://ao.jctech888.com.cn

if x > 0 then print("正") end
来源：http://tj.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://hg.szsharing.cn

string.find(s, "%d+")
来源：http://ti.colortex.cn

[T40] Lua：元表
来源：http://gi.9csxet.cn

setmetatable({}, { __index = base })
来源：http://vy.wgjwhj.cn

[T41] Perl：Hello World
来源：http://ix.szsharing.cn

print "Hello\n";
来源：http://mb.hnjuh.cn

[T42] Perl：变量类型
来源：http://aw.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pi.nicolike.cn

[T43] Perl：字符串插值
来源：http://im.shtwfgs.cn

"值: $a"
来源：http://jh.szxytkj.cn

[T44] Perl：条件
来源：http://by.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ft.shxzukj.cn

[T45] Perl：数组遍历
来源：http://es.colortex.cn

for my $x (@arr) { print $x; }
来源：http://lo.newstarts.cn

[T46] Perl：哈希操作
来源：http://bo.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qw.hahajie.cn

[T47] Perl：正则捕获
来源：http://mg.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lj.hnjuh.cn

[T48] Perl：正则替换
来源：http://by.nicolike.cn

$s =~ s/old/new/g;
来源：http://si.jctech888.com.cn

[T49] Perl：函数
来源：http://wm.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dk.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://yb.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hh.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://fx.colortex.cn

[T51] Scala：Hello World
来源：http://ep.jctech888.com.cn

println("Hello")
来源：http://wc.bjjhwx.cn

[T52] Scala：变量
来源：http://dd.gzmigu.cn

val a = 1;  var b = 2
来源：http://be.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://ga.huixinmuqiang.cn

s"值: $b"
来源：http://mm.huanxung.cn

[T54] Scala：集合映射
来源：http://ig.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://wz.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://ev.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ju.szxytkj.cn

[T56] Scala：样例类
来源：http://om.panjiajie.cn

case class User(name: String, age: Int)
来源：http://rr.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://wb.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jd.haigaiapp.cn

[T58] Scala：函数定义
来源：http://ec.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xe.bjjhwx.cn

[T59] Scala：循环
来源：http://dz.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://mq.haigaiapp.cn

[T60] Scala：折叠
来源：http://he.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yl.nicolike.cn

================================================================================
来源：http://ds.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sq.hahajie.cn

================================================================================
来源：http://lu.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://lj.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cp.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://gt.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ls.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://cd.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zi.shxzukj.cn

[U04] Py：变量调试打印
来源：http://bl.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wy.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://fn.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://vb.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://sr.gzmigu.cn

{**a, **b}
来源：http://du.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://xj.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://qi.lnxyls.cn

[U08] Py：展平二维列表
来源：http://xi.panjiajie.cn

[y for x in nested for y in x]
来源：http://ei.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://at.yuntaijiaju.cn

max(d, key=d.get)
来源：http://ut.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://em.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tw.hahajie.cn

[U11] Py：生成器表达式
来源：http://bn.haigaiapp.cn

(x * 2 for x in arr)
来源：http://oq.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yw.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://nz.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://fe.hnjuh.cn

deque(maxlen=10)
来源：http://ax.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://wf.asd995.cn

defaultdict(list)
来源：http://oc.shtwfgs.cn

[U15] Py：高精度计时
来源：http://ft.yuexingan06.cn

t = time.perf_counter()
来源：http://zo.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://uy.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://an.bjjhwx.cn

[U17] Py：初始化日志
来源：http://ag.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://vr.jianghongdianzi.cn

[U18] Py：预编译正则
来源：http://bq.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://ag.yuntaijiaju.cn


<!-- 参考信息 -->