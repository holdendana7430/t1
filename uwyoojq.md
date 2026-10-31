代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://im.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://wj.bookmarksfly.cn

time ./run.sh
来源：http://yo.yuntaijiaju.cn

================================================================================
来源：http://sg.jctech888.com.cn

S. C / C++ 专题
来源：http://cc.bookmarksfly.cn

================================================================================
来源：http://kz.yuntaijiaju.cn

[S01] C：Hello World
来源：http://qc.newstarts.cn

#include <stdio.h>
来源：http://kl.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pa.colortex.cn

[S02] C：变量与格式化输出
来源：http://hc.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://rs.shxzukj.cn

[S03] C：读入整数
来源：http://ek.szxytkj.cn

int x; scanf("%d", &x);
来源：http://vk.bjjhwx.cn

[S04] C：字符串复制
来源：http://yy.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vn.panjiajie.cn

[S05] C：字符串长度
来源：http://oq.huixiangedu.cn

strlen(s)
来源：http://xg.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ke.colortex.cn

strcmp(a, b) == 0
来源：http://xa.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://rd.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ve.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://os.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bv.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://yy.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://br.panjiajie.cn

[S10] C：指针与解引用
来源：http://jf.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://ne.chemitech.net.cn

[S11] C：逐行读文件
来源：http://kb.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://kg.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mn.hahajie.cn

fclose(f);
来源：http://ls.jianghongdianzi.cn

[S12] C：写文件
来源：http://mo.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qz.bjjhwx.cn

[S13] C：宏定义
来源：http://zj.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dj.huixiangedu.cn

[S14] C：枚举
来源：http://jk.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ri.gzmigu.cn

[S15] C：类型转换
来源：http://ad.hnjuh.cn

(double) a / b
来源：http://pe.hahajie.cn

[S16] C：位操作置位
来源：http://kz.huixinmuqiang.cn

x |= (1 << 3);
来源：http://bu.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://fc.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ud.huixiangedu.cn

[S18] C：命令行参数
来源：http://ct.huanxung.cn

int main(int argc, char **argv)
来源：http://gh.yuexingan06.cn

[S19] C：快速排序
来源：http://sj.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gc.huanxung.cn

[S20] C：二分查找
来源：http://zz.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tq.asd995.cn

[S21] C：字符类别判断
来源：http://yg.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://he.521024.cn

[S22] C：字符串转数字
来源：http://ar.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://la.hahajie.cn

[S23] C：随机数
来源：http://ex.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mg.yuexingan06.cn

[S24] C：获取本地时间
来源：http://us.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ho.muxihuayi.cn

[S25] C：内存拷贝
来源：http://ys.hahajie.cn

memcpy(dst, src, n);
来源：http://te.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ai.colortex.cn

memset(a, 0, sizeof a);
来源：http://qk.huixinmuqiang.cn

[S27] C：定义常量
来源：http://tm.wgjwhj.cn

const double PI = 3.14159;
来源：http://wt.colortex.cn

[S28] C：静态变量
来源：http://bb.chemitech.net.cn

static int counter = 0;
来源：http://gf.hnjuh.cn

[S29] C：变参函数
来源：http://ca.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uz.bookmarksfly.cn

[S30] C：头文件保护
来源：http://wr.521024.cn

#ifndef X_H
来源：http://ok.muxihuayi.cn

#define X_H
来源：http://yn.gzmigu.cn

#endif
来源：http://th.szsharing.cn

[S31] C++：Hello World
来源：http://oz.szxytkj.cn

#include <iostream>
来源：http://am.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://kr.nszjky.cn

[S32] C++：字符串
来源：http://nv.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://bo.nszjky.cn

[S33] C++：vector 增删
来源：http://gl.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tn.panjiajie.cn

[S34] C++：遍历 vector
来源：http://ii.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ag.shxzukj.cn

[S35] C++：map
来源：http://jc.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zf.shtwfgs.cn

[S36] C++：unordered_map
来源：http://ut.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uz.chemitech.net.cn

[S37] C++：set
来源：http://pz.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qz.huanxung.cn

[S38] C++：排序
来源：http://ej.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://cb.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://it.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yf.huixiangedu.cn

[S40] C++：查找元素
来源：http://mf.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cg.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://dv.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cg.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://sf.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://zs.haigaiapp.cn

[S43] C++：智能指针
来源：http://ie.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://mc.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://ob.asd995.cn

void inc(int &x) { ++x; }
来源：http://xw.huixiangedu.cn

[S45] C++：lambda
来源：http://jl.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://km.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://yo.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rj.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://aj.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jj.szxytkj.cn

[S48] C++：逐行读文件
来源：http://ie.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qv.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://yc.haigaiapp.cn

[S49] C++：写文件
来源：http://cx.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dz.huanxung.cn

[S50] C++：格式化数字
来源：http://px.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pt.shxzukj.cn

[S51] C++：显式类型转换
来源：http://up.yuexingan06.cn

static_cast<double>(a) / b
来源：http://vq.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://aa.9csxet.cn

int size() const noexcept { return n_; }
来源：http://jx.huixiangedu.cn

[S53] C++：移动语义
来源：http://dc.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://ug.wgjwhj.cn

[S54] C++：异常处理
来源：http://zg.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wq.gzmigu.cn

[S55] C++：结构化绑定
来源：http://nm.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pk.yuexingan06.cn

[S56] C++：optional
来源：http://ye.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xg.panjiajie.cn

[S57] C++：编译期常量
来源：http://ll.panjiajie.cn

constexpr int N = 10;
来源：http://xu.asd995.cn

[S58] C++：命名空间
来源：http://uu.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://kv.jctech888.com.cn

[S59] C++：静态断言
来源：http://uh.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://il.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://kt.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wi.shxzskj.cn

================================================================================
来源：http://ud.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mo.panjiajie.cn

================================================================================
来源：http://er.nicolike.cn

[T01] Kotlin：Hello World
来源：http://yg.521024.cn

println("Hello")
来源：http://kf.wgjwhj.cn

[T02] Kotlin：变量
来源：http://cj.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sl.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://rw.chemitech.net.cn

"值: $b"
来源：http://hw.colortex.cn

[T04] Kotlin：空安全
来源：http://il.nicolike.cn

val n: String? = null;  n?.length
来源：http://ne.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://vn.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qx.521024.cn

[T06] Kotlin：集合映射
来源：http://xo.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sn.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://yp.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zo.nszjky.cn

[T08] Kotlin：数据类
来源：http://gj.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://hm.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://ce.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://pf.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://mg.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qg.asd995.cn

[T11] Kotlin：协程
来源：http://pd.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uo.szsharing.cn

[T12] Kotlin：解构声明
来源：http://yt.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://tw.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://as.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://tz.shxzskj.cn

[T14] Kotlin：循环
来源：http://bp.huanxung.cn

for (i in 1..10) println(i)
来源：http://kt.panjiajie.cn

[T15] Kotlin：接口
来源：http://md.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://ij.haigaiapp.cn

[T16] Swift：Hello World
来源：http://hd.9csxet.cn

print("Hello")
来源：http://uu.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://sf.szxytkj.cn

var a = 1;  let b = 2
来源：http://fd.colortex.cn

[T18] Swift：字符串插值
来源：http://yh.chemitech.net.cn

"值: \(b)"
来源：http://os.gzmigu.cn

[T19] Swift：可选绑定
来源：http://ry.nicolike.cn

if let n = opt { print(n) }
来源：http://js.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://ma.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ma.nicolike.cn

[T21] Swift：遍历
来源：http://fh.shxzskj.cn

for x in a { print(x) }
来源：http://iq.hnjuh.cn

[T22] Swift：字典
来源：http://ld.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://au.yuntaijiaju.cn

[T23] Swift：函数
来源：http://xa.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qe.huixiangedu.cn

[T24] Swift：闭包
来源：http://qv.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ch.shxzskj.cn

[T25] Swift：结构体
来源：http://pq.gzmigu.cn

struct P { var x: Int }
来源：http://jf.bjjhwx.cn

[T26] Swift：类与重写
来源：http://gd.szsharing.cn

class A: Base { override func f() {} }
来源：http://ht.huanxung.cn

[T27] Swift：错误处理
来源：http://ax.newstarts.cn

do { try f() } catch { print(error) }
来源：http://it.muxihuayi.cn

[T28] Swift：枚举
来源：http://vx.muxihuayi.cn

enum Color { case red, green }
来源：http://km.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://xf.bookmarksfly.cn

guard let x = opt else { return }
来源：http://xc.huixinmuqiang.cn

[T30] Swift：协议
来源：http://le.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://qo.jctech888.com.cn

[T31] Lua：Hello World
来源：http://sl.jctech888.com.cn

print("Hello")
来源：http://ac.9csxet.cn

[T32] Lua：局部变量
来源：http://wh.jctech888.com.cn

local a = 1
来源：http://nb.szsharing.cn

[T33] Lua：表（数组）
来源：http://pu.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ml.colortex.cn

[T34] Lua：遍历表
来源：http://gx.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bq.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://rl.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://uh.shtwfgs.cn

[T36] Lua：函数
来源：http://ov.shxzukj.cn

function add(a, b) return a + b end
来源：http://yx.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://nx.muxihuayi.cn

"a" .. "b"
来源：http://yw.szxytkj.cn

[T38] Lua：条件
来源：http://vm.9csxet.cn

if x > 0 then print("正") end
来源：http://hv.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://kh.shxzukj.cn

string.find(s, "%d+")
来源：http://sc.shxzukj.cn

[T40] Lua：元表
来源：http://wa.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://po.bjjhwx.cn

[T41] Perl：Hello World
来源：http://pq.nszjky.cn

print "Hello\n";
来源：http://wi.hahajie.cn

[T42] Perl：变量类型
来源：http://ne.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bq.521024.cn

[T43] Perl：字符串插值
来源：http://fm.panjiajie.cn

"值: $a"
来源：http://np.huixinmuqiang.cn

[T44] Perl：条件
来源：http://bs.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://aq.asd995.cn

[T45] Perl：数组遍历
来源：http://yf.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://he.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://pw.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gp.lnxyls.cn

[T47] Perl：正则捕获
来源：http://vd.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nd.yuexingan06.cn

[T48] Perl：正则替换
来源：http://kg.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://fa.521024.cn

[T49] Perl：函数
来源：http://jl.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://va.newstarts.cn

[T50] Perl：逐行读文件
来源：http://ho.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ut.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://jj.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://qy.nicolike.cn

println("Hello")
来源：http://lg.szxytkj.cn

[T52] Scala：变量
来源：http://ud.shxzukj.cn

val a = 1;  var b = 2
来源：http://ky.521024.cn

[T53] Scala：字符串插值
来源：http://ga.hahajie.cn

s"值: $b"
来源：http://bx.huixiangedu.cn

[T54] Scala：集合映射
来源：http://rw.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://zd.nicolike.cn

[T55] Scala：集合过滤
来源：http://ib.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kq.9csxet.cn

[T56] Scala：样例类
来源：http://me.newstarts.cn

case class User(name: String, age: Int)
来源：http://zg.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://rp.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wi.huanxung.cn

[T58] Scala：函数定义
来源：http://zz.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iu.muxihuayi.cn

[T59] Scala：循环
来源：http://vs.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://gz.jctech888.com.cn

[T60] Scala：折叠
来源：http://ow.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ab.bookmarksfly.cn

================================================================================
来源：http://op.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gy.colortex.cn

================================================================================
来源：http://se.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://ka.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://js.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://st.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xf.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://fj.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pe.hahajie.cn

[U04] Py：变量调试打印
来源：http://mu.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jg.asd995.cn

[U05] Py：列表去重且保序
来源：http://ed.newstarts.cn

list(dict.fromkeys(arr))
来源：http://uo.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://lv.newstarts.cn

{**a, **b}
来源：http://vv.shxzukj.cn

[U07] Py：反转字典键值
来源：http://la.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://ky.lnxyls.cn

[U08] Py：展平二维列表
来源：http://cb.shtwfgs.cn

[y for x in nested for y in x]
来源：http://cy.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://wm.shxzskj.cn

max(d, key=d.get)
来源：http://cy.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://ah.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pp.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://td.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://bx.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vj.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://lt.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://ew.nicolike.cn

deque(maxlen=10)
来源：http://qd.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://yt.huixiangedu.cn

defaultdict(list)
来源：http://pn.jctech888.com.cn

[U15] Py：高精度计时
来源：http://jf.panjiajie.cn

t = time.perf_counter()
来源：http://ew.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://td.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ms.wgjwhj.cn

[U17] Py：初始化日志
来源：http://en.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://ur.lnxyls.cn

[U18] Py：预编译正则
来源：http://pw.nszjky.cn

pat = re.compile(r"\d+")
来源：http://gk.newstarts.cn

[U19] Py：正则替换带回调
来源：http://tj.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ey.newstarts.cn

[U20] Py：缓存函数结果
来源：http://uv.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ni.lnxyls.cn


<!-- 参考信息 -->