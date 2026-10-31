代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://bg.huanxung.cn

[R76] 使用临时文件
来源：http://ed.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sq.muxihuayi.cn

[R77] 读取用户输入
来源：http://dl.asd995.cn

read -rp "请输入: " ans
来源：http://tn.asd995.cn

[R78] 交互式菜单
来源：http://bt.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qp.panjiajie.cn

[R79] 解析命令行选项
来源：http://wu.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cu.colortex.cn

[R80] 查看脚本执行耗时
来源：http://un.haigaiapp.cn

time ./run.sh
来源：http://ak.newstarts.cn

================================================================================
来源：http://ws.521024.cn

S. C / C++ 专题
来源：http://yv.gzmigu.cn

================================================================================
来源：http://kt.lnxyls.cn

[S01] C：Hello World
来源：http://et.shxzskj.cn

#include <stdio.h>
来源：http://ij.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xp.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://bv.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://gy.bookmarksfly.cn

[S03] C：读入整数
来源：http://hb.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://bh.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://yq.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xr.colortex.cn

[S05] C：字符串长度
来源：http://we.huixiangedu.cn

strlen(s)
来源：http://zm.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://bj.asd995.cn

strcmp(a, b) == 0
来源：http://ze.gzmigu.cn

[S07] C：数组遍历求和
来源：http://uq.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ro.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://uk.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sr.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://bl.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zc.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://qz.9csxet.cn

int *p = &a;  *p = 5;
来源：http://jd.nszjky.cn

[S11] C：逐行读文件
来源：http://tb.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://sn.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zv.jctech888.com.cn

fclose(f);
来源：http://eo.chemitech.net.cn

[S12] C：写文件
来源：http://ul.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wq.hahajie.cn

[S13] C：宏定义
来源：http://td.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jb.szsharing.cn

[S14] C：枚举
来源：http://uz.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://kg.shxzskj.cn

[S15] C：类型转换
来源：http://mx.huixinmuqiang.cn

(double) a / b
来源：http://mn.muxihuayi.cn

[S16] C：位操作置位
来源：http://ju.shtwfgs.cn

x |= (1 << 3);
来源：http://da.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://xx.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jn.huanxung.cn

[S18] C：命令行参数
来源：http://oc.nszjky.cn

int main(int argc, char **argv)
来源：http://pg.szsharing.cn

[S19] C：快速排序
来源：http://wn.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ff.newstarts.cn

[S20] C：二分查找
来源：http://za.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wp.wgjwhj.cn

[S21] C：字符类别判断
来源：http://cf.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hb.shxzukj.cn

[S22] C：字符串转数字
来源：http://qr.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uh.wgjwhj.cn

[S23] C：随机数
来源：http://cj.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lr.huanxung.cn

[S24] C：获取本地时间
来源：http://sn.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ho.yuexingan06.cn

[S25] C：内存拷贝
来源：http://rq.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://dj.9csxet.cn

[S26] C：内存清零
来源：http://kr.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://vm.shtwfgs.cn

[S27] C：定义常量
来源：http://eg.newstarts.cn

const double PI = 3.14159;
来源：http://xl.jianghongdianzi.cn

[S28] C：静态变量
来源：http://pd.szsharing.cn

static int counter = 0;
来源：http://wb.yuexingan06.cn

[S29] C：变参函数
来源：http://cv.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iq.hnjuh.cn

[S30] C：头文件保护
来源：http://rj.asd995.cn

#ifndef X_H
来源：http://ob.huanxung.cn

#define X_H
来源：http://hr.shxzukj.cn

#endif
来源：http://ns.521024.cn

[S31] C++：Hello World
来源：http://sx.hnjuh.cn

#include <iostream>
来源：http://ys.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://tv.hahajie.cn

[S32] C++：字符串
来源：http://br.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://lt.shtwfgs.cn

[S33] C++：vector 增删
来源：http://ae.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kw.hahajie.cn

[S34] C++：遍历 vector
来源：http://wo.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://qx.szxytkj.cn

[S35] C++：map
来源：http://zu.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qm.gzmigu.cn

[S36] C++：unordered_map
来源：http://zh.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nh.panjiajie.cn

[S37] C++：set
来源：http://oy.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fj.panjiajie.cn

[S38] C++：排序
来源：http://bx.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://rx.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://uj.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ws.shxzskj.cn

[S40] C++：查找元素
来源：http://ew.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ot.huanxung.cn

[S41] C++：类与构造函数
来源：http://zn.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ca.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://hc.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://qn.haigaiapp.cn

[S43] C++：智能指针
来源：http://jr.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://go.jctech888.com.cn

[S44] C++：引用传参
来源：http://kc.hahajie.cn

void inc(int &x) { ++x; }
来源：http://wp.szsharing.cn

[S45] C++：lambda
来源：http://vd.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oj.9csxet.cn

[S46] C++：函数模板
来源：http://mq.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jr.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://rh.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bq.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://pt.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dy.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://dq.huanxung.cn

[S49] C++：写文件
来源：http://wp.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ge.nicolike.cn

[S50] C++：格式化数字
来源：http://vh.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jc.panjiajie.cn

[S51] C++：显式类型转换
来源：http://jn.asd995.cn

static_cast<double>(a) / b
来源：http://ec.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://hl.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://yf.shxzskj.cn

[S53] C++：移动语义
来源：http://rl.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://uc.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://zd.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gf.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://pk.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fu.jctech888.com.cn

[S56] C++：optional
来源：http://ct.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uq.colortex.cn

[S57] C++：编译期常量
来源：http://in.haigaiapp.cn

constexpr int N = 10;
来源：http://rs.huanxung.cn

[S58] C++：命名空间
来源：http://qx.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://kp.panjiajie.cn

[S59] C++：静态断言
来源：http://ha.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ot.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://zc.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cm.panjiajie.cn

================================================================================
来源：http://tv.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kj.shtwfgs.cn

================================================================================
来源：http://fr.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://yc.gzmigu.cn

println("Hello")
来源：http://yq.shxzukj.cn

[T02] Kotlin：变量
来源：http://ec.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nd.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://jw.521024.cn

"值: $b"
来源：http://li.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://rf.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://pu.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://xy.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pb.9csxet.cn

[T06] Kotlin：集合映射
来源：http://ma.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ym.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://ai.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qq.colortex.cn

[T08] Kotlin：数据类
来源：http://bf.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://bt.colortex.cn

[T09] Kotlin：扩展函数
来源：http://cv.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://fh.nszjky.cn

[T10] Kotlin：默认参数
来源：http://us.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zf.hahajie.cn

[T11] Kotlin：协程
来源：http://sm.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ct.hahajie.cn

[T12] Kotlin：解构声明
来源：http://wd.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://rn.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://cz.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://oi.lnxyls.cn

[T14] Kotlin：循环
来源：http://vo.newstarts.cn

for (i in 1..10) println(i)
来源：http://ta.521024.cn

[T15] Kotlin：接口
来源：http://rh.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://tp.newstarts.cn

[T16] Swift：Hello World
来源：http://ix.jianghongdianzi.cn

print("Hello")
来源：http://uq.colortex.cn

[T17] Swift：变量与常量
来源：http://bg.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://to.hnjuh.cn

[T18] Swift：字符串插值
来源：http://xv.hnjuh.cn

"值: \(b)"
来源：http://vi.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://pb.panjiajie.cn

if let n = opt { print(n) }
来源：http://dt.huixiangedu.cn

[T20] Swift：数组操作
来源：http://uq.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ah.lnxyls.cn

[T21] Swift：遍历
来源：http://gg.huixiangedu.cn

for x in a { print(x) }
来源：http://fe.huixinmuqiang.cn

[T22] Swift：字典
来源：http://ea.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wo.shxzukj.cn

[T23] Swift：函数
来源：http://ny.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jb.huanxung.cn

[T24] Swift：闭包
来源：http://cx.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lf.haigaiapp.cn

[T25] Swift：结构体
来源：http://ws.9csxet.cn

struct P { var x: Int }
来源：http://sw.9csxet.cn

[T26] Swift：类与重写
来源：http://qr.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://dg.panjiajie.cn

[T27] Swift：错误处理
来源：http://cx.hahajie.cn

do { try f() } catch { print(error) }
来源：http://de.panjiajie.cn

[T28] Swift：枚举
来源：http://bi.shxzukj.cn

enum Color { case red, green }
来源：http://oz.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://tj.wgjwhj.cn

guard let x = opt else { return }
来源：http://vp.panjiajie.cn

[T30] Swift：协议
来源：http://vm.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ny.yuexingan06.cn

[T31] Lua：Hello World
来源：http://cx.asd995.cn

print("Hello")
来源：http://bt.szsharing.cn

[T32] Lua：局部变量
来源：http://bu.szsharing.cn

local a = 1
来源：http://zp.hahajie.cn

[T33] Lua：表（数组）
来源：http://fh.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ow.hahajie.cn

[T34] Lua：遍历表
来源：http://to.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hs.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://dt.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://ry.huixinmuqiang.cn

[T36] Lua：函数
来源：http://la.9csxet.cn

function add(a, b) return a + b end
来源：http://ty.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://bb.huixinmuqiang.cn

"a" .. "b"
来源：http://is.haigaiapp.cn

[T38] Lua：条件
来源：http://jr.nicolike.cn

if x > 0 then print("正") end
来源：http://oj.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://nz.yuexingan06.cn

string.find(s, "%d+")
来源：http://az.nicolike.cn

[T40] Lua：元表
来源：http://rw.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://ao.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://wg.huanxung.cn

print "Hello\n";
来源：http://fg.shxzskj.cn

[T42] Perl：变量类型
来源：http://et.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vx.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://xh.gzmigu.cn

"值: $a"
来源：http://rb.nszjky.cn

[T44] Perl：条件
来源：http://np.asd995.cn

if ($a > 0) { print "正"; }
来源：http://pd.hahajie.cn

[T45] Perl：数组遍历
来源：http://yu.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://gs.szsharing.cn

[T46] Perl：哈希操作
来源：http://go.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hn.shxzukj.cn

[T47] Perl：正则捕获
来源：http://pb.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vs.szxytkj.cn

[T48] Perl：正则替换
来源：http://br.hnjuh.cn

$s =~ s/old/new/g;
来源：http://fv.panjiajie.cn

[T49] Perl：函数
来源：http://ob.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ig.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://sy.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ba.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://bv.521024.cn

[T51] Scala：Hello World
来源：http://ry.jctech888.com.cn

println("Hello")
来源：http://vx.hahajie.cn

[T52] Scala：变量
来源：http://uk.huanxung.cn

val a = 1;  var b = 2
来源：http://im.521024.cn

[T53] Scala：字符串插值
来源：http://dz.szxytkj.cn

s"值: $b"
来源：http://mw.jctech888.com.cn

[T54] Scala：集合映射
来源：http://cc.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://gd.szxytkj.cn

[T55] Scala：集合过滤
来源：http://km.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gl.panjiajie.cn

[T56] Scala：样例类
来源：http://rt.nszjky.cn

case class User(name: String, age: Int)
来源：http://ju.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://fj.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eo.huixiangedu.cn

[T58] Scala：函数定义
来源：http://nj.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kz.colortex.cn

[T59] Scala：循环
来源：http://dl.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://si.hahajie.cn

[T60] Scala：折叠
来源：http://nh.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vm.9csxet.cn

================================================================================
来源：http://yi.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zc.wgjwhj.cn

================================================================================
来源：http://gq.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://tk.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xa.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://tz.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uq.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://dp.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wx.szsharing.cn

[U04] Py：变量调试打印
来源：http://iv.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wa.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://qe.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://vo.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://lj.bookmarksfly.cn

{**a, **b}
来源：http://yb.lnxyls.cn

[U07] Py：反转字典键值
来源：http://xr.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://da.szxytkj.cn

[U08] Py：展平二维列表
来源：http://bb.haigaiapp.cn

[y for x in nested for y in x]
来源：http://ob.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://qk.hahajie.cn

max(d, key=d.get)
来源：http://jh.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://nj.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kp.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://fg.hnjuh.cn

(x * 2 for x in arr)
来源：http://br.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ob.lnxyls.cn

Counter(arr).most_common(3)
来源：http://ys.newstarts.cn

[U13] Py：固定长度队列
来源：http://xc.yuntaijiaju.cn

deque(maxlen=10)
来源：http://xj.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://yw.huanxung.cn

defaultdict(list)
来源：http://nj.muxihuayi.cn

[U15] Py：高精度计时
来源：http://fe.hahajie.cn

t = time.perf_counter()
来源：http://vu.nszjky.cn

[U16] Py：命令行参数解析
来源：http://el.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jt.lnxyls.cn


<!-- 参考信息 -->