代发 wailian999

read -rp "请输入: " ans
来源：http://wd.haigaiapp.cn

[R78] 交互式菜单
来源：http://qn.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jq.jctech888.com.cn

[R79] 解析命令行选项
来源：http://tb.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lm.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://pl.huixinmuqiang.cn

time ./run.sh
来源：http://ak.shtwfgs.cn

================================================================================
来源：http://ab.colortex.cn

S. C / C++ 专题
来源：http://ba.9csxet.cn

================================================================================
来源：http://nw.521024.cn

[S01] C：Hello World
来源：http://zf.szsharing.cn

#include <stdio.h>
来源：http://xt.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pj.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://vt.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://rj.szxytkj.cn

[S03] C：读入整数
来源：http://zz.szxytkj.cn

int x; scanf("%d", &x);
来源：http://oq.yuexingan06.cn

[S04] C：字符串复制
来源：http://ey.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://de.shxzskj.cn

[S05] C：字符串长度
来源：http://xg.jianghongdianzi.cn

strlen(s)
来源：http://ju.yuexingan06.cn

[S06] C：字符串比较
来源：http://fv.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://tv.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://yo.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vl.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://yb.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://un.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://bj.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ph.hnjuh.cn

[S10] C：指针与解引用
来源：http://oq.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://ow.hnjuh.cn

[S11] C：逐行读文件
来源：http://rz.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://ht.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://py.asd995.cn

fclose(f);
来源：http://xh.szxytkj.cn

[S12] C：写文件
来源：http://nq.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vm.asd995.cn

[S13] C：宏定义
来源：http://xu.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qq.nicolike.cn

[S14] C：枚举
来源：http://pc.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://zy.huixiangedu.cn

[S15] C：类型转换
来源：http://tt.lnxyls.cn

(double) a / b
来源：http://nd.hahajie.cn

[S16] C：位操作置位
来源：http://bo.lnxyls.cn

x |= (1 << 3);
来源：http://li.asd995.cn

[S17] C：安全拼接字符串
来源：http://wy.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rh.asd995.cn

[S18] C：命令行参数
来源：http://ro.asd995.cn

int main(int argc, char **argv)
来源：http://od.chemitech.net.cn

[S19] C：快速排序
来源：http://ow.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xy.muxihuayi.cn

[S20] C：二分查找
来源：http://is.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ce.wgjwhj.cn

[S21] C：字符类别判断
来源：http://hu.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fz.jctech888.com.cn

[S22] C：字符串转数字
来源：http://nv.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tx.lnxyls.cn

[S23] C：随机数
来源：http://mr.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gb.nicolike.cn

[S24] C：获取本地时间
来源：http://xc.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vv.wgjwhj.cn

[S25] C：内存拷贝
来源：http://ct.panjiajie.cn

memcpy(dst, src, n);
来源：http://ok.huixiangedu.cn

[S26] C：内存清零
来源：http://oc.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://xi.colortex.cn

[S27] C：定义常量
来源：http://ii.yuexingan06.cn

const double PI = 3.14159;
来源：http://ot.521024.cn

[S28] C：静态变量
来源：http://ku.bookmarksfly.cn

static int counter = 0;
来源：http://bm.yuntaijiaju.cn

[S29] C：变参函数
来源：http://ou.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gw.szxytkj.cn

[S30] C：头文件保护
来源：http://zq.huixiangedu.cn

#ifndef X_H
来源：http://io.nszjky.cn

#define X_H
来源：http://ak.chemitech.net.cn

#endif
来源：http://oj.huanxung.cn

[S31] C++：Hello World
来源：http://lr.chemitech.net.cn

#include <iostream>
来源：http://od.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ld.gzmigu.cn

[S32] C++：字符串
来源：http://gd.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://zt.huanxung.cn

[S33] C++：vector 增删
来源：http://kj.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xx.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://df.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://kw.bjjhwx.cn

[S35] C++：map
来源：http://ov.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kx.shxzskj.cn

[S36] C++：unordered_map
来源：http://cm.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ii.hahajie.cn

[S37] C++：set
来源：http://an.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://or.szsharing.cn

[S38] C++：排序
来源：http://zl.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://bg.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://lh.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://el.9csxet.cn

[S40] C++：查找元素
来源：http://as.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fh.shxzskj.cn

[S41] C++：类与构造函数
来源：http://et.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gd.newstarts.cn

[S42] C++：继承与虚函数
来源：http://sr.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://og.bjjhwx.cn

[S43] C++：智能指针
来源：http://yc.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://st.bookmarksfly.cn

[S44] C++：引用传参
来源：http://bj.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://pa.hnjuh.cn

[S45] C++：lambda
来源：http://xg.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ab.szsharing.cn

[S46] C++：函数模板
来源：http://dm.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xj.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ve.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://au.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://jw.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dc.newstarts.cn

while (std::getline(in, line)) { }
来源：http://nk.szxytkj.cn

[S49] C++：写文件
来源：http://cw.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fc.szsharing.cn

[S50] C++：格式化数字
来源：http://up.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nh.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://qo.nicolike.cn

static_cast<double>(a) / b
来源：http://lb.colortex.cn

[S52] C++：const 与 noexcept
来源：http://js.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://pp.hnjuh.cn

[S53] C++：移动语义
来源：http://mp.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://co.jctech888.com.cn

[S54] C++：异常处理
来源：http://me.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gf.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://vq.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qo.bjjhwx.cn

[S56] C++：optional
来源：http://sq.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cd.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://hb.jianghongdianzi.cn

constexpr int N = 10;
来源：http://iu.huixiangedu.cn

[S58] C++：命名空间
来源：http://fr.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://dc.nicolike.cn

[S59] C++：静态断言
来源：http://ww.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ot.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://yz.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lz.shxzukj.cn

================================================================================
来源：http://no.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jv.huixiangedu.cn

================================================================================
来源：http://yh.asd995.cn

[T01] Kotlin：Hello World
来源：http://xl.huixinmuqiang.cn

println("Hello")
来源：http://mc.chemitech.net.cn

[T02] Kotlin：变量
来源：http://xd.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xb.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://dk.panjiajie.cn

"值: $b"
来源：http://nt.gzmigu.cn

[T04] Kotlin：空安全
来源：http://cl.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://or.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://pu.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bc.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://js.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xg.colortex.cn

[T07] Kotlin：集合过滤
来源：http://wp.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://am.colortex.cn

[T08] Kotlin：数据类
来源：http://tv.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://gh.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ie.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://ux.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://lb.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vt.lnxyls.cn

[T11] Kotlin：协程
来源：http://so.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vx.newstarts.cn

[T12] Kotlin：解构声明
来源：http://cr.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://pw.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://zw.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://sm.shxzukj.cn

[T14] Kotlin：循环
来源：http://ex.huanxung.cn

for (i in 1..10) println(i)
来源：http://ea.wgjwhj.cn

[T15] Kotlin：接口
来源：http://tg.colortex.cn

interface Shape { fun area(): Double }
来源：http://wq.shtwfgs.cn

[T16] Swift：Hello World
来源：http://sk.szxytkj.cn

print("Hello")
来源：http://jg.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://kc.newstarts.cn

var a = 1;  let b = 2
来源：http://og.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://zy.yuntaijiaju.cn

"值: \(b)"
来源：http://tj.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://lg.9csxet.cn

if let n = opt { print(n) }
来源：http://zi.huixiangedu.cn

[T20] Swift：数组操作
来源：http://ij.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lk.colortex.cn

[T21] Swift：遍历
来源：http://xx.jianghongdianzi.cn

for x in a { print(x) }
来源：http://eq.huixiangedu.cn

[T22] Swift：字典
来源：http://nc.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ok.gzmigu.cn

[T23] Swift：函数
来源：http://et.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ms.shtwfgs.cn

[T24] Swift：闭包
来源：http://zg.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qa.huanxung.cn

[T25] Swift：结构体
来源：http://rh.lnxyls.cn

struct P { var x: Int }
来源：http://mw.colortex.cn

[T26] Swift：类与重写
来源：http://bc.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://ku.gzmigu.cn

[T27] Swift：错误处理
来源：http://bb.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://nl.hahajie.cn

[T28] Swift：枚举
来源：http://ru.shxzskj.cn

enum Color { case red, green }
来源：http://hc.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://um.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://sn.chemitech.net.cn

[T30] Swift：协议
来源：http://sm.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://yh.nszjky.cn

[T31] Lua：Hello World
来源：http://yd.hnjuh.cn

print("Hello")
来源：http://te.shtwfgs.cn

[T32] Lua：局部变量
来源：http://kz.yuntaijiaju.cn

local a = 1
来源：http://mj.nszjky.cn

[T33] Lua：表（数组）
来源：http://zl.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hr.colortex.cn

[T34] Lua：遍历表
来源：http://ik.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ot.bookmarksfly.cn

[T35] Lua：字典表
来源：http://iz.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://mo.huanxung.cn

[T36] Lua：函数
来源：http://bb.panjiajie.cn

function add(a, b) return a + b end
来源：http://pg.9csxet.cn

[T37] Lua：字符串拼接
来源：http://sn.muxihuayi.cn

"a" .. "b"
来源：http://gi.wgjwhj.cn

[T38] Lua：条件
来源：http://ki.jctech888.com.cn

if x > 0 then print("正") end
来源：http://vv.asd995.cn

[T39] Lua：模式匹配
来源：http://mf.colortex.cn

string.find(s, "%d+")
来源：http://ij.huixinmuqiang.cn

[T40] Lua：元表
来源：http://av.nszjky.cn

setmetatable({}, { __index = base })
来源：http://hp.hnjuh.cn

[T41] Perl：Hello World
来源：http://ij.haigaiapp.cn

print "Hello\n";
来源：http://vl.szsharing.cn

[T42] Perl：变量类型
来源：http://je.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zb.nicolike.cn

[T43] Perl：字符串插值
来源：http://ad.huanxung.cn

"值: $a"
来源：http://pn.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ng.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://hi.lnxyls.cn

[T45] Perl：数组遍历
来源：http://ee.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://ri.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://qn.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dw.asd995.cn

[T47] Perl：正则捕获
来源：http://hb.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pw.nicolike.cn

[T48] Perl：正则替换
来源：http://ey.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://ow.shxzukj.cn

[T49] Perl：函数
来源：http://rv.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vc.newstarts.cn

[T50] Perl：逐行读文件
来源：http://bo.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tf.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://gw.bjjhwx.cn

[T51] Scala：Hello World
来源：http://hq.shtwfgs.cn

println("Hello")
来源：http://jy.jctech888.com.cn

[T52] Scala：变量
来源：http://tp.shxzskj.cn

val a = 1;  var b = 2
来源：http://mq.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://eo.9csxet.cn

s"值: $b"
来源：http://ys.huanxung.cn

[T54] Scala：集合映射
来源：http://eg.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ht.9csxet.cn

[T55] Scala：集合过滤
来源：http://dr.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vr.haigaiapp.cn

[T56] Scala：样例类
来源：http://gl.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://qg.huanxung.cn

[T57] Scala：模式匹配
来源：http://sz.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aa.lnxyls.cn

[T58] Scala：函数定义
来源：http://wd.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xy.szxytkj.cn

[T59] Scala：循环
来源：http://pj.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ej.huanxung.cn

[T60] Scala：折叠
来源：http://ac.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uh.jctech888.com.cn

================================================================================
来源：http://je.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cm.nicolike.cn

================================================================================
来源：http://jb.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://yt.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vs.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://ka.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://by.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://it.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jx.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://my.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pe.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://ss.521024.cn

list(dict.fromkeys(arr))
来源：http://be.shxzukj.cn

[U06] Py：合并两个字典
来源：http://id.chemitech.net.cn

{**a, **b}
来源：http://hv.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://ma.newstarts.cn

{v: k for k, v in d.items()}
来源：http://gb.nicolike.cn

[U08] Py：展平二维列表
来源：http://oe.wgjwhj.cn

[y for x in nested for y in x]
来源：http://fn.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://co.gzmigu.cn

max(d, key=d.get)
来源：http://wd.nicolike.cn

[U10] Py：按值排序字典
来源：http://kj.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ka.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://sl.wgjwhj.cn

(x * 2 for x in arr)
来源：http://gb.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mi.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://vm.gzmigu.cn

[U13] Py：固定长度队列
来源：http://ny.lnxyls.cn

deque(maxlen=10)
来源：http://eq.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://cx.newstarts.cn

defaultdict(list)
来源：http://up.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://sq.gzmigu.cn

t = time.perf_counter()
来源：http://lj.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://ep.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vs.shxzskj.cn

[U17] Py：初始化日志
来源：http://st.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://vu.newstarts.cn

[U18] Py：预编译正则
来源：http://vy.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://iv.bjjhwx.cn


<!-- 参考信息 -->