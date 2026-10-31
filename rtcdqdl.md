代发 wailian999

read -rp "请输入: " ans
来源：http://hb.haigaiapp.cn

[R78] 交互式菜单
来源：http://jr.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pj.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://bg.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sc.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://gl.shxzskj.cn

time ./run.sh
来源：http://zu.szxytkj.cn

================================================================================
来源：http://pg.hahajie.cn

S. C / C++ 专题
来源：http://ui.huanxung.cn

================================================================================
来源：http://rf.bookmarksfly.cn

[S01] C：Hello World
来源：http://yw.9csxet.cn

#include <stdio.h>
来源：http://xm.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://im.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://cm.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://eo.yuntaijiaju.cn

[S03] C：读入整数
来源：http://iv.nicolike.cn

int x; scanf("%d", &x);
来源：http://zb.haigaiapp.cn

[S04] C：字符串复制
来源：http://ik.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zk.lnxyls.cn

[S05] C：字符串长度
来源：http://vq.521024.cn

strlen(s)
来源：http://bq.szxytkj.cn

[S06] C：字符串比较
来源：http://qo.nszjky.cn

strcmp(a, b) == 0
来源：http://nc.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://pt.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vj.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://hi.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yw.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://jj.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jq.521024.cn

[S10] C：指针与解引用
来源：http://cp.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://ti.colortex.cn

[S11] C：逐行读文件
来源：http://ld.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://im.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jl.chemitech.net.cn

fclose(f);
来源：http://cw.colortex.cn

[S12] C：写文件
来源：http://er.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ce.nicolike.cn

[S13] C：宏定义
来源：http://hz.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tt.bjjhwx.cn

[S14] C：枚举
来源：http://jk.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://jc.szxytkj.cn

[S15] C：类型转换
来源：http://cr.szsharing.cn

(double) a / b
来源：http://hy.lnxyls.cn

[S16] C：位操作置位
来源：http://dv.hnjuh.cn

x |= (1 << 3);
来源：http://vp.newstarts.cn

[S17] C：安全拼接字符串
来源：http://ye.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mo.newstarts.cn

[S18] C：命令行参数
来源：http://sg.szsharing.cn

int main(int argc, char **argv)
来源：http://qb.bjjhwx.cn

[S19] C：快速排序
来源：http://ac.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gl.nicolike.cn

[S20] C：二分查找
来源：http://ms.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://re.shtwfgs.cn

[S21] C：字符类别判断
来源：http://zo.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ab.hnjuh.cn

[S22] C：字符串转数字
来源：http://oy.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://px.hahajie.cn

[S23] C：随机数
来源：http://kx.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qn.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://il.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wq.panjiajie.cn

[S25] C：内存拷贝
来源：http://tt.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://rp.hahajie.cn

[S26] C：内存清零
来源：http://ye.hahajie.cn

memset(a, 0, sizeof a);
来源：http://nb.nszjky.cn

[S27] C：定义常量
来源：http://vn.gzmigu.cn

const double PI = 3.14159;
来源：http://sw.jctech888.com.cn

[S28] C：静态变量
来源：http://ii.colortex.cn

static int counter = 0;
来源：http://ta.jctech888.com.cn

[S29] C：变参函数
来源：http://dv.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ei.shxzskj.cn

[S30] C：头文件保护
来源：http://ek.jianghongdianzi.cn

#ifndef X_H
来源：http://cz.521024.cn

#define X_H
来源：http://ej.521024.cn

#endif
来源：http://zb.jctech888.com.cn

[S31] C++：Hello World
来源：http://aa.shxzskj.cn

#include <iostream>
来源：http://ho.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://mx.hnjuh.cn

[S32] C++：字符串
来源：http://rv.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://mz.huanxung.cn

[S33] C++：vector 增删
来源：http://kq.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fp.lnxyls.cn

[S34] C++：遍历 vector
来源：http://km.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://vr.huanxung.cn

[S35] C++：map
来源：http://sm.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ux.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://pz.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://om.lnxyls.cn

[S37] C++：set
来源：http://tx.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lu.wgjwhj.cn

[S38] C++：排序
来源：http://rp.colortex.cn

std::sort(v.begin(), v.end());
来源：http://tt.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://nn.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vn.huixiangedu.cn

[S40] C++：查找元素
来源：http://mi.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dh.shxzukj.cn

[S41] C++：类与构造函数
来源：http://ls.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fi.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://dt.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://yr.wgjwhj.cn

[S43] C++：智能指针
来源：http://nd.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://hc.newstarts.cn

[S44] C++：引用传参
来源：http://oa.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://zz.521024.cn

[S45] C++：lambda
来源：http://sl.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fj.szxytkj.cn

[S46] C++：函数模板
来源：http://tx.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dt.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://jp.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rb.521024.cn

[S48] C++：逐行读文件
来源：http://up.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xz.newstarts.cn

while (std::getline(in, line)) { }
来源：http://gt.bookmarksfly.cn

[S49] C++：写文件
来源：http://ru.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fg.yuexingan06.cn

[S50] C++：格式化数字
来源：http://tc.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qi.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://bo.yuexingan06.cn

static_cast<double>(a) / b
来源：http://ba.asd995.cn

[S52] C++：const 与 noexcept
来源：http://rl.nicolike.cn

int size() const noexcept { return n_; }
来源：http://kb.shxzskj.cn

[S53] C++：移动语义
来源：http://wz.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://pb.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://zk.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yf.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://ae.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wh.muxihuayi.cn

[S56] C++：optional
来源：http://cd.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zk.shxzukj.cn

[S57] C++：编译期常量
来源：http://gu.nszjky.cn

constexpr int N = 10;
来源：http://fa.wgjwhj.cn

[S58] C++：命名空间
来源：http://ud.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://nn.asd995.cn

[S59] C++：静态断言
来源：http://iu.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ej.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://dg.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bj.nicolike.cn

================================================================================
来源：http://lh.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fu.jctech888.com.cn

================================================================================
来源：http://ik.newstarts.cn

[T01] Kotlin：Hello World
来源：http://ax.shxzukj.cn

println("Hello")
来源：http://py.wgjwhj.cn

[T02] Kotlin：变量
来源：http://vv.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wg.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://wh.jianghongdianzi.cn

"值: $b"
来源：http://id.newstarts.cn

[T04] Kotlin：空安全
来源：http://fq.gzmigu.cn

val n: String? = null;  n?.length
来源：http://qv.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://kx.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tq.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ef.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cr.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://zb.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bs.nszjky.cn

[T08] Kotlin：数据类
来源：http://uc.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://gt.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://pb.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://gb.huanxung.cn

[T10] Kotlin：默认参数
来源：http://ls.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oj.nszjky.cn

[T11] Kotlin：协程
来源：http://rc.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iz.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://dy.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://no.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://vj.newstarts.cn

val m = mapOf("a" to 1)
来源：http://kc.newstarts.cn

[T14] Kotlin：循环
来源：http://uj.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://ld.bjjhwx.cn

[T15] Kotlin：接口
来源：http://lq.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://vi.yuexingan06.cn

[T16] Swift：Hello World
来源：http://eu.nszjky.cn

print("Hello")
来源：http://vd.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://rq.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://nz.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://eg.bookmarksfly.cn

"值: \(b)"
来源：http://xq.gzmigu.cn

[T19] Swift：可选绑定
来源：http://vy.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://ot.huanxung.cn

[T20] Swift：数组操作
来源：http://ht.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ya.shtwfgs.cn

[T21] Swift：遍历
来源：http://zs.hahajie.cn

for x in a { print(x) }
来源：http://ry.shtwfgs.cn

[T22] Swift：字典
来源：http://qc.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sv.huixiangedu.cn

[T23] Swift：函数
来源：http://rh.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yf.521024.cn

[T24] Swift：闭包
来源：http://sc.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lb.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://eu.haigaiapp.cn

struct P { var x: Int }
来源：http://pv.shtwfgs.cn

[T26] Swift：类与重写
来源：http://oo.shxzskj.cn

class A: Base { override func f() {} }
来源：http://rc.shxzskj.cn

[T27] Swift：错误处理
来源：http://mu.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://pp.panjiajie.cn

[T28] Swift：枚举
来源：http://ig.panjiajie.cn

enum Color { case red, green }
来源：http://fk.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://kz.9csxet.cn

guard let x = opt else { return }
来源：http://ea.hnjuh.cn

[T30] Swift：协议
来源：http://yr.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://od.9csxet.cn

[T31] Lua：Hello World
来源：http://mu.haigaiapp.cn

print("Hello")
来源：http://hy.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://kn.asd995.cn

local a = 1
来源：http://bu.hnjuh.cn

[T33] Lua：表（数组）
来源：http://bc.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://no.huixiangedu.cn

[T34] Lua：遍历表
来源：http://cc.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kk.chemitech.net.cn

[T35] Lua：字典表
来源：http://hy.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://gt.gzmigu.cn

[T36] Lua：函数
来源：http://vf.nszjky.cn

function add(a, b) return a + b end
来源：http://ud.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://kc.bookmarksfly.cn

"a" .. "b"
来源：http://nm.newstarts.cn

[T38] Lua：条件
来源：http://rd.huanxung.cn

if x > 0 then print("正") end
来源：http://ct.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://mh.asd995.cn

string.find(s, "%d+")
来源：http://ey.shxzukj.cn

[T40] Lua：元表
来源：http://fs.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://kh.szsharing.cn

[T41] Perl：Hello World
来源：http://rh.shtwfgs.cn

print "Hello\n";
来源：http://ek.newstarts.cn

[T42] Perl：变量类型
来源：http://co.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sp.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://lf.asd995.cn

"值: $a"
来源：http://jl.yuexingan06.cn

[T44] Perl：条件
来源：http://uh.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://xo.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://mb.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://qc.asd995.cn

[T46] Perl：哈希操作
来源：http://aq.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://za.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://ta.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pe.521024.cn

[T48] Perl：正则替换
来源：http://yt.lnxyls.cn

$s =~ s/old/new/g;
来源：http://uf.haigaiapp.cn

[T49] Perl：函数
来源：http://rz.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jt.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://fh.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dr.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://iy.chemitech.net.cn

[T51] Scala：Hello World
来源：http://jn.panjiajie.cn

println("Hello")
来源：http://zl.huanxung.cn

[T52] Scala：变量
来源：http://dd.yuexingan06.cn

val a = 1;  var b = 2
来源：http://qd.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://mu.haigaiapp.cn

s"值: $b"
来源：http://gc.szsharing.cn

[T54] Scala：集合映射
来源：http://ii.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://gt.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://qw.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cf.hnjuh.cn

[T56] Scala：样例类
来源：http://ik.panjiajie.cn

case class User(name: String, age: Int)
来源：http://hp.nszjky.cn

[T57] Scala：模式匹配
来源：http://zp.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yi.nszjky.cn

[T58] Scala：函数定义
来源：http://eq.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zy.shxzskj.cn

[T59] Scala：循环
来源：http://vq.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://dg.shxzskj.cn

[T60] Scala：折叠
来源：http://mw.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://el.asd995.cn

================================================================================
来源：http://fb.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cd.shxzskj.cn

================================================================================
来源：http://mc.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://cr.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nw.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://lm.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yz.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://ug.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ow.asd995.cn

[U04] Py：变量调试打印
来源：http://lu.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mk.colortex.cn

[U05] Py：列表去重且保序
来源：http://ph.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://tg.nicolike.cn

[U06] Py：合并两个字典
来源：http://az.muxihuayi.cn

{**a, **b}
来源：http://sc.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://bf.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://od.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://mj.wgjwhj.cn

[y for x in nested for y in x]
来源：http://wc.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://iy.521024.cn

max(d, key=d.get)
来源：http://up.nicolike.cn

[U10] Py：按值排序字典
来源：http://mk.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ys.521024.cn

[U11] Py：生成器表达式
来源：http://oa.colortex.cn

(x * 2 for x in arr)
来源：http://cn.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rd.521024.cn

Counter(arr).most_common(3)
来源：http://si.shxzskj.cn

[U13] Py：固定长度队列
来源：http://mg.shtwfgs.cn

deque(maxlen=10)
来源：http://mw.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://bm.nszjky.cn

defaultdict(list)
来源：http://ce.nszjky.cn

[U15] Py：高精度计时
来源：http://jz.nszjky.cn

t = time.perf_counter()
来源：http://wa.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://ck.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zn.nicolike.cn

[U17] Py：初始化日志
来源：http://xb.hahajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://sp.shtwfgs.cn

[U18] Py：预编译正则
来源：http://ct.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://hf.bookmarksfly.cn


<!-- 参考信息 -->