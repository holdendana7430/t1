代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://rh.szxytkj.cn

[R76] 使用临时文件
来源：http://xf.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://db.hnjuh.cn

[R77] 读取用户输入
来源：http://sh.chemitech.net.cn

read -rp "请输入: " ans
来源：http://mx.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://xh.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mh.yuexingan06.cn

[R79] 解析命令行选项
来源：http://ke.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://os.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://lm.jianghongdianzi.cn

time ./run.sh
来源：http://ww.jctech888.com.cn

================================================================================
来源：http://xr.szxytkj.cn

S. C / C++ 专题
来源：http://of.hnjuh.cn

================================================================================
来源：http://xk.muxihuayi.cn

[S01] C：Hello World
来源：http://rh.szsharing.cn

#include <stdio.h>
来源：http://wq.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://za.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://bf.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://dj.muxihuayi.cn

[S03] C：读入整数
来源：http://dg.nszjky.cn

int x; scanf("%d", &x);
来源：http://mc.haigaiapp.cn

[S04] C：字符串复制
来源：http://mk.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uo.shxzukj.cn

[S05] C：字符串长度
来源：http://pf.hahajie.cn

strlen(s)
来源：http://sw.szxytkj.cn

[S06] C：字符串比较
来源：http://xt.hahajie.cn

strcmp(a, b) == 0
来源：http://gj.szxytkj.cn

[S07] C：数组遍历求和
来源：http://ix.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yc.asd995.cn

[S08] C：动态内存分配与释放
来源：http://ts.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ay.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://it.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vv.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://gq.9csxet.cn

int *p = &a;  *p = 5;
来源：http://jo.hnjuh.cn

[S11] C：逐行读文件
来源：http://zw.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://dl.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kz.hahajie.cn

fclose(f);
来源：http://kx.nicolike.cn

[S12] C：写文件
来源：http://qk.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ec.521024.cn

[S13] C：宏定义
来源：http://ur.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gi.shtwfgs.cn

[S14] C：枚举
来源：http://fd.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://py.panjiajie.cn

[S15] C：类型转换
来源：http://yo.hnjuh.cn

(double) a / b
来源：http://pe.nicolike.cn

[S16] C：位操作置位
来源：http://qk.9csxet.cn

x |= (1 << 3);
来源：http://bu.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://bl.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gj.huanxung.cn

[S18] C：命令行参数
来源：http://jv.asd995.cn

int main(int argc, char **argv)
来源：http://hw.nszjky.cn

[S19] C：快速排序
来源：http://fh.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cu.bjjhwx.cn

[S20] C：二分查找
来源：http://bc.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ai.shxzskj.cn

[S21] C：字符类别判断
来源：http://to.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kf.jctech888.com.cn

[S22] C：字符串转数字
来源：http://um.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wm.hahajie.cn

[S23] C：随机数
来源：http://cw.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tk.jctech888.com.cn

[S24] C：获取本地时间
来源：http://ic.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ra.521024.cn

[S25] C：内存拷贝
来源：http://ue.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://hn.haigaiapp.cn

[S26] C：内存清零
来源：http://nl.521024.cn

memset(a, 0, sizeof a);
来源：http://zq.muxihuayi.cn

[S27] C：定义常量
来源：http://yh.nszjky.cn

const double PI = 3.14159;
来源：http://hd.bjjhwx.cn

[S28] C：静态变量
来源：http://kl.shtwfgs.cn

static int counter = 0;
来源：http://kb.newstarts.cn

[S29] C：变参函数
来源：http://wt.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lk.muxihuayi.cn

[S30] C：头文件保护
来源：http://qb.shxzskj.cn

#ifndef X_H
来源：http://bh.chemitech.net.cn

#define X_H
来源：http://uc.muxihuayi.cn

#endif
来源：http://nd.hnjuh.cn

[S31] C++：Hello World
来源：http://at.huixiangedu.cn

#include <iostream>
来源：http://zr.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://hl.hnjuh.cn

[S32] C++：字符串
来源：http://jb.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://zi.bjjhwx.cn

[S33] C++：vector 增删
来源：http://tz.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zg.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://jc.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://cj.lnxyls.cn

[S35] C++：map
来源：http://jh.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hy.shtwfgs.cn

[S36] C++：unordered_map
来源：http://eh.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yt.lnxyls.cn

[S37] C++：set
来源：http://vl.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://im.huixiangedu.cn

[S38] C++：排序
来源：http://oi.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://ki.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://aa.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bn.9csxet.cn

[S40] C++：查找元素
来源：http://hx.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dn.lnxyls.cn

[S41] C++：类与构造函数
来源：http://gh.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oh.asd995.cn

[S42] C++：继承与虚函数
来源：http://yc.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://qf.huanxung.cn

[S43] C++：智能指针
来源：http://vd.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://ax.colortex.cn

[S44] C++：引用传参
来源：http://wk.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://sy.9csxet.cn

[S45] C++：lambda
来源：http://fs.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ux.szxytkj.cn

[S46] C++：函数模板
来源：http://bz.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wp.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://aq.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gs.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://qm.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hu.hahajie.cn

while (std::getline(in, line)) { }
来源：http://bs.nicolike.cn

[S49] C++：写文件
来源：http://oa.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lf.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://ah.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zj.hnjuh.cn

[S51] C++：显式类型转换
来源：http://ci.yuexingan06.cn

static_cast<double>(a) / b
来源：http://ob.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://yu.colortex.cn

int size() const noexcept { return n_; }
来源：http://da.bookmarksfly.cn

[S53] C++：移动语义
来源：http://xp.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://uo.huanxung.cn

[S54] C++：异常处理
来源：http://yf.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yj.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://ha.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qw.newstarts.cn

[S56] C++：optional
来源：http://sn.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wb.shxzukj.cn

[S57] C++：编译期常量
来源：http://zh.jctech888.com.cn

constexpr int N = 10;
来源：http://zd.huixiangedu.cn

[S58] C++：命名空间
来源：http://yx.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://th.colortex.cn

[S59] C++：静态断言
来源：http://vm.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yw.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://nt.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nh.asd995.cn

================================================================================
来源：http://bz.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mv.szsharing.cn

================================================================================
来源：http://ya.521024.cn

[T01] Kotlin：Hello World
来源：http://fs.colortex.cn

println("Hello")
来源：http://we.panjiajie.cn

[T02] Kotlin：变量
来源：http://ow.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fp.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://xh.huanxung.cn

"值: $b"
来源：http://ss.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://gs.szsharing.cn

val n: String? = null;  n?.length
来源：http://ss.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://qx.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://of.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://rt.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wr.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://lb.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sg.colortex.cn

[T08] Kotlin：数据类
来源：http://li.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://fl.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://md.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://dq.nszjky.cn

[T10] Kotlin：默认参数
来源：http://fr.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ad.newstarts.cn

[T11] Kotlin：协程
来源：http://us.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kw.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://rm.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://un.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://om.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://us.muxihuayi.cn

[T14] Kotlin：循环
来源：http://vy.521024.cn

for (i in 1..10) println(i)
来源：http://pu.panjiajie.cn

[T15] Kotlin：接口
来源：http://aw.asd995.cn

interface Shape { fun area(): Double }
来源：http://pu.hahajie.cn

[T16] Swift：Hello World
来源：http://er.wgjwhj.cn

print("Hello")
来源：http://uk.szxytkj.cn

[T17] Swift：变量与常量
来源：http://nc.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://ar.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://kj.yuntaijiaju.cn

"值: \(b)"
来源：http://vs.521024.cn

[T19] Swift：可选绑定
来源：http://ep.gzmigu.cn

if let n = opt { print(n) }
来源：http://ew.nszjky.cn

[T20] Swift：数组操作
来源：http://hu.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qv.521024.cn

[T21] Swift：遍历
来源：http://rg.gzmigu.cn

for x in a { print(x) }
来源：http://jd.huanxung.cn

[T22] Swift：字典
来源：http://wk.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mt.muxihuayi.cn

[T23] Swift：函数
来源：http://ji.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ed.hnjuh.cn

[T24] Swift：闭包
来源：http://go.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sa.gzmigu.cn

[T25] Swift：结构体
来源：http://uz.szsharing.cn

struct P { var x: Int }
来源：http://yz.chemitech.net.cn

[T26] Swift：类与重写
来源：http://cy.gzmigu.cn

class A: Base { override func f() {} }
来源：http://oo.nszjky.cn

[T27] Swift：错误处理
来源：http://fh.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ph.muxihuayi.cn

[T28] Swift：枚举
来源：http://bi.shtwfgs.cn

enum Color { case red, green }
来源：http://rx.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://xy.chemitech.net.cn

guard let x = opt else { return }
来源：http://vw.muxihuayi.cn

[T30] Swift：协议
来源：http://ms.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://ko.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://ho.hnjuh.cn

print("Hello")
来源：http://vu.panjiajie.cn

[T32] Lua：局部变量
来源：http://ta.nicolike.cn

local a = 1
来源：http://ll.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://gh.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://re.panjiajie.cn

[T34] Lua：遍历表
来源：http://bv.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ke.huanxung.cn

[T35] Lua：字典表
来源：http://nn.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://ha.chemitech.net.cn

[T36] Lua：函数
来源：http://gj.wgjwhj.cn

function add(a, b) return a + b end
来源：http://aq.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://fp.colortex.cn

"a" .. "b"
来源：http://vv.hnjuh.cn

[T38] Lua：条件
来源：http://zc.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://vl.huanxung.cn

[T39] Lua：模式匹配
来源：http://wo.wgjwhj.cn

string.find(s, "%d+")
来源：http://tt.bookmarksfly.cn

[T40] Lua：元表
来源：http://oa.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://bh.huanxung.cn

[T41] Perl：Hello World
来源：http://tm.colortex.cn

print "Hello\n";
来源：http://uk.lnxyls.cn

[T42] Perl：变量类型
来源：http://os.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nl.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://pp.hnjuh.cn

"值: $a"
来源：http://ly.huixiangedu.cn

[T44] Perl：条件
来源：http://vs.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://kt.9csxet.cn

[T45] Perl：数组遍历
来源：http://eh.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://co.huanxung.cn

[T46] Perl：哈希操作
来源：http://cb.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://um.gzmigu.cn

[T47] Perl：正则捕获
来源：http://rr.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yc.muxihuayi.cn

[T48] Perl：正则替换
来源：http://no.hnjuh.cn

$s =~ s/old/new/g;
来源：http://wf.huixiangedu.cn

[T49] Perl：函数
来源：http://au.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sg.nszjky.cn

[T50] Perl：逐行读文件
来源：http://ch.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nr.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://fy.yuexingan06.cn

[T51] Scala：Hello World
来源：http://tq.chemitech.net.cn

println("Hello")
来源：http://qn.hahajie.cn

[T52] Scala：变量
来源：http://vz.hnjuh.cn

val a = 1;  var b = 2
来源：http://ey.nicolike.cn

[T53] Scala：字符串插值
来源：http://yz.bookmarksfly.cn

s"值: $b"
来源：http://ln.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://lg.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://dp.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://gz.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jz.nszjky.cn

[T56] Scala：样例类
来源：http://oi.colortex.cn

case class User(name: String, age: Int)
来源：http://ha.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://xw.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xa.jctech888.com.cn

[T58] Scala：函数定义
来源：http://ve.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ca.bookmarksfly.cn

[T59] Scala：循环
来源：http://wv.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://uy.asd995.cn

[T60] Scala：折叠
来源：http://ct.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nu.hahajie.cn

================================================================================
来源：http://ag.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ni.shxzukj.cn

================================================================================
来源：http://lt.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://kn.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cg.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://ee.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rq.521024.cn

[U03] Py：加载 .env 配置
来源：http://ei.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wj.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://ql.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eg.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://jy.nicolike.cn

list(dict.fromkeys(arr))
来源：http://fz.shxzskj.cn

[U06] Py：合并两个字典
来源：http://as.szsharing.cn

{**a, **b}
来源：http://yj.newstarts.cn

[U07] Py：反转字典键值
来源：http://py.521024.cn

{v: k for k, v in d.items()}
来源：http://as.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://pe.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://yv.asd995.cn

[U09] Py：字典取最大值的键
来源：http://jb.chemitech.net.cn

max(d, key=d.get)
来源：http://sp.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://lu.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lp.nicolike.cn

[U11] Py：生成器表达式
来源：http://mg.lnxyls.cn

(x * 2 for x in arr)
来源：http://bz.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lw.nicolike.cn

Counter(arr).most_common(3)
来源：http://zu.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://fo.huixinmuqiang.cn

deque(maxlen=10)
来源：http://sh.colortex.cn

[U14] Py：分组收集到列表
来源：http://fo.shtwfgs.cn

defaultdict(list)
来源：http://ly.asd995.cn

[U15] Py：高精度计时
来源：http://ef.jctech888.com.cn

t = time.perf_counter()
来源：http://tm.huanxung.cn

[U16] Py：命令行参数解析
来源：http://hp.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uc.bjjhwx.cn


<!-- 参考信息 -->