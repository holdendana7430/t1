代发 wailian999

S. C / C++ 专题
来源：http://cd.szsharing.cn

================================================================================
来源：http://oa.huanxung.cn

[S01] C：Hello World
来源：http://vr.haigaiapp.cn

#include <stdio.h>
来源：http://jb.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dr.newstarts.cn

[S02] C：变量与格式化输出
来源：http://xl.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://rn.jianghongdianzi.cn

[S03] C：读入整数
来源：http://my.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://pv.9csxet.cn

[S04] C：字符串复制
来源：http://os.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dw.wgjwhj.cn

[S05] C：字符串长度
来源：http://bp.nicolike.cn

strlen(s)
来源：http://zs.hahajie.cn

[S06] C：字符串比较
来源：http://gy.huixiangedu.cn

strcmp(a, b) == 0
来源：http://hu.asd995.cn

[S07] C：数组遍历求和
来源：http://jm.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bl.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://in.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nk.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://uo.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dz.hahajie.cn

[S10] C：指针与解引用
来源：http://dk.9csxet.cn

int *p = &a;  *p = 5;
来源：http://mz.asd995.cn

[S11] C：逐行读文件
来源：http://nh.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://ye.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ze.colortex.cn

fclose(f);
来源：http://lc.nicolike.cn

[S12] C：写文件
来源：http://in.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qt.haigaiapp.cn

[S13] C：宏定义
来源：http://qj.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://so.asd995.cn

[S14] C：枚举
来源：http://hl.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ea.colortex.cn

[S15] C：类型转换
来源：http://yd.huixiangedu.cn

(double) a / b
来源：http://kh.huixiangedu.cn

[S16] C：位操作置位
来源：http://lk.521024.cn

x |= (1 << 3);
来源：http://ri.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://qd.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jg.521024.cn

[S18] C：命令行参数
来源：http://fg.muxihuayi.cn

int main(int argc, char **argv)
来源：http://es.huanxung.cn

[S19] C：快速排序
来源：http://md.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gu.wgjwhj.cn

[S20] C：二分查找
来源：http://xj.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://la.chemitech.net.cn

[S21] C：字符类别判断
来源：http://tr.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sr.chemitech.net.cn

[S22] C：字符串转数字
来源：http://ox.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lj.panjiajie.cn

[S23] C：随机数
来源：http://df.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kz.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://wq.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ug.wgjwhj.cn

[S25] C：内存拷贝
来源：http://xi.haigaiapp.cn

memcpy(dst, src, n);
来源：http://jk.szsharing.cn

[S26] C：内存清零
来源：http://vz.szsharing.cn

memset(a, 0, sizeof a);
来源：http://wj.bookmarksfly.cn

[S27] C：定义常量
来源：http://tc.huanxung.cn

const double PI = 3.14159;
来源：http://if.shxzukj.cn

[S28] C：静态变量
来源：http://ts.szxytkj.cn

static int counter = 0;
来源：http://mr.521024.cn

[S29] C：变参函数
来源：http://ab.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yn.521024.cn

[S30] C：头文件保护
来源：http://bn.haigaiapp.cn

#ifndef X_H
来源：http://ml.huixinmuqiang.cn

#define X_H
来源：http://ld.nszjky.cn

#endif
来源：http://de.hahajie.cn

[S31] C++：Hello World
来源：http://ps.shtwfgs.cn

#include <iostream>
来源：http://dd.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://au.nszjky.cn

[S32] C++：字符串
来源：http://bh.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://lo.shtwfgs.cn

[S33] C++：vector 增删
来源：http://ph.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ia.lnxyls.cn

[S34] C++：遍历 vector
来源：http://zk.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://mo.521024.cn

[S35] C++：map
来源：http://mi.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eo.hnjuh.cn

[S36] C++：unordered_map
来源：http://yw.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cc.jctech888.com.cn

[S37] C++：set
来源：http://vx.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oy.shtwfgs.cn

[S38] C++：排序
来源：http://zu.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://we.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://sn.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ky.bjjhwx.cn

[S40] C++：查找元素
来源：http://kg.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jz.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://nf.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ln.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://zh.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://vd.muxihuayi.cn

[S43] C++：智能指针
来源：http://du.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://kh.wgjwhj.cn

[S44] C++：引用传参
来源：http://bc.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://hj.asd995.cn

[S45] C++：lambda
来源：http://se.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://af.shtwfgs.cn

[S46] C++：函数模板
来源：http://ur.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sl.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://ip.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pf.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://iu.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bl.521024.cn

while (std::getline(in, line)) { }
来源：http://ws.muxihuayi.cn

[S49] C++：写文件
来源：http://nl.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cb.9csxet.cn

[S50] C++：格式化数字
来源：http://cb.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qg.newstarts.cn

[S51] C++：显式类型转换
来源：http://gu.shxzukj.cn

static_cast<double>(a) / b
来源：http://kx.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://wb.9csxet.cn

int size() const noexcept { return n_; }
来源：http://vf.shxzukj.cn

[S53] C++：移动语义
来源：http://fr.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://uq.panjiajie.cn

[S54] C++：异常处理
来源：http://cp.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fl.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://vk.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ca.gzmigu.cn

[S56] C++：optional
来源：http://lz.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ec.asd995.cn

[S57] C++：编译期常量
来源：http://wk.szsharing.cn

constexpr int N = 10;
来源：http://mh.colortex.cn

[S58] C++：命名空间
来源：http://mi.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://fe.shtwfgs.cn

[S59] C++：静态断言
来源：http://re.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wh.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://rw.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ju.huixinmuqiang.cn

================================================================================
来源：http://hg.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mr.bjjhwx.cn

================================================================================
来源：http://bp.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://ad.muxihuayi.cn

println("Hello")
来源：http://rh.szsharing.cn

[T02] Kotlin：变量
来源：http://uh.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dy.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://vd.hnjuh.cn

"值: $b"
来源：http://ff.hahajie.cn

[T04] Kotlin：空安全
来源：http://fa.nszjky.cn

val n: String? = null;  n?.length
来源：http://rw.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://ug.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nr.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://ve.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ki.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://sh.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pn.lnxyls.cn

[T08] Kotlin：数据类
来源：http://kv.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://rs.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://sb.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://am.colortex.cn

[T10] Kotlin：默认参数
来源：http://zh.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kr.nicolike.cn

[T11] Kotlin：协程
来源：http://hb.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://op.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://hh.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://fq.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://so.asd995.cn

val m = mapOf("a" to 1)
来源：http://mg.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://na.shxzukj.cn

for (i in 1..10) println(i)
来源：http://ne.hnjuh.cn

[T15] Kotlin：接口
来源：http://dl.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://xl.asd995.cn

[T16] Swift：Hello World
来源：http://st.hnjuh.cn

print("Hello")
来源：http://jr.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://ey.wgjwhj.cn

var a = 1;  let b = 2
来源：http://gy.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://fg.bjjhwx.cn

"值: \(b)"
来源：http://os.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://vo.lnxyls.cn

if let n = opt { print(n) }
来源：http://hr.szsharing.cn

[T20] Swift：数组操作
来源：http://xp.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xo.asd995.cn

[T21] Swift：遍历
来源：http://ua.jctech888.com.cn

for x in a { print(x) }
来源：http://pr.asd995.cn

[T22] Swift：字典
来源：http://nw.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nr.hnjuh.cn

[T23] Swift：函数
来源：http://le.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dq.haigaiapp.cn

[T24] Swift：闭包
来源：http://ma.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://as.bookmarksfly.cn

[T25] Swift：结构体
来源：http://kv.jianghongdianzi.cn

struct P { var x: Int }
来源：http://vm.haigaiapp.cn

[T26] Swift：类与重写
来源：http://oq.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://je.chemitech.net.cn

[T27] Swift：错误处理
来源：http://hm.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://pp.chemitech.net.cn

[T28] Swift：枚举
来源：http://dw.jianghongdianzi.cn

enum Color { case red, green }
来源：http://ua.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://ga.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://wm.huixiangedu.cn

[T30] Swift：协议
来源：http://gn.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://fh.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://gj.nicolike.cn

print("Hello")
来源：http://xe.shtwfgs.cn

[T32] Lua：局部变量
来源：http://ri.wgjwhj.cn

local a = 1
来源：http://vj.9csxet.cn

[T33] Lua：表（数组）
来源：http://cm.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yi.bjjhwx.cn

[T34] Lua：遍历表
来源：http://fz.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gt.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://na.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://mh.newstarts.cn

[T36] Lua：函数
来源：http://xo.shxzukj.cn

function add(a, b) return a + b end
来源：http://xy.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://ge.nicolike.cn

"a" .. "b"
来源：http://zs.asd995.cn

[T38] Lua：条件
来源：http://hu.hahajie.cn

if x > 0 then print("正") end
来源：http://fo.szsharing.cn

[T39] Lua：模式匹配
来源：http://od.szxytkj.cn

string.find(s, "%d+")
来源：http://ij.shtwfgs.cn

[T40] Lua：元表
来源：http://tx.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://kb.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://vc.haigaiapp.cn

print "Hello\n";
来源：http://gm.hahajie.cn

[T42] Perl：变量类型
来源：http://xt.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pb.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://wo.huixiangedu.cn

"值: $a"
来源：http://oy.gzmigu.cn

[T44] Perl：条件
来源：http://lr.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://eb.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://pn.asd995.cn

for my $x (@arr) { print $x; }
来源：http://vp.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://dz.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ug.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://db.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gu.newstarts.cn

[T48] Perl：正则替换
来源：http://rs.huanxung.cn

$s =~ s/old/new/g;
来源：http://co.haigaiapp.cn

[T49] Perl：函数
来源：http://ju.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dd.9csxet.cn

[T50] Perl：逐行读文件
来源：http://wp.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yw.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ys.lnxyls.cn

[T51] Scala：Hello World
来源：http://vx.jianghongdianzi.cn

println("Hello")
来源：http://yy.yuexingan06.cn

[T52] Scala：变量
来源：http://jh.huixiangedu.cn

val a = 1;  var b = 2
来源：http://ks.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://xr.yuexingan06.cn

s"值: $b"
来源：http://kh.9csxet.cn

[T54] Scala：集合映射
来源：http://kw.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://py.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://tp.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xw.nszjky.cn

[T56] Scala：样例类
来源：http://dh.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://ah.shxzskj.cn

[T57] Scala：模式匹配
来源：http://ma.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ub.muxihuayi.cn

[T58] Scala：函数定义
来源：http://ch.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bq.asd995.cn

[T59] Scala：循环
来源：http://xo.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://ym.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://rv.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ur.chemitech.net.cn

================================================================================
来源：http://bb.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ss.muxihuayi.cn

================================================================================
来源：http://ph.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://vh.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hk.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://od.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yb.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://dh.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://my.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://la.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dl.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://tp.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://tv.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://hq.bjjhwx.cn

{**a, **b}
来源：http://hj.szsharing.cn

[U07] Py：反转字典键值
来源：http://sj.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://tb.shxzukj.cn

[U08] Py：展平二维列表
来源：http://yf.muxihuayi.cn

[y for x in nested for y in x]
来源：http://zt.colortex.cn

[U09] Py：字典取最大值的键
来源：http://ue.nicolike.cn

max(d, key=d.get)
来源：http://yu.nicolike.cn

[U10] Py：按值排序字典
来源：http://wy.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zs.shxzskj.cn

[U11] Py：生成器表达式
来源：http://ca.shtwfgs.cn

(x * 2 for x in arr)
来源：http://xv.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wu.9csxet.cn

Counter(arr).most_common(3)
来源：http://kj.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ni.yuntaijiaju.cn

deque(maxlen=10)
来源：http://wf.huanxung.cn

[U14] Py：分组收集到列表
来源：http://sk.yuexingan06.cn

defaultdict(list)
来源：http://fr.9csxet.cn

[U15] Py：高精度计时
来源：http://wc.yuexingan06.cn

t = time.perf_counter()
来源：http://zy.asd995.cn

[U16] Py：命令行参数解析
来源：http://sq.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ud.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://wa.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://qg.nszjky.cn

[U18] Py：预编译正则
来源：http://vx.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://ci.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://xq.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vg.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://si.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://wr.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://it.chemitech.net.cn

@contextlib.contextmanager
来源：http://xd.nszjky.cn

[U22] Py：矩阵转置
来源：http://zs.yuntaijiaju.cn

list(zip(*m))
来源：http://lg.panjiajie.cn


<!-- 参考信息 -->