代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://af.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://oc.asd995.cn

time ./run.sh
来源：http://qs.huixiangedu.cn

================================================================================
来源：http://wr.9csxet.cn

S. C / C++ 专题
来源：http://qi.panjiajie.cn

================================================================================
来源：http://ka.szxytkj.cn

[S01] C：Hello World
来源：http://tl.panjiajie.cn

#include <stdio.h>
来源：http://sk.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uk.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://kh.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://qn.lnxyls.cn

[S03] C：读入整数
来源：http://qi.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ld.hnjuh.cn

[S04] C：字符串复制
来源：http://cc.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ui.huixiangedu.cn

[S05] C：字符串长度
来源：http://ff.shtwfgs.cn

strlen(s)
来源：http://xh.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://fy.hnjuh.cn

strcmp(a, b) == 0
来源：http://wg.panjiajie.cn

[S07] C：数组遍历求和
来源：http://ml.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ux.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://xv.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ke.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://kc.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rf.lnxyls.cn

[S10] C：指针与解引用
来源：http://dd.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://sd.szsharing.cn

[S11] C：逐行读文件
来源：http://dr.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://uv.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sx.huixiangedu.cn

fclose(f);
来源：http://vq.lnxyls.cn

[S12] C：写文件
来源：http://bf.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://io.jctech888.com.cn

[S13] C：宏定义
来源：http://zz.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ze.nicolike.cn

[S14] C：枚举
来源：http://fu.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://od.huanxung.cn

[S15] C：类型转换
来源：http://gk.asd995.cn

(double) a / b
来源：http://dt.shxzskj.cn

[S16] C：位操作置位
来源：http://bz.hahajie.cn

x |= (1 << 3);
来源：http://oz.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://nu.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iy.9csxet.cn

[S18] C：命令行参数
来源：http://ss.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://dj.9csxet.cn

[S19] C：快速排序
来源：http://vm.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zw.wgjwhj.cn

[S20] C：二分查找
来源：http://vb.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ry.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://er.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ey.shxzskj.cn

[S22] C：字符串转数字
来源：http://hd.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ef.asd995.cn

[S23] C：随机数
来源：http://uk.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ov.9csxet.cn

[S24] C：获取本地时间
来源：http://zt.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jh.huixiangedu.cn

[S25] C：内存拷贝
来源：http://fy.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ni.521024.cn

[S26] C：内存清零
来源：http://yp.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://ki.szsharing.cn

[S27] C：定义常量
来源：http://vo.hahajie.cn

const double PI = 3.14159;
来源：http://bk.wgjwhj.cn

[S28] C：静态变量
来源：http://mn.shtwfgs.cn

static int counter = 0;
来源：http://hn.jianghongdianzi.cn

[S29] C：变参函数
来源：http://ry.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bs.szxytkj.cn

[S30] C：头文件保护
来源：http://bs.bjjhwx.cn

#ifndef X_H
来源：http://ca.shtwfgs.cn

#define X_H
来源：http://va.bjjhwx.cn

#endif
来源：http://es.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://tj.szsharing.cn

#include <iostream>
来源：http://hm.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://yj.hahajie.cn

[S32] C++：字符串
来源：http://jn.asd995.cn

std::string s = "hi";  s += "!";
来源：http://pm.shxzskj.cn

[S33] C++：vector 增删
来源：http://rg.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ng.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://cr.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://al.lnxyls.cn

[S35] C++：map
来源：http://cd.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gh.huanxung.cn

[S36] C++：unordered_map
来源：http://xw.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wh.yuntaijiaju.cn

[S37] C++：set
来源：http://en.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qb.muxihuayi.cn

[S38] C++：排序
来源：http://px.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://jo.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://bd.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uo.chemitech.net.cn

[S40] C++：查找元素
来源：http://cp.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gq.newstarts.cn

[S41] C++：类与构造函数
来源：http://uw.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nd.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://he.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://ke.jctech888.com.cn

[S43] C++：智能指针
来源：http://fe.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://hv.jctech888.com.cn

[S44] C++：引用传参
来源：http://qc.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://wd.bjjhwx.cn

[S45] C++：lambda
来源：http://qy.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oa.521024.cn

[S46] C++：函数模板
来源：http://qy.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bm.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://vj.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wm.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://pq.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ie.szsharing.cn

while (std::getline(in, line)) { }
来源：http://hn.yuntaijiaju.cn

[S49] C++：写文件
来源：http://wt.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pd.panjiajie.cn

[S50] C++：格式化数字
来源：http://si.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ww.nszjky.cn

[S51] C++：显式类型转换
来源：http://sj.panjiajie.cn

static_cast<double>(a) / b
来源：http://xe.colortex.cn

[S52] C++：const 与 noexcept
来源：http://ge.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://yx.gzmigu.cn

[S53] C++：移动语义
来源：http://qq.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://ja.asd995.cn

[S54] C++：异常处理
来源：http://hj.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ga.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://cq.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://if.asd995.cn

[S56] C++：optional
来源：http://hx.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qb.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://ir.huanxung.cn

constexpr int N = 10;
来源：http://xb.bjjhwx.cn

[S58] C++：命名空间
来源：http://my.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://jl.shtwfgs.cn

[S59] C++：静态断言
来源：http://om.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nt.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://xu.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ed.chemitech.net.cn

================================================================================
来源：http://tz.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gv.jctech888.com.cn

================================================================================
来源：http://ri.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://pi.521024.cn

println("Hello")
来源：http://ls.wgjwhj.cn

[T02] Kotlin：变量
来源：http://vm.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dj.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://qz.gzmigu.cn

"值: $b"
来源：http://mk.shxzskj.cn

[T04] Kotlin：空安全
来源：http://cs.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://rc.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://wm.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ku.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://jl.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xx.521024.cn

[T07] Kotlin：集合过滤
来源：http://hh.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bu.nszjky.cn

[T08] Kotlin：数据类
来源：http://ng.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://ji.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://wr.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://cs.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ty.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hv.szsharing.cn

[T11] Kotlin：协程
来源：http://eq.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://go.521024.cn

[T12] Kotlin：解构声明
来源：http://vv.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://ea.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://qx.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://yq.nszjky.cn

[T14] Kotlin：循环
来源：http://yv.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://wq.9csxet.cn

[T15] Kotlin：接口
来源：http://lr.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://lg.colortex.cn

[T16] Swift：Hello World
来源：http://vw.chemitech.net.cn

print("Hello")
来源：http://zh.szxytkj.cn

[T17] Swift：变量与常量
来源：http://wf.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://zg.shxzukj.cn

[T18] Swift：字符串插值
来源：http://ba.colortex.cn

"值: \(b)"
来源：http://in.asd995.cn

[T19] Swift：可选绑定
来源：http://dt.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://th.nszjky.cn

[T20] Swift：数组操作
来源：http://bq.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qc.nicolike.cn

[T21] Swift：遍历
来源：http://fx.521024.cn

for x in a { print(x) }
来源：http://ud.9csxet.cn

[T22] Swift：字典
来源：http://ba.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://od.gzmigu.cn

[T23] Swift：函数
来源：http://ia.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dq.shtwfgs.cn

[T24] Swift：闭包
来源：http://ps.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qp.panjiajie.cn

[T25] Swift：结构体
来源：http://ea.hahajie.cn

struct P { var x: Int }
来源：http://ko.hnjuh.cn

[T26] Swift：类与重写
来源：http://og.gzmigu.cn

class A: Base { override func f() {} }
来源：http://py.bjjhwx.cn

[T27] Swift：错误处理
来源：http://hb.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://dd.wgjwhj.cn

[T28] Swift：枚举
来源：http://ry.shxzskj.cn

enum Color { case red, green }
来源：http://av.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://xm.muxihuayi.cn

guard let x = opt else { return }
来源：http://nr.huanxung.cn

[T30] Swift：协议
来源：http://ff.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://ib.chemitech.net.cn

[T31] Lua：Hello World
来源：http://kz.9csxet.cn

print("Hello")
来源：http://sh.hnjuh.cn

[T32] Lua：局部变量
来源：http://hi.muxihuayi.cn

local a = 1
来源：http://dw.9csxet.cn

[T33] Lua：表（数组）
来源：http://nf.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rf.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://mk.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zr.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://pr.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://se.wgjwhj.cn

[T36] Lua：函数
来源：http://op.szxytkj.cn

function add(a, b) return a + b end
来源：http://ji.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://gn.muxihuayi.cn

"a" .. "b"
来源：http://wx.huixiangedu.cn

[T38] Lua：条件
来源：http://wf.nicolike.cn

if x > 0 then print("正") end
来源：http://xx.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://lp.asd995.cn

string.find(s, "%d+")
来源：http://sq.szsharing.cn

[T40] Lua：元表
来源：http://wj.9csxet.cn

setmetatable({}, { __index = base })
来源：http://te.panjiajie.cn

[T41] Perl：Hello World
来源：http://mk.jctech888.com.cn

print "Hello\n";
来源：http://ls.newstarts.cn

[T42] Perl：变量类型
来源：http://jb.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gm.szsharing.cn

[T43] Perl：字符串插值
来源：http://tc.shxzskj.cn

"值: $a"
来源：http://zo.521024.cn

[T44] Perl：条件
来源：http://ff.asd995.cn

if ($a > 0) { print "正"; }
来源：http://is.newstarts.cn

[T45] Perl：数组遍历
来源：http://wb.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://vb.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://cg.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xo.szsharing.cn

[T47] Perl：正则捕获
来源：http://be.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ex.newstarts.cn

[T48] Perl：正则替换
来源：http://uz.nicolike.cn

$s =~ s/old/new/g;
来源：http://vd.jctech888.com.cn

[T49] Perl：函数
来源：http://kn.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ju.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://wr.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hn.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://zw.yuexingan06.cn

[T51] Scala：Hello World
来源：http://pb.yuntaijiaju.cn

println("Hello")
来源：http://mx.huixinmuqiang.cn

[T52] Scala：变量
来源：http://xs.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://gn.hnjuh.cn

[T53] Scala：字符串插值
来源：http://zg.jianghongdianzi.cn

s"值: $b"
来源：http://ca.hahajie.cn

[T54] Scala：集合映射
来源：http://ul.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ig.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://bm.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://go.yuexingan06.cn

[T56] Scala：样例类
来源：http://vu.hahajie.cn

case class User(name: String, age: Int)
来源：http://vm.newstarts.cn

[T57] Scala：模式匹配
来源：http://us.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vc.panjiajie.cn

[T58] Scala：函数定义
来源：http://ct.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://to.wgjwhj.cn

[T59] Scala：循环
来源：http://zu.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://ww.huanxung.cn

[T60] Scala：折叠
来源：http://gk.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ie.szsharing.cn

================================================================================
来源：http://cg.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mw.yuexingan06.cn

================================================================================
来源：http://oc.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://rp.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ko.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://pt.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://so.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://pn.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ae.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://nk.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zp.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://ln.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://ka.521024.cn

[U06] Py：合并两个字典
来源：http://qb.bookmarksfly.cn

{**a, **b}
来源：http://pe.newstarts.cn

[U07] Py：反转字典键值
来源：http://wu.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://pl.szxytkj.cn

[U08] Py：展平二维列表
来源：http://sr.nszjky.cn

[y for x in nested for y in x]
来源：http://wa.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://ut.colortex.cn

max(d, key=d.get)
来源：http://ik.shxzukj.cn

[U10] Py：按值排序字典
来源：http://tu.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yr.shxzukj.cn

[U11] Py：生成器表达式
来源：http://iw.9csxet.cn

(x * 2 for x in arr)
来源：http://lo.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tg.521024.cn

Counter(arr).most_common(3)
来源：http://xx.szsharing.cn

[U13] Py：固定长度队列
来源：http://mq.bjjhwx.cn

deque(maxlen=10)
来源：http://as.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://vp.shtwfgs.cn

defaultdict(list)
来源：http://rd.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://ha.asd995.cn

t = time.perf_counter()
来源：http://qp.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://dg.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pw.hnjuh.cn

[U17] Py：初始化日志
来源：http://xz.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://nz.shxzskj.cn

[U18] Py：预编译正则
来源：http://jh.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://kx.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://wv.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://px.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://pp.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://vl.wgjwhj.cn


<!-- 参考信息 -->