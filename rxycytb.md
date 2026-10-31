代发 wailian999

read -rp "请输入: " ans
来源：http://np.muxihuayi.cn

[R78] 交互式菜单
来源：http://ui.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://el.nszjky.cn

[R79] 解析命令行选项
来源：http://hc.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mz.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://hq.chemitech.net.cn

time ./run.sh
来源：http://as.newstarts.cn

================================================================================
来源：http://qy.bookmarksfly.cn

S. C / C++ 专题
来源：http://lk.bjjhwx.cn

================================================================================
来源：http://yy.yuntaijiaju.cn

[S01] C：Hello World
来源：http://pq.jianghongdianzi.cn

#include <stdio.h>
来源：http://fi.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sa.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://uo.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://tx.bookmarksfly.cn

[S03] C：读入整数
来源：http://ku.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://zb.521024.cn

[S04] C：字符串复制
来源：http://wt.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iy.gzmigu.cn

[S05] C：字符串长度
来源：http://re.huixiangedu.cn

strlen(s)
来源：http://xa.nicolike.cn

[S06] C：字符串比较
来源：http://ca.hnjuh.cn

strcmp(a, b) == 0
来源：http://be.newstarts.cn

[S07] C：数组遍历求和
来源：http://qa.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jm.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://gz.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hk.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://lu.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gf.521024.cn

[S10] C：指针与解引用
来源：http://lk.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://kd.huanxung.cn

[S11] C：逐行读文件
来源：http://sg.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://kp.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fc.gzmigu.cn

fclose(f);
来源：http://kz.wgjwhj.cn

[S12] C：写文件
来源：http://mn.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pt.jctech888.com.cn

[S13] C：宏定义
来源：http://uj.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://im.hahajie.cn

[S14] C：枚举
来源：http://wc.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://yz.newstarts.cn

[S15] C：类型转换
来源：http://qz.colortex.cn

(double) a / b
来源：http://nd.nicolike.cn

[S16] C：位操作置位
来源：http://dc.yuexingan06.cn

x |= (1 << 3);
来源：http://oh.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://aa.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ye.asd995.cn

[S18] C：命令行参数
来源：http://jc.szxytkj.cn

int main(int argc, char **argv)
来源：http://ja.gzmigu.cn

[S19] C：快速排序
来源：http://kl.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fe.muxihuayi.cn

[S20] C：二分查找
来源：http://hj.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tl.chemitech.net.cn

[S21] C：字符类别判断
来源：http://is.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cp.hnjuh.cn

[S22] C：字符串转数字
来源：http://jp.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ps.wgjwhj.cn

[S23] C：随机数
来源：http://by.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://do.muxihuayi.cn

[S24] C：获取本地时间
来源：http://rw.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ao.asd995.cn

[S25] C：内存拷贝
来源：http://ig.hnjuh.cn

memcpy(dst, src, n);
来源：http://ic.nicolike.cn

[S26] C：内存清零
来源：http://my.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://gh.521024.cn

[S27] C：定义常量
来源：http://nw.huanxung.cn

const double PI = 3.14159;
来源：http://uo.colortex.cn

[S28] C：静态变量
来源：http://rj.huanxung.cn

static int counter = 0;
来源：http://rf.521024.cn

[S29] C：变参函数
来源：http://vi.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gh.hahajie.cn

[S30] C：头文件保护
来源：http://ik.panjiajie.cn

#ifndef X_H
来源：http://ds.bjjhwx.cn

#define X_H
来源：http://xg.szxytkj.cn

#endif
来源：http://wm.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ta.haigaiapp.cn

#include <iostream>
来源：http://hs.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://we.yuexingan06.cn

[S32] C++：字符串
来源：http://rt.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://yj.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://it.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://br.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://qi.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://sh.yuntaijiaju.cn

[S35] C++：map
来源：http://jn.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wm.wgjwhj.cn

[S36] C++：unordered_map
来源：http://vm.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://of.newstarts.cn

[S37] C++：set
来源：http://rm.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ge.szsharing.cn

[S38] C++：排序
来源：http://om.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://wp.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://ot.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uz.hnjuh.cn

[S40] C++：查找元素
来源：http://fh.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hu.shxzskj.cn

[S41] C++：类与构造函数
来源：http://ij.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sp.huanxung.cn

[S42] C++：继承与虚函数
来源：http://iz.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://nn.shxzskj.cn

[S43] C++：智能指针
来源：http://ou.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://dd.9csxet.cn

[S44] C++：引用传参
来源：http://hg.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://dr.jianghongdianzi.cn

[S45] C++：lambda
来源：http://hz.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zw.bjjhwx.cn

[S46] C++：函数模板
来源：http://qv.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://km.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://ao.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yg.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://ev.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fu.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://sp.nszjky.cn

[S49] C++：写文件
来源：http://jj.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ss.panjiajie.cn

[S50] C++：格式化数字
来源：http://lm.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rb.9csxet.cn

[S51] C++：显式类型转换
来源：http://ha.lnxyls.cn

static_cast<double>(a) / b
来源：http://ml.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ys.szsharing.cn

int size() const noexcept { return n_; }
来源：http://zz.shtwfgs.cn

[S53] C++：移动语义
来源：http://he.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://by.yuexingan06.cn

[S54] C++：异常处理
来源：http://ex.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rm.szxytkj.cn

[S55] C++：结构化绑定
来源：http://co.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ga.yuexingan06.cn

[S56] C++：optional
来源：http://nk.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dd.chemitech.net.cn

[S57] C++：编译期常量
来源：http://sf.lnxyls.cn

constexpr int N = 10;
来源：http://xp.nszjky.cn

[S58] C++：命名空间
来源：http://uo.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://ku.bookmarksfly.cn

[S59] C++：静态断言
来源：http://id.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hn.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://cy.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cc.shxzukj.cn

================================================================================
来源：http://ol.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ci.haigaiapp.cn

================================================================================
来源：http://ps.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://cv.haigaiapp.cn

println("Hello")
来源：http://ot.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://re.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dn.colortex.cn

[T03] Kotlin：字符串模板
来源：http://vp.haigaiapp.cn

"值: $b"
来源：http://fd.shxzskj.cn

[T04] Kotlin：空安全
来源：http://xn.szxytkj.cn

val n: String? = null;  n?.length
来源：http://zs.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://kt.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xh.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://gg.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qe.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://om.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rk.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://eu.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://ry.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://tu.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://lb.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://de.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mp.asd995.cn

[T11] Kotlin：协程
来源：http://dg.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zi.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://vs.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://zu.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://bk.nszjky.cn

val m = mapOf("a" to 1)
来源：http://ii.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://cm.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://jq.huixiangedu.cn

[T15] Kotlin：接口
来源：http://np.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://ki.shxzukj.cn

[T16] Swift：Hello World
来源：http://dl.newstarts.cn

print("Hello")
来源：http://ql.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://le.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://as.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://ht.shxzskj.cn

"值: \(b)"
来源：http://gb.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://mc.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://fd.jctech888.com.cn

[T20] Swift：数组操作
来源：http://am.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fw.shtwfgs.cn

[T21] Swift：遍历
来源：http://gi.jctech888.com.cn

for x in a { print(x) }
来源：http://vj.yuexingan06.cn

[T22] Swift：字典
来源：http://yk.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ee.szxytkj.cn

[T23] Swift：函数
来源：http://dj.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dt.shtwfgs.cn

[T24] Swift：闭包
来源：http://rr.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://na.nicolike.cn

[T25] Swift：结构体
来源：http://nq.shxzskj.cn

struct P { var x: Int }
来源：http://gl.newstarts.cn

[T26] Swift：类与重写
来源：http://yv.gzmigu.cn

class A: Base { override func f() {} }
来源：http://rd.huanxung.cn

[T27] Swift：错误处理
来源：http://zf.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://cp.gzmigu.cn

[T28] Swift：枚举
来源：http://bx.lnxyls.cn

enum Color { case red, green }
来源：http://ah.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://xf.szsharing.cn

guard let x = opt else { return }
来源：http://sz.szsharing.cn

[T30] Swift：协议
来源：http://zz.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://zm.panjiajie.cn

[T31] Lua：Hello World
来源：http://gx.9csxet.cn

print("Hello")
来源：http://qq.chemitech.net.cn

[T32] Lua：局部变量
来源：http://pm.jctech888.com.cn

local a = 1
来源：http://ff.521024.cn

[T33] Lua：表（数组）
来源：http://ce.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xa.wgjwhj.cn

[T34] Lua：遍历表
来源：http://ny.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gc.lnxyls.cn

[T35] Lua：字典表
来源：http://dp.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://su.huixiangedu.cn

[T36] Lua：函数
来源：http://xi.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://xl.521024.cn

[T37] Lua：字符串拼接
来源：http://wx.shxzskj.cn

"a" .. "b"
来源：http://ve.hnjuh.cn

[T38] Lua：条件
来源：http://xi.hahajie.cn

if x > 0 then print("正") end
来源：http://fu.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://mx.huanxung.cn

string.find(s, "%d+")
来源：http://gh.lnxyls.cn

[T40] Lua：元表
来源：http://qm.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://mi.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://xy.nicolike.cn

print "Hello\n";
来源：http://pa.lnxyls.cn

[T42] Perl：变量类型
来源：http://od.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cs.hnjuh.cn

[T43] Perl：字符串插值
来源：http://mt.jianghongdianzi.cn

"值: $a"
来源：http://jz.szxytkj.cn

[T44] Perl：条件
来源：http://io.521024.cn

if ($a > 0) { print "正"; }
来源：http://iu.shxzukj.cn

[T45] Perl：数组遍历
来源：http://sm.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ku.newstarts.cn

[T46] Perl：哈希操作
来源：http://cp.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://au.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://qu.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ra.521024.cn

[T48] Perl：正则替换
来源：http://am.nszjky.cn

$s =~ s/old/new/g;
来源：http://vu.hahajie.cn

[T49] Perl：函数
来源：http://yf.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nr.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://vb.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vr.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://iz.lnxyls.cn

[T51] Scala：Hello World
来源：http://pb.huixiangedu.cn

println("Hello")
来源：http://sh.huixinmuqiang.cn

[T52] Scala：变量
来源：http://rb.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://km.colortex.cn

[T53] Scala：字符串插值
来源：http://sn.521024.cn

s"值: $b"
来源：http://vd.panjiajie.cn

[T54] Scala：集合映射
来源：http://ny.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://ih.shxzskj.cn

[T55] Scala：集合过滤
来源：http://fk.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pc.haigaiapp.cn

[T56] Scala：样例类
来源：http://xc.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://tg.521024.cn

[T57] Scala：模式匹配
来源：http://vy.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ws.jctech888.com.cn

[T58] Scala：函数定义
来源：http://or.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jo.hahajie.cn

[T59] Scala：循环
来源：http://rm.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://ne.shxzskj.cn

[T60] Scala：折叠
来源：http://vl.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jg.wgjwhj.cn

================================================================================
来源：http://hl.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://io.chemitech.net.cn

================================================================================
来源：http://rq.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://cb.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dt.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ox.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wx.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://ug.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nf.shxzukj.cn

[U04] Py：变量调试打印
来源：http://ge.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vx.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://jw.asd995.cn

list(dict.fromkeys(arr))
来源：http://zm.asd995.cn

[U06] Py：合并两个字典
来源：http://ng.asd995.cn

{**a, **b}
来源：http://mg.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://do.colortex.cn

{v: k for k, v in d.items()}
来源：http://yn.gzmigu.cn

[U08] Py：展平二维列表
来源：http://nw.hahajie.cn

[y for x in nested for y in x]
来源：http://pz.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://rq.jctech888.com.cn

max(d, key=d.get)
来源：http://jd.nszjky.cn

[U10] Py：按值排序字典
来源：http://ca.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xs.szsharing.cn

[U11] Py：生成器表达式
来源：http://bh.muxihuayi.cn

(x * 2 for x in arr)
来源：http://hj.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vf.colortex.cn

Counter(arr).most_common(3)
来源：http://wl.newstarts.cn

[U13] Py：固定长度队列
来源：http://eo.9csxet.cn

deque(maxlen=10)
来源：http://jd.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://yl.hnjuh.cn

defaultdict(list)
来源：http://af.szsharing.cn

[U15] Py：高精度计时
来源：http://ug.gzmigu.cn

t = time.perf_counter()
来源：http://rd.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://hk.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sw.hahajie.cn

[U17] Py：初始化日志
来源：http://nm.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://xw.panjiajie.cn

[U18] Py：预编译正则
来源：http://ye.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://rj.lnxyls.cn


<!-- 参考信息 -->