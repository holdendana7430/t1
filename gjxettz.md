代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://ug.shxzskj.cn

[R76] 使用临时文件
来源：http://wn.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dt.asd995.cn

[R77] 读取用户输入
来源：http://df.panjiajie.cn

read -rp "请输入: " ans
来源：http://wh.szsharing.cn

[R78] 交互式菜单
来源：http://xu.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ez.szsharing.cn

[R79] 解析命令行选项
来源：http://kv.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ep.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://ah.haigaiapp.cn

time ./run.sh
来源：http://zi.9csxet.cn

================================================================================
来源：http://fl.szxytkj.cn

S. C / C++ 专题
来源：http://za.shxzukj.cn

================================================================================
来源：http://vi.hnjuh.cn

[S01] C：Hello World
来源：http://wi.jianghongdianzi.cn

#include <stdio.h>
来源：http://nq.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ru.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://ca.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://wd.newstarts.cn

[S03] C：读入整数
来源：http://hx.hnjuh.cn

int x; scanf("%d", &x);
来源：http://jm.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://rg.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kr.huanxung.cn

[S05] C：字符串长度
来源：http://gn.chemitech.net.cn

strlen(s)
来源：http://xf.shxzukj.cn

[S06] C：字符串比较
来源：http://tc.shtwfgs.cn

strcmp(a, b) == 0
来源：http://hu.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://bn.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nu.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://na.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aw.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://ex.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uc.szxytkj.cn

[S10] C：指针与解引用
来源：http://ek.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://le.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://pg.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://fr.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ix.lnxyls.cn

fclose(f);
来源：http://nc.shxzskj.cn

[S12] C：写文件
来源：http://je.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wu.szxytkj.cn

[S13] C：宏定义
来源：http://jh.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zs.bookmarksfly.cn

[S14] C：枚举
来源：http://qh.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://qd.jianghongdianzi.cn

[S15] C：类型转换
来源：http://ro.bookmarksfly.cn

(double) a / b
来源：http://mf.hnjuh.cn

[S16] C：位操作置位
来源：http://lr.jctech888.com.cn

x |= (1 << 3);
来源：http://gn.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://bt.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tw.nszjky.cn

[S18] C：命令行参数
来源：http://rc.colortex.cn

int main(int argc, char **argv)
来源：http://gj.jianghongdianzi.cn

[S19] C：快速排序
来源：http://ys.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eu.panjiajie.cn

[S20] C：二分查找
来源：http://lp.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qy.jctech888.com.cn

[S21] C：字符类别判断
来源：http://bp.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zk.muxihuayi.cn

[S22] C：字符串转数字
来源：http://qm.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qh.muxihuayi.cn

[S23] C：随机数
来源：http://aq.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zr.lnxyls.cn

[S24] C：获取本地时间
来源：http://ay.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rv.nicolike.cn

[S25] C：内存拷贝
来源：http://qw.bjjhwx.cn

memcpy(dst, src, n);
来源：http://ka.szsharing.cn

[S26] C：内存清零
来源：http://eo.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://pi.bjjhwx.cn

[S27] C：定义常量
来源：http://wn.asd995.cn

const double PI = 3.14159;
来源：http://hi.huixiangedu.cn

[S28] C：静态变量
来源：http://ag.muxihuayi.cn

static int counter = 0;
来源：http://mj.jctech888.com.cn

[S29] C：变参函数
来源：http://ej.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dl.szxytkj.cn

[S30] C：头文件保护
来源：http://tm.huanxung.cn

#ifndef X_H
来源：http://lh.huixiangedu.cn

#define X_H
来源：http://rs.szsharing.cn

#endif
来源：http://fy.asd995.cn

[S31] C++：Hello World
来源：http://mw.newstarts.cn

#include <iostream>
来源：http://er.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://vq.yuexingan06.cn

[S32] C++：字符串
来源：http://gx.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://us.521024.cn

[S33] C++：vector 增删
来源：http://pq.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oh.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://fp.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://oc.hahajie.cn

[S35] C++：map
来源：http://qm.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://su.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://gn.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wb.shtwfgs.cn

[S37] C++：set
来源：http://dw.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cl.jianghongdianzi.cn

[S38] C++：排序
来源：http://qv.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://zq.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://xf.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rv.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://sj.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bc.hahajie.cn

[S41] C++：类与构造函数
来源：http://xj.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ut.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://ic.521024.cn

class B : public Base { public: void f() override {} };
来源：http://ff.bookmarksfly.cn

[S43] C++：智能指针
来源：http://am.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://av.521024.cn

[S44] C++：引用传参
来源：http://gj.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://go.colortex.cn

[S45] C++：lambda
来源：http://cr.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zu.szxytkj.cn

[S46] C++：函数模板
来源：http://uk.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wt.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://js.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oz.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://jt.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eg.nszjky.cn

while (std::getline(in, line)) { }
来源：http://yr.shtwfgs.cn

[S49] C++：写文件
来源：http://xr.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nh.9csxet.cn

[S50] C++：格式化数字
来源：http://qq.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bn.nszjky.cn

[S51] C++：显式类型转换
来源：http://cr.gzmigu.cn

static_cast<double>(a) / b
来源：http://bk.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://uz.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://hz.jctech888.com.cn

[S53] C++：移动语义
来源：http://jz.colortex.cn

std::vector<int> w = std::move(v);
来源：http://jl.huixiangedu.cn

[S54] C++：异常处理
来源：http://px.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nx.newstarts.cn

[S55] C++：结构化绑定
来源：http://av.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iw.bjjhwx.cn

[S56] C++：optional
来源：http://mj.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bm.yuexingan06.cn

[S57] C++：编译期常量
来源：http://cm.gzmigu.cn

constexpr int N = 10;
来源：http://pi.newstarts.cn

[S58] C++：命名空间
来源：http://fe.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://zp.lnxyls.cn

[S59] C++：静态断言
来源：http://qr.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hk.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://lb.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gd.hnjuh.cn

================================================================================
来源：http://fg.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jv.nszjky.cn

================================================================================
来源：http://uh.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://zk.muxihuayi.cn

println("Hello")
来源：http://ut.wgjwhj.cn

[T02] Kotlin：变量
来源：http://kq.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xo.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://xf.shxzukj.cn

"值: $b"
来源：http://qn.shxzukj.cn

[T04] Kotlin：空安全
来源：http://yw.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://eh.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://pe.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yx.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://wb.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bk.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://dp.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bl.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://kc.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://qr.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://fv.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://fo.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://cb.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ao.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://ce.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pk.szsharing.cn

[T12] Kotlin：解构声明
来源：http://ii.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://ui.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://rb.asd995.cn

val m = mapOf("a" to 1)
来源：http://sm.yuexingan06.cn

[T14] Kotlin：循环
来源：http://wb.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://gp.shxzskj.cn

[T15] Kotlin：接口
来源：http://cl.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://zi.panjiajie.cn

[T16] Swift：Hello World
来源：http://fq.huanxung.cn

print("Hello")
来源：http://ak.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://cm.hahajie.cn

var a = 1;  let b = 2
来源：http://tw.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://lj.jctech888.com.cn

"值: \(b)"
来源：http://qr.panjiajie.cn

[T19] Swift：可选绑定
来源：http://iv.huanxung.cn

if let n = opt { print(n) }
来源：http://dg.szsharing.cn

[T20] Swift：数组操作
来源：http://xw.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ns.asd995.cn

[T21] Swift：遍历
来源：http://yz.hnjuh.cn

for x in a { print(x) }
来源：http://dg.yuexingan06.cn

[T22] Swift：字典
来源：http://fj.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ej.yuexingan06.cn

[T23] Swift：函数
来源：http://gv.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lo.panjiajie.cn

[T24] Swift：闭包
来源：http://qc.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yk.hahajie.cn

[T25] Swift：结构体
来源：http://rr.lnxyls.cn

struct P { var x: Int }
来源：http://tl.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://lb.asd995.cn

class A: Base { override func f() {} }
来源：http://iy.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://es.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://ie.muxihuayi.cn

[T28] Swift：枚举
来源：http://bp.szsharing.cn

enum Color { case red, green }
来源：http://gl.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://ur.nszjky.cn

guard let x = opt else { return }
来源：http://gs.huixinmuqiang.cn

[T30] Swift：协议
来源：http://jl.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://pa.haigaiapp.cn

[T31] Lua：Hello World
来源：http://bw.haigaiapp.cn

print("Hello")
来源：http://is.panjiajie.cn

[T32] Lua：局部变量
来源：http://gl.jianghongdianzi.cn

local a = 1
来源：http://ej.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://pu.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wy.hahajie.cn

[T34] Lua：遍历表
来源：http://gj.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xg.bjjhwx.cn

[T35] Lua：字典表
来源：http://xj.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://ri.hahajie.cn

[T36] Lua：函数
来源：http://jx.huixiangedu.cn

function add(a, b) return a + b end
来源：http://zr.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://vr.shxzukj.cn

"a" .. "b"
来源：http://ac.jctech888.com.cn

[T38] Lua：条件
来源：http://vl.asd995.cn

if x > 0 then print("正") end
来源：http://mu.521024.cn

[T39] Lua：模式匹配
来源：http://no.huixiangedu.cn

string.find(s, "%d+")
来源：http://ug.9csxet.cn

[T40] Lua：元表
来源：http://et.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://ue.szxytkj.cn

[T41] Perl：Hello World
来源：http://nf.panjiajie.cn

print "Hello\n";
来源：http://zl.yuexingan06.cn

[T42] Perl：变量类型
来源：http://gt.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ht.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://ew.yuexingan06.cn

"值: $a"
来源：http://fg.szxytkj.cn

[T44] Perl：条件
来源：http://ty.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://bf.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://uw.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://eo.hnjuh.cn

[T46] Perl：哈希操作
来源：http://mh.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pp.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://lg.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hn.gzmigu.cn

[T48] Perl：正则替换
来源：http://em.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://ms.shxzskj.cn

[T49] Perl：函数
来源：http://sx.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://su.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://ey.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fj.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://px.nicolike.cn

[T51] Scala：Hello World
来源：http://ac.szsharing.cn

println("Hello")
来源：http://fn.521024.cn

[T52] Scala：变量
来源：http://ru.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://ux.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ni.nszjky.cn

s"值: $b"
来源：http://ua.shxzukj.cn

[T54] Scala：集合映射
来源：http://ug.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://jy.9csxet.cn

[T55] Scala：集合过滤
来源：http://jm.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cb.shtwfgs.cn

[T56] Scala：样例类
来源：http://cz.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://hy.9csxet.cn

[T57] Scala：模式匹配
来源：http://dx.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vm.colortex.cn

[T58] Scala：函数定义
来源：http://jc.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ds.szsharing.cn

[T59] Scala：循环
来源：http://qe.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://vv.521024.cn

[T60] Scala：折叠
来源：http://ay.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hc.shxzskj.cn

================================================================================
来源：http://vz.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vr.gzmigu.cn

================================================================================
来源：http://gk.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://rc.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wb.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://ti.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uh.colortex.cn

[U03] Py：加载 .env 配置
来源：http://oi.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ts.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://ag.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://im.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://dx.nszjky.cn

list(dict.fromkeys(arr))
来源：http://ph.huanxung.cn

[U06] Py：合并两个字典
来源：http://do.jianghongdianzi.cn

{**a, **b}
来源：http://xr.lnxyls.cn

[U07] Py：反转字典键值
来源：http://sf.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://wz.lnxyls.cn

[U08] Py：展平二维列表
来源：http://ao.huixiangedu.cn

[y for x in nested for y in x]
来源：http://yo.colortex.cn

[U09] Py：字典取最大值的键
来源：http://ja.bjjhwx.cn

max(d, key=d.get)
来源：http://ky.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://jg.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fn.nszjky.cn

[U11] Py：生成器表达式
来源：http://jr.newstarts.cn

(x * 2 for x in arr)
来源：http://xa.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://to.colortex.cn

Counter(arr).most_common(3)
来源：http://cn.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://zx.szsharing.cn

deque(maxlen=10)
来源：http://vj.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://le.shxzskj.cn

defaultdict(list)
来源：http://qj.nicolike.cn

[U15] Py：高精度计时
来源：http://jr.huanxung.cn

t = time.perf_counter()
来源：http://es.521024.cn

[U16] Py：命令行参数解析
来源：http://yu.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yo.huixinmuqiang.cn


<!-- 参考信息 -->