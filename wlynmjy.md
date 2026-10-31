代发 wailian999

read -rp "请输入: " ans
来源：http://yr.hnjuh.cn

[R78] 交互式菜单
来源：http://lu.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kk.muxihuayi.cn

[R79] 解析命令行选项
来源：http://al.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://up.521024.cn

[R80] 查看脚本执行耗时
来源：http://qh.asd995.cn

time ./run.sh
来源：http://kc.gzmigu.cn

================================================================================
来源：http://lz.muxihuayi.cn

S. C / C++ 专题
来源：http://di.jctech888.com.cn

================================================================================
来源：http://fy.asd995.cn

[S01] C：Hello World
来源：http://hk.huanxung.cn

#include <stdio.h>
来源：http://wd.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bg.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://bf.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://se.newstarts.cn

[S03] C：读入整数
来源：http://de.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://ie.nicolike.cn

[S04] C：字符串复制
来源：http://kt.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vf.yuexingan06.cn

[S05] C：字符串长度
来源：http://bd.haigaiapp.cn

strlen(s)
来源：http://en.shxzukj.cn

[S06] C：字符串比较
来源：http://iu.hahajie.cn

strcmp(a, b) == 0
来源：http://ke.shxzskj.cn

[S07] C：数组遍历求和
来源：http://kn.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zv.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://nv.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ow.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://xg.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dv.shxzukj.cn

[S10] C：指针与解引用
来源：http://yb.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://zg.nszjky.cn

[S11] C：逐行读文件
来源：http://rd.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://vw.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nj.newstarts.cn

fclose(f);
来源：http://en.muxihuayi.cn

[S12] C：写文件
来源：http://pr.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://er.shtwfgs.cn

[S13] C：宏定义
来源：http://bp.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yj.hahajie.cn

[S14] C：枚举
来源：http://xd.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ur.haigaiapp.cn

[S15] C：类型转换
来源：http://lz.huanxung.cn

(double) a / b
来源：http://vv.colortex.cn

[S16] C：位操作置位
来源：http://gl.colortex.cn

x |= (1 << 3);
来源：http://wi.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://au.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tl.bjjhwx.cn

[S18] C：命令行参数
来源：http://am.9csxet.cn

int main(int argc, char **argv)
来源：http://vo.huanxung.cn

[S19] C：快速排序
来源：http://wi.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rk.wgjwhj.cn

[S20] C：二分查找
来源：http://ku.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://om.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://jf.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uy.szxytkj.cn

[S22] C：字符串转数字
来源：http://ka.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sy.yuntaijiaju.cn

[S23] C：随机数
来源：http://tf.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ah.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://hw.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oh.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://tq.huixiangedu.cn

memcpy(dst, src, n);
来源：http://lf.yuntaijiaju.cn

[S26] C：内存清零
来源：http://vw.9csxet.cn

memset(a, 0, sizeof a);
来源：http://em.shxzukj.cn

[S27] C：定义常量
来源：http://um.nszjky.cn

const double PI = 3.14159;
来源：http://ae.shxzukj.cn

[S28] C：静态变量
来源：http://hx.chemitech.net.cn

static int counter = 0;
来源：http://os.9csxet.cn

[S29] C：变参函数
来源：http://no.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oe.szsharing.cn

[S30] C：头文件保护
来源：http://hv.nicolike.cn

#ifndef X_H
来源：http://rp.colortex.cn

#define X_H
来源：http://pl.shxzskj.cn

#endif
来源：http://ig.szxytkj.cn

[S31] C++：Hello World
来源：http://eq.muxihuayi.cn

#include <iostream>
来源：http://lf.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://rd.szxytkj.cn

[S32] C++：字符串
来源：http://wr.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://bi.panjiajie.cn

[S33] C++：vector 增删
来源：http://zj.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uv.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://ll.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://rf.nicolike.cn

[S35] C++：map
来源：http://cd.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zh.newstarts.cn

[S36] C++：unordered_map
来源：http://zz.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ec.gzmigu.cn

[S37] C++：set
来源：http://qt.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gl.shtwfgs.cn

[S38] C++：排序
来源：http://ki.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://vk.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://bp.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xq.hahajie.cn

[S40] C++：查找元素
来源：http://ty.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mx.newstarts.cn

[S41] C++：类与构造函数
来源：http://aa.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pb.asd995.cn

[S42] C++：继承与虚函数
来源：http://bk.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://ec.szxytkj.cn

[S43] C++：智能指针
来源：http://su.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://gq.shtwfgs.cn

[S44] C++：引用传参
来源：http://xz.newstarts.cn

void inc(int &x) { ++x; }
来源：http://yl.huixinmuqiang.cn

[S45] C++：lambda
来源：http://gw.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wk.yuexingan06.cn

[S46] C++：函数模板
来源：http://ko.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jm.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://ay.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sr.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://vf.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lb.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://vv.szxytkj.cn

[S49] C++：写文件
来源：http://rl.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iz.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://tm.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jj.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://xi.szsharing.cn

static_cast<double>(a) / b
来源：http://pj.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://fw.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://ym.asd995.cn

[S53] C++：移动语义
来源：http://bk.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://iv.szsharing.cn

[S54] C++：异常处理
来源：http://jh.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pm.colortex.cn

[S55] C++：结构化绑定
来源：http://yk.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jo.hnjuh.cn

[S56] C++：optional
来源：http://qe.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nb.szxytkj.cn

[S57] C++：编译期常量
来源：http://cs.szsharing.cn

constexpr int N = 10;
来源：http://zq.9csxet.cn

[S58] C++：命名空间
来源：http://dw.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://iw.newstarts.cn

[S59] C++：静态断言
来源：http://wk.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xv.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://lv.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zr.shxzskj.cn

================================================================================
来源：http://zd.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cf.huixiangedu.cn

================================================================================
来源：http://xa.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://tr.panjiajie.cn

println("Hello")
来源：http://pq.asd995.cn

[T02] Kotlin：变量
来源：http://dh.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tw.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://my.huixiangedu.cn

"值: $b"
来源：http://nk.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://id.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://it.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://xs.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ns.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://wj.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nn.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://ts.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dh.newstarts.cn

[T08] Kotlin：数据类
来源：http://pw.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://wr.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://yx.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://kr.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://gb.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rt.jctech888.com.cn

[T11] Kotlin：协程
来源：http://lc.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dy.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://ve.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://wa.colortex.cn

[T13] Kotlin：只读 Map
来源：http://jg.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://ph.shxzskj.cn

[T14] Kotlin：循环
来源：http://eg.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://vy.wgjwhj.cn

[T15] Kotlin：接口
来源：http://yr.nicolike.cn

interface Shape { fun area(): Double }
来源：http://ij.521024.cn

[T16] Swift：Hello World
来源：http://mf.gzmigu.cn

print("Hello")
来源：http://eg.shxzskj.cn

[T17] Swift：变量与常量
来源：http://ty.nicolike.cn

var a = 1;  let b = 2
来源：http://xq.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://ud.huanxung.cn

"值: \(b)"
来源：http://bx.521024.cn

[T19] Swift：可选绑定
来源：http://ag.huanxung.cn

if let n = opt { print(n) }
来源：http://gv.haigaiapp.cn

[T20] Swift：数组操作
来源：http://qf.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vc.hnjuh.cn

[T21] Swift：遍历
来源：http://tf.shtwfgs.cn

for x in a { print(x) }
来源：http://cu.hahajie.cn

[T22] Swift：字典
来源：http://mg.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fd.huixiangedu.cn

[T23] Swift：函数
来源：http://qj.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lx.shtwfgs.cn

[T24] Swift：闭包
来源：http://xv.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wg.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://ia.shxzukj.cn

struct P { var x: Int }
来源：http://hq.hnjuh.cn

[T26] Swift：类与重写
来源：http://gc.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://nx.asd995.cn

[T27] Swift：错误处理
来源：http://og.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://qx.haigaiapp.cn

[T28] Swift：枚举
来源：http://uh.huixiangedu.cn

enum Color { case red, green }
来源：http://th.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://rj.9csxet.cn

guard let x = opt else { return }
来源：http://ui.huanxung.cn

[T30] Swift：协议
来源：http://zr.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://xk.shtwfgs.cn

[T31] Lua：Hello World
来源：http://cz.huanxung.cn

print("Hello")
来源：http://yt.jctech888.com.cn

[T32] Lua：局部变量
来源：http://rb.lnxyls.cn

local a = 1
来源：http://tx.nicolike.cn

[T33] Lua：表（数组）
来源：http://ja.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hp.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://bx.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yi.nicolike.cn

[T35] Lua：字典表
来源：http://dw.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://ob.panjiajie.cn

[T36] Lua：函数
来源：http://kb.szsharing.cn

function add(a, b) return a + b end
来源：http://qk.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://vx.nszjky.cn

"a" .. "b"
来源：http://qo.colortex.cn

[T38] Lua：条件
来源：http://qe.hnjuh.cn

if x > 0 then print("正") end
来源：http://sl.newstarts.cn

[T39] Lua：模式匹配
来源：http://lo.shtwfgs.cn

string.find(s, "%d+")
来源：http://fm.huanxung.cn

[T40] Lua：元表
来源：http://qr.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://vt.shxzukj.cn

[T41] Perl：Hello World
来源：http://ob.huanxung.cn

print "Hello\n";
来源：http://bt.colortex.cn

[T42] Perl：变量类型
来源：http://uj.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kv.nicolike.cn

[T43] Perl：字符串插值
来源：http://zz.jianghongdianzi.cn

"值: $a"
来源：http://il.haigaiapp.cn

[T44] Perl：条件
来源：http://wc.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://kd.szsharing.cn

[T45] Perl：数组遍历
来源：http://qa.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://un.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://ho.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kv.shxzskj.cn

[T47] Perl：正则捕获
来源：http://aq.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qo.shtwfgs.cn

[T48] Perl：正则替换
来源：http://vk.nszjky.cn

$s =~ s/old/new/g;
来源：http://rv.shtwfgs.cn

[T49] Perl：函数
来源：http://zo.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nr.521024.cn

[T50] Perl：逐行读文件
来源：http://jx.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jq.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://zu.huanxung.cn

[T51] Scala：Hello World
来源：http://bl.bookmarksfly.cn

println("Hello")
来源：http://oh.gzmigu.cn

[T52] Scala：变量
来源：http://fo.9csxet.cn

val a = 1;  var b = 2
来源：http://ia.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://oq.hahajie.cn

s"值: $b"
来源：http://oq.asd995.cn

[T54] Scala：集合映射
来源：http://th.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://zp.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://yy.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://in.521024.cn

[T56] Scala：样例类
来源：http://yn.hnjuh.cn

case class User(name: String, age: Int)
来源：http://tt.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://di.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://br.shxzskj.cn

[T58] Scala：函数定义
来源：http://wu.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tn.jianghongdianzi.cn

[T59] Scala：循环
来源：http://st.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://qu.jctech888.com.cn

[T60] Scala：折叠
来源：http://kh.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.huixinmuqiang.cn

================================================================================
来源：http://vt.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tb.yuexingan06.cn

================================================================================
来源：http://mp.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://vp.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iu.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://zj.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ku.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://pr.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pg.nszjky.cn

[U04] Py：变量调试打印
来源：http://om.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://re.szsharing.cn

[U05] Py：列表去重且保序
来源：http://kd.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://jo.nicolike.cn

[U06] Py：合并两个字典
来源：http://sc.shtwfgs.cn

{**a, **b}
来源：http://yn.nszjky.cn

[U07] Py：反转字典键值
来源：http://do.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://sx.szsharing.cn

[U08] Py：展平二维列表
来源：http://sf.nicolike.cn

[y for x in nested for y in x]
来源：http://dg.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://jw.521024.cn

max(d, key=d.get)
来源：http://dc.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://fl.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://us.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://qf.9csxet.cn

(x * 2 for x in arr)
来源：http://ij.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wh.nicolike.cn

Counter(arr).most_common(3)
来源：http://df.shxzskj.cn

[U13] Py：固定长度队列
来源：http://cy.yuntaijiaju.cn

deque(maxlen=10)
来源：http://rw.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://yx.huanxung.cn

defaultdict(list)
来源：http://wi.chemitech.net.cn

[U15] Py：高精度计时
来源：http://gr.lnxyls.cn

t = time.perf_counter()
来源：http://jq.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://ko.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ki.haigaiapp.cn

[U17] Py：初始化日志
来源：http://te.shxzukj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nh.huixiangedu.cn

[U18] Py：预编译正则
来源：http://mc.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://ai.jianghongdianzi.cn


<!-- 参考信息 -->