代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hx.panjiajie.cn

[R76] 使用临时文件
来源：http://zo.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wx.bjjhwx.cn

[R77] 读取用户输入
来源：http://cs.szsharing.cn

read -rp "请输入: " ans
来源：http://ii.nszjky.cn

[R78] 交互式菜单
来源：http://st.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ra.yuexingan06.cn

[R79] 解析命令行选项
来源：http://eg.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vn.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://ay.hahajie.cn

time ./run.sh
来源：http://ej.gzmigu.cn

================================================================================
来源：http://id.haigaiapp.cn

S. C / C++ 专题
来源：http://xy.nszjky.cn

================================================================================
来源：http://ii.shxzukj.cn

[S01] C：Hello World
来源：http://lv.hnjuh.cn

#include <stdio.h>
来源：http://aw.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uv.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ss.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://og.nszjky.cn

[S03] C：读入整数
来源：http://kg.521024.cn

int x; scanf("%d", &x);
来源：http://xx.huixiangedu.cn

[S04] C：字符串复制
来源：http://ti.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zs.huixiangedu.cn

[S05] C：字符串长度
来源：http://to.szxytkj.cn

strlen(s)
来源：http://xa.hahajie.cn

[S06] C：字符串比较
来源：http://fv.shxzukj.cn

strcmp(a, b) == 0
来源：http://je.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://lk.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eo.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://kx.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sn.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://eg.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://je.gzmigu.cn

[S10] C：指针与解引用
来源：http://sv.nszjky.cn

int *p = &a;  *p = 5;
来源：http://lv.hahajie.cn

[S11] C：逐行读文件
来源：http://gb.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://rw.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://an.huanxung.cn

fclose(f);
来源：http://kb.chemitech.net.cn

[S12] C：写文件
来源：http://rl.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wp.jctech888.com.cn

[S13] C：宏定义
来源：http://lw.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://df.shxzukj.cn

[S14] C：枚举
来源：http://jk.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://ea.shxzukj.cn

[S15] C：类型转换
来源：http://jx.jctech888.com.cn

(double) a / b
来源：http://mt.bookmarksfly.cn

[S16] C：位操作置位
来源：http://ew.muxihuayi.cn

x |= (1 << 3);
来源：http://aw.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://nf.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fn.huanxung.cn

[S18] C：命令行参数
来源：http://cx.muxihuayi.cn

int main(int argc, char **argv)
来源：http://nu.yuntaijiaju.cn

[S19] C：快速排序
来源：http://dp.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ma.szxytkj.cn

[S20] C：二分查找
来源：http://us.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ju.hahajie.cn

[S21] C：字符类别判断
来源：http://xi.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://te.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://dk.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cf.szxytkj.cn

[S23] C：随机数
来源：http://as.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xx.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://yh.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dz.jctech888.com.cn

[S25] C：内存拷贝
来源：http://li.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://pq.hnjuh.cn

[S26] C：内存清零
来源：http://pv.huanxung.cn

memset(a, 0, sizeof a);
来源：http://hu.huixinmuqiang.cn

[S27] C：定义常量
来源：http://yt.asd995.cn

const double PI = 3.14159;
来源：http://hj.muxihuayi.cn

[S28] C：静态变量
来源：http://mm.lnxyls.cn

static int counter = 0;
来源：http://sw.szsharing.cn

[S29] C：变参函数
来源：http://jr.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gl.bookmarksfly.cn

[S30] C：头文件保护
来源：http://de.shtwfgs.cn

#ifndef X_H
来源：http://gn.chemitech.net.cn

#define X_H
来源：http://xh.hnjuh.cn

#endif
来源：http://dk.asd995.cn

[S31] C++：Hello World
来源：http://hi.9csxet.cn

#include <iostream>
来源：http://sf.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://zp.hnjuh.cn

[S32] C++：字符串
来源：http://wm.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://df.haigaiapp.cn

[S33] C++：vector 增删
来源：http://gh.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uh.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://mi.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://xh.shtwfgs.cn

[S35] C++：map
来源：http://ut.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gr.nszjky.cn

[S36] C++：unordered_map
来源：http://ly.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://al.lnxyls.cn

[S37] C++：set
来源：http://mt.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qy.huixiangedu.cn

[S38] C++：排序
来源：http://bf.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://qv.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://sj.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qj.colortex.cn

[S40] C++：查找元素
来源：http://qm.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fc.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://aw.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ev.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://vn.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://li.huixiangedu.cn

[S43] C++：智能指针
来源：http://db.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://vk.9csxet.cn

[S44] C++：引用传参
来源：http://ks.nszjky.cn

void inc(int &x) { ++x; }
来源：http://xd.szxytkj.cn

[S45] C++：lambda
来源：http://dy.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ss.colortex.cn

[S46] C++：函数模板
来源：http://fw.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nc.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://ua.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ry.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://rv.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wn.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://kh.shxzukj.cn

[S49] C++：写文件
来源：http://hd.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zt.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://rk.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ts.colortex.cn

[S51] C++：显式类型转换
来源：http://nk.szxytkj.cn

static_cast<double>(a) / b
来源：http://mc.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://mh.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://ap.panjiajie.cn

[S53] C++：移动语义
来源：http://be.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://cn.newstarts.cn

[S54] C++：异常处理
来源：http://ah.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zw.gzmigu.cn

[S55] C++：结构化绑定
来源：http://mv.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mq.newstarts.cn

[S56] C++：optional
来源：http://hg.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://va.hahajie.cn

[S57] C++：编译期常量
来源：http://tf.yuntaijiaju.cn

constexpr int N = 10;
来源：http://ne.panjiajie.cn

[S58] C++：命名空间
来源：http://ls.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://tx.colortex.cn

[S59] C++：静态断言
来源：http://uh.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sj.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://bn.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kf.521024.cn

================================================================================
来源：http://cw.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://el.haigaiapp.cn

================================================================================
来源：http://iw.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://vi.wgjwhj.cn

println("Hello")
来源：http://hv.lnxyls.cn

[T02] Kotlin：变量
来源：http://ev.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ot.asd995.cn

[T03] Kotlin：字符串模板
来源：http://fa.chemitech.net.cn

"值: $b"
来源：http://ax.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://ei.nszjky.cn

val n: String? = null;  n?.length
来源：http://ix.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://yb.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qv.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://oj.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bg.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://fj.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://on.asd995.cn

[T08] Kotlin：数据类
来源：http://bj.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://sx.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://bk.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://yn.huanxung.cn

[T10] Kotlin：默认参数
来源：http://wm.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ce.chemitech.net.cn

[T11] Kotlin：协程
来源：http://sm.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rh.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://is.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://nh.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://gq.colortex.cn

val m = mapOf("a" to 1)
来源：http://wb.9csxet.cn

[T14] Kotlin：循环
来源：http://nn.nszjky.cn

for (i in 1..10) println(i)
来源：http://gi.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://hb.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://tw.gzmigu.cn

[T16] Swift：Hello World
来源：http://ga.huixiangedu.cn

print("Hello")
来源：http://ko.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://jg.muxihuayi.cn

var a = 1;  let b = 2
来源：http://yu.shxzskj.cn

[T18] Swift：字符串插值
来源：http://wq.nszjky.cn

"值: \(b)"
来源：http://sa.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://qo.gzmigu.cn

if let n = opt { print(n) }
来源：http://cr.nicolike.cn

[T20] Swift：数组操作
来源：http://vo.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tf.gzmigu.cn

[T21] Swift：遍历
来源：http://ky.colortex.cn

for x in a { print(x) }
来源：http://wu.nicolike.cn

[T22] Swift：字典
来源：http://pr.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ij.huanxung.cn

[T23] Swift：函数
来源：http://rl.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yx.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://ik.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sb.nicolike.cn

[T25] Swift：结构体
来源：http://kc.huixinmuqiang.cn

struct P { var x: Int }
来源：http://fo.szsharing.cn

[T26] Swift：类与重写
来源：http://om.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ac.muxihuayi.cn

[T27] Swift：错误处理
来源：http://ac.szsharing.cn

do { try f() } catch { print(error) }
来源：http://yy.lnxyls.cn

[T28] Swift：枚举
来源：http://so.panjiajie.cn

enum Color { case red, green }
来源：http://bl.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://rs.shtwfgs.cn

guard let x = opt else { return }
来源：http://hl.huixiangedu.cn

[T30] Swift：协议
来源：http://wn.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://pd.yuexingan06.cn

[T31] Lua：Hello World
来源：http://zf.521024.cn

print("Hello")
来源：http://in.shtwfgs.cn

[T32] Lua：局部变量
来源：http://sv.jianghongdianzi.cn

local a = 1
来源：http://jm.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://fh.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ip.shxzukj.cn

[T34] Lua：遍历表
来源：http://xy.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ji.hnjuh.cn

[T35] Lua：字典表
来源：http://ap.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://vq.szsharing.cn

[T36] Lua：函数
来源：http://hv.panjiajie.cn

function add(a, b) return a + b end
来源：http://en.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://qq.wgjwhj.cn

"a" .. "b"
来源：http://mv.bookmarksfly.cn

[T38] Lua：条件
来源：http://ay.yuexingan06.cn

if x > 0 then print("正") end
来源：http://bv.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://ne.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://he.muxihuayi.cn

[T40] Lua：元表
来源：http://it.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://xk.newstarts.cn

[T41] Perl：Hello World
来源：http://zr.chemitech.net.cn

print "Hello\n";
来源：http://dz.nszjky.cn

[T42] Perl：变量类型
来源：http://pk.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bo.hahajie.cn

[T43] Perl：字符串插值
来源：http://nw.nicolike.cn

"值: $a"
来源：http://bg.asd995.cn

[T44] Perl：条件
来源：http://lv.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://no.hahajie.cn

[T45] Perl：数组遍历
来源：http://yk.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://jl.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://lx.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ea.huanxung.cn

[T47] Perl：正则捕获
来源：http://gm.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tc.hahajie.cn

[T48] Perl：正则替换
来源：http://ge.asd995.cn

$s =~ s/old/new/g;
来源：http://rw.chemitech.net.cn

[T49] Perl：函数
来源：http://jy.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vk.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://zg.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qx.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://pa.lnxyls.cn

[T51] Scala：Hello World
来源：http://eg.shxzukj.cn

println("Hello")
来源：http://pv.muxihuayi.cn

[T52] Scala：变量
来源：http://rd.huanxung.cn

val a = 1;  var b = 2
来源：http://eq.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://me.colortex.cn

s"值: $b"
来源：http://wm.huanxung.cn

[T54] Scala：集合映射
来源：http://ra.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://la.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://gt.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kk.szxytkj.cn

[T56] Scala：样例类
来源：http://yz.huanxung.cn

case class User(name: String, age: Int)
来源：http://ml.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ck.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vd.muxihuayi.cn

[T58] Scala：函数定义
来源：http://lm.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ts.huixinmuqiang.cn

[T59] Scala：循环
来源：http://us.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://df.wgjwhj.cn

[T60] Scala：折叠
来源：http://tt.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qs.jianghongdianzi.cn

================================================================================
来源：http://de.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pi.9csxet.cn

================================================================================
来源：http://he.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://so.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jf.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://ls.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bj.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://pm.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oo.gzmigu.cn

[U04] Py：变量调试打印
来源：http://qh.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eu.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://mi.newstarts.cn

list(dict.fromkeys(arr))
来源：http://sl.hnjuh.cn

[U06] Py：合并两个字典
来源：http://fc.shxzukj.cn

{**a, **b}
来源：http://vx.newstarts.cn

[U07] Py：反转字典键值
来源：http://ry.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://ov.nicolike.cn

[U08] Py：展平二维列表
来源：http://ne.newstarts.cn

[y for x in nested for y in x]
来源：http://rm.colortex.cn

[U09] Py：字典取最大值的键
来源：http://al.shxzskj.cn

max(d, key=d.get)
来源：http://mn.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://de.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yk.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://ar.nicolike.cn

(x * 2 for x in arr)
来源：http://iu.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ii.asd995.cn

Counter(arr).most_common(3)
来源：http://oh.szsharing.cn

[U13] Py：固定长度队列
来源：http://ls.szsharing.cn

deque(maxlen=10)
来源：http://qg.huanxung.cn

[U14] Py：分组收集到列表
来源：http://ev.shtwfgs.cn

defaultdict(list)
来源：http://rj.muxihuayi.cn

[U15] Py：高精度计时
来源：http://xn.521024.cn

t = time.perf_counter()
来源：http://wz.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://fj.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://el.hnjuh.cn


<!-- 参考信息 -->