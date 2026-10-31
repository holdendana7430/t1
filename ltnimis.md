代发 wailian999

split -l 1000 big.log part_
来源：http://mw.jctech888.com.cn

[R74] 批量重命名
来源：http://na.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sv.panjiajie.cn

[R75] 导出环境变量
来源：http://if.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://bt.gzmigu.cn

[R76] 使用临时文件
来源：http://gv.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dy.9csxet.cn

[R77] 读取用户输入
来源：http://pf.haigaiapp.cn

read -rp "请输入: " ans
来源：http://oz.panjiajie.cn

[R78] 交互式菜单
来源：http://bt.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xz.gzmigu.cn

[R79] 解析命令行选项
来源：http://pb.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://be.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://hz.newstarts.cn

time ./run.sh
来源：http://ac.huanxung.cn

================================================================================
来源：http://eb.hnjuh.cn

S. C / C++ 专题
来源：http://os.jianghongdianzi.cn

================================================================================
来源：http://uu.wgjwhj.cn

[S01] C：Hello World
来源：http://zx.gzmigu.cn

#include <stdio.h>
来源：http://md.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jp.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://lf.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://pa.haigaiapp.cn

[S03] C：读入整数
来源：http://wg.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://yy.wgjwhj.cn

[S04] C：字符串复制
来源：http://ty.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xj.nszjky.cn

[S05] C：字符串长度
来源：http://es.nicolike.cn

strlen(s)
来源：http://cy.gzmigu.cn

[S06] C：字符串比较
来源：http://vc.jctech888.com.cn

strcmp(a, b) == 0
来源：http://yi.9csxet.cn

[S07] C：数组遍历求和
来源：http://in.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yj.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://bp.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zf.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://zy.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pp.nicolike.cn

[S10] C：指针与解引用
来源：http://qo.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://xn.huixiangedu.cn

[S11] C：逐行读文件
来源：http://fm.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ch.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tf.bjjhwx.cn

fclose(f);
来源：http://cl.shxzskj.cn

[S12] C：写文件
来源：http://lx.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rm.haigaiapp.cn

[S13] C：宏定义
来源：http://pf.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xl.nszjky.cn

[S14] C：枚举
来源：http://iq.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://rd.haigaiapp.cn

[S15] C：类型转换
来源：http://fy.shxzukj.cn

(double) a / b
来源：http://kt.panjiajie.cn

[S16] C：位操作置位
来源：http://en.szxytkj.cn

x |= (1 << 3);
来源：http://wd.huanxung.cn

[S17] C：安全拼接字符串
来源：http://el.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qa.lnxyls.cn

[S18] C：命令行参数
来源：http://lj.panjiajie.cn

int main(int argc, char **argv)
来源：http://vm.huixinmuqiang.cn

[S19] C：快速排序
来源：http://jy.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ug.chemitech.net.cn

[S20] C：二分查找
来源：http://av.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vd.wgjwhj.cn

[S21] C：字符类别判断
来源：http://me.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bh.hahajie.cn

[S22] C：字符串转数字
来源：http://yq.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xb.wgjwhj.cn

[S23] C：随机数
来源：http://ml.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fe.hahajie.cn

[S24] C：获取本地时间
来源：http://vm.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dq.gzmigu.cn

[S25] C：内存拷贝
来源：http://vy.szxytkj.cn

memcpy(dst, src, n);
来源：http://qg.shxzskj.cn

[S26] C：内存清零
来源：http://tq.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://yf.asd995.cn

[S27] C：定义常量
来源：http://cq.asd995.cn

const double PI = 3.14159;
来源：http://vv.lnxyls.cn

[S28] C：静态变量
来源：http://xs.szsharing.cn

static int counter = 0;
来源：http://st.wgjwhj.cn

[S29] C：变参函数
来源：http://ac.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gp.shxzskj.cn

[S30] C：头文件保护
来源：http://ug.wgjwhj.cn

#ifndef X_H
来源：http://zq.nicolike.cn

#define X_H
来源：http://iv.lnxyls.cn

#endif
来源：http://pe.szsharing.cn

[S31] C++：Hello World
来源：http://qm.hnjuh.cn

#include <iostream>
来源：http://oo.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://yn.9csxet.cn

[S32] C++：字符串
来源：http://lw.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://cd.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://eo.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qr.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://jc.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://vp.shxzskj.cn

[S35] C++：map
来源：http://yo.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://im.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://mq.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mn.521024.cn

[S37] C++：set
来源：http://yr.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qr.nszjky.cn

[S38] C++：排序
来源：http://si.asd995.cn

std::sort(v.begin(), v.end());
来源：http://bd.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://at.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wr.huixiangedu.cn

[S40] C++：查找元素
来源：http://bz.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mb.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://rd.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://om.521024.cn

[S42] C++：继承与虚函数
来源：http://zm.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://ea.hnjuh.cn

[S43] C++：智能指针
来源：http://mi.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://nv.muxihuayi.cn

[S44] C++：引用传参
来源：http://pj.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://pw.wgjwhj.cn

[S45] C++：lambda
来源：http://ao.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vr.asd995.cn

[S46] C++：函数模板
来源：http://gn.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zw.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://rc.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bs.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ng.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://at.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://zn.bjjhwx.cn

[S49] C++：写文件
来源：http://tz.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dd.haigaiapp.cn

[S50] C++：格式化数字
来源：http://ap.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kg.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://gg.panjiajie.cn

static_cast<double>(a) / b
来源：http://zo.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://vv.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://ec.muxihuayi.cn

[S53] C++：移动语义
来源：http://qq.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ej.asd995.cn

[S54] C++：异常处理
来源：http://uq.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tr.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://po.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qo.huixinmuqiang.cn

[S56] C++：optional
来源：http://kn.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://he.shtwfgs.cn

[S57] C++：编译期常量
来源：http://ep.colortex.cn

constexpr int N = 10;
来源：http://dg.wgjwhj.cn

[S58] C++：命名空间
来源：http://lf.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://ml.huanxung.cn

[S59] C++：静态断言
来源：http://ug.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aj.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://rs.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vp.haigaiapp.cn

================================================================================
来源：http://pi.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fv.bjjhwx.cn

================================================================================
来源：http://pu.521024.cn

[T01] Kotlin：Hello World
来源：http://iv.9csxet.cn

println("Hello")
来源：http://fz.chemitech.net.cn

[T02] Kotlin：变量
来源：http://br.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cb.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://ir.shxzukj.cn

"值: $b"
来源：http://qu.521024.cn

[T04] Kotlin：空安全
来源：http://jh.9csxet.cn

val n: String? = null;  n?.length
来源：http://qz.colortex.cn

[T05] Kotlin：when 表达式
来源：http://av.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xc.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ad.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rh.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://dg.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fo.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://kv.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://qn.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://rl.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://hn.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://lj.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rb.nszjky.cn

[T11] Kotlin：协程
来源：http://sn.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nc.521024.cn

[T12] Kotlin：解构声明
来源：http://yu.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://pg.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://ok.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://qi.newstarts.cn

[T14] Kotlin：循环
来源：http://ed.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://lk.asd995.cn

[T15] Kotlin：接口
来源：http://ov.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://pe.haigaiapp.cn

[T16] Swift：Hello World
来源：http://sy.shxzskj.cn

print("Hello")
来源：http://bf.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://vx.muxihuayi.cn

var a = 1;  let b = 2
来源：http://ss.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://ul.szxytkj.cn

"值: \(b)"
来源：http://lh.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://wm.bjjhwx.cn

if let n = opt { print(n) }
来源：http://wn.haigaiapp.cn

[T20] Swift：数组操作
来源：http://tq.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dj.jctech888.com.cn

[T21] Swift：遍历
来源：http://lc.chemitech.net.cn

for x in a { print(x) }
来源：http://va.wgjwhj.cn

[T22] Swift：字典
来源：http://xd.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ve.jianghongdianzi.cn

[T23] Swift：函数
来源：http://ol.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gb.bookmarksfly.cn

[T24] Swift：闭包
来源：http://gv.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lx.yuexingan06.cn

[T25] Swift：结构体
来源：http://dt.asd995.cn

struct P { var x: Int }
来源：http://ko.bjjhwx.cn

[T26] Swift：类与重写
来源：http://ty.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://dx.jctech888.com.cn

[T27] Swift：错误处理
来源：http://px.nicolike.cn

do { try f() } catch { print(error) }
来源：http://qh.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://am.lnxyls.cn

enum Color { case red, green }
来源：http://uo.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://dz.shxzukj.cn

guard let x = opt else { return }
来源：http://jf.jianghongdianzi.cn

[T30] Swift：协议
来源：http://vk.521024.cn

protocol Shape { func area() -> Double }
来源：http://io.shxzukj.cn

[T31] Lua：Hello World
来源：http://fu.huixinmuqiang.cn

print("Hello")
来源：http://rm.521024.cn

[T32] Lua：局部变量
来源：http://cv.yuntaijiaju.cn

local a = 1
来源：http://go.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://nq.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ir.hnjuh.cn

[T34] Lua：遍历表
来源：http://ib.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://im.lnxyls.cn

[T35] Lua：字典表
来源：http://hh.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://lz.hnjuh.cn

[T36] Lua：函数
来源：http://ki.bjjhwx.cn

function add(a, b) return a + b end
来源：http://gi.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://jf.521024.cn

"a" .. "b"
来源：http://ww.hahajie.cn

[T38] Lua：条件
来源：http://wn.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://lz.szxytkj.cn

[T39] Lua：模式匹配
来源：http://tk.gzmigu.cn

string.find(s, "%d+")
来源：http://tz.gzmigu.cn

[T40] Lua：元表
来源：http://uk.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://hc.huanxung.cn

[T41] Perl：Hello World
来源：http://df.hahajie.cn

print "Hello\n";
来源：http://no.huixiangedu.cn

[T42] Perl：变量类型
来源：http://qh.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dw.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://ua.chemitech.net.cn

"值: $a"
来源：http://sy.newstarts.cn

[T44] Perl：条件
来源：http://bq.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://dh.szxytkj.cn

[T45] Perl：数组遍历
来源：http://kx.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ve.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://we.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lu.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://xh.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cr.9csxet.cn

[T48] Perl：正则替换
来源：http://sv.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://ks.hnjuh.cn

[T49] Perl：函数
来源：http://qd.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pe.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://gv.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dm.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://da.hahajie.cn

[T51] Scala：Hello World
来源：http://hl.asd995.cn

println("Hello")
来源：http://yf.colortex.cn

[T52] Scala：变量
来源：http://mf.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://ht.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://eg.shxzskj.cn

s"值: $b"
来源：http://yi.chemitech.net.cn

[T54] Scala：集合映射
来源：http://wn.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://yj.521024.cn

[T55] Scala：集合过滤
来源：http://yl.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gd.shxzukj.cn

[T56] Scala：样例类
来源：http://nd.szsharing.cn

case class User(name: String, age: Int)
来源：http://rw.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://ga.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qi.yuexingan06.cn

[T58] Scala：函数定义
来源：http://uv.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fh.nicolike.cn

[T59] Scala：循环
来源：http://qp.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://ia.szsharing.cn

[T60] Scala：折叠
来源：http://su.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iv.szsharing.cn

================================================================================
来源：http://bs.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ht.asd995.cn

================================================================================
来源：http://ig.asd995.cn

[U01] Py：创建虚拟环境
来源：http://gb.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uu.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://ga.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://me.asd995.cn

[U03] Py：加载 .env 配置
来源：http://qi.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gs.nszjky.cn

[U04] Py：变量调试打印
来源：http://er.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lw.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://co.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://kg.panjiajie.cn

[U06] Py：合并两个字典
来源：http://at.shxzskj.cn

{**a, **b}
来源：http://wl.shxzskj.cn

[U07] Py：反转字典键值
来源：http://ta.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://fi.szsharing.cn

[U08] Py：展平二维列表
来源：http://kh.haigaiapp.cn

[y for x in nested for y in x]
来源：http://dn.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://ot.yuexingan06.cn

max(d, key=d.get)
来源：http://bc.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://al.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xa.asd995.cn

[U11] Py：生成器表达式
来源：http://ad.newstarts.cn

(x * 2 for x in arr)
来源：http://vz.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ir.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://yt.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://pa.huixinmuqiang.cn

deque(maxlen=10)
来源：http://xm.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://bq.9csxet.cn

defaultdict(list)
来源：http://ud.colortex.cn


<!-- 参考信息 -->