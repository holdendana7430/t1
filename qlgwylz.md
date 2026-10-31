代发 wailian999

split -l 1000 big.log part_
来源：http://ey.muxihuayi.cn

[R74] 批量重命名
来源：http://qd.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ns.wgjwhj.cn

[R75] 导出环境变量
来源：http://ya.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://il.wgjwhj.cn

[R76] 使用临时文件
来源：http://tk.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tn.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ep.chemitech.net.cn

read -rp "请输入: " ans
来源：http://dp.bookmarksfly.cn

[R78] 交互式菜单
来源：http://lo.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oy.hahajie.cn

[R79] 解析命令行选项
来源：http://aa.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://or.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://qn.wgjwhj.cn

time ./run.sh
来源：http://jv.szxytkj.cn

================================================================================
来源：http://iv.huixiangedu.cn

S. C / C++ 专题
来源：http://ze.muxihuayi.cn

================================================================================
来源：http://fc.lnxyls.cn

[S01] C：Hello World
来源：http://qx.haigaiapp.cn

#include <stdio.h>
来源：http://bf.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nm.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://va.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://fw.colortex.cn

[S03] C：读入整数
来源：http://kt.huanxung.cn

int x; scanf("%d", &x);
来源：http://jh.shtwfgs.cn

[S04] C：字符串复制
来源：http://tq.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qa.szsharing.cn

[S05] C：字符串长度
来源：http://mb.lnxyls.cn

strlen(s)
来源：http://yo.shxzukj.cn

[S06] C：字符串比较
来源：http://md.colortex.cn

strcmp(a, b) == 0
来源：http://bs.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://mg.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gj.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://rh.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mv.asd995.cn

[S09] C：结构体定义与初始化
来源：http://lv.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fk.haigaiapp.cn

[S10] C：指针与解引用
来源：http://vg.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://tp.szsharing.cn

[S11] C：逐行读文件
来源：http://rb.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://tt.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fc.jianghongdianzi.cn

fclose(f);
来源：http://ez.nicolike.cn

[S12] C：写文件
来源：http://cq.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mt.nicolike.cn

[S13] C：宏定义
来源：http://qp.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://al.bookmarksfly.cn

[S14] C：枚举
来源：http://qt.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://mq.lnxyls.cn

[S15] C：类型转换
来源：http://vp.szxytkj.cn

(double) a / b
来源：http://ae.yuexingan06.cn

[S16] C：位操作置位
来源：http://wm.haigaiapp.cn

x |= (1 << 3);
来源：http://xt.newstarts.cn

[S17] C：安全拼接字符串
来源：http://zc.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wc.chemitech.net.cn

[S18] C：命令行参数
来源：http://dp.huixiangedu.cn

int main(int argc, char **argv)
来源：http://mf.asd995.cn

[S19] C：快速排序
来源：http://ad.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://il.wgjwhj.cn

[S20] C：二分查找
来源：http://zs.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://id.521024.cn

[S21] C：字符类别判断
来源：http://eh.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hm.haigaiapp.cn

[S22] C：字符串转数字
来源：http://ix.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xh.huixinmuqiang.cn

[S23] C：随机数
来源：http://pl.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pa.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://od.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://so.szxytkj.cn

[S25] C：内存拷贝
来源：http://vj.szxytkj.cn

memcpy(dst, src, n);
来源：http://lh.asd995.cn

[S26] C：内存清零
来源：http://vi.hahajie.cn

memset(a, 0, sizeof a);
来源：http://gn.nszjky.cn

[S27] C：定义常量
来源：http://ed.chemitech.net.cn

const double PI = 3.14159;
来源：http://oz.bjjhwx.cn

[S28] C：静态变量
来源：http://ck.yuntaijiaju.cn

static int counter = 0;
来源：http://zq.gzmigu.cn

[S29] C：变参函数
来源：http://tm.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oq.newstarts.cn

[S30] C：头文件保护
来源：http://kg.9csxet.cn

#ifndef X_H
来源：http://oc.huixiangedu.cn

#define X_H
来源：http://rs.huixiangedu.cn

#endif
来源：http://lw.colortex.cn

[S31] C++：Hello World
来源：http://eo.yuntaijiaju.cn

#include <iostream>
来源：http://et.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://yx.shxzukj.cn

[S32] C++：字符串
来源：http://ii.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://sg.newstarts.cn

[S33] C++：vector 增删
来源：http://xu.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://la.asd995.cn

[S34] C++：遍历 vector
来源：http://bt.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://rv.nszjky.cn

[S35] C++：map
来源：http://vu.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://se.9csxet.cn

[S36] C++：unordered_map
来源：http://js.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://br.muxihuayi.cn

[S37] C++：set
来源：http://tc.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gq.asd995.cn

[S38] C++：排序
来源：http://hs.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://wm.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://zv.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ql.colortex.cn

[S40] C++：查找元素
来源：http://vf.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mo.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://vy.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://en.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://ev.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://fp.muxihuayi.cn

[S43] C++：智能指针
来源：http://uh.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://ku.521024.cn

[S44] C++：引用传参
来源：http://qe.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://pm.bookmarksfly.cn

[S45] C++：lambda
来源：http://qt.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fv.9csxet.cn

[S46] C++：函数模板
来源：http://tz.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gp.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://ek.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uu.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://ll.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ht.9csxet.cn

while (std::getline(in, line)) { }
来源：http://eh.newstarts.cn

[S49] C++：写文件
来源：http://ry.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zq.huixiangedu.cn

[S50] C++：格式化数字
来源：http://ax.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gn.hahajie.cn

[S51] C++：显式类型转换
来源：http://ja.szxytkj.cn

static_cast<double>(a) / b
来源：http://wv.colortex.cn

[S52] C++：const 与 noexcept
来源：http://yy.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://cd.9csxet.cn

[S53] C++：移动语义
来源：http://zd.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://pq.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://qg.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://as.szxytkj.cn

[S55] C++：结构化绑定
来源：http://ob.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ml.szsharing.cn

[S56] C++：optional
来源：http://uc.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xy.nicolike.cn

[S57] C++：编译期常量
来源：http://vj.shxzskj.cn

constexpr int N = 10;
来源：http://vg.shxzskj.cn

[S58] C++：命名空间
来源：http://ju.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://pb.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://rm.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fk.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://wm.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ye.hahajie.cn

================================================================================
来源：http://sl.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vj.szsharing.cn

================================================================================
来源：http://ht.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://fo.nicolike.cn

println("Hello")
来源：http://gz.nszjky.cn

[T02] Kotlin：变量
来源：http://zo.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wq.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://qr.jctech888.com.cn

"值: $b"
来源：http://zs.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://yr.szxytkj.cn

val n: String? = null;  n?.length
来源：http://xh.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://py.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rp.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://ei.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jr.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://cg.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ua.521024.cn

[T08] Kotlin：数据类
来源：http://yd.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://iq.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://jp.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://ng.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://ua.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zn.colortex.cn

[T11] Kotlin：协程
来源：http://hs.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xj.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://tr.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://uh.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://nt.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://ga.colortex.cn

[T14] Kotlin：循环
来源：http://hs.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://bv.lnxyls.cn

[T15] Kotlin：接口
来源：http://bt.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://jc.colortex.cn

[T16] Swift：Hello World
来源：http://dx.shtwfgs.cn

print("Hello")
来源：http://qa.panjiajie.cn

[T17] Swift：变量与常量
来源：http://fa.shxzskj.cn

var a = 1;  let b = 2
来源：http://st.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://ja.panjiajie.cn

"值: \(b)"
来源：http://vl.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://vp.nicolike.cn

if let n = opt { print(n) }
来源：http://he.wgjwhj.cn

[T20] Swift：数组操作
来源：http://ay.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dp.szsharing.cn

[T21] Swift：遍历
来源：http://bh.yuexingan06.cn

for x in a { print(x) }
来源：http://qk.nszjky.cn

[T22] Swift：字典
来源：http://sa.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://to.panjiajie.cn

[T23] Swift：函数
来源：http://ce.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zh.nicolike.cn

[T24] Swift：闭包
来源：http://rb.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ef.yuexingan06.cn

[T25] Swift：结构体
来源：http://lc.521024.cn

struct P { var x: Int }
来源：http://yy.521024.cn

[T26] Swift：类与重写
来源：http://um.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://tk.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://bk.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://cf.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://ha.chemitech.net.cn

enum Color { case red, green }
来源：http://ml.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://ff.muxihuayi.cn

guard let x = opt else { return }
来源：http://tm.yuntaijiaju.cn

[T30] Swift：协议
来源：http://sk.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://an.shxzukj.cn

[T31] Lua：Hello World
来源：http://cs.szsharing.cn

print("Hello")
来源：http://us.lnxyls.cn

[T32] Lua：局部变量
来源：http://jb.shxzukj.cn

local a = 1
来源：http://pe.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://gi.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kn.lnxyls.cn

[T34] Lua：遍历表
来源：http://ar.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://us.muxihuayi.cn

[T35] Lua：字典表
来源：http://li.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://vp.jianghongdianzi.cn

[T36] Lua：函数
来源：http://ti.bjjhwx.cn

function add(a, b) return a + b end
来源：http://nd.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://rj.wgjwhj.cn

"a" .. "b"
来源：http://ar.shxzukj.cn

[T38] Lua：条件
来源：http://ns.muxihuayi.cn

if x > 0 then print("正") end
来源：http://cu.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://qm.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://ij.panjiajie.cn

[T40] Lua：元表
来源：http://qp.521024.cn

setmetatable({}, { __index = base })
来源：http://us.shxzukj.cn

[T41] Perl：Hello World
来源：http://vo.9csxet.cn

print "Hello\n";
来源：http://rt.hnjuh.cn

[T42] Perl：变量类型
来源：http://yv.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dp.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://cy.szxytkj.cn

"值: $a"
来源：http://gv.521024.cn

[T44] Perl：条件
来源：http://ta.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://sb.nszjky.cn

[T45] Perl：数组遍历
来源：http://pv.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://zv.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://ps.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qe.szsharing.cn

[T47] Perl：正则捕获
来源：http://qm.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ng.muxihuayi.cn

[T48] Perl：正则替换
来源：http://za.521024.cn

$s =~ s/old/new/g;
来源：http://ur.szxytkj.cn

[T49] Perl：函数
来源：http://vr.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kg.521024.cn

[T50] Perl：逐行读文件
来源：http://dy.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fb.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://yj.colortex.cn

[T51] Scala：Hello World
来源：http://ew.asd995.cn

println("Hello")
来源：http://vj.jctech888.com.cn

[T52] Scala：变量
来源：http://hc.panjiajie.cn

val a = 1;  var b = 2
来源：http://cs.lnxyls.cn

[T53] Scala：字符串插值
来源：http://kv.shtwfgs.cn

s"值: $b"
来源：http://qg.gzmigu.cn

[T54] Scala：集合映射
来源：http://cj.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://mp.lnxyls.cn

[T55] Scala：集合过滤
来源：http://wr.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ls.asd995.cn

[T56] Scala：样例类
来源：http://fs.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://xg.hahajie.cn

[T57] Scala：模式匹配
来源：http://yh.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jz.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://zf.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ci.lnxyls.cn

[T59] Scala：循环
来源：http://ns.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://rc.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://yj.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aa.shtwfgs.cn

================================================================================
来源：http://on.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jp.9csxet.cn

================================================================================
来源：http://ci.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://sn.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bj.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://mx.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ij.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://fh.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zt.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://qx.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aj.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://gr.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://rj.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://gy.shtwfgs.cn

{**a, **b}
来源：http://ao.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://ep.nicolike.cn

{v: k for k, v in d.items()}
来源：http://rz.shxzukj.cn

[U08] Py：展平二维列表
来源：http://vu.shxzukj.cn

[y for x in nested for y in x]
来源：http://xs.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://zw.haigaiapp.cn

max(d, key=d.get)
来源：http://kz.szsharing.cn

[U10] Py：按值排序字典
来源：http://zk.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wq.hahajie.cn

[U11] Py：生成器表达式
来源：http://fo.yuexingan06.cn

(x * 2 for x in arr)
来源：http://wt.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tz.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://gp.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://po.panjiajie.cn

deque(maxlen=10)
来源：http://gs.asd995.cn

[U14] Py：分组收集到列表
来源：http://vt.521024.cn

defaultdict(list)
来源：http://ei.colortex.cn


<!-- 参考信息 -->