代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://kg.9csxet.cn

[R76] 使用临时文件
来源：http://mg.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rz.chemitech.net.cn

[R77] 读取用户输入
来源：http://ox.bjjhwx.cn

read -rp "请输入: " ans
来源：http://kt.shxzskj.cn

[R78] 交互式菜单
来源：http://cp.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xf.9csxet.cn

[R79] 解析命令行选项
来源：http://zw.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bi.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ut.huixinmuqiang.cn

time ./run.sh
来源：http://vw.nszjky.cn

================================================================================
来源：http://xv.bjjhwx.cn

S. C / C++ 专题
来源：http://pn.bjjhwx.cn

================================================================================
来源：http://gx.hnjuh.cn

[S01] C：Hello World
来源：http://wq.wgjwhj.cn

#include <stdio.h>
来源：http://ld.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kf.hahajie.cn

[S02] C：变量与格式化输出
来源：http://hh.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://oo.nszjky.cn

[S03] C：读入整数
来源：http://tp.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://mj.hnjuh.cn

[S04] C：字符串复制
来源：http://wz.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://il.panjiajie.cn

[S05] C：字符串长度
来源：http://xk.shxzskj.cn

strlen(s)
来源：http://dt.hnjuh.cn

[S06] C：字符串比较
来源：http://qo.wgjwhj.cn

strcmp(a, b) == 0
来源：http://yg.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://ul.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kv.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://qc.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ne.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://fq.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sx.szxytkj.cn

[S10] C：指针与解引用
来源：http://yc.nszjky.cn

int *p = &a;  *p = 5;
来源：http://hg.shxzskj.cn

[S11] C：逐行读文件
来源：http://kr.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://ge.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pu.chemitech.net.cn

fclose(f);
来源：http://no.yuntaijiaju.cn

[S12] C：写文件
来源：http://ni.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yd.szxytkj.cn

[S13] C：宏定义
来源：http://kl.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cz.yuexingan06.cn

[S14] C：枚举
来源：http://lp.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://on.szxytkj.cn

[S15] C：类型转换
来源：http://uq.jianghongdianzi.cn

(double) a / b
来源：http://aa.asd995.cn

[S16] C：位操作置位
来源：http://hb.haigaiapp.cn

x |= (1 << 3);
来源：http://mi.asd995.cn

[S17] C：安全拼接字符串
来源：http://xa.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ek.chemitech.net.cn

[S18] C：命令行参数
来源：http://bs.huanxung.cn

int main(int argc, char **argv)
来源：http://ha.hnjuh.cn

[S19] C：快速排序
来源：http://xo.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oj.panjiajie.cn

[S20] C：二分查找
来源：http://qa.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ir.panjiajie.cn

[S21] C：字符类别判断
来源：http://we.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iq.wgjwhj.cn

[S22] C：字符串转数字
来源：http://ue.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iq.asd995.cn

[S23] C：随机数
来源：http://ur.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hu.lnxyls.cn

[S24] C：获取本地时间
来源：http://vk.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lo.lnxyls.cn

[S25] C：内存拷贝
来源：http://za.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://vn.nszjky.cn

[S26] C：内存清零
来源：http://gt.nicolike.cn

memset(a, 0, sizeof a);
来源：http://li.szsharing.cn

[S27] C：定义常量
来源：http://er.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://tp.521024.cn

[S28] C：静态变量
来源：http://ip.chemitech.net.cn

static int counter = 0;
来源：http://nq.9csxet.cn

[S29] C：变参函数
来源：http://dz.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ox.muxihuayi.cn

[S30] C：头文件保护
来源：http://qn.haigaiapp.cn

#ifndef X_H
来源：http://fy.shxzskj.cn

#define X_H
来源：http://lw.hahajie.cn

#endif
来源：http://em.lnxyls.cn

[S31] C++：Hello World
来源：http://lg.huixiangedu.cn

#include <iostream>
来源：http://ip.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://qn.521024.cn

[S32] C++：字符串
来源：http://eb.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://fj.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://hs.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ys.panjiajie.cn

[S34] C++：遍历 vector
来源：http://fg.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ja.bookmarksfly.cn

[S35] C++：map
来源：http://et.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xb.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://ug.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vh.wgjwhj.cn

[S37] C++：set
来源：http://er.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dw.yuexingan06.cn

[S38] C++：排序
来源：http://og.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://gp.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://wc.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fw.huanxung.cn

[S40] C++：查找元素
来源：http://uv.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nx.nicolike.cn

[S41] C++：类与构造函数
来源：http://fr.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nf.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://ud.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://xn.shxzskj.cn

[S43] C++：智能指针
来源：http://jw.521024.cn

auto p = std::make_unique<int>(5);
来源：http://uq.muxihuayi.cn

[S44] C++：引用传参
来源：http://ff.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://ci.521024.cn

[S45] C++：lambda
来源：http://kf.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qv.huixiangedu.cn

[S46] C++：函数模板
来源：http://pc.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mi.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://fp.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rv.9csxet.cn

[S48] C++：逐行读文件
来源：http://zw.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fd.nicolike.cn

while (std::getline(in, line)) { }
来源：http://qi.shtwfgs.cn

[S49] C++：写文件
来源：http://jy.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wq.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://ry.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ge.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://aq.shxzskj.cn

static_cast<double>(a) / b
来源：http://zm.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://kk.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://cy.shxzskj.cn

[S53] C++：移动语义
来源：http://jd.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://vq.9csxet.cn

[S54] C++：异常处理
来源：http://mn.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xk.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://zb.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ia.shxzskj.cn

[S56] C++：optional
来源：http://vs.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tz.muxihuayi.cn

[S57] C++：编译期常量
来源：http://tt.nszjky.cn

constexpr int N = 10;
来源：http://sn.wgjwhj.cn

[S58] C++：命名空间
来源：http://qs.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://go.lnxyls.cn

[S59] C++：静态断言
来源：http://gv.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eu.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://gq.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yh.colortex.cn

================================================================================
来源：http://io.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://br.haigaiapp.cn

================================================================================
来源：http://mg.nicolike.cn

[T01] Kotlin：Hello World
来源：http://lk.hahajie.cn

println("Hello")
来源：http://zt.jctech888.com.cn

[T02] Kotlin：变量
来源：http://vt.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zj.colortex.cn

[T03] Kotlin：字符串模板
来源：http://ki.bjjhwx.cn

"值: $b"
来源：http://zf.9csxet.cn

[T04] Kotlin：空安全
来源：http://yt.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://qa.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://lc.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wa.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://ua.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ex.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://jq.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://my.newstarts.cn

[T08] Kotlin：数据类
来源：http://uw.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://di.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://ar.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://ti.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://vc.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sy.szsharing.cn

[T11] Kotlin：协程
来源：http://pv.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lu.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://cm.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://dq.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://am.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://kd.shtwfgs.cn

[T14] Kotlin：循环
来源：http://aa.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://fm.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://rv.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://ty.nicolike.cn

[T16] Swift：Hello World
来源：http://dg.huixiangedu.cn

print("Hello")
来源：http://sl.9csxet.cn

[T17] Swift：变量与常量
来源：http://zo.szxytkj.cn

var a = 1;  let b = 2
来源：http://vp.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://se.lnxyls.cn

"值: \(b)"
来源：http://fq.panjiajie.cn

[T19] Swift：可选绑定
来源：http://rc.shtwfgs.cn

if let n = opt { print(n) }
来源：http://tf.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://rb.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xt.521024.cn

[T21] Swift：遍历
来源：http://gy.521024.cn

for x in a { print(x) }
来源：http://gi.shxzskj.cn

[T22] Swift：字典
来源：http://mq.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://di.newstarts.cn

[T23] Swift：函数
来源：http://uh.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yf.huanxung.cn

[T24] Swift：闭包
来源：http://zf.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lu.bookmarksfly.cn

[T25] Swift：结构体
来源：http://ef.panjiajie.cn

struct P { var x: Int }
来源：http://kj.jctech888.com.cn

[T26] Swift：类与重写
来源：http://sa.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://zc.szxytkj.cn

[T27] Swift：错误处理
来源：http://qg.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://sv.haigaiapp.cn

[T28] Swift：枚举
来源：http://jz.muxihuayi.cn

enum Color { case red, green }
来源：http://yd.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://xr.nicolike.cn

guard let x = opt else { return }
来源：http://ic.yuexingan06.cn

[T30] Swift：协议
来源：http://sy.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://yl.colortex.cn

[T31] Lua：Hello World
来源：http://ry.jianghongdianzi.cn

print("Hello")
来源：http://np.colortex.cn

[T32] Lua：局部变量
来源：http://bh.wgjwhj.cn

local a = 1
来源：http://pu.521024.cn

[T33] Lua：表（数组）
来源：http://zl.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ls.chemitech.net.cn

[T34] Lua：遍历表
来源：http://ru.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ql.nszjky.cn

[T35] Lua：字典表
来源：http://st.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://fh.hahajie.cn

[T36] Lua：函数
来源：http://lc.bjjhwx.cn

function add(a, b) return a + b end
来源：http://ml.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://xg.shxzskj.cn

"a" .. "b"
来源：http://kh.szxytkj.cn

[T38] Lua：条件
来源：http://uy.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://de.lnxyls.cn

[T39] Lua：模式匹配
来源：http://bh.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://bq.szsharing.cn

[T40] Lua：元表
来源：http://kg.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://je.muxihuayi.cn

[T41] Perl：Hello World
来源：http://ol.hnjuh.cn

print "Hello\n";
来源：http://vg.colortex.cn

[T42] Perl：变量类型
来源：http://jq.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pl.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://ba.gzmigu.cn

"值: $a"
来源：http://fs.shxzskj.cn

[T44] Perl：条件
来源：http://us.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://zd.hnjuh.cn

[T45] Perl：数组遍历
来源：http://iy.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ke.521024.cn

[T46] Perl：哈希操作
来源：http://jg.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gb.gzmigu.cn

[T47] Perl：正则捕获
来源：http://xp.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jd.asd995.cn

[T48] Perl：正则替换
来源：http://bc.9csxet.cn

$s =~ s/old/new/g;
来源：http://yu.asd995.cn

[T49] Perl：函数
来源：http://uc.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dp.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://jb.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cp.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://nz.yuexingan06.cn

[T51] Scala：Hello World
来源：http://vk.colortex.cn

println("Hello")
来源：http://vk.szxytkj.cn

[T52] Scala：变量
来源：http://lw.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://gv.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://ir.chemitech.net.cn

s"值: $b"
来源：http://is.shxzskj.cn

[T54] Scala：集合映射
来源：http://ui.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://oh.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://cs.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jr.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://kh.shxzskj.cn

case class User(name: String, age: Int)
来源：http://sl.szsharing.cn

[T57] Scala：模式匹配
来源：http://aa.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ci.wgjwhj.cn

[T58] Scala：函数定义
来源：http://yf.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ug.colortex.cn

[T59] Scala：循环
来源：http://wd.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://wi.jctech888.com.cn

[T60] Scala：折叠
来源：http://jq.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qo.9csxet.cn

================================================================================
来源：http://mk.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ei.yuntaijiaju.cn

================================================================================
来源：http://yc.521024.cn

[U01] Py：创建虚拟环境
来源：http://av.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jv.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://oz.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kp.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://un.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ns.nszjky.cn

[U04] Py：变量调试打印
来源：http://yt.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ym.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://nh.nicolike.cn

list(dict.fromkeys(arr))
来源：http://jz.huanxung.cn

[U06] Py：合并两个字典
来源：http://bu.panjiajie.cn

{**a, **b}
来源：http://mt.panjiajie.cn

[U07] Py：反转字典键值
来源：http://xo.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://wp.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://xu.shxzskj.cn

[y for x in nested for y in x]
来源：http://lg.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://bp.shxzskj.cn

max(d, key=d.get)
来源：http://th.hahajie.cn

[U10] Py：按值排序字典
来源：http://oz.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hu.521024.cn

[U11] Py：生成器表达式
来源：http://cl.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://rn.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://el.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://uf.panjiajie.cn

[U13] Py：固定长度队列
来源：http://bb.muxihuayi.cn

deque(maxlen=10)
来源：http://na.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://jn.shtwfgs.cn

defaultdict(list)
来源：http://pn.nszjky.cn

[U15] Py：高精度计时
来源：http://jd.colortex.cn

t = time.perf_counter()
来源：http://tj.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://tg.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wk.shtwfgs.cn


<!-- 参考信息 -->