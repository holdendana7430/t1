代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://zd.wgjwhj.cn

[R72] 等待端口就绪
来源：http://ay.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cm.haigaiapp.cn

[R73] 分割大日志
来源：http://qn.colortex.cn

split -l 1000 big.log part_
来源：http://qv.jctech888.com.cn

[R74] 批量重命名
来源：http://tw.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nu.gzmigu.cn

[R75] 导出环境变量
来源：http://lp.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://rv.szsharing.cn

[R76] 使用临时文件
来源：http://pm.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nh.nszjky.cn

[R77] 读取用户输入
来源：http://ve.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://uc.chemitech.net.cn

[R78] 交互式菜单
来源：http://sd.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vx.bjjhwx.cn

[R79] 解析命令行选项
来源：http://pw.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dj.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ph.gzmigu.cn

time ./run.sh
来源：http://pc.bookmarksfly.cn

================================================================================
来源：http://oa.shxzskj.cn

S. C / C++ 专题
来源：http://dd.wgjwhj.cn

================================================================================
来源：http://cv.huixinmuqiang.cn

[S01] C：Hello World
来源：http://dc.wgjwhj.cn

#include <stdio.h>
来源：http://wu.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mj.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://hn.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://bb.nszjky.cn

[S03] C：读入整数
来源：http://kl.shxzskj.cn

int x; scanf("%d", &x);
来源：http://kq.asd995.cn

[S04] C：字符串复制
来源：http://jn.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mw.gzmigu.cn

[S05] C：字符串长度
来源：http://ay.jianghongdianzi.cn

strlen(s)
来源：http://rr.shtwfgs.cn

[S06] C：字符串比较
来源：http://ft.shtwfgs.cn

strcmp(a, b) == 0
来源：http://ir.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://dt.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jo.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://kf.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gx.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://qk.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ef.huanxung.cn

[S10] C：指针与解引用
来源：http://mn.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://wg.bjjhwx.cn

[S11] C：逐行读文件
来源：http://rq.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ue.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mx.gzmigu.cn

fclose(f);
来源：http://mx.yuntaijiaju.cn

[S12] C：写文件
来源：http://is.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sv.shxzukj.cn

[S13] C：宏定义
来源：http://nj.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xw.nicolike.cn

[S14] C：枚举
来源：http://bx.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://eg.hnjuh.cn

[S15] C：类型转换
来源：http://my.wgjwhj.cn

(double) a / b
来源：http://xa.newstarts.cn

[S16] C：位操作置位
来源：http://pu.lnxyls.cn

x |= (1 << 3);
来源：http://xq.521024.cn

[S17] C：安全拼接字符串
来源：http://jc.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wc.gzmigu.cn

[S18] C：命令行参数
来源：http://qg.hahajie.cn

int main(int argc, char **argv)
来源：http://uc.huanxung.cn

[S19] C：快速排序
来源：http://od.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sm.newstarts.cn

[S20] C：二分查找
来源：http://vv.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vb.shxzskj.cn

[S21] C：字符类别判断
来源：http://lm.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lg.muxihuayi.cn

[S22] C：字符串转数字
来源：http://kq.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gj.haigaiapp.cn

[S23] C：随机数
来源：http://bp.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qv.panjiajie.cn

[S24] C：获取本地时间
来源：http://zr.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zv.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://tf.colortex.cn

memcpy(dst, src, n);
来源：http://ut.newstarts.cn

[S26] C：内存清零
来源：http://up.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://jp.huanxung.cn

[S27] C：定义常量
来源：http://dd.huixiangedu.cn

const double PI = 3.14159;
来源：http://lq.shtwfgs.cn

[S28] C：静态变量
来源：http://aq.nicolike.cn

static int counter = 0;
来源：http://ix.hahajie.cn

[S29] C：变参函数
来源：http://sz.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yl.wgjwhj.cn

[S30] C：头文件保护
来源：http://up.jctech888.com.cn

#ifndef X_H
来源：http://nl.lnxyls.cn

#define X_H
来源：http://gl.yuexingan06.cn

#endif
来源：http://im.muxihuayi.cn

[S31] C++：Hello World
来源：http://au.huixiangedu.cn

#include <iostream>
来源：http://uc.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ma.lnxyls.cn

[S32] C++：字符串
来源：http://kf.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://ft.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://th.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rz.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://sb.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ly.muxihuayi.cn

[S35] C++：map
来源：http://tv.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hu.yuexingan06.cn

[S36] C++：unordered_map
来源：http://tx.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ot.bookmarksfly.cn

[S37] C++：set
来源：http://el.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zv.bookmarksfly.cn

[S38] C++：排序
来源：http://mr.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://nv.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://kp.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nf.bjjhwx.cn

[S40] C++：查找元素
来源：http://oc.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uk.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://np.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kh.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://gu.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://zj.panjiajie.cn

[S43] C++：智能指针
来源：http://rs.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://dl.hnjuh.cn

[S44] C++：引用传参
来源：http://xi.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://rc.chemitech.net.cn

[S45] C++：lambda
来源：http://dq.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gzmigu.cn

[S46] C++：函数模板
来源：http://pa.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gj.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://al.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iw.nszjky.cn

[S48] C++：逐行读文件
来源：http://qk.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zw.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://qc.hahajie.cn

[S49] C++：写文件
来源：http://nf.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rx.lnxyls.cn

[S50] C++：格式化数字
来源：http://ww.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oo.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://rr.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://ub.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://lj.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://pa.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ay.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://gd.newstarts.cn

[S54] C++：异常处理
来源：http://jf.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bp.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://nv.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xq.gzmigu.cn

[S56] C++：optional
来源：http://dv.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pd.shxzskj.cn

[S57] C++：编译期常量
来源：http://ly.chemitech.net.cn

constexpr int N = 10;
来源：http://sx.shxzskj.cn

[S58] C++：命名空间
来源：http://tx.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://di.yuexingan06.cn

[S59] C++：静态断言
来源：http://ov.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fj.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://pw.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mo.jianghongdianzi.cn

================================================================================
来源：http://zu.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hp.szsharing.cn

================================================================================
来源：http://wt.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://gt.chemitech.net.cn

println("Hello")
来源：http://ht.nszjky.cn

[T02] Kotlin：变量
来源：http://er.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qh.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://qu.nszjky.cn

"值: $b"
来源：http://nv.hnjuh.cn

[T04] Kotlin：空安全
来源：http://cx.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://mf.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://xp.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vn.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://hd.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iw.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://ye.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cm.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://rs.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://zb.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://vv.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://pw.521024.cn

[T10] Kotlin：默认参数
来源：http://yi.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yx.521024.cn

[T11] Kotlin：协程
来源：http://jv.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ee.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://aj.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://hd.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://st.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://ma.shxzskj.cn

[T14] Kotlin：循环
来源：http://bc.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://yy.nszjky.cn

[T15] Kotlin：接口
来源：http://no.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://aq.hahajie.cn

[T16] Swift：Hello World
来源：http://jl.bookmarksfly.cn

print("Hello")
来源：http://hn.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://ty.9csxet.cn

var a = 1;  let b = 2
来源：http://vq.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://wv.asd995.cn

"值: \(b)"
来源：http://sl.lnxyls.cn

[T19] Swift：可选绑定
来源：http://dg.haigaiapp.cn

if let n = opt { print(n) }
来源：http://ho.chemitech.net.cn

[T20] Swift：数组操作
来源：http://qs.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ad.hnjuh.cn

[T21] Swift：遍历
来源：http://jy.nicolike.cn

for x in a { print(x) }
来源：http://mg.huixinmuqiang.cn

[T22] Swift：字典
来源：http://ts.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oz.jctech888.com.cn

[T23] Swift：函数
来源：http://mr.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ct.chemitech.net.cn

[T24] Swift：闭包
来源：http://gp.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pd.huixiangedu.cn

[T25] Swift：结构体
来源：http://oi.521024.cn

struct P { var x: Int }
来源：http://cr.gzmigu.cn

[T26] Swift：类与重写
来源：http://gi.panjiajie.cn

class A: Base { override func f() {} }
来源：http://wg.shxzskj.cn

[T27] Swift：错误处理
来源：http://jo.huanxung.cn

do { try f() } catch { print(error) }
来源：http://fx.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://xs.lnxyls.cn

enum Color { case red, green }
来源：http://yf.521024.cn

[T29] Swift：guard 提前返回
来源：http://mi.9csxet.cn

guard let x = opt else { return }
来源：http://la.muxihuayi.cn

[T30] Swift：协议
来源：http://xl.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://jr.shxzskj.cn

[T31] Lua：Hello World
来源：http://wt.jianghongdianzi.cn

print("Hello")
来源：http://mf.9csxet.cn

[T32] Lua：局部变量
来源：http://of.yuntaijiaju.cn

local a = 1
来源：http://zc.521024.cn

[T33] Lua：表（数组）
来源：http://ar.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wd.huanxung.cn

[T34] Lua：遍历表
来源：http://fu.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://te.bookmarksfly.cn

[T35] Lua：字典表
来源：http://rc.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://xv.shxzskj.cn

[T36] Lua：函数
来源：http://ex.colortex.cn

function add(a, b) return a + b end
来源：http://hn.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://ca.nszjky.cn

"a" .. "b"
来源：http://tv.chemitech.net.cn

[T38] Lua：条件
来源：http://qj.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://hm.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://su.muxihuayi.cn

string.find(s, "%d+")
来源：http://be.colortex.cn

[T40] Lua：元表
来源：http://tk.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://nu.lnxyls.cn

[T41] Perl：Hello World
来源：http://sf.bjjhwx.cn

print "Hello\n";
来源：http://uw.521024.cn

[T42] Perl：变量类型
来源：http://zt.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rg.9csxet.cn

[T43] Perl：字符串插值
来源：http://zn.yuntaijiaju.cn

"值: $a"
来源：http://av.shtwfgs.cn

[T44] Perl：条件
来源：http://ro.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://xl.shxzukj.cn

[T45] Perl：数组遍历
来源：http://oj.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://og.hahajie.cn

[T46] Perl：哈希操作
来源：http://bb.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nk.9csxet.cn

[T47] Perl：正则捕获
来源：http://sy.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tw.newstarts.cn

[T48] Perl：正则替换
来源：http://wi.szxytkj.cn

$s =~ s/old/new/g;
来源：http://cj.yuntaijiaju.cn

[T49] Perl：函数
来源：http://hp.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yn.szsharing.cn

[T50] Perl：逐行读文件
来源：http://og.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mk.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vd.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://cb.szxytkj.cn

println("Hello")
来源：http://hk.yuexingan06.cn

[T52] Scala：变量
来源：http://ws.gzmigu.cn

val a = 1;  var b = 2
来源：http://oi.asd995.cn

[T53] Scala：字符串插值
来源：http://st.newstarts.cn

s"值: $b"
来源：http://hb.hnjuh.cn

[T54] Scala：集合映射
来源：http://gp.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://ue.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://ys.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ov.hnjuh.cn

[T56] Scala：样例类
来源：http://nv.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://sh.huanxung.cn

[T57] Scala：模式匹配
来源：http://wf.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://al.szsharing.cn

[T58] Scala：函数定义
来源：http://tu.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qn.chemitech.net.cn

[T59] Scala：循环
来源：http://zg.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://lu.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://nr.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wu.hahajie.cn

================================================================================
来源：http://mf.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xl.huixinmuqiang.cn

================================================================================
来源：http://we.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://th.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ri.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://af.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://np.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://es.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tp.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://aw.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pk.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://tl.nicolike.cn

list(dict.fromkeys(arr))
来源：http://ti.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://gg.szsharing.cn

{**a, **b}
来源：http://rc.shxzukj.cn

[U07] Py：反转字典键值
来源：http://zk.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://is.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://sq.hahajie.cn

[y for x in nested for y in x]
来源：http://ha.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://yx.shtwfgs.cn

max(d, key=d.get)
来源：http://nl.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://lb.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xd.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://yc.panjiajie.cn

(x * 2 for x in arr)
来源：http://kv.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cd.hnjuh.cn

Counter(arr).most_common(3)
来源：http://jw.huixiangedu.cn


<!-- 参考信息 -->