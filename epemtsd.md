代发 wailian999

split -l 1000 big.log part_
来源：http://tt.szsharing.cn

[R74] 批量重命名
来源：http://uk.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lu.hnjuh.cn

[R75] 导出环境变量
来源：http://yg.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://lq.chemitech.net.cn

[R76] 使用临时文件
来源：http://nb.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ye.bjjhwx.cn

[R77] 读取用户输入
来源：http://up.nicolike.cn

read -rp "请输入: " ans
来源：http://ar.yuexingan06.cn

[R78] 交互式菜单
来源：http://zz.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mp.nicolike.cn

[R79] 解析命令行选项
来源：http://wj.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ne.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://im.huanxung.cn

time ./run.sh
来源：http://us.shtwfgs.cn

================================================================================
来源：http://ct.nszjky.cn

S. C / C++ 专题
来源：http://ls.521024.cn

================================================================================
来源：http://hx.muxihuayi.cn

[S01] C：Hello World
来源：http://to.nszjky.cn

#include <stdio.h>
来源：http://oa.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pw.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://lw.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://go.gzmigu.cn

[S03] C：读入整数
来源：http://jd.panjiajie.cn

int x; scanf("%d", &x);
来源：http://lo.chemitech.net.cn

[S04] C：字符串复制
来源：http://bh.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mt.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://oq.yuexingan06.cn

strlen(s)
来源：http://db.colortex.cn

[S06] C：字符串比较
来源：http://pe.muxihuayi.cn

strcmp(a, b) == 0
来源：http://cx.shxzskj.cn

[S07] C：数组遍历求和
来源：http://ya.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xd.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://cl.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uy.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://aw.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wh.jctech888.com.cn

[S10] C：指针与解引用
来源：http://xg.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://yf.huixiangedu.cn

[S11] C：逐行读文件
来源：http://jh.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://du.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xc.newstarts.cn

fclose(f);
来源：http://ua.haigaiapp.cn

[S12] C：写文件
来源：http://gy.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aj.asd995.cn

[S13] C：宏定义
来源：http://vy.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lm.nicolike.cn

[S14] C：枚举
来源：http://iv.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://xw.wgjwhj.cn

[S15] C：类型转换
来源：http://xj.huixiangedu.cn

(double) a / b
来源：http://ce.shxzskj.cn

[S16] C：位操作置位
来源：http://vk.shxzukj.cn

x |= (1 << 3);
来源：http://pf.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://vc.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gy.bjjhwx.cn

[S18] C：命令行参数
来源：http://ej.szxytkj.cn

int main(int argc, char **argv)
来源：http://fd.shxzskj.cn

[S19] C：快速排序
来源：http://lk.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jp.panjiajie.cn

[S20] C：二分查找
来源：http://kp.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lk.nszjky.cn

[S21] C：字符类别判断
来源：http://cv.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://km.huixiangedu.cn

[S22] C：字符串转数字
来源：http://no.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nj.jianghongdianzi.cn

[S23] C：随机数
来源：http://tc.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bn.asd995.cn

[S24] C：获取本地时间
来源：http://qw.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ta.asd995.cn

[S25] C：内存拷贝
来源：http://rn.asd995.cn

memcpy(dst, src, n);
来源：http://vl.nicolike.cn

[S26] C：内存清零
来源：http://fb.asd995.cn

memset(a, 0, sizeof a);
来源：http://ps.muxihuayi.cn

[S27] C：定义常量
来源：http://ac.hahajie.cn

const double PI = 3.14159;
来源：http://sv.gzmigu.cn

[S28] C：静态变量
来源：http://ev.shxzskj.cn

static int counter = 0;
来源：http://ci.shxzskj.cn

[S29] C：变参函数
来源：http://ca.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ip.chemitech.net.cn

[S30] C：头文件保护
来源：http://hs.huixinmuqiang.cn

#ifndef X_H
来源：http://ni.521024.cn

#define X_H
来源：http://gn.panjiajie.cn

#endif
来源：http://iv.colortex.cn

[S31] C++：Hello World
来源：http://eo.jianghongdianzi.cn

#include <iostream>
来源：http://bs.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://qm.huixiangedu.cn

[S32] C++：字符串
来源：http://er.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://kl.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://db.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rn.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://tl.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://oh.shxzukj.cn

[S35] C++：map
来源：http://vn.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xi.yuexingan06.cn

[S36] C++：unordered_map
来源：http://vu.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lu.gzmigu.cn

[S37] C++：set
来源：http://dx.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uk.szsharing.cn

[S38] C++：排序
来源：http://ti.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://le.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://va.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wz.huixiangedu.cn

[S40] C++：查找元素
来源：http://tn.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tf.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://la.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qb.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://sb.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://yf.gzmigu.cn

[S43] C++：智能指针
来源：http://nz.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://gi.newstarts.cn

[S44] C++：引用传参
来源：http://bm.colortex.cn

void inc(int &x) { ++x; }
来源：http://vq.yuntaijiaju.cn

[S45] C++：lambda
来源：http://tz.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://et.shtwfgs.cn

[S46] C++：函数模板
来源：http://qu.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tl.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://vb.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://la.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://eg.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vo.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://lm.haigaiapp.cn

[S49] C++：写文件
来源：http://bt.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sq.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://fp.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nq.szxytkj.cn

[S51] C++：显式类型转换
来源：http://ho.colortex.cn

static_cast<double>(a) / b
来源：http://yk.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://lq.asd995.cn

int size() const noexcept { return n_; }
来源：http://hp.muxihuayi.cn

[S53] C++：移动语义
来源：http://nm.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ed.nszjky.cn

[S54] C++：异常处理
来源：http://im.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vq.521024.cn

[S55] C++：结构化绑定
来源：http://eo.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fw.szsharing.cn

[S56] C++：optional
来源：http://rq.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wk.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://wq.asd995.cn

constexpr int N = 10;
来源：http://nv.asd995.cn

[S58] C++：命名空间
来源：http://aq.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://nt.jctech888.com.cn

[S59] C++：静态断言
来源：http://fh.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://en.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://vz.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yt.shxzukj.cn

================================================================================
来源：http://lm.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://db.szxytkj.cn

================================================================================
来源：http://xq.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://qn.asd995.cn

println("Hello")
来源：http://ag.lnxyls.cn

[T02] Kotlin：变量
来源：http://ea.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://of.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://wk.shxzukj.cn

"值: $b"
来源：http://wa.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://vb.hahajie.cn

val n: String? = null;  n?.length
来源：http://ri.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://qn.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://we.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://gx.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://en.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://go.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jy.gzmigu.cn

[T08] Kotlin：数据类
来源：http://po.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://bh.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://fg.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://wt.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://fb.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jw.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://er.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hu.colortex.cn

[T12] Kotlin：解构声明
来源：http://dp.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://ud.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://ka.521024.cn

val m = mapOf("a" to 1)
来源：http://qp.hahajie.cn

[T14] Kotlin：循环
来源：http://xf.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://rs.chemitech.net.cn

[T15] Kotlin：接口
来源：http://gc.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://gh.gzmigu.cn

[T16] Swift：Hello World
来源：http://at.muxihuayi.cn

print("Hello")
来源：http://pz.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://qo.yuexingan06.cn

var a = 1;  let b = 2
来源：http://zs.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://pn.nicolike.cn

"值: \(b)"
来源：http://tq.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://zb.shxzukj.cn

if let n = opt { print(n) }
来源：http://cw.asd995.cn

[T20] Swift：数组操作
来源：http://ec.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ld.huanxung.cn

[T21] Swift：遍历
来源：http://iq.hahajie.cn

for x in a { print(x) }
来源：http://vj.asd995.cn

[T22] Swift：字典
来源：http://po.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://va.hahajie.cn

[T23] Swift：函数
来源：http://qm.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mk.hahajie.cn

[T24] Swift：闭包
来源：http://bq.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uu.asd995.cn

[T25] Swift：结构体
来源：http://lb.wgjwhj.cn

struct P { var x: Int }
来源：http://rn.nszjky.cn

[T26] Swift：类与重写
来源：http://po.szsharing.cn

class A: Base { override func f() {} }
来源：http://xp.bjjhwx.cn

[T27] Swift：错误处理
来源：http://ks.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://dm.hnjuh.cn

[T28] Swift：枚举
来源：http://dx.shxzukj.cn

enum Color { case red, green }
来源：http://nw.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://oz.shxzukj.cn

guard let x = opt else { return }
来源：http://ra.jianghongdianzi.cn

[T30] Swift：协议
来源：http://pl.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://wa.shxzskj.cn

[T31] Lua：Hello World
来源：http://oj.9csxet.cn

print("Hello")
来源：http://ct.wgjwhj.cn

[T32] Lua：局部变量
来源：http://oo.bjjhwx.cn

local a = 1
来源：http://iq.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://dp.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wq.jctech888.com.cn

[T34] Lua：遍历表
来源：http://vr.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ii.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://yy.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://cc.nszjky.cn

[T36] Lua：函数
来源：http://cr.szsharing.cn

function add(a, b) return a + b end
来源：http://zs.nszjky.cn

[T37] Lua：字符串拼接
来源：http://ez.hnjuh.cn

"a" .. "b"
来源：http://jj.jctech888.com.cn

[T38] Lua：条件
来源：http://zi.colortex.cn

if x > 0 then print("正") end
来源：http://gx.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://wp.haigaiapp.cn

string.find(s, "%d+")
来源：http://gt.haigaiapp.cn

[T40] Lua：元表
来源：http://ko.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://zo.gzmigu.cn

[T41] Perl：Hello World
来源：http://pr.haigaiapp.cn

print "Hello\n";
来源：http://kb.gzmigu.cn

[T42] Perl：变量类型
来源：http://nr.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ix.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://yr.yuntaijiaju.cn

"值: $a"
来源：http://wy.bjjhwx.cn

[T44] Perl：条件
来源：http://bj.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://tr.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://eg.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://et.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://gu.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wy.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://hf.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gs.shxzskj.cn

[T48] Perl：正则替换
来源：http://bv.gzmigu.cn

$s =~ s/old/new/g;
来源：http://za.yuntaijiaju.cn

[T49] Perl：函数
来源：http://ix.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hy.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://ha.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mm.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://bz.asd995.cn

[T51] Scala：Hello World
来源：http://go.szxytkj.cn

println("Hello")
来源：http://pz.gzmigu.cn

[T52] Scala：变量
来源：http://qt.shxzukj.cn

val a = 1;  var b = 2
来源：http://ev.nszjky.cn

[T53] Scala：字符串插值
来源：http://ea.shtwfgs.cn

s"值: $b"
来源：http://wa.huanxung.cn

[T54] Scala：集合映射
来源：http://ri.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://sr.521024.cn

[T55] Scala：集合过滤
来源：http://he.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iu.yuexingan06.cn

[T56] Scala：样例类
来源：http://is.nszjky.cn

case class User(name: String, age: Int)
来源：http://jd.nszjky.cn

[T57] Scala：模式匹配
来源：http://kk.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ey.jctech888.com.cn

[T58] Scala：函数定义
来源：http://bw.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mk.newstarts.cn

[T59] Scala：循环
来源：http://lk.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://rv.colortex.cn

[T60] Scala：折叠
来源：http://pn.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cv.lnxyls.cn

================================================================================
来源：http://mz.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hy.huixiangedu.cn

================================================================================
来源：http://bq.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://uu.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oa.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://lf.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dw.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://zh.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mg.colortex.cn

[U04] Py：变量调试打印
来源：http://ny.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vd.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://wr.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://of.nicolike.cn

[U06] Py：合并两个字典
来源：http://ub.jianghongdianzi.cn

{**a, **b}
来源：http://is.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://nc.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://ma.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://xm.9csxet.cn

[y for x in nested for y in x]
来源：http://cq.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://wb.szsharing.cn

max(d, key=d.get)
来源：http://nl.szsharing.cn

[U10] Py：按值排序字典
来源：http://tl.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wy.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://ap.szsharing.cn

(x * 2 for x in arr)
来源：http://je.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xd.nszjky.cn

Counter(arr).most_common(3)
来源：http://va.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://pw.muxihuayi.cn

deque(maxlen=10)
来源：http://fv.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://kx.shxzskj.cn

defaultdict(list)
来源：http://xz.nszjky.cn


<!-- 参考信息 -->