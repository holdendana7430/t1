代发 wailian999

split -l 1000 big.log part_
来源：http://ao.yuntaijiaju.cn

[R74] 批量重命名
来源：http://tl.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iy.hnjuh.cn

[R75] 导出环境变量
来源：http://us.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://yw.colortex.cn

[R76] 使用临时文件
来源：http://od.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zg.wgjwhj.cn

[R77] 读取用户输入
来源：http://ob.szsharing.cn

read -rp "请输入: " ans
来源：http://oc.asd995.cn

[R78] 交互式菜单
来源：http://ap.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gh.hahajie.cn

[R79] 解析命令行选项
来源：http://ow.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pq.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://ks.szsharing.cn

time ./run.sh
来源：http://vy.shtwfgs.cn

================================================================================
来源：http://nz.huanxung.cn

S. C / C++ 专题
来源：http://vd.bjjhwx.cn

================================================================================
来源：http://xg.colortex.cn

[S01] C：Hello World
来源：http://gd.szsharing.cn

#include <stdio.h>
来源：http://vo.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ng.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://ls.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://bp.huixiangedu.cn

[S03] C：读入整数
来源：http://gz.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://xi.521024.cn

[S04] C：字符串复制
来源：http://iv.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oj.nicolike.cn

[S05] C：字符串长度
来源：http://sm.colortex.cn

strlen(s)
来源：http://fp.muxihuayi.cn

[S06] C：字符串比较
来源：http://jm.colortex.cn

strcmp(a, b) == 0
来源：http://bk.colortex.cn

[S07] C：数组遍历求和
来源：http://xt.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eu.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://yx.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pa.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://lb.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gs.wgjwhj.cn

[S10] C：指针与解引用
来源：http://ih.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://as.nicolike.cn

[S11] C：逐行读文件
来源：http://ax.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://go.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nf.huixinmuqiang.cn

fclose(f);
来源：http://vi.newstarts.cn

[S12] C：写文件
来源：http://wd.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zr.lnxyls.cn

[S13] C：宏定义
来源：http://gb.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://st.hahajie.cn

[S14] C：枚举
来源：http://zb.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://ej.hahajie.cn

[S15] C：类型转换
来源：http://ta.haigaiapp.cn

(double) a / b
来源：http://zk.muxihuayi.cn

[S16] C：位操作置位
来源：http://jv.bookmarksfly.cn

x |= (1 << 3);
来源：http://te.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://eg.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ef.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://md.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://bg.jianghongdianzi.cn

[S19] C：快速排序
来源：http://ot.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ed.521024.cn

[S20] C：二分查找
来源：http://iy.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iw.nszjky.cn

[S21] C：字符类别判断
来源：http://hh.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jl.521024.cn

[S22] C：字符串转数字
来源：http://dx.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kt.nicolike.cn

[S23] C：随机数
来源：http://vf.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qk.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ci.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://to.yuexingan06.cn

[S25] C：内存拷贝
来源：http://fd.shxzskj.cn

memcpy(dst, src, n);
来源：http://mv.lnxyls.cn

[S26] C：内存清零
来源：http://vt.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://fk.521024.cn

[S27] C：定义常量
来源：http://rt.asd995.cn

const double PI = 3.14159;
来源：http://ez.huixiangedu.cn

[S28] C：静态变量
来源：http://xw.lnxyls.cn

static int counter = 0;
来源：http://zq.gzmigu.cn

[S29] C：变参函数
来源：http://wa.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hk.hnjuh.cn

[S30] C：头文件保护
来源：http://ud.shtwfgs.cn

#ifndef X_H
来源：http://wv.bjjhwx.cn

#define X_H
来源：http://qw.jianghongdianzi.cn

#endif
来源：http://ua.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://jb.jctech888.com.cn

#include <iostream>
来源：http://at.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://az.muxihuayi.cn

[S32] C++：字符串
来源：http://oa.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://qo.huixiangedu.cn

[S33] C++：vector 增删
来源：http://le.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://um.colortex.cn

[S34] C++：遍历 vector
来源：http://bz.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://jt.521024.cn

[S35] C++：map
来源：http://ow.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zj.hahajie.cn

[S36] C++：unordered_map
来源：http://ks.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ml.yuexingan06.cn

[S37] C++：set
来源：http://gc.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wy.colortex.cn

[S38] C++：排序
来源：http://we.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://vd.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://ay.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lf.shtwfgs.cn

[S40] C++：查找元素
来源：http://ox.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nm.huanxung.cn

[S41] C++：类与构造函数
来源：http://si.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ml.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://lk.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://ab.newstarts.cn

[S43] C++：智能指针
来源：http://uk.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://vl.shxzskj.cn

[S44] C++：引用传参
来源：http://jm.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://hc.jctech888.com.cn

[S45] C++：lambda
来源：http://mq.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ig.shxzukj.cn

[S46] C++：函数模板
来源：http://il.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hb.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://gf.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ck.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://ev.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yy.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://it.huanxung.cn

[S49] C++：写文件
来源：http://dq.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iw.shxzskj.cn

[S50] C++：格式化数字
来源：http://cx.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vq.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://vo.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ko.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://qa.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://vj.colortex.cn

[S53] C++：移动语义
来源：http://jp.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://iv.jctech888.com.cn

[S54] C++：异常处理
来源：http://xr.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hy.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://vy.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://en.lnxyls.cn

[S56] C++：optional
来源：http://ua.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bz.gzmigu.cn

[S57] C++：编译期常量
来源：http://cc.shtwfgs.cn

constexpr int N = 10;
来源：http://tw.wgjwhj.cn

[S58] C++：命名空间
来源：http://xr.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://fz.jctech888.com.cn

[S59] C++：静态断言
来源：http://up.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xi.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://qt.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://na.jianghongdianzi.cn

================================================================================
来源：http://ui.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bk.muxihuayi.cn

================================================================================
来源：http://qa.nszjky.cn

[T01] Kotlin：Hello World
来源：http://li.bookmarksfly.cn

println("Hello")
来源：http://sc.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ya.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ec.521024.cn

[T03] Kotlin：字符串模板
来源：http://iq.yuexingan06.cn

"值: $b"
来源：http://di.shxzskj.cn

[T04] Kotlin：空安全
来源：http://tm.huanxung.cn

val n: String? = null;  n?.length
来源：http://pe.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://hk.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mw.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://re.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yo.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://kk.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fs.gzmigu.cn

[T08] Kotlin：数据类
来源：http://yg.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://vl.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://kg.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://zu.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://hq.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dc.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ka.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nz.huanxung.cn

[T12] Kotlin：解构声明
来源：http://jc.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://bv.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://go.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://ne.yuexingan06.cn

[T14] Kotlin：循环
来源：http://md.gzmigu.cn

for (i in 1..10) println(i)
来源：http://tp.yuexingan06.cn

[T15] Kotlin：接口
来源：http://dx.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://lm.nszjky.cn

[T16] Swift：Hello World
来源：http://zb.9csxet.cn

print("Hello")
来源：http://gh.hnjuh.cn

[T17] Swift：变量与常量
来源：http://jn.szsharing.cn

var a = 1;  let b = 2
来源：http://xk.hnjuh.cn

[T18] Swift：字符串插值
来源：http://ua.huanxung.cn

"值: \(b)"
来源：http://up.521024.cn

[T19] Swift：可选绑定
来源：http://bu.asd995.cn

if let n = opt { print(n) }
来源：http://ao.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://hj.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ma.newstarts.cn

[T21] Swift：遍历
来源：http://ow.huanxung.cn

for x in a { print(x) }
来源：http://cg.lnxyls.cn

[T22] Swift：字典
来源：http://dw.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jo.hahajie.cn

[T23] Swift：函数
来源：http://jc.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lq.yuexingan06.cn

[T24] Swift：闭包
来源：http://kr.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://de.asd995.cn

[T25] Swift：结构体
来源：http://lp.wgjwhj.cn

struct P { var x: Int }
来源：http://ol.chemitech.net.cn

[T26] Swift：类与重写
来源：http://mp.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://gv.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://we.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://qv.hnjuh.cn

[T28] Swift：枚举
来源：http://rw.jianghongdianzi.cn

enum Color { case red, green }
来源：http://ng.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://iu.shxzskj.cn

guard let x = opt else { return }
来源：http://cx.panjiajie.cn

[T30] Swift：协议
来源：http://jd.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://rk.colortex.cn

[T31] Lua：Hello World
来源：http://gr.hahajie.cn

print("Hello")
来源：http://ec.szsharing.cn

[T32] Lua：局部变量
来源：http://wu.shtwfgs.cn

local a = 1
来源：http://ik.shxzukj.cn

[T33] Lua：表（数组）
来源：http://ek.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zt.bjjhwx.cn

[T34] Lua：遍历表
来源：http://ib.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ua.bjjhwx.cn

[T35] Lua：字典表
来源：http://nb.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://xu.shtwfgs.cn

[T36] Lua：函数
来源：http://ta.shxzukj.cn

function add(a, b) return a + b end
来源：http://ra.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://ed.panjiajie.cn

"a" .. "b"
来源：http://vy.521024.cn

[T38] Lua：条件
来源：http://hg.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://si.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://zp.shtwfgs.cn

string.find(s, "%d+")
来源：http://rn.shxzskj.cn

[T40] Lua：元表
来源：http://dy.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://zt.gzmigu.cn

[T41] Perl：Hello World
来源：http://ev.jianghongdianzi.cn

print "Hello\n";
来源：http://db.huanxung.cn

[T42] Perl：变量类型
来源：http://bo.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qq.szsharing.cn

[T43] Perl：字符串插值
来源：http://fj.lnxyls.cn

"值: $a"
来源：http://ng.haigaiapp.cn

[T44] Perl：条件
来源：http://up.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://rc.shxzukj.cn

[T45] Perl：数组遍历
来源：http://ja.colortex.cn

for my $x (@arr) { print $x; }
来源：http://vw.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://rn.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xk.panjiajie.cn

[T47] Perl：正则捕获
来源：http://on.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pv.nicolike.cn

[T48] Perl：正则替换
来源：http://ro.shxzskj.cn

$s =~ s/old/new/g;
来源：http://op.yuexingan06.cn

[T49] Perl：函数
来源：http://jp.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fz.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://mk.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yn.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://oo.newstarts.cn

[T51] Scala：Hello World
来源：http://cz.wgjwhj.cn

println("Hello")
来源：http://az.shxzskj.cn

[T52] Scala：变量
来源：http://nr.lnxyls.cn

val a = 1;  var b = 2
来源：http://rd.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://xy.yuexingan06.cn

s"值: $b"
来源：http://ld.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://jk.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://be.huanxung.cn

[T55] Scala：集合过滤
来源：http://fo.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bl.huanxung.cn

[T56] Scala：样例类
来源：http://js.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://xv.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://mf.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ix.newstarts.cn

[T58] Scala：函数定义
来源：http://fs.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pc.huanxung.cn

[T59] Scala：循环
来源：http://py.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://ty.shxzskj.cn

[T60] Scala：折叠
来源：http://yf.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nn.jctech888.com.cn

================================================================================
来源：http://qf.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iy.bjjhwx.cn

================================================================================
来源：http://vj.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://wf.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gm.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://ru.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zg.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://pv.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ob.nicolike.cn

[U04] Py：变量调试打印
来源：http://bd.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xg.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://cj.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://wn.nszjky.cn

[U06] Py：合并两个字典
来源：http://bt.bookmarksfly.cn

{**a, **b}
来源：http://qd.lnxyls.cn

[U07] Py：反转字典键值
来源：http://rs.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://bt.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://zc.haigaiapp.cn

[y for x in nested for y in x]
来源：http://nk.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ie.szxytkj.cn

max(d, key=d.get)
来源：http://yx.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://nc.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jl.9csxet.cn

[U11] Py：生成器表达式
来源：http://bk.yuexingan06.cn

(x * 2 for x in arr)
来源：http://gh.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lm.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://ze.panjiajie.cn

[U13] Py：固定长度队列
来源：http://mg.hnjuh.cn

deque(maxlen=10)
来源：http://mj.hahajie.cn

[U14] Py：分组收集到列表
来源：http://gu.jctech888.com.cn

defaultdict(list)
来源：http://me.nszjky.cn


<!-- 参考信息 -->