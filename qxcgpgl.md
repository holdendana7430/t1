代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://np.asd995.cn

[R80] 查看脚本执行耗时
来源：http://oy.nicolike.cn

time ./run.sh
来源：http://cn.shxzukj.cn

================================================================================
来源：http://ut.yuntaijiaju.cn

S. C / C++ 专题
来源：http://tj.panjiajie.cn

================================================================================
来源：http://oz.hnjuh.cn

[S01] C：Hello World
来源：http://gq.yuntaijiaju.cn

#include <stdio.h>
来源：http://xx.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wk.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://ru.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://tg.shtwfgs.cn

[S03] C：读入整数
来源：http://ed.newstarts.cn

int x; scanf("%d", &x);
来源：http://ar.nicolike.cn

[S04] C：字符串复制
来源：http://wz.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fj.bookmarksfly.cn

[S05] C：字符串长度
来源：http://zg.huixiangedu.cn

strlen(s)
来源：http://le.colortex.cn

[S06] C：字符串比较
来源：http://da.muxihuayi.cn

strcmp(a, b) == 0
来源：http://mw.asd995.cn

[S07] C：数组遍历求和
来源：http://gz.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://np.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://dq.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hm.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://dt.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nj.panjiajie.cn

[S10] C：指针与解引用
来源：http://tv.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://bx.bjjhwx.cn

[S11] C：逐行读文件
来源：http://lr.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://tw.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yo.newstarts.cn

fclose(f);
来源：http://nz.yuexingan06.cn

[S12] C：写文件
来源：http://cm.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yl.lnxyls.cn

[S13] C：宏定义
来源：http://sy.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://um.jctech888.com.cn

[S14] C：枚举
来源：http://ll.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://jr.shtwfgs.cn

[S15] C：类型转换
来源：http://mo.bjjhwx.cn

(double) a / b
来源：http://qz.yuexingan06.cn

[S16] C：位操作置位
来源：http://hy.shxzukj.cn

x |= (1 << 3);
来源：http://vy.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ow.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hv.nicolike.cn

[S18] C：命令行参数
来源：http://vy.hnjuh.cn

int main(int argc, char **argv)
来源：http://ba.asd995.cn

[S19] C：快速排序
来源：http://zu.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pr.newstarts.cn

[S20] C：二分查找
来源：http://ve.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uk.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://zn.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bk.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://el.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ix.hnjuh.cn

[S23] C：随机数
来源：http://vv.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://th.huixiangedu.cn

[S24] C：获取本地时间
来源：http://fr.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ej.newstarts.cn

[S25] C：内存拷贝
来源：http://ii.yuexingan06.cn

memcpy(dst, src, n);
来源：http://gu.bjjhwx.cn

[S26] C：内存清零
来源：http://ac.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://nk.shxzukj.cn

[S27] C：定义常量
来源：http://bf.bookmarksfly.cn

const double PI = 3.14159;
来源：http://sj.521024.cn

[S28] C：静态变量
来源：http://cv.lnxyls.cn

static int counter = 0;
来源：http://tv.szsharing.cn

[S29] C：变参函数
来源：http://fr.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pp.lnxyls.cn

[S30] C：头文件保护
来源：http://kt.colortex.cn

#ifndef X_H
来源：http://hp.hnjuh.cn

#define X_H
来源：http://on.huixinmuqiang.cn

#endif
来源：http://iz.shtwfgs.cn

[S31] C++：Hello World
来源：http://pg.jctech888.com.cn

#include <iostream>
来源：http://zc.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://il.huanxung.cn

[S32] C++：字符串
来源：http://zi.colortex.cn

std::string s = "hi";  s += "!";
来源：http://cd.muxihuayi.cn

[S33] C++：vector 增删
来源：http://un.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jk.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://mc.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://xp.colortex.cn

[S35] C++：map
来源：http://qa.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xu.gzmigu.cn

[S36] C++：unordered_map
来源：http://tx.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wp.muxihuayi.cn

[S37] C++：set
来源：http://ad.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nf.wgjwhj.cn

[S38] C++：排序
来源：http://zf.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://vu.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://ts.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tv.hnjuh.cn

[S40] C++：查找元素
来源：http://bw.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jj.colortex.cn

[S41] C++：类与构造函数
来源：http://ge.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yp.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://ep.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ze.panjiajie.cn

[S43] C++：智能指针
来源：http://we.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://wb.szxytkj.cn

[S44] C++：引用传参
来源：http://ab.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://hd.jctech888.com.cn

[S45] C++：lambda
来源：http://ko.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ti.szsharing.cn

[S46] C++：函数模板
来源：http://mk.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://va.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://sa.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sx.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://he.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rk.nszjky.cn

while (std::getline(in, line)) { }
来源：http://ho.haigaiapp.cn

[S49] C++：写文件
来源：http://du.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fe.gzmigu.cn

[S50] C++：格式化数字
来源：http://za.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jj.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://sw.shxzukj.cn

static_cast<double>(a) / b
来源：http://bi.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://qc.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ch.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://lo.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://gb.521024.cn

[S54] C++：异常处理
来源：http://ew.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gw.newstarts.cn

[S55] C++：结构化绑定
来源：http://so.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mp.newstarts.cn

[S56] C++：optional
来源：http://vc.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vi.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ue.colortex.cn

constexpr int N = 10;
来源：http://il.shtwfgs.cn

[S58] C++：命名空间
来源：http://pz.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://os.wgjwhj.cn

[S59] C++：静态断言
来源：http://ss.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pr.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://og.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pt.yuntaijiaju.cn

================================================================================
来源：http://qd.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ok.yuexingan06.cn

================================================================================
来源：http://zj.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://aw.lnxyls.cn

println("Hello")
来源：http://js.haigaiapp.cn

[T02] Kotlin：变量
来源：http://hi.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gv.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://rs.muxihuayi.cn

"值: $b"
来源：http://uq.521024.cn

[T04] Kotlin：空安全
来源：http://to.nicolike.cn

val n: String? = null;  n?.length
来源：http://vr.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://ql.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fv.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ip.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://im.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://ej.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wo.gzmigu.cn

[T08] Kotlin：数据类
来源：http://gc.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://uj.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://jj.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ca.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://rd.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jp.huanxung.cn

[T11] Kotlin：协程
来源：http://jp.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aw.hahajie.cn

[T12] Kotlin：解构声明
来源：http://oj.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://aa.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://of.szsharing.cn

val m = mapOf("a" to 1)
来源：http://gz.shtwfgs.cn

[T14] Kotlin：循环
来源：http://uy.shxzskj.cn

for (i in 1..10) println(i)
来源：http://pk.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://qg.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://xu.haigaiapp.cn

[T16] Swift：Hello World
来源：http://hj.gzmigu.cn

print("Hello")
来源：http://wi.hnjuh.cn

[T17] Swift：变量与常量
来源：http://ah.bjjhwx.cn

var a = 1;  let b = 2
来源：http://cr.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://nv.shxzukj.cn

"值: \(b)"
来源：http://qv.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://xs.chemitech.net.cn

if let n = opt { print(n) }
来源：http://oy.hnjuh.cn

[T20] Swift：数组操作
来源：http://vu.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wr.yuexingan06.cn

[T21] Swift：遍历
来源：http://et.huanxung.cn

for x in a { print(x) }
来源：http://fi.huixiangedu.cn

[T22] Swift：字典
来源：http://rj.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dw.jianghongdianzi.cn

[T23] Swift：函数
来源：http://wq.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bq.bookmarksfly.cn

[T24] Swift：闭包
来源：http://ea.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ki.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://bk.asd995.cn

struct P { var x: Int }
来源：http://po.huanxung.cn

[T26] Swift：类与重写
来源：http://wp.panjiajie.cn

class A: Base { override func f() {} }
来源：http://rx.bjjhwx.cn

[T27] Swift：错误处理
来源：http://sv.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://wa.lnxyls.cn

[T28] Swift：枚举
来源：http://vw.bjjhwx.cn

enum Color { case red, green }
来源：http://zc.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://mq.huanxung.cn

guard let x = opt else { return }
来源：http://ph.colortex.cn

[T30] Swift：协议
来源：http://lb.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://ki.9csxet.cn

[T31] Lua：Hello World
来源：http://vg.chemitech.net.cn

print("Hello")
来源：http://jz.colortex.cn

[T32] Lua：局部变量
来源：http://su.hahajie.cn

local a = 1
来源：http://mc.newstarts.cn

[T33] Lua：表（数组）
来源：http://jf.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zp.shxzskj.cn

[T34] Lua：遍历表
来源：http://pu.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ys.chemitech.net.cn

[T35] Lua：字典表
来源：http://kq.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://tz.wgjwhj.cn

[T36] Lua：函数
来源：http://ej.szsharing.cn

function add(a, b) return a + b end
来源：http://cz.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://ds.lnxyls.cn

"a" .. "b"
来源：http://uz.yuntaijiaju.cn

[T38] Lua：条件
来源：http://cb.shxzskj.cn

if x > 0 then print("正") end
来源：http://jn.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://nr.newstarts.cn

string.find(s, "%d+")
来源：http://ka.gzmigu.cn

[T40] Lua：元表
来源：http://on.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://mw.haigaiapp.cn

[T41] Perl：Hello World
来源：http://gi.newstarts.cn

print "Hello\n";
来源：http://zw.shtwfgs.cn

[T42] Perl：变量类型
来源：http://ph.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://za.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://tv.521024.cn

"值: $a"
来源：http://bp.chemitech.net.cn

[T44] Perl：条件
来源：http://ff.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://vt.szsharing.cn

[T45] Perl：数组遍历
来源：http://do.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://zh.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://jy.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mx.asd995.cn

[T47] Perl：正则捕获
来源：http://uu.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ey.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://hz.hnjuh.cn

$s =~ s/old/new/g;
来源：http://nf.gzmigu.cn

[T49] Perl：函数
来源：http://td.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vy.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://fi.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jp.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://qv.colortex.cn

[T51] Scala：Hello World
来源：http://zz.panjiajie.cn

println("Hello")
来源：http://zq.haigaiapp.cn

[T52] Scala：变量
来源：http://rc.gzmigu.cn

val a = 1;  var b = 2
来源：http://nx.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://pn.yuexingan06.cn

s"值: $b"
来源：http://iz.gzmigu.cn

[T54] Scala：集合映射
来源：http://wx.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://sl.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://ud.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ju.shxzskj.cn

[T56] Scala：样例类
来源：http://px.szsharing.cn

case class User(name: String, age: Int)
来源：http://vk.nszjky.cn

[T57] Scala：模式匹配
来源：http://og.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oi.9csxet.cn

[T58] Scala：函数定义
来源：http://dl.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gd.jctech888.com.cn

[T59] Scala：循环
来源：http://cz.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://tk.hahajie.cn

[T60] Scala：折叠
来源：http://sh.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://om.haigaiapp.cn

================================================================================
来源：http://eq.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zd.szsharing.cn

================================================================================
来源：http://it.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://kr.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://su.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://mu.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ce.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://pt.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pw.nicolike.cn

[U04] Py：变量调试打印
来源：http://is.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qi.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://md.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://cj.nszjky.cn

[U06] Py：合并两个字典
来源：http://tu.gzmigu.cn

{**a, **b}
来源：http://re.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://rk.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://os.nicolike.cn

[U08] Py：展平二维列表
来源：http://ex.szxytkj.cn

[y for x in nested for y in x]
来源：http://al.asd995.cn

[U09] Py：字典取最大值的键
来源：http://gg.521024.cn

max(d, key=d.get)
来源：http://cr.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://mn.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pi.9csxet.cn

[U11] Py：生成器表达式
来源：http://gq.bjjhwx.cn

(x * 2 for x in arr)
来源：http://iu.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rb.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://bk.newstarts.cn

[U13] Py：固定长度队列
来源：http://qz.shxzukj.cn

deque(maxlen=10)
来源：http://xk.9csxet.cn

[U14] Py：分组收集到列表
来源：http://mf.panjiajie.cn

defaultdict(list)
来源：http://ke.chemitech.net.cn

[U15] Py：高精度计时
来源：http://ef.yuntaijiaju.cn

t = time.perf_counter()
来源：http://my.nszjky.cn

[U16] Py：命令行参数解析
来源：http://yo.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hr.haigaiapp.cn

[U17] Py：初始化日志
来源：http://oi.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://bu.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://qm.hahajie.cn

pat = re.compile(r"\d+")
来源：http://ca.9csxet.cn

[U19] Py：正则替换带回调
来源：http://im.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oj.szsharing.cn

[U20] Py：缓存函数结果
来源：http://ta.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://hr.gzmigu.cn


<!-- 参考信息 -->