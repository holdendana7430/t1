代发 wailian999

S. C / C++ 专题
来源：http://mx.shxzskj.cn

================================================================================
来源：http://qi.521024.cn

[S01] C：Hello World
来源：http://gc.szsharing.cn

#include <stdio.h>
来源：http://dj.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fo.newstarts.cn

[S02] C：变量与格式化输出
来源：http://of.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://is.yuexingan06.cn

[S03] C：读入整数
来源：http://xz.hnjuh.cn

int x; scanf("%d", &x);
来源：http://ua.yuexingan06.cn

[S04] C：字符串复制
来源：http://pu.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gv.huixiangedu.cn

[S05] C：字符串长度
来源：http://ak.colortex.cn

strlen(s)
来源：http://mp.yuexingan06.cn

[S06] C：字符串比较
来源：http://ld.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://do.shxzskj.cn

[S07] C：数组遍历求和
来源：http://sj.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wf.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://te.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rw.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://bz.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ja.chemitech.net.cn

[S10] C：指针与解引用
来源：http://qn.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://jq.szsharing.cn

[S11] C：逐行读文件
来源：http://ai.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://jq.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ie.bjjhwx.cn

fclose(f);
来源：http://zs.shtwfgs.cn

[S12] C：写文件
来源：http://yg.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cy.colortex.cn

[S13] C：宏定义
来源：http://oj.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qe.hnjuh.cn

[S14] C：枚举
来源：http://iu.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://it.szxytkj.cn

[S15] C：类型转换
来源：http://te.hahajie.cn

(double) a / b
来源：http://br.hnjuh.cn

[S16] C：位操作置位
来源：http://hg.bjjhwx.cn

x |= (1 << 3);
来源：http://sz.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://qi.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lx.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://vl.chemitech.net.cn

int main(int argc, char **argv)
来源：http://uu.wgjwhj.cn

[S19] C：快速排序
来源：http://vu.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hz.muxihuayi.cn

[S20] C：二分查找
来源：http://gb.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wf.lnxyls.cn

[S21] C：字符类别判断
来源：http://eu.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mk.huanxung.cn

[S22] C：字符串转数字
来源：http://be.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qs.bookmarksfly.cn

[S23] C：随机数
来源：http://uh.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ql.bjjhwx.cn

[S24] C：获取本地时间
来源：http://cb.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xl.hnjuh.cn

[S25] C：内存拷贝
来源：http://be.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://bv.bjjhwx.cn

[S26] C：内存清零
来源：http://xj.colortex.cn

memset(a, 0, sizeof a);
来源：http://xe.chemitech.net.cn

[S27] C：定义常量
来源：http://ui.chemitech.net.cn

const double PI = 3.14159;
来源：http://wz.521024.cn

[S28] C：静态变量
来源：http://yq.shxzukj.cn

static int counter = 0;
来源：http://kj.bjjhwx.cn

[S29] C：变参函数
来源：http://ua.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oo.muxihuayi.cn

[S30] C：头文件保护
来源：http://tr.muxihuayi.cn

#ifndef X_H
来源：http://sk.szsharing.cn

#define X_H
来源：http://lm.newstarts.cn

#endif
来源：http://ce.shxzskj.cn

[S31] C++：Hello World
来源：http://lz.nszjky.cn

#include <iostream>
来源：http://gz.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://dh.shxzskj.cn

[S32] C++：字符串
来源：http://cl.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://no.shxzukj.cn

[S33] C++：vector 增删
来源：http://qp.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://in.521024.cn

[S34] C++：遍历 vector
来源：http://ie.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://fd.huixinmuqiang.cn

[S35] C++：map
来源：http://si.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://po.newstarts.cn

[S36] C++：unordered_map
来源：http://hg.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xq.hnjuh.cn

[S37] C++：set
来源：http://ck.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bv.shxzskj.cn

[S38] C++：排序
来源：http://or.521024.cn

std::sort(v.begin(), v.end());
来源：http://ty.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://xy.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cy.bjjhwx.cn

[S40] C++：查找元素
来源：http://ue.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qp.colortex.cn

[S41] C++：类与构造函数
来源：http://yb.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hy.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://jv.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://fb.wgjwhj.cn

[S43] C++：智能指针
来源：http://cg.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://vq.gzmigu.cn

[S44] C++：引用传参
来源：http://zi.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://qc.jianghongdianzi.cn

[S45] C++：lambda
来源：http://et.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nt.521024.cn

[S46] C++：函数模板
来源：http://dw.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ng.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://tf.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lx.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://jj.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zw.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://xp.colortex.cn

[S49] C++：写文件
来源：http://gj.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ne.gzmigu.cn

[S50] C++：格式化数字
来源：http://fd.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fs.asd995.cn

[S51] C++：显式类型转换
来源：http://aw.panjiajie.cn

static_cast<double>(a) / b
来源：http://pq.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://jd.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://rl.newstarts.cn

[S53] C++：移动语义
来源：http://rt.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://im.huanxung.cn

[S54] C++：异常处理
来源：http://sz.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qr.lnxyls.cn

[S55] C++：结构化绑定
来源：http://tp.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bm.nszjky.cn

[S56] C++：optional
来源：http://td.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lh.panjiajie.cn

[S57] C++：编译期常量
来源：http://cz.jctech888.com.cn

constexpr int N = 10;
来源：http://jn.lnxyls.cn

[S58] C++：命名空间
来源：http://et.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://td.asd995.cn

[S59] C++：静态断言
来源：http://vq.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bz.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://vl.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ng.nszjky.cn

================================================================================
来源：http://co.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qx.chemitech.net.cn

================================================================================
来源：http://tv.nszjky.cn

[T01] Kotlin：Hello World
来源：http://an.yuntaijiaju.cn

println("Hello")
来源：http://so.shxzskj.cn

[T02] Kotlin：变量
来源：http://zj.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ah.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://xt.nszjky.cn

"值: $b"
来源：http://rx.szxytkj.cn

[T04] Kotlin：空安全
来源：http://dk.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://mu.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://gw.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://us.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://kt.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tr.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://zi.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nq.colortex.cn

[T08] Kotlin：数据类
来源：http://de.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://kj.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://pr.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://ip.521024.cn

[T10] Kotlin：默认参数
来源：http://jo.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pl.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ec.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vw.9csxet.cn

[T12] Kotlin：解构声明
来源：http://zo.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://bc.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://ce.521024.cn

val m = mapOf("a" to 1)
来源：http://fl.shxzskj.cn

[T14] Kotlin：循环
来源：http://jn.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://tn.9csxet.cn

[T15] Kotlin：接口
来源：http://wq.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://mu.nszjky.cn

[T16] Swift：Hello World
来源：http://qb.shxzskj.cn

print("Hello")
来源：http://tb.nicolike.cn

[T17] Swift：变量与常量
来源：http://vx.shxzskj.cn

var a = 1;  let b = 2
来源：http://rp.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://ww.huixiangedu.cn

"值: \(b)"
来源：http://dl.asd995.cn

[T19] Swift：可选绑定
来源：http://mh.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://hg.wgjwhj.cn

[T20] Swift：数组操作
来源：http://ud.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zd.szsharing.cn

[T21] Swift：遍历
来源：http://jy.nicolike.cn

for x in a { print(x) }
来源：http://ix.shtwfgs.cn

[T22] Swift：字典
来源：http://tn.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pv.szxytkj.cn

[T23] Swift：函数
来源：http://ln.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bw.szsharing.cn

[T24] Swift：闭包
来源：http://qb.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wu.shtwfgs.cn

[T25] Swift：结构体
来源：http://mh.9csxet.cn

struct P { var x: Int }
来源：http://wc.colortex.cn

[T26] Swift：类与重写
来源：http://wt.panjiajie.cn

class A: Base { override func f() {} }
来源：http://al.shtwfgs.cn

[T27] Swift：错误处理
来源：http://hr.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://cb.gzmigu.cn

[T28] Swift：枚举
来源：http://mr.szsharing.cn

enum Color { case red, green }
来源：http://et.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://do.huanxung.cn

guard let x = opt else { return }
来源：http://pk.szxytkj.cn

[T30] Swift：协议
来源：http://gz.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://um.nszjky.cn

[T31] Lua：Hello World
来源：http://ht.asd995.cn

print("Hello")
来源：http://zz.szsharing.cn

[T32] Lua：局部变量
来源：http://rv.hnjuh.cn

local a = 1
来源：http://lj.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://mz.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zx.jctech888.com.cn

[T34] Lua：遍历表
来源：http://gp.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sb.chemitech.net.cn

[T35] Lua：字典表
来源：http://bg.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://at.9csxet.cn

[T36] Lua：函数
来源：http://nn.colortex.cn

function add(a, b) return a + b end
来源：http://qg.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://gd.shxzukj.cn

"a" .. "b"
来源：http://hq.yuexingan06.cn

[T38] Lua：条件
来源：http://va.huanxung.cn

if x > 0 then print("正") end
来源：http://fk.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://yz.chemitech.net.cn

string.find(s, "%d+")
来源：http://sj.panjiajie.cn

[T40] Lua：元表
来源：http://lp.nicolike.cn

setmetatable({}, { __index = base })
来源：http://ny.muxihuayi.cn

[T41] Perl：Hello World
来源：http://uq.muxihuayi.cn

print "Hello\n";
来源：http://ow.huixiangedu.cn

[T42] Perl：变量类型
来源：http://kq.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gk.9csxet.cn

[T43] Perl：字符串插值
来源：http://ld.hnjuh.cn

"值: $a"
来源：http://rx.szsharing.cn

[T44] Perl：条件
来源：http://dd.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://fo.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://gc.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://uh.gzmigu.cn

[T46] Perl：哈希操作
来源：http://ku.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://by.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://lh.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dq.yuexingan06.cn

[T48] Perl：正则替换
来源：http://oa.shxzukj.cn

$s =~ s/old/new/g;
来源：http://vb.lnxyls.cn

[T49] Perl：函数
来源：http://df.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wn.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://zl.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rg.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://pg.asd995.cn

[T51] Scala：Hello World
来源：http://mr.hnjuh.cn

println("Hello")
来源：http://xp.shxzukj.cn

[T52] Scala：变量
来源：http://qh.nszjky.cn

val a = 1;  var b = 2
来源：http://fp.szxytkj.cn

[T53] Scala：字符串插值
来源：http://wd.huixiangedu.cn

s"值: $b"
来源：http://po.colortex.cn

[T54] Scala：集合映射
来源：http://jg.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://xr.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://tr.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ha.gzmigu.cn

[T56] Scala：样例类
来源：http://ce.colortex.cn

case class User(name: String, age: Int)
来源：http://dy.panjiajie.cn

[T57] Scala：模式匹配
来源：http://bq.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jt.shxzukj.cn

[T58] Scala：函数定义
来源：http://pk.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fk.szxytkj.cn

[T59] Scala：循环
来源：http://wz.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://nb.bookmarksfly.cn

[T60] Scala：折叠
来源：http://gz.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nm.yuntaijiaju.cn

================================================================================
来源：http://my.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pi.nicolike.cn

================================================================================
来源：http://ff.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://rf.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xc.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://xx.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kd.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://zq.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kx.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://lw.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wr.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://ox.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://fr.9csxet.cn

[U06] Py：合并两个字典
来源：http://dr.lnxyls.cn

{**a, **b}
来源：http://go.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://ll.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://fw.gzmigu.cn

[U08] Py：展平二维列表
来源：http://at.huanxung.cn

[y for x in nested for y in x]
来源：http://xb.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://tt.9csxet.cn

max(d, key=d.get)
来源：http://im.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://hl.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://th.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://tc.panjiajie.cn

(x * 2 for x in arr)
来源：http://wc.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ds.szxytkj.cn

Counter(arr).most_common(3)
来源：http://qr.panjiajie.cn

[U13] Py：固定长度队列
来源：http://dm.muxihuayi.cn

deque(maxlen=10)
来源：http://fx.nszjky.cn

[U14] Py：分组收集到列表
来源：http://mp.muxihuayi.cn

defaultdict(list)
来源：http://sn.bjjhwx.cn

[U15] Py：高精度计时
来源：http://sy.wgjwhj.cn

t = time.perf_counter()
来源：http://it.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://xx.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sp.wgjwhj.cn

[U17] Py：初始化日志
来源：http://jv.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://ka.hahajie.cn

[U18] Py：预编译正则
来源：http://nh.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://lg.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://op.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://en.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://zy.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://mp.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://nr.szsharing.cn

@contextlib.contextmanager
来源：http://wr.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://fu.hnjuh.cn

list(zip(*m))
来源：http://od.panjiajie.cn


<!-- 参考信息 -->