代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://wi.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://xz.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://gi.yuntaijiaju.cn

[R71] 日期格式化
来源：http://af.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rq.szsharing.cn

[R72] 等待端口就绪
来源：http://na.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ns.haigaiapp.cn

[R73] 分割大日志
来源：http://jm.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://lr.szsharing.cn

[R74] 批量重命名
来源：http://yf.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tj.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://ke.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://fa.bjjhwx.cn

[R76] 使用临时文件
来源：http://qq.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wt.newstarts.cn

[R77] 读取用户输入
来源：http://hd.colortex.cn

read -rp "请输入: " ans
来源：http://mb.521024.cn

[R78] 交互式菜单
来源：http://jj.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://id.huanxung.cn

[R79] 解析命令行选项
来源：http://do.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mh.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://eb.haigaiapp.cn

time ./run.sh
来源：http://jo.bjjhwx.cn

================================================================================
来源：http://dx.jctech888.com.cn

S. C / C++ 专题
来源：http://qk.chemitech.net.cn

================================================================================
来源：http://zq.lnxyls.cn

[S01] C：Hello World
来源：http://nm.hnjuh.cn

#include <stdio.h>
来源：http://vj.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aj.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://qc.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://it.hahajie.cn

[S03] C：读入整数
来源：http://kc.hahajie.cn

int x; scanf("%d", &x);
来源：http://yp.nszjky.cn

[S04] C：字符串复制
来源：http://dj.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://my.colortex.cn

[S05] C：字符串长度
来源：http://ga.521024.cn

strlen(s)
来源：http://ej.asd995.cn

[S06] C：字符串比较
来源：http://ta.wgjwhj.cn

strcmp(a, b) == 0
来源：http://vp.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://yd.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ew.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://lg.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ql.asd995.cn

[S09] C：结构体定义与初始化
来源：http://ca.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dl.haigaiapp.cn

[S10] C：指针与解引用
来源：http://vn.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://an.hahajie.cn

[S11] C：逐行读文件
来源：http://xs.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://dt.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://up.lnxyls.cn

fclose(f);
来源：http://hp.shxzskj.cn

[S12] C：写文件
来源：http://wu.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ad.yuexingan06.cn

[S13] C：宏定义
来源：http://na.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xw.yuntaijiaju.cn

[S14] C：枚举
来源：http://nu.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://nm.haigaiapp.cn

[S15] C：类型转换
来源：http://tj.shtwfgs.cn

(double) a / b
来源：http://an.hahajie.cn

[S16] C：位操作置位
来源：http://od.521024.cn

x |= (1 << 3);
来源：http://cy.huanxung.cn

[S17] C：安全拼接字符串
来源：http://vh.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ad.hnjuh.cn

[S18] C：命令行参数
来源：http://uq.521024.cn

int main(int argc, char **argv)
来源：http://jx.hnjuh.cn

[S19] C：快速排序
来源：http://ev.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dj.szxytkj.cn

[S20] C：二分查找
来源：http://tu.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bt.nicolike.cn

[S21] C：字符类别判断
来源：http://gs.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ci.szxytkj.cn

[S22] C：字符串转数字
来源：http://sm.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jm.nszjky.cn

[S23] C：随机数
来源：http://lo.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pt.newstarts.cn

[S24] C：获取本地时间
来源：http://nf.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pt.haigaiapp.cn

[S25] C：内存拷贝
来源：http://bf.hnjuh.cn

memcpy(dst, src, n);
来源：http://qu.huanxung.cn

[S26] C：内存清零
来源：http://wz.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://cj.huixiangedu.cn

[S27] C：定义常量
来源：http://lj.jctech888.com.cn

const double PI = 3.14159;
来源：http://qq.lnxyls.cn

[S28] C：静态变量
来源：http://av.shxzukj.cn

static int counter = 0;
来源：http://cb.colortex.cn

[S29] C：变参函数
来源：http://ab.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zc.newstarts.cn

[S30] C：头文件保护
来源：http://qt.lnxyls.cn

#ifndef X_H
来源：http://ud.gzmigu.cn

#define X_H
来源：http://pv.panjiajie.cn

#endif
来源：http://ti.nicolike.cn

[S31] C++：Hello World
来源：http://su.chemitech.net.cn

#include <iostream>
来源：http://rw.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://bk.jctech888.com.cn

[S32] C++：字符串
来源：http://kp.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://hf.shxzukj.cn

[S33] C++：vector 增删
来源：http://of.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ua.szxytkj.cn

[S34] C++：遍历 vector
来源：http://ae.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ac.bookmarksfly.cn

[S35] C++：map
来源：http://ai.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dc.yuexingan06.cn

[S36] C++：unordered_map
来源：http://pm.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oi.colortex.cn

[S37] C++：set
来源：http://ju.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uu.nicolike.cn

[S38] C++：排序
来源：http://cn.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://oh.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://hz.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tx.nszjky.cn

[S40] C++：查找元素
来源：http://bt.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://di.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://vu.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://td.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://pv.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://ro.bjjhwx.cn

[S43] C++：智能指针
来源：http://nw.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://vp.asd995.cn

[S44] C++：引用传参
来源：http://bl.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://xe.yuexingan06.cn

[S45] C++：lambda
来源：http://rw.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xw.chemitech.net.cn

[S46] C++：函数模板
来源：http://jy.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fv.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://wu.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xz.panjiajie.cn

[S48] C++：逐行读文件
来源：http://ee.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hq.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://nv.newstarts.cn

[S49] C++：写文件
来源：http://uu.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uj.newstarts.cn

[S50] C++：格式化数字
来源：http://jn.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mv.newstarts.cn

[S51] C++：显式类型转换
来源：http://rv.nszjky.cn

static_cast<double>(a) / b
来源：http://my.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://mu.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://tj.nszjky.cn

[S53] C++：移动语义
来源：http://aj.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://zf.jctech888.com.cn

[S54] C++：异常处理
来源：http://nz.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://of.panjiajie.cn

[S55] C++：结构化绑定
来源：http://zw.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oj.jianghongdianzi.cn

[S56] C++：optional
来源：http://bj.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zl.9csxet.cn

[S57] C++：编译期常量
来源：http://vb.nszjky.cn

constexpr int N = 10;
来源：http://el.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://kb.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://me.newstarts.cn

[S59] C++：静态断言
来源：http://oc.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cr.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://rv.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jb.yuntaijiaju.cn

================================================================================
来源：http://ba.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jb.yuntaijiaju.cn

================================================================================
来源：http://eb.colortex.cn

[T01] Kotlin：Hello World
来源：http://qc.lnxyls.cn

println("Hello")
来源：http://qw.gzmigu.cn

[T02] Kotlin：变量
来源：http://er.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oo.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://uz.9csxet.cn

"值: $b"
来源：http://pj.521024.cn

[T04] Kotlin：空安全
来源：http://mz.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://mj.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://db.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cy.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://no.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vb.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://qj.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xt.hahajie.cn

[T08] Kotlin：数据类
来源：http://wu.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://aw.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://tq.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://la.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://mb.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yb.gzmigu.cn

[T11] Kotlin：协程
来源：http://zc.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gw.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://qo.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://xa.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://om.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://tj.colortex.cn

[T14] Kotlin：循环
来源：http://id.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://bs.wgjwhj.cn

[T15] Kotlin：接口
来源：http://fi.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://xo.shtwfgs.cn

[T16] Swift：Hello World
来源：http://cn.huixinmuqiang.cn

print("Hello")
来源：http://ow.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://sx.gzmigu.cn

var a = 1;  let b = 2
来源：http://zz.huanxung.cn

[T18] Swift：字符串插值
来源：http://zz.asd995.cn

"值: \(b)"
来源：http://db.shxzskj.cn

[T19] Swift：可选绑定
来源：http://nr.gzmigu.cn

if let n = opt { print(n) }
来源：http://vx.newstarts.cn

[T20] Swift：数组操作
来源：http://dm.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://an.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://cp.shtwfgs.cn

for x in a { print(x) }
来源：http://kw.521024.cn

[T22] Swift：字典
来源：http://uj.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xu.shxzskj.cn

[T23] Swift：函数
来源：http://vf.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://se.lnxyls.cn

[T24] Swift：闭包
来源：http://gw.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fi.shxzukj.cn

[T25] Swift：结构体
来源：http://ow.asd995.cn

struct P { var x: Int }
来源：http://wy.lnxyls.cn

[T26] Swift：类与重写
来源：http://wz.hnjuh.cn

class A: Base { override func f() {} }
来源：http://ew.huixiangedu.cn

[T27] Swift：错误处理
来源：http://ct.szsharing.cn

do { try f() } catch { print(error) }
来源：http://in.muxihuayi.cn

[T28] Swift：枚举
来源：http://ic.jianghongdianzi.cn

enum Color { case red, green }
来源：http://rx.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://bd.colortex.cn

guard let x = opt else { return }
来源：http://hl.colortex.cn

[T30] Swift：协议
来源：http://yt.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://vo.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://im.haigaiapp.cn

print("Hello")
来源：http://kf.asd995.cn

[T32] Lua：局部变量
来源：http://jt.jianghongdianzi.cn

local a = 1
来源：http://ty.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://ks.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ub.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://ie.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wr.bookmarksfly.cn

[T35] Lua：字典表
来源：http://ap.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://el.jianghongdianzi.cn

[T36] Lua：函数
来源：http://de.jctech888.com.cn

function add(a, b) return a + b end
来源：http://om.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://pm.lnxyls.cn

"a" .. "b"
来源：http://hk.asd995.cn

[T38] Lua：条件
来源：http://dw.gzmigu.cn

if x > 0 then print("正") end
来源：http://rk.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://kf.bjjhwx.cn

string.find(s, "%d+")
来源：http://nx.huanxung.cn

[T40] Lua：元表
来源：http://mf.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://vb.hahajie.cn

[T41] Perl：Hello World
来源：http://xg.521024.cn

print "Hello\n";
来源：http://gx.nicolike.cn

[T42] Perl：变量类型
来源：http://xn.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://na.nszjky.cn

[T43] Perl：字符串插值
来源：http://gn.jctech888.com.cn

"值: $a"
来源：http://sx.szsharing.cn

[T44] Perl：条件
来源：http://ha.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://dk.szsharing.cn

[T45] Perl：数组遍历
来源：http://ro.asd995.cn

for my $x (@arr) { print $x; }
来源：http://hf.521024.cn

[T46] Perl：哈希操作
来源：http://au.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xx.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://je.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jz.huixiangedu.cn

[T48] Perl：正则替换
来源：http://sm.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://ml.nicolike.cn

[T49] Perl：函数
来源：http://lh.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zy.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://zb.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ir.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://ri.jctech888.com.cn

[T51] Scala：Hello World
来源：http://du.gzmigu.cn

println("Hello")
来源：http://fj.lnxyls.cn

[T52] Scala：变量
来源：http://ds.szxytkj.cn

val a = 1;  var b = 2
来源：http://mw.shxzukj.cn

[T53] Scala：字符串插值
来源：http://ra.521024.cn

s"值: $b"
来源：http://cb.huanxung.cn

[T54] Scala：集合映射
来源：http://xi.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ty.nszjky.cn

[T55] Scala：集合过滤
来源：http://em.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xr.shxzukj.cn

[T56] Scala：样例类
来源：http://ay.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://yk.9csxet.cn

[T57] Scala：模式匹配
来源：http://wl.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vf.panjiajie.cn

[T58] Scala：函数定义
来源：http://de.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dk.muxihuayi.cn

[T59] Scala：循环
来源：http://zb.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://pm.shxzukj.cn

[T60] Scala：折叠
来源：http://af.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://he.521024.cn

================================================================================
来源：http://ue.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rv.shxzukj.cn

================================================================================
来源：http://dv.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://yr.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jy.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://md.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ja.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://ps.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rg.asd995.cn

[U04] Py：变量调试打印
来源：http://iy.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ia.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://os.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://fj.nszjky.cn

[U06] Py：合并两个字典
来源：http://xp.chemitech.net.cn

{**a, **b}
来源：http://jl.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://ds.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://lw.nszjky.cn

[U08] Py：展平二维列表
来源：http://yz.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://dq.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://zz.asd995.cn

max(d, key=d.get)
来源：http://uq.hahajie.cn

[U10] Py：按值排序字典
来源：http://is.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qz.yuntaijiaju.cn


<!-- 参考信息 -->