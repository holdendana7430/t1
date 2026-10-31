代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hw.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://fe.9csxet.cn

time ./run.sh
来源：http://zz.yuexingan06.cn

================================================================================
来源：http://lc.hnjuh.cn

S. C / C++ 专题
来源：http://cr.szxytkj.cn

================================================================================
来源：http://xz.szxytkj.cn

[S01] C：Hello World
来源：http://os.panjiajie.cn

#include <stdio.h>
来源：http://gg.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jy.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://fg.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://lm.huixiangedu.cn

[S03] C：读入整数
来源：http://ja.newstarts.cn

int x; scanf("%d", &x);
来源：http://gi.huanxung.cn

[S04] C：字符串复制
来源：http://qv.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dy.9csxet.cn

[S05] C：字符串长度
来源：http://vu.haigaiapp.cn

strlen(s)
来源：http://au.huanxung.cn

[S06] C：字符串比较
来源：http://oe.lnxyls.cn

strcmp(a, b) == 0
来源：http://ln.nicolike.cn

[S07] C：数组遍历求和
来源：http://in.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dt.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://dz.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ed.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://px.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://al.szsharing.cn

[S10] C：指针与解引用
来源：http://lw.521024.cn

int *p = &a;  *p = 5;
来源：http://bz.9csxet.cn

[S11] C：逐行读文件
来源：http://al.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://tm.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ba.asd995.cn

fclose(f);
来源：http://ua.yuntaijiaju.cn

[S12] C：写文件
来源：http://zk.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ry.nszjky.cn

[S13] C：宏定义
来源：http://vu.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cy.asd995.cn

[S14] C：枚举
来源：http://zf.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://fn.9csxet.cn

[S15] C：类型转换
来源：http://vi.newstarts.cn

(double) a / b
来源：http://qx.nicolike.cn

[S16] C：位操作置位
来源：http://mg.shtwfgs.cn

x |= (1 << 3);
来源：http://yz.9csxet.cn

[S17] C：安全拼接字符串
来源：http://mp.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hd.huanxung.cn

[S18] C：命令行参数
来源：http://lt.panjiajie.cn

int main(int argc, char **argv)
来源：http://nr.yuntaijiaju.cn

[S19] C：快速排序
来源：http://gl.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mu.yuntaijiaju.cn

[S20] C：二分查找
来源：http://ef.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ac.newstarts.cn

[S21] C：字符类别判断
来源：http://pq.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ze.hahajie.cn

[S22] C：字符串转数字
来源：http://da.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oy.jianghongdianzi.cn

[S23] C：随机数
来源：http://xn.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rw.shtwfgs.cn

[S24] C：获取本地时间
来源：http://mm.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ov.521024.cn

[S25] C：内存拷贝
来源：http://ap.9csxet.cn

memcpy(dst, src, n);
来源：http://ns.jianghongdianzi.cn

[S26] C：内存清零
来源：http://mq.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://wl.yuntaijiaju.cn

[S27] C：定义常量
来源：http://ab.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://xx.colortex.cn

[S28] C：静态变量
来源：http://hi.chemitech.net.cn

static int counter = 0;
来源：http://et.huixinmuqiang.cn

[S29] C：变参函数
来源：http://tz.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gk.hahajie.cn

[S30] C：头文件保护
来源：http://hf.haigaiapp.cn

#ifndef X_H
来源：http://bj.newstarts.cn

#define X_H
来源：http://rz.nicolike.cn

#endif
来源：http://ya.hahajie.cn

[S31] C++：Hello World
来源：http://sx.huixinmuqiang.cn

#include <iostream>
来源：http://ln.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://iu.wgjwhj.cn

[S32] C++：字符串
来源：http://ig.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://ya.muxihuayi.cn

[S33] C++：vector 增删
来源：http://zf.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fq.nszjky.cn

[S34] C++：遍历 vector
来源：http://sj.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://mg.chemitech.net.cn

[S35] C++：map
来源：http://dy.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ku.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://fu.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ex.lnxyls.cn

[S37] C++：set
来源：http://nr.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fi.newstarts.cn

[S38] C++：排序
来源：http://sr.521024.cn

std::sort(v.begin(), v.end());
来源：http://ve.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://dt.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ff.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://qv.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dt.hnjuh.cn

[S41] C++：类与构造函数
来源：http://ne.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ek.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://jx.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://bm.wgjwhj.cn

[S43] C++：智能指针
来源：http://uw.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://zp.haigaiapp.cn

[S44] C++：引用传参
来源：http://po.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://bp.szsharing.cn

[S45] C++：lambda
来源：http://pu.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ve.huanxung.cn

[S46] C++：函数模板
来源：http://pa.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jh.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://uq.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mh.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://zf.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gr.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://hd.shxzskj.cn

[S49] C++：写文件
来源：http://eu.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kn.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ni.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uc.newstarts.cn

[S51] C++：显式类型转换
来源：http://kj.chemitech.net.cn

static_cast<double>(a) / b
来源：http://qd.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://lx.521024.cn

int size() const noexcept { return n_; }
来源：http://nn.shxzukj.cn

[S53] C++：移动语义
来源：http://cg.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://qr.hahajie.cn

[S54] C++：异常处理
来源：http://aa.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wu.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://fc.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jr.newstarts.cn

[S56] C++：optional
来源：http://jc.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jj.wgjwhj.cn

[S57] C++：编译期常量
来源：http://rk.muxihuayi.cn

constexpr int N = 10;
来源：http://ro.newstarts.cn

[S58] C++：命名空间
来源：http://cz.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://kh.wgjwhj.cn

[S59] C++：静态断言
来源：http://gp.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dp.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://mo.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zp.521024.cn

================================================================================
来源：http://cc.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ns.colortex.cn

================================================================================
来源：http://mp.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://le.9csxet.cn

println("Hello")
来源：http://ps.gzmigu.cn

[T02] Kotlin：变量
来源：http://gd.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cg.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://ed.jianghongdianzi.cn

"值: $b"
来源：http://lq.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://bg.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://pj.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://zd.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zw.521024.cn

[T06] Kotlin：集合映射
来源：http://dd.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qe.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://mo.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ey.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://ak.colortex.cn

data class User(val name: String, val age: Int)
来源：http://ln.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://fz.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://dz.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://de.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mh.chemitech.net.cn

[T11] Kotlin：协程
来源：http://sq.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pb.hahajie.cn

[T12] Kotlin：解构声明
来源：http://wt.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://ji.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://gi.newstarts.cn

val m = mapOf("a" to 1)
来源：http://hk.newstarts.cn

[T14] Kotlin：循环
来源：http://lg.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://sy.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://hb.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://zs.hnjuh.cn

[T16] Swift：Hello World
来源：http://jq.gzmigu.cn

print("Hello")
来源：http://lk.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://wj.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://nv.newstarts.cn

[T18] Swift：字符串插值
来源：http://bk.huixinmuqiang.cn

"值: \(b)"
来源：http://mh.521024.cn

[T19] Swift：可选绑定
来源：http://nj.szsharing.cn

if let n = opt { print(n) }
来源：http://sb.huanxung.cn

[T20] Swift：数组操作
来源：http://ar.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jp.haigaiapp.cn

[T21] Swift：遍历
来源：http://vq.haigaiapp.cn

for x in a { print(x) }
来源：http://yp.yuntaijiaju.cn

[T22] Swift：字典
来源：http://my.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yw.asd995.cn

[T23] Swift：函数
来源：http://de.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cx.bjjhwx.cn

[T24] Swift：闭包
来源：http://wl.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fb.huixiangedu.cn

[T25] Swift：结构体
来源：http://qj.szxytkj.cn

struct P { var x: Int }
来源：http://ux.bjjhwx.cn

[T26] Swift：类与重写
来源：http://eo.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://wi.colortex.cn

[T27] Swift：错误处理
来源：http://zt.hahajie.cn

do { try f() } catch { print(error) }
来源：http://cq.szxytkj.cn

[T28] Swift：枚举
来源：http://yz.yuntaijiaju.cn

enum Color { case red, green }
来源：http://le.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://oc.yuexingan06.cn

guard let x = opt else { return }
来源：http://tw.nicolike.cn

[T30] Swift：协议
来源：http://ol.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://qi.shxzskj.cn

[T31] Lua：Hello World
来源：http://rx.jctech888.com.cn

print("Hello")
来源：http://sr.bjjhwx.cn

[T32] Lua：局部变量
来源：http://ed.huanxung.cn

local a = 1
来源：http://lg.nszjky.cn

[T33] Lua：表（数组）
来源：http://ky.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oe.asd995.cn

[T34] Lua：遍历表
来源：http://gw.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lv.bookmarksfly.cn

[T35] Lua：字典表
来源：http://gs.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://gc.szsharing.cn

[T36] Lua：函数
来源：http://pm.lnxyls.cn

function add(a, b) return a + b end
来源：http://eb.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://jd.huixinmuqiang.cn

"a" .. "b"
来源：http://bu.wgjwhj.cn

[T38] Lua：条件
来源：http://gs.szsharing.cn

if x > 0 then print("正") end
来源：http://gp.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://lt.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://cg.gzmigu.cn

[T40] Lua：元表
来源：http://tf.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://ak.newstarts.cn

[T41] Perl：Hello World
来源：http://fw.nszjky.cn

print "Hello\n";
来源：http://qo.huanxung.cn

[T42] Perl：变量类型
来源：http://yg.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ek.lnxyls.cn

[T43] Perl：字符串插值
来源：http://mf.hnjuh.cn

"值: $a"
来源：http://hg.huixinmuqiang.cn

[T44] Perl：条件
来源：http://cg.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://lj.newstarts.cn

[T45] Perl：数组遍历
来源：http://fk.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://yb.szxytkj.cn

[T46] Perl：哈希操作
来源：http://bj.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iy.shxzskj.cn

[T47] Perl：正则捕获
来源：http://ey.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jq.szsharing.cn

[T48] Perl：正则替换
来源：http://ps.9csxet.cn

$s =~ s/old/new/g;
来源：http://wa.newstarts.cn

[T49] Perl：函数
来源：http://cs.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qn.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://cc.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vg.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://on.newstarts.cn

[T51] Scala：Hello World
来源：http://ed.nszjky.cn

println("Hello")
来源：http://jk.gzmigu.cn

[T52] Scala：变量
来源：http://tc.muxihuayi.cn

val a = 1;  var b = 2
来源：http://tx.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://at.gzmigu.cn

s"值: $b"
来源：http://ag.szxytkj.cn

[T54] Scala：集合映射
来源：http://de.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://pg.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://pu.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dz.bjjhwx.cn

[T56] Scala：样例类
来源：http://pr.panjiajie.cn

case class User(name: String, age: Int)
来源：http://tr.asd995.cn

[T57] Scala：模式匹配
来源：http://fs.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://is.shtwfgs.cn

[T58] Scala：函数定义
来源：http://ob.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bw.colortex.cn

[T59] Scala：循环
来源：http://qw.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://el.9csxet.cn

[T60] Scala：折叠
来源：http://qq.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://in.jianghongdianzi.cn

================================================================================
来源：http://hl.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gj.chemitech.net.cn

================================================================================
来源：http://aj.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ti.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://de.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://sn.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://be.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://ws.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vj.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://zv.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uw.colortex.cn

[U05] Py：列表去重且保序
来源：http://tz.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://du.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://ls.nszjky.cn

{**a, **b}
来源：http://fz.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://zi.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://li.shxzskj.cn

[U08] Py：展平二维列表
来源：http://au.asd995.cn

[y for x in nested for y in x]
来源：http://ia.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://fd.shtwfgs.cn

max(d, key=d.get)
来源：http://hm.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://md.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qm.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ym.huixiangedu.cn

(x * 2 for x in arr)
来源：http://zp.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sq.panjiajie.cn

Counter(arr).most_common(3)
来源：http://kc.nicolike.cn

[U13] Py：固定长度队列
来源：http://pr.szxytkj.cn

deque(maxlen=10)
来源：http://mp.newstarts.cn

[U14] Py：分组收集到列表
来源：http://yk.huanxung.cn

defaultdict(list)
来源：http://ar.shtwfgs.cn

[U15] Py：高精度计时
来源：http://wo.huixiangedu.cn

t = time.perf_counter()
来源：http://og.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://we.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yz.shxzskj.cn

[U17] Py：初始化日志
来源：http://qp.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://tc.asd995.cn

[U18] Py：预编译正则
来源：http://gf.huanxung.cn

pat = re.compile(r"\d+")
来源：http://jh.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://dv.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nt.huanxung.cn

[U20] Py：缓存函数结果
来源：http://kc.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://st.wgjwhj.cn


<!-- 参考信息 -->