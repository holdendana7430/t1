代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ti.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://lt.bjjhwx.cn

time ./run.sh
来源：http://ps.gzmigu.cn

================================================================================
来源：http://cd.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ob.nicolike.cn

================================================================================
来源：http://cs.hnjuh.cn

[S01] C：Hello World
来源：http://em.hnjuh.cn

#include <stdio.h>
来源：http://xr.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pg.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://by.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://hs.nicolike.cn

[S03] C：读入整数
来源：http://rf.szsharing.cn

int x; scanf("%d", &x);
来源：http://hd.shtwfgs.cn

[S04] C：字符串复制
来源：http://pz.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vm.lnxyls.cn

[S05] C：字符串长度
来源：http://pl.bjjhwx.cn

strlen(s)
来源：http://sz.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://ao.shxzukj.cn

strcmp(a, b) == 0
来源：http://ud.gzmigu.cn

[S07] C：数组遍历求和
来源：http://ck.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ty.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://vp.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wj.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://bd.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ih.newstarts.cn

[S10] C：指针与解引用
来源：http://ye.nicolike.cn

int *p = &a;  *p = 5;
来源：http://xj.shxzskj.cn

[S11] C：逐行读文件
来源：http://en.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://xa.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hv.newstarts.cn

fclose(f);
来源：http://jf.shtwfgs.cn

[S12] C：写文件
来源：http://em.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jo.haigaiapp.cn

[S13] C：宏定义
来源：http://mo.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ha.yuntaijiaju.cn

[S14] C：枚举
来源：http://hd.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://tt.yuexingan06.cn

[S15] C：类型转换
来源：http://hy.nszjky.cn

(double) a / b
来源：http://dk.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://jo.hahajie.cn

x |= (1 << 3);
来源：http://kn.huanxung.cn

[S17] C：安全拼接字符串
来源：http://bg.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fx.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://mv.shtwfgs.cn

int main(int argc, char **argv)
来源：http://hj.wgjwhj.cn

[S19] C：快速排序
来源：http://om.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fk.9csxet.cn

[S20] C：二分查找
来源：http://oo.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dh.hahajie.cn

[S21] C：字符类别判断
来源：http://wz.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gm.hnjuh.cn

[S22] C：字符串转数字
来源：http://lz.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mj.bjjhwx.cn

[S23] C：随机数
来源：http://ok.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ok.wgjwhj.cn

[S24] C：获取本地时间
来源：http://br.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kr.hnjuh.cn

[S25] C：内存拷贝
来源：http://ti.nszjky.cn

memcpy(dst, src, n);
来源：http://eg.hnjuh.cn

[S26] C：内存清零
来源：http://on.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://yh.bookmarksfly.cn

[S27] C：定义常量
来源：http://bt.hnjuh.cn

const double PI = 3.14159;
来源：http://gq.muxihuayi.cn

[S28] C：静态变量
来源：http://tt.chemitech.net.cn

static int counter = 0;
来源：http://wu.jctech888.com.cn

[S29] C：变参函数
来源：http://kl.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zl.asd995.cn

[S30] C：头文件保护
来源：http://zt.shtwfgs.cn

#ifndef X_H
来源：http://ee.wgjwhj.cn

#define X_H
来源：http://vt.yuexingan06.cn

#endif
来源：http://it.huanxung.cn

[S31] C++：Hello World
来源：http://bd.lnxyls.cn

#include <iostream>
来源：http://jt.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ch.wgjwhj.cn

[S32] C++：字符串
来源：http://zx.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://tk.lnxyls.cn

[S33] C++：vector 增删
来源：http://jg.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://it.szxytkj.cn

[S34] C++：遍历 vector
来源：http://sk.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://sd.huixiangedu.cn

[S35] C++：map
来源：http://zr.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nb.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://kt.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mw.yuntaijiaju.cn

[S37] C++：set
来源：http://zr.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dy.huixinmuqiang.cn

[S38] C++：排序
来源：http://yr.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://jd.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://ll.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xe.9csxet.cn

[S40] C++：查找元素
来源：http://qk.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kl.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://cx.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nq.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://bx.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://lk.bjjhwx.cn

[S43] C++：智能指针
来源：http://zn.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://ux.nicolike.cn

[S44] C++：引用传参
来源：http://mi.9csxet.cn

void inc(int &x) { ++x; }
来源：http://si.hnjuh.cn

[S45] C++：lambda
来源：http://dm.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cw.9csxet.cn

[S46] C++：函数模板
来源：http://dl.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dx.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://xy.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://go.asd995.cn

[S48] C++：逐行读文件
来源：http://ia.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wu.521024.cn

while (std::getline(in, line)) { }
来源：http://ai.9csxet.cn

[S49] C++：写文件
来源：http://hc.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://na.nszjky.cn

[S50] C++：格式化数字
来源：http://uf.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ol.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://rc.bjjhwx.cn

static_cast<double>(a) / b
来源：http://hg.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://na.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ec.colortex.cn

[S53] C++：移动语义
来源：http://cu.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://yc.shtwfgs.cn

[S54] C++：异常处理
来源：http://id.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rr.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://hh.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nm.shtwfgs.cn

[S56] C++：optional
来源：http://rw.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vx.yuexingan06.cn

[S57] C++：编译期常量
来源：http://lm.haigaiapp.cn

constexpr int N = 10;
来源：http://br.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://vq.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://zi.szxytkj.cn

[S59] C++：静态断言
来源：http://qx.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gw.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://uh.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vm.jianghongdianzi.cn

================================================================================
来源：http://aw.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://an.colortex.cn

================================================================================
来源：http://ix.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://mb.colortex.cn

println("Hello")
来源：http://fb.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://bn.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ib.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://jn.hahajie.cn

"值: $b"
来源：http://jv.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://ee.szxytkj.cn

val n: String? = null;  n?.length
来源：http://fp.asd995.cn

[T05] Kotlin：when 表达式
来源：http://cm.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bt.asd995.cn

[T06] Kotlin：集合映射
来源：http://du.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bw.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://ni.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lk.shxzskj.cn

[T08] Kotlin：数据类
来源：http://mo.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://my.colortex.cn

[T09] Kotlin：扩展函数
来源：http://qq.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://zx.colortex.cn

[T10] Kotlin：默认参数
来源：http://ej.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bj.szxytkj.cn

[T11] Kotlin：协程
来源：http://bo.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kk.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://rs.521024.cn

val (a, b) = Pair(1, 2)
来源：http://vs.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://ih.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://nu.haigaiapp.cn

[T14] Kotlin：循环
来源：http://et.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://ae.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://rs.nszjky.cn

interface Shape { fun area(): Double }
来源：http://jy.shtwfgs.cn

[T16] Swift：Hello World
来源：http://fr.nszjky.cn

print("Hello")
来源：http://ag.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://rg.521024.cn

var a = 1;  let b = 2
来源：http://fa.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://yc.haigaiapp.cn

"值: \(b)"
来源：http://sv.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://ul.haigaiapp.cn

if let n = opt { print(n) }
来源：http://jw.shxzskj.cn

[T20] Swift：数组操作
来源：http://he.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ax.huixiangedu.cn

[T21] Swift：遍历
来源：http://jk.szxytkj.cn

for x in a { print(x) }
来源：http://nu.wgjwhj.cn

[T22] Swift：字典
来源：http://ba.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rv.hnjuh.cn

[T23] Swift：函数
来源：http://hr.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dj.gzmigu.cn

[T24] Swift：闭包
来源：http://ap.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rh.521024.cn

[T25] Swift：结构体
来源：http://nf.huanxung.cn

struct P { var x: Int }
来源：http://vl.hnjuh.cn

[T26] Swift：类与重写
来源：http://ga.huanxung.cn

class A: Base { override func f() {} }
来源：http://ts.chemitech.net.cn

[T27] Swift：错误处理
来源：http://ut.colortex.cn

do { try f() } catch { print(error) }
来源：http://xm.bookmarksfly.cn

[T28] Swift：枚举
来源：http://as.huixiangedu.cn

enum Color { case red, green }
来源：http://cy.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://dl.szsharing.cn

guard let x = opt else { return }
来源：http://pm.newstarts.cn

[T30] Swift：协议
来源：http://or.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://qy.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://rv.hahajie.cn

print("Hello")
来源：http://on.newstarts.cn

[T32] Lua：局部变量
来源：http://qq.huixinmuqiang.cn

local a = 1
来源：http://ke.szsharing.cn

[T33] Lua：表（数组）
来源：http://an.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hi.haigaiapp.cn

[T34] Lua：遍历表
来源：http://tn.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ty.muxihuayi.cn

[T35] Lua：字典表
来源：http://on.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://zl.shtwfgs.cn

[T36] Lua：函数
来源：http://aj.chemitech.net.cn

function add(a, b) return a + b end
来源：http://ke.newstarts.cn

[T37] Lua：字符串拼接
来源：http://tv.lnxyls.cn

"a" .. "b"
来源：http://ea.nicolike.cn

[T38] Lua：条件
来源：http://as.szxytkj.cn

if x > 0 then print("正") end
来源：http://kj.gzmigu.cn

[T39] Lua：模式匹配
来源：http://hj.9csxet.cn

string.find(s, "%d+")
来源：http://oh.huixinmuqiang.cn

[T40] Lua：元表
来源：http://ul.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://vf.szsharing.cn

[T41] Perl：Hello World
来源：http://rv.shtwfgs.cn

print "Hello\n";
来源：http://bt.9csxet.cn

[T42] Perl：变量类型
来源：http://qf.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fx.521024.cn

[T43] Perl：字符串插值
来源：http://ku.colortex.cn

"值: $a"
来源：http://cb.chemitech.net.cn

[T44] Perl：条件
来源：http://fv.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://xb.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://ta.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://ss.panjiajie.cn

[T46] Perl：哈希操作
来源：http://rn.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sg.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://oc.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ob.521024.cn

[T48] Perl：正则替换
来源：http://uf.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://ai.nszjky.cn

[T49] Perl：函数
来源：http://fe.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ta.huanxung.cn

[T50] Perl：逐行读文件
来源：http://nx.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qg.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://wi.chemitech.net.cn

[T51] Scala：Hello World
来源：http://ib.hnjuh.cn

println("Hello")
来源：http://rs.newstarts.cn

[T52] Scala：变量
来源：http://hf.asd995.cn

val a = 1;  var b = 2
来源：http://px.lnxyls.cn

[T53] Scala：字符串插值
来源：http://bl.yuntaijiaju.cn

s"值: $b"
来源：http://dq.colortex.cn

[T54] Scala：集合映射
来源：http://mj.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://qq.asd995.cn

[T55] Scala：集合过滤
来源：http://bc.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zz.szxytkj.cn

[T56] Scala：样例类
来源：http://bt.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://lx.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ej.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lx.shtwfgs.cn

[T58] Scala：函数定义
来源：http://as.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vq.yuntaijiaju.cn

[T59] Scala：循环
来源：http://pz.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://zl.huanxung.cn

[T60] Scala：折叠
来源：http://bm.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bo.shxzukj.cn

================================================================================
来源：http://uh.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ic.szxytkj.cn

================================================================================
来源：http://kb.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://vi.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oe.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://qf.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://re.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://uf.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://si.panjiajie.cn

[U04] Py：变量调试打印
来源：http://za.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yi.nszjky.cn

[U05] Py：列表去重且保序
来源：http://pq.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://pp.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://da.9csxet.cn

{**a, **b}
来源：http://sv.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://ed.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://up.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://rq.nszjky.cn

[y for x in nested for y in x]
来源：http://iy.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://tv.huixiangedu.cn

max(d, key=d.get)
来源：http://dv.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://wq.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hf.szxytkj.cn

[U11] Py：生成器表达式
来源：http://dw.muxihuayi.cn

(x * 2 for x in arr)
来源：http://ni.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zg.szxytkj.cn

Counter(arr).most_common(3)
来源：http://kr.newstarts.cn

[U13] Py：固定长度队列
来源：http://qx.jctech888.com.cn

deque(maxlen=10)
来源：http://vk.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://vc.huixinmuqiang.cn

defaultdict(list)
来源：http://wx.asd995.cn

[U15] Py：高精度计时
来源：http://cn.jianghongdianzi.cn

t = time.perf_counter()
来源：http://il.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://eo.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kp.9csxet.cn

[U17] Py：初始化日志
来源：http://vt.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://te.newstarts.cn

[U18] Py：预编译正则
来源：http://bm.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://nl.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://me.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fv.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://hg.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ut.jctech888.com.cn


<!-- 参考信息 -->