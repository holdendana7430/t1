代发 wailian999

split -l 1000 big.log part_
来源：http://yp.huixinmuqiang.cn

[R74] 批量重命名
来源：http://rz.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vb.chemitech.net.cn

[R75] 导出环境变量
来源：http://az.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://ak.shxzskj.cn

[R76] 使用临时文件
来源：http://ud.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cn.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://il.asd995.cn

read -rp "请输入: " ans
来源：http://ne.wgjwhj.cn

[R78] 交互式菜单
来源：http://dp.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bo.yuexingan06.cn

[R79] 解析命令行选项
来源：http://wm.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bg.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://dn.nszjky.cn

time ./run.sh
来源：http://fc.huixinmuqiang.cn

================================================================================
来源：http://fc.9csxet.cn

S. C / C++ 专题
来源：http://jz.huixinmuqiang.cn

================================================================================
来源：http://xf.panjiajie.cn

[S01] C：Hello World
来源：http://hg.asd995.cn

#include <stdio.h>
来源：http://tx.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://st.521024.cn

[S02] C：变量与格式化输出
来源：http://wf.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://dc.hnjuh.cn

[S03] C：读入整数
来源：http://ab.newstarts.cn

int x; scanf("%d", &x);
来源：http://iw.nszjky.cn

[S04] C：字符串复制
来源：http://jv.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jo.9csxet.cn

[S05] C：字符串长度
来源：http://kx.panjiajie.cn

strlen(s)
来源：http://ua.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://pu.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://md.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://ba.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wh.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://ep.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lh.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://hp.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sn.gzmigu.cn

[S10] C：指针与解引用
来源：http://vv.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://dl.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://vf.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://as.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ou.jianghongdianzi.cn

fclose(f);
来源：http://oq.lnxyls.cn

[S12] C：写文件
来源：http://pn.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dk.huanxung.cn

[S13] C：宏定义
来源：http://gn.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hk.panjiajie.cn

[S14] C：枚举
来源：http://ae.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://au.9csxet.cn

[S15] C：类型转换
来源：http://nx.wgjwhj.cn

(double) a / b
来源：http://oy.huixiangedu.cn

[S16] C：位操作置位
来源：http://dw.jianghongdianzi.cn

x |= (1 << 3);
来源：http://zm.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://my.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fg.huixiangedu.cn

[S18] C：命令行参数
来源：http://si.panjiajie.cn

int main(int argc, char **argv)
来源：http://vz.nszjky.cn

[S19] C：快速排序
来源：http://kv.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wy.jctech888.com.cn

[S20] C：二分查找
来源：http://sb.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bo.nszjky.cn

[S21] C：字符类别判断
来源：http://wf.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ui.nszjky.cn

[S22] C：字符串转数字
来源：http://ym.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zh.521024.cn

[S23] C：随机数
来源：http://ja.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pg.521024.cn

[S24] C：获取本地时间
来源：http://bn.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nf.huanxung.cn

[S25] C：内存拷贝
来源：http://bz.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://ij.wgjwhj.cn

[S26] C：内存清零
来源：http://vc.nszjky.cn

memset(a, 0, sizeof a);
来源：http://ao.gzmigu.cn

[S27] C：定义常量
来源：http://xc.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://zq.huixinmuqiang.cn

[S28] C：静态变量
来源：http://eb.bjjhwx.cn

static int counter = 0;
来源：http://aj.szsharing.cn

[S29] C：变参函数
来源：http://rq.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nc.szxytkj.cn

[S30] C：头文件保护
来源：http://qf.jctech888.com.cn

#ifndef X_H
来源：http://tp.szsharing.cn

#define X_H
来源：http://vp.wgjwhj.cn

#endif
来源：http://rf.newstarts.cn

[S31] C++：Hello World
来源：http://op.szsharing.cn

#include <iostream>
来源：http://pv.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://mz.huixiangedu.cn

[S32] C++：字符串
来源：http://ip.521024.cn

std::string s = "hi";  s += "!";
来源：http://vv.nicolike.cn

[S33] C++：vector 增删
来源：http://mc.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fh.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://rx.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://pp.haigaiapp.cn

[S35] C++：map
来源：http://jj.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zs.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://bu.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vb.hnjuh.cn

[S37] C++：set
来源：http://mj.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://en.521024.cn

[S38] C++：排序
来源：http://ci.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://cy.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://kt.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fh.colortex.cn

[S40] C++：查找元素
来源：http://pf.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ba.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://ey.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ve.huanxung.cn

[S42] C++：继承与虚函数
来源：http://kp.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://ob.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://gr.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://fw.bjjhwx.cn

[S44] C++：引用传参
来源：http://gd.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://kn.nszjky.cn

[S45] C++：lambda
来源：http://to.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mm.haigaiapp.cn

[S46] C++：函数模板
来源：http://rj.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jh.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://zf.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jq.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://my.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dl.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://ed.huanxung.cn

[S49] C++：写文件
来源：http://ad.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rt.asd995.cn

[S50] C++：格式化数字
来源：http://pk.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ex.nszjky.cn

[S51] C++：显式类型转换
来源：http://oc.wgjwhj.cn

static_cast<double>(a) / b
来源：http://gh.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://nt.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://av.asd995.cn

[S53] C++：移动语义
来源：http://qi.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://fu.chemitech.net.cn

[S54] C++：异常处理
来源：http://vw.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ja.szsharing.cn

[S55] C++：结构化绑定
来源：http://wp.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bd.wgjwhj.cn

[S56] C++：optional
来源：http://cc.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bj.chemitech.net.cn

[S57] C++：编译期常量
来源：http://mx.9csxet.cn

constexpr int N = 10;
来源：http://jw.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://eb.521024.cn

namespace ns { int f() { return 1; } }
来源：http://gb.bookmarksfly.cn

[S59] C++：静态断言
来源：http://vx.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pt.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://kv.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hx.szsharing.cn

================================================================================
来源：http://bn.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://si.szsharing.cn

================================================================================
来源：http://im.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://zb.chemitech.net.cn

println("Hello")
来源：http://ta.newstarts.cn

[T02] Kotlin：变量
来源：http://eo.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ru.521024.cn

[T03] Kotlin：字符串模板
来源：http://ko.szsharing.cn

"值: $b"
来源：http://kq.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://ep.huanxung.cn

val n: String? = null;  n?.length
来源：http://nd.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://kc.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vv.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://lw.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lb.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://yz.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uo.huanxung.cn

[T08] Kotlin：数据类
来源：http://jc.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://ey.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://kt.521024.cn

fun String.exclaim() = this + "!"
来源：http://iy.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://zw.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xe.shxzukj.cn

[T11] Kotlin：协程
来源：http://ad.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uy.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://bg.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://mg.colortex.cn

[T13] Kotlin：只读 Map
来源：http://gd.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://us.newstarts.cn

[T14] Kotlin：循环
来源：http://sh.lnxyls.cn

for (i in 1..10) println(i)
来源：http://nb.lnxyls.cn

[T15] Kotlin：接口
来源：http://jt.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://ca.shtwfgs.cn

[T16] Swift：Hello World
来源：http://bb.chemitech.net.cn

print("Hello")
来源：http://nb.shxzukj.cn

[T17] Swift：变量与常量
来源：http://fr.shxzskj.cn

var a = 1;  let b = 2
来源：http://de.newstarts.cn

[T18] Swift：字符串插值
来源：http://xp.szxytkj.cn

"值: \(b)"
来源：http://yx.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ym.shxzukj.cn

if let n = opt { print(n) }
来源：http://bu.shxzskj.cn

[T20] Swift：数组操作
来源：http://lj.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vr.gzmigu.cn

[T21] Swift：遍历
来源：http://ci.szsharing.cn

for x in a { print(x) }
来源：http://yl.yuntaijiaju.cn

[T22] Swift：字典
来源：http://pz.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fa.wgjwhj.cn

[T23] Swift：函数
来源：http://qz.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ik.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ay.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://or.haigaiapp.cn

[T25] Swift：结构体
来源：http://nj.colortex.cn

struct P { var x: Int }
来源：http://gb.haigaiapp.cn

[T26] Swift：类与重写
来源：http://vm.521024.cn

class A: Base { override func f() {} }
来源：http://ra.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://rd.521024.cn

do { try f() } catch { print(error) }
来源：http://oi.colortex.cn

[T28] Swift：枚举
来源：http://ai.jctech888.com.cn

enum Color { case red, green }
来源：http://cq.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ux.szxytkj.cn

guard let x = opt else { return }
来源：http://lp.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ju.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://mc.chemitech.net.cn

[T31] Lua：Hello World
来源：http://tp.szxytkj.cn

print("Hello")
来源：http://iv.shxzskj.cn

[T32] Lua：局部变量
来源：http://ut.asd995.cn

local a = 1
来源：http://so.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://se.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ar.newstarts.cn

[T34] Lua：遍历表
来源：http://ht.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hs.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://dd.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://zc.nszjky.cn

[T36] Lua：函数
来源：http://gc.wgjwhj.cn

function add(a, b) return a + b end
来源：http://nd.hahajie.cn

[T37] Lua：字符串拼接
来源：http://lp.yuexingan06.cn

"a" .. "b"
来源：http://kj.shxzukj.cn

[T38] Lua：条件
来源：http://yd.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://pw.shxzukj.cn

[T39] Lua：模式匹配
来源：http://ia.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://id.huixinmuqiang.cn

[T40] Lua：元表
来源：http://lu.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://fm.shxzukj.cn

[T41] Perl：Hello World
来源：http://nm.huixiangedu.cn

print "Hello\n";
来源：http://rr.newstarts.cn

[T42] Perl：变量类型
来源：http://pd.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xo.9csxet.cn

[T43] Perl：字符串插值
来源：http://hw.shtwfgs.cn

"值: $a"
来源：http://kv.bjjhwx.cn

[T44] Perl：条件
来源：http://ac.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://gk.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://fl.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://np.nszjky.cn

[T46] Perl：哈希操作
来源：http://om.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fm.lnxyls.cn

[T47] Perl：正则捕获
来源：http://hs.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sx.szxytkj.cn

[T48] Perl：正则替换
来源：http://de.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://ht.shxzskj.cn

[T49] Perl：函数
来源：http://pa.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ia.huanxung.cn

[T50] Perl：逐行读文件
来源：http://ut.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qf.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://ag.muxihuayi.cn

[T51] Scala：Hello World
来源：http://oi.shxzskj.cn

println("Hello")
来源：http://ly.newstarts.cn

[T52] Scala：变量
来源：http://dh.shxzskj.cn

val a = 1;  var b = 2
来源：http://vj.panjiajie.cn

[T53] Scala：字符串插值
来源：http://wm.yuexingan06.cn

s"值: $b"
来源：http://fa.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://qf.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://ug.hnjuh.cn

[T55] Scala：集合过滤
来源：http://xz.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sv.bjjhwx.cn

[T56] Scala：样例类
来源：http://af.lnxyls.cn

case class User(name: String, age: Int)
来源：http://fi.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://of.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qe.bjjhwx.cn

[T58] Scala：函数定义
来源：http://mj.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ei.chemitech.net.cn

[T59] Scala：循环
来源：http://ui.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://bs.szsharing.cn

[T60] Scala：折叠
来源：http://ie.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bs.huanxung.cn

================================================================================
来源：http://qx.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lt.huixinmuqiang.cn

================================================================================
来源：http://qt.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://kc.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://do.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://af.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://an.asd995.cn

[U03] Py：加载 .env 配置
来源：http://lx.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mk.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://ve.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://an.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://ya.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://cf.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://cp.szxytkj.cn

{**a, **b}
来源：http://je.asd995.cn

[U07] Py：反转字典键值
来源：http://wa.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://ji.521024.cn

[U08] Py：展平二维列表
来源：http://ai.jctech888.com.cn

[y for x in nested for y in x]
来源：http://kd.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://th.jctech888.com.cn

max(d, key=d.get)
来源：http://xs.hahajie.cn

[U10] Py：按值排序字典
来源：http://nx.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dz.gzmigu.cn

[U11] Py：生成器表达式
来源：http://ed.haigaiapp.cn

(x * 2 for x in arr)
来源：http://er.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wo.lnxyls.cn

Counter(arr).most_common(3)
来源：http://ql.newstarts.cn

[U13] Py：固定长度队列
来源：http://lm.yuexingan06.cn

deque(maxlen=10)
来源：http://nw.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://ga.shxzskj.cn

defaultdict(list)
来源：http://ug.521024.cn


<!-- 参考信息 -->