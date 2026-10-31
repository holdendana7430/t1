代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://xn.szxytkj.cn

[R76] 使用临时文件
来源：http://sx.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://th.hahajie.cn

[R77] 读取用户输入
来源：http://xz.huanxung.cn

read -rp "请输入: " ans
来源：http://ma.szsharing.cn

[R78] 交互式菜单
来源：http://kh.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ef.panjiajie.cn

[R79] 解析命令行选项
来源：http://ys.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iy.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://fe.szsharing.cn

time ./run.sh
来源：http://cy.chemitech.net.cn

================================================================================
来源：http://gy.lnxyls.cn

S. C / C++ 专题
来源：http://mg.colortex.cn

================================================================================
来源：http://ox.shxzukj.cn

[S01] C：Hello World
来源：http://mm.jianghongdianzi.cn

#include <stdio.h>
来源：http://yr.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nd.hahajie.cn

[S02] C：变量与格式化输出
来源：http://tl.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://fj.muxihuayi.cn

[S03] C：读入整数
来源：http://sr.huanxung.cn

int x; scanf("%d", &x);
来源：http://mo.panjiajie.cn

[S04] C：字符串复制
来源：http://cs.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nz.szsharing.cn

[S05] C：字符串长度
来源：http://ms.jctech888.com.cn

strlen(s)
来源：http://ua.colortex.cn

[S06] C：字符串比较
来源：http://gr.shtwfgs.cn

strcmp(a, b) == 0
来源：http://js.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://vf.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qw.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://yc.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pp.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://vf.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sg.shxzukj.cn

[S10] C：指针与解引用
来源：http://hq.asd995.cn

int *p = &a;  *p = 5;
来源：http://es.szsharing.cn

[S11] C：逐行读文件
来源：http://ne.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://no.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lb.bookmarksfly.cn

fclose(f);
来源：http://qd.nicolike.cn

[S12] C：写文件
来源：http://lv.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lf.yuntaijiaju.cn

[S13] C：宏定义
来源：http://um.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wc.szxytkj.cn

[S14] C：枚举
来源：http://ir.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://fk.nszjky.cn

[S15] C：类型转换
来源：http://oe.haigaiapp.cn

(double) a / b
来源：http://zg.521024.cn

[S16] C：位操作置位
来源：http://ge.shxzskj.cn

x |= (1 << 3);
来源：http://ba.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://kt.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sa.chemitech.net.cn

[S18] C：命令行参数
来源：http://ly.bjjhwx.cn

int main(int argc, char **argv)
来源：http://qb.chemitech.net.cn

[S19] C：快速排序
来源：http://sk.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rd.shxzskj.cn

[S20] C：二分查找
来源：http://ur.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cx.huanxung.cn

[S21] C：字符类别判断
来源：http://rb.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xw.huixiangedu.cn

[S22] C：字符串转数字
来源：http://gj.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sq.yuexingan06.cn

[S23] C：随机数
来源：http://ty.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://np.9csxet.cn

[S24] C：获取本地时间
来源：http://ha.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://el.lnxyls.cn

[S25] C：内存拷贝
来源：http://rx.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://ll.bjjhwx.cn

[S26] C：内存清零
来源：http://zx.huanxung.cn

memset(a, 0, sizeof a);
来源：http://jk.asd995.cn

[S27] C：定义常量
来源：http://ge.asd995.cn

const double PI = 3.14159;
来源：http://el.lnxyls.cn

[S28] C：静态变量
来源：http://ke.521024.cn

static int counter = 0;
来源：http://pz.yuexingan06.cn

[S29] C：变参函数
来源：http://ke.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jc.chemitech.net.cn

[S30] C：头文件保护
来源：http://xa.huixiangedu.cn

#ifndef X_H
来源：http://pr.newstarts.cn

#define X_H
来源：http://ft.szsharing.cn

#endif
来源：http://mt.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://gy.asd995.cn

#include <iostream>
来源：http://hd.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://vo.shtwfgs.cn

[S32] C++：字符串
来源：http://rm.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://lr.bjjhwx.cn

[S33] C++：vector 增删
来源：http://pn.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yj.asd995.cn

[S34] C++：遍历 vector
来源：http://bs.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://zu.wgjwhj.cn

[S35] C++：map
来源：http://xn.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oy.lnxyls.cn

[S36] C++：unordered_map
来源：http://ld.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sj.colortex.cn

[S37] C++：set
来源：http://ig.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wo.colortex.cn

[S38] C++：排序
来源：http://jb.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://ky.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://lf.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vv.521024.cn

[S40] C++：查找元素
来源：http://md.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://on.shxzskj.cn

[S41] C++：类与构造函数
来源：http://nj.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bq.huanxung.cn

[S42] C++：继承与虚函数
来源：http://hr.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://pp.huixiangedu.cn

[S43] C++：智能指针
来源：http://cz.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://cx.newstarts.cn

[S44] C++：引用传参
来源：http://lc.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://jk.asd995.cn

[S45] C++：lambda
来源：http://qo.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uo.shtwfgs.cn

[S46] C++：函数模板
来源：http://eq.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sv.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://nw.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xa.asd995.cn

[S48] C++：逐行读文件
来源：http://ea.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fs.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://sz.yuexingan06.cn

[S49] C++：写文件
来源：http://sc.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bj.chemitech.net.cn

[S50] C++：格式化数字
来源：http://sq.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yj.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://qt.haigaiapp.cn

static_cast<double>(a) / b
来源：http://ej.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://ed.521024.cn

int size() const noexcept { return n_; }
来源：http://zw.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://gt.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://kr.hahajie.cn

[S54] C++：异常处理
来源：http://xg.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fw.lnxyls.cn

[S55] C++：结构化绑定
来源：http://hx.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://il.nszjky.cn

[S56] C++：optional
来源：http://vi.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fl.lnxyls.cn

[S57] C++：编译期常量
来源：http://xv.bookmarksfly.cn

constexpr int N = 10;
来源：http://fr.bjjhwx.cn

[S58] C++：命名空间
来源：http://ba.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://oe.szxytkj.cn

[S59] C++：静态断言
来源：http://tu.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nb.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://dv.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fh.wgjwhj.cn

================================================================================
来源：http://tx.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wy.nicolike.cn

================================================================================
来源：http://oy.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://nk.gzmigu.cn

println("Hello")
来源：http://hp.hahajie.cn

[T02] Kotlin：变量
来源：http://sn.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dl.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://cf.shxzskj.cn

"值: $b"
来源：http://oq.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://er.hahajie.cn

val n: String? = null;  n?.length
来源：http://it.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://kh.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://di.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://ks.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ku.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://rs.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ut.hahajie.cn

[T08] Kotlin：数据类
来源：http://fj.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://jc.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://gn.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://vp.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://ao.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vd.nszjky.cn

[T11] Kotlin：协程
来源：http://nk.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ah.hahajie.cn

[T12] Kotlin：解构声明
来源：http://be.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://kr.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://ld.hahajie.cn

val m = mapOf("a" to 1)
来源：http://by.haigaiapp.cn

[T14] Kotlin：循环
来源：http://kw.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://qz.huanxung.cn

[T15] Kotlin：接口
来源：http://lc.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://wq.nszjky.cn

[T16] Swift：Hello World
来源：http://hj.gzmigu.cn

print("Hello")
来源：http://ad.shxzskj.cn

[T17] Swift：变量与常量
来源：http://mv.haigaiapp.cn

var a = 1;  let b = 2
来源：http://tu.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://kh.shtwfgs.cn

"值: \(b)"
来源：http://vd.szsharing.cn

[T19] Swift：可选绑定
来源：http://ha.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://ly.chemitech.net.cn

[T20] Swift：数组操作
来源：http://sx.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ix.shtwfgs.cn

[T21] Swift：遍历
来源：http://dx.lnxyls.cn

for x in a { print(x) }
来源：http://tw.bookmarksfly.cn

[T22] Swift：字典
来源：http://jn.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xf.gzmigu.cn

[T23] Swift：函数
来源：http://vi.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pp.szxytkj.cn

[T24] Swift：闭包
来源：http://am.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hx.haigaiapp.cn

[T25] Swift：结构体
来源：http://hi.shxzukj.cn

struct P { var x: Int }
来源：http://qx.nszjky.cn

[T26] Swift：类与重写
来源：http://pi.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://se.jctech888.com.cn

[T27] Swift：错误处理
来源：http://zz.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://em.muxihuayi.cn

[T28] Swift：枚举
来源：http://wm.jctech888.com.cn

enum Color { case red, green }
来源：http://wo.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://nq.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://dt.huanxung.cn

[T30] Swift：协议
来源：http://wl.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://rs.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://gd.muxihuayi.cn

print("Hello")
来源：http://gk.jctech888.com.cn

[T32] Lua：局部变量
来源：http://wj.lnxyls.cn

local a = 1
来源：http://ts.hahajie.cn

[T33] Lua：表（数组）
来源：http://pl.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kk.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://gb.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ai.szxytkj.cn

[T35] Lua：字典表
来源：http://tz.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://ht.bookmarksfly.cn

[T36] Lua：函数
来源：http://ud.huanxung.cn

function add(a, b) return a + b end
来源：http://eh.szsharing.cn

[T37] Lua：字符串拼接
来源：http://js.gzmigu.cn

"a" .. "b"
来源：http://to.nszjky.cn

[T38] Lua：条件
来源：http://nh.gzmigu.cn

if x > 0 then print("正") end
来源：http://hy.shxzskj.cn

[T39] Lua：模式匹配
来源：http://pl.shtwfgs.cn

string.find(s, "%d+")
来源：http://se.bookmarksfly.cn

[T40] Lua：元表
来源：http://ti.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://dg.nszjky.cn

[T41] Perl：Hello World
来源：http://mi.huanxung.cn

print "Hello\n";
来源：http://gu.newstarts.cn

[T42] Perl：变量类型
来源：http://af.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vy.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://qz.yuexingan06.cn

"值: $a"
来源：http://kr.gzmigu.cn

[T44] Perl：条件
来源：http://xr.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://xx.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://vc.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://qy.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://su.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sa.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ur.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ju.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://qp.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://it.521024.cn

[T49] Perl：函数
来源：http://cj.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://km.newstarts.cn

[T50] Perl：逐行读文件
来源：http://xq.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qy.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://rw.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://jp.nicolike.cn

println("Hello")
来源：http://jq.bjjhwx.cn

[T52] Scala：变量
来源：http://pz.huanxung.cn

val a = 1;  var b = 2
来源：http://vl.nicolike.cn

[T53] Scala：字符串插值
来源：http://ex.newstarts.cn

s"值: $b"
来源：http://mt.bjjhwx.cn

[T54] Scala：集合映射
来源：http://yf.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://ep.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://at.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wb.9csxet.cn

[T56] Scala：样例类
来源：http://ir.9csxet.cn

case class User(name: String, age: Int)
来源：http://yh.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://hz.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ff.huixiangedu.cn

[T58] Scala：函数定义
来源：http://ow.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zb.szsharing.cn

[T59] Scala：循环
来源：http://qr.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://af.newstarts.cn

[T60] Scala：折叠
来源：http://cv.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://la.yuntaijiaju.cn

================================================================================
来源：http://bs.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kz.nszjky.cn

================================================================================
来源：http://vi.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://mv.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dn.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://vc.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wc.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://bf.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ot.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://jc.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sy.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://zb.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://tr.szsharing.cn

[U06] Py：合并两个字典
来源：http://vy.yuntaijiaju.cn

{**a, **b}
来源：http://bx.huanxung.cn

[U07] Py：反转字典键值
来源：http://ss.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://pe.nszjky.cn

[U08] Py：展平二维列表
来源：http://ub.shxzskj.cn

[y for x in nested for y in x]
来源：http://fe.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://tm.hnjuh.cn

max(d, key=d.get)
来源：http://fl.huanxung.cn

[U10] Py：按值排序字典
来源：http://ix.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cx.hahajie.cn

[U11] Py：生成器表达式
来源：http://vf.9csxet.cn

(x * 2 for x in arr)
来源：http://rq.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ie.newstarts.cn

Counter(arr).most_common(3)
来源：http://ql.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://xb.nicolike.cn

deque(maxlen=10)
来源：http://pw.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://hc.muxihuayi.cn

defaultdict(list)
来源：http://vb.yuexingan06.cn

[U15] Py：高精度计时
来源：http://dw.newstarts.cn

t = time.perf_counter()
来源：http://ny.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://gf.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://py.huixiangedu.cn


<!-- 参考信息 -->