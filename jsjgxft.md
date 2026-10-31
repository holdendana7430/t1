代发 wailian999

read -rp "请输入: " ans
来源：http://py.muxihuayi.cn

[R78] 交互式菜单
来源：http://va.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ja.hahajie.cn

[R79] 解析命令行选项
来源：http://pl.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wx.asd995.cn

[R80] 查看脚本执行耗时
来源：http://fx.chemitech.net.cn

time ./run.sh
来源：http://gf.bjjhwx.cn

================================================================================
来源：http://ie.hahajie.cn

S. C / C++ 专题
来源：http://tw.bookmarksfly.cn

================================================================================
来源：http://kl.lnxyls.cn

[S01] C：Hello World
来源：http://un.shtwfgs.cn

#include <stdio.h>
来源：http://yy.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xv.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://fn.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://zt.bookmarksfly.cn

[S03] C：读入整数
来源：http://yx.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://bv.shxzukj.cn

[S04] C：字符串复制
来源：http://uc.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xs.hahajie.cn

[S05] C：字符串长度
来源：http://ol.haigaiapp.cn

strlen(s)
来源：http://tj.szsharing.cn

[S06] C：字符串比较
来源：http://yj.huanxung.cn

strcmp(a, b) == 0
来源：http://bw.gzmigu.cn

[S07] C：数组遍历求和
来源：http://nx.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://js.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://hl.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sa.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://ai.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lf.nszjky.cn

[S10] C：指针与解引用
来源：http://rf.nszjky.cn

int *p = &a;  *p = 5;
来源：http://dg.jctech888.com.cn

[S11] C：逐行读文件
来源：http://zo.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://dz.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pf.521024.cn

fclose(f);
来源：http://bg.asd995.cn

[S12] C：写文件
来源：http://em.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qi.nszjky.cn

[S13] C：宏定义
来源：http://yn.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fv.yuexingan06.cn

[S14] C：枚举
来源：http://ps.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://ul.nszjky.cn

[S15] C：类型转换
来源：http://qt.lnxyls.cn

(double) a / b
来源：http://yq.nszjky.cn

[S16] C：位操作置位
来源：http://cb.muxihuayi.cn

x |= (1 << 3);
来源：http://sw.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://jg.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rm.muxihuayi.cn

[S18] C：命令行参数
来源：http://em.hahajie.cn

int main(int argc, char **argv)
来源：http://in.huanxung.cn

[S19] C：快速排序
来源：http://yx.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jg.shxzskj.cn

[S20] C：二分查找
来源：http://cj.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gg.nicolike.cn

[S21] C：字符类别判断
来源：http://qf.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hy.colortex.cn

[S22] C：字符串转数字
来源：http://dw.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qz.shxzskj.cn

[S23] C：随机数
来源：http://yh.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wf.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://dx.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ui.huixiangedu.cn

[S25] C：内存拷贝
来源：http://ua.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://kd.jianghongdianzi.cn

[S26] C：内存清零
来源：http://ll.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://um.panjiajie.cn

[S27] C：定义常量
来源：http://xm.lnxyls.cn

const double PI = 3.14159;
来源：http://iw.jianghongdianzi.cn

[S28] C：静态变量
来源：http://ob.lnxyls.cn

static int counter = 0;
来源：http://pe.yuexingan06.cn

[S29] C：变参函数
来源：http://ir.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yl.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://rd.hahajie.cn

#ifndef X_H
来源：http://vw.521024.cn

#define X_H
来源：http://fu.9csxet.cn

#endif
来源：http://df.hnjuh.cn

[S31] C++：Hello World
来源：http://vf.hnjuh.cn

#include <iostream>
来源：http://av.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://fg.haigaiapp.cn

[S32] C++：字符串
来源：http://sb.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://lu.asd995.cn

[S33] C++：vector 增删
来源：http://uo.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uj.nszjky.cn

[S34] C++：遍历 vector
来源：http://rj.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://am.wgjwhj.cn

[S35] C++：map
来源：http://qr.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fb.521024.cn

[S36] C++：unordered_map
来源：http://zz.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zd.gzmigu.cn

[S37] C++：set
来源：http://gl.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qp.gzmigu.cn

[S38] C++：排序
来源：http://ia.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://je.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://ag.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uz.yuexingan06.cn

[S40] C++：查找元素
来源：http://yg.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://re.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://rn.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wa.521024.cn

[S42] C++：继承与虚函数
来源：http://sn.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://gm.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://et.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://fz.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://zi.9csxet.cn

void inc(int &x) { ++x; }
来源：http://dr.shxzskj.cn

[S45] C++：lambda
来源：http://my.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pa.szxytkj.cn

[S46] C++：函数模板
来源：http://vm.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hb.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://sd.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qn.gzmigu.cn

[S48] C++：逐行读文件
来源：http://fn.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sb.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://nq.yuntaijiaju.cn

[S49] C++：写文件
来源：http://tq.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pa.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://jh.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hs.panjiajie.cn

[S51] C++：显式类型转换
来源：http://pg.panjiajie.cn

static_cast<double>(a) / b
来源：http://dj.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://hn.szsharing.cn

int size() const noexcept { return n_; }
来源：http://mj.huanxung.cn

[S53] C++：移动语义
来源：http://zd.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://qw.nszjky.cn

[S54] C++：异常处理
来源：http://mg.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jd.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://cu.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ng.shxzskj.cn

[S56] C++：optional
来源：http://sc.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cl.panjiajie.cn

[S57] C++：编译期常量
来源：http://ay.wgjwhj.cn

constexpr int N = 10;
来源：http://aa.chemitech.net.cn

[S58] C++：命名空间
来源：http://tg.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://wg.bookmarksfly.cn

[S59] C++：静态断言
来源：http://vw.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mg.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://vk.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eu.nszjky.cn

================================================================================
来源：http://nh.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ws.huanxung.cn

================================================================================
来源：http://rp.huanxung.cn

[T01] Kotlin：Hello World
来源：http://fx.szxytkj.cn

println("Hello")
来源：http://xw.bjjhwx.cn

[T02] Kotlin：变量
来源：http://zy.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ht.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://kh.wgjwhj.cn

"值: $b"
来源：http://dv.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://ug.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://di.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://gc.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ut.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://er.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://of.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://yz.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vx.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://wb.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://nb.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://bw.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://by.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://zz.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pp.huanxung.cn

[T11] Kotlin：协程
来源：http://db.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ov.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://fe.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://sg.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://za.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://oy.nszjky.cn

[T14] Kotlin：循环
来源：http://ka.521024.cn

for (i in 1..10) println(i)
来源：http://le.gzmigu.cn

[T15] Kotlin：接口
来源：http://rt.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://il.szxytkj.cn

[T16] Swift：Hello World
来源：http://ma.chemitech.net.cn

print("Hello")
来源：http://yx.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://bt.nszjky.cn

var a = 1;  let b = 2
来源：http://gl.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://tf.muxihuayi.cn

"值: \(b)"
来源：http://qx.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://mo.jctech888.com.cn

if let n = opt { print(n) }
来源：http://zd.colortex.cn

[T20] Swift：数组操作
来源：http://ig.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ag.haigaiapp.cn

[T21] Swift：遍历
来源：http://rw.nszjky.cn

for x in a { print(x) }
来源：http://ad.gzmigu.cn

[T22] Swift：字典
来源：http://ii.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pm.nicolike.cn

[T23] Swift：函数
来源：http://yc.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wi.chemitech.net.cn

[T24] Swift：闭包
来源：http://bi.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ue.haigaiapp.cn

[T25] Swift：结构体
来源：http://vr.muxihuayi.cn

struct P { var x: Int }
来源：http://mv.newstarts.cn

[T26] Swift：类与重写
来源：http://zu.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://yl.lnxyls.cn

[T27] Swift：错误处理
来源：http://sf.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://tq.newstarts.cn

[T28] Swift：枚举
来源：http://sz.huixinmuqiang.cn

enum Color { case red, green }
来源：http://ir.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://cu.nicolike.cn

guard let x = opt else { return }
来源：http://in.lnxyls.cn

[T30] Swift：协议
来源：http://sx.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://ot.panjiajie.cn

[T31] Lua：Hello World
来源：http://zc.newstarts.cn

print("Hello")
来源：http://ez.lnxyls.cn

[T32] Lua：局部变量
来源：http://ap.colortex.cn

local a = 1
来源：http://lv.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://cd.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xy.huixiangedu.cn

[T34] Lua：遍历表
来源：http://uj.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ui.yuexingan06.cn

[T35] Lua：字典表
来源：http://mf.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://oy.hnjuh.cn

[T36] Lua：函数
来源：http://tb.9csxet.cn

function add(a, b) return a + b end
来源：http://my.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://rs.9csxet.cn

"a" .. "b"
来源：http://jt.bookmarksfly.cn

[T38] Lua：条件
来源：http://my.huanxung.cn

if x > 0 then print("正") end
来源：http://px.newstarts.cn

[T39] Lua：模式匹配
来源：http://qx.huixiangedu.cn

string.find(s, "%d+")
来源：http://pz.colortex.cn

[T40] Lua：元表
来源：http://co.9csxet.cn

setmetatable({}, { __index = base })
来源：http://pc.colortex.cn

[T41] Perl：Hello World
来源：http://yc.yuntaijiaju.cn

print "Hello\n";
来源：http://nv.shxzukj.cn

[T42] Perl：变量类型
来源：http://rs.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vg.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://po.szxytkj.cn

"值: $a"
来源：http://qz.szsharing.cn

[T44] Perl：条件
来源：http://tz.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://jz.lnxyls.cn

[T45] Perl：数组遍历
来源：http://xq.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://nn.colortex.cn

[T46] Perl：哈希操作
来源：http://zz.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ft.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://zy.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fk.panjiajie.cn

[T48] Perl：正则替换
来源：http://jw.nicolike.cn

$s =~ s/old/new/g;
来源：http://tt.szsharing.cn

[T49] Perl：函数
来源：http://gz.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kl.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://to.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xy.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://ca.huixiangedu.cn

[T51] Scala：Hello World
来源：http://xe.jctech888.com.cn

println("Hello")
来源：http://qg.panjiajie.cn

[T52] Scala：变量
来源：http://te.szsharing.cn

val a = 1;  var b = 2
来源：http://ll.asd995.cn

[T53] Scala：字符串插值
来源：http://oc.shtwfgs.cn

s"值: $b"
来源：http://ob.shtwfgs.cn

[T54] Scala：集合映射
来源：http://ex.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://nn.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://si.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iz.muxihuayi.cn

[T56] Scala：样例类
来源：http://zj.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://ba.colortex.cn

[T57] Scala：模式匹配
来源：http://tr.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kh.chemitech.net.cn

[T58] Scala：函数定义
来源：http://sz.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cq.huixiangedu.cn

[T59] Scala：循环
来源：http://gc.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://fq.9csxet.cn

[T60] Scala：折叠
来源：http://wc.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jh.asd995.cn

================================================================================
来源：http://nj.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jx.shxzukj.cn

================================================================================
来源：http://wz.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://hy.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jj.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://uw.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qj.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://ay.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fk.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://fm.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://md.colortex.cn

[U05] Py：列表去重且保序
来源：http://bc.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://ay.9csxet.cn

[U06] Py：合并两个字典
来源：http://ld.hnjuh.cn

{**a, **b}
来源：http://fu.hahajie.cn

[U07] Py：反转字典键值
来源：http://is.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://at.panjiajie.cn

[U08] Py：展平二维列表
来源：http://is.panjiajie.cn

[y for x in nested for y in x]
来源：http://le.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://qr.bookmarksfly.cn

max(d, key=d.get)
来源：http://xa.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://un.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kk.521024.cn

[U11] Py：生成器表达式
来源：http://vp.chemitech.net.cn

(x * 2 for x in arr)
来源：http://bv.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://af.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://hy.asd995.cn

[U13] Py：固定长度队列
来源：http://ms.colortex.cn

deque(maxlen=10)
来源：http://pm.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://jb.huixiangedu.cn

defaultdict(list)
来源：http://jj.muxihuayi.cn

[U15] Py：高精度计时
来源：http://zu.shxzskj.cn

t = time.perf_counter()
来源：http://su.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://ab.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cx.bjjhwx.cn

[U17] Py：初始化日志
来源：http://jy.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://pq.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://oa.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://ly.newstarts.cn


<!-- 参考信息 -->