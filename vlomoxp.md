代发 wailian999

read -rp "请输入: " ans
来源：http://bp.newstarts.cn

[R78] 交互式菜单
来源：http://xs.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hd.jctech888.com.cn

[R79] 解析命令行选项
来源：http://sy.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kx.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://le.nicolike.cn

time ./run.sh
来源：http://ql.newstarts.cn

================================================================================
来源：http://gq.newstarts.cn

S. C / C++ 专题
来源：http://hm.jianghongdianzi.cn

================================================================================
来源：http://fk.szxytkj.cn

[S01] C：Hello World
来源：http://ge.huixinmuqiang.cn

#include <stdio.h>
来源：http://fs.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jf.huanxung.cn

[S02] C：变量与格式化输出
来源：http://ci.521024.cn

int a = 10; printf("%d\n", a);
来源：http://rd.colortex.cn

[S03] C：读入整数
来源：http://pn.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://wz.hnjuh.cn

[S04] C：字符串复制
来源：http://ig.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mz.hahajie.cn

[S05] C：字符串长度
来源：http://ze.lnxyls.cn

strlen(s)
来源：http://cv.hnjuh.cn

[S06] C：字符串比较
来源：http://vr.gzmigu.cn

strcmp(a, b) == 0
来源：http://hb.gzmigu.cn

[S07] C：数组遍历求和
来源：http://jl.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ae.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://ms.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ok.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://rv.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://va.asd995.cn

[S10] C：指针与解引用
来源：http://nc.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://kr.521024.cn

[S11] C：逐行读文件
来源：http://zb.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ll.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xx.huixinmuqiang.cn

fclose(f);
来源：http://em.haigaiapp.cn

[S12] C：写文件
来源：http://ze.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ij.nszjky.cn

[S13] C：宏定义
来源：http://pg.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xo.hnjuh.cn

[S14] C：枚举
来源：http://ix.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://jr.lnxyls.cn

[S15] C：类型转换
来源：http://kh.yuexingan06.cn

(double) a / b
来源：http://vp.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ox.bjjhwx.cn

x |= (1 << 3);
来源：http://xs.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ku.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qb.asd995.cn

[S18] C：命令行参数
来源：http://fw.nszjky.cn

int main(int argc, char **argv)
来源：http://zz.huanxung.cn

[S19] C：快速排序
来源：http://rt.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ut.nszjky.cn

[S20] C：二分查找
来源：http://ia.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fa.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://hu.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://le.wgjwhj.cn

[S22] C：字符串转数字
来源：http://yi.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tz.huixiangedu.cn

[S23] C：随机数
来源：http://sj.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bc.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://to.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://by.shxzukj.cn

[S25] C：内存拷贝
来源：http://fi.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://wm.gzmigu.cn

[S26] C：内存清零
来源：http://el.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://gz.shtwfgs.cn

[S27] C：定义常量
来源：http://ta.huanxung.cn

const double PI = 3.14159;
来源：http://fp.hahajie.cn

[S28] C：静态变量
来源：http://pl.huixinmuqiang.cn

static int counter = 0;
来源：http://iu.szxytkj.cn

[S29] C：变参函数
来源：http://zj.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ws.jctech888.com.cn

[S30] C：头文件保护
来源：http://cz.haigaiapp.cn

#ifndef X_H
来源：http://xe.nicolike.cn

#define X_H
来源：http://yy.hnjuh.cn

#endif
来源：http://gf.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://cx.huixinmuqiang.cn

#include <iostream>
来源：http://oq.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://jt.hnjuh.cn

[S32] C++：字符串
来源：http://rr.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://sn.huanxung.cn

[S33] C++：vector 增删
来源：http://fq.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jq.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://rh.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://no.bjjhwx.cn

[S35] C++：map
来源：http://vh.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fq.wgjwhj.cn

[S36] C++：unordered_map
来源：http://tp.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qk.newstarts.cn

[S37] C++：set
来源：http://mc.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xv.hahajie.cn

[S38] C++：排序
来源：http://zp.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://yk.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://lt.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kh.hahajie.cn

[S40] C++：查找元素
来源：http://dr.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pf.huanxung.cn

[S41] C++：类与构造函数
来源：http://gs.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lk.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://ik.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://rj.muxihuayi.cn

[S43] C++：智能指针
来源：http://uz.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://hi.shxzukj.cn

[S44] C++：引用传参
来源：http://cl.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://fp.gzmigu.cn

[S45] C++：lambda
来源：http://sv.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lh.wgjwhj.cn

[S46] C++：函数模板
来源：http://nn.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tt.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://as.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oh.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://vy.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oh.nicolike.cn

while (std::getline(in, line)) { }
来源：http://az.shxzskj.cn

[S49] C++：写文件
来源：http://lc.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://na.panjiajie.cn

[S50] C++：格式化数字
来源：http://bo.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://to.szxytkj.cn

[S51] C++：显式类型转换
来源：http://ee.haigaiapp.cn

static_cast<double>(a) / b
来源：http://co.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://uf.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://bt.huanxung.cn

[S53] C++：移动语义
来源：http://fo.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://wz.muxihuayi.cn

[S54] C++：异常处理
来源：http://wg.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rs.521024.cn

[S55] C++：结构化绑定
来源：http://hl.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ga.hnjuh.cn

[S56] C++：optional
来源：http://rf.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hj.hnjuh.cn

[S57] C++：编译期常量
来源：http://vx.nszjky.cn

constexpr int N = 10;
来源：http://uf.lnxyls.cn

[S58] C++：命名空间
来源：http://bc.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://sm.newstarts.cn

[S59] C++：静态断言
来源：http://qb.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tz.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://gl.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ti.chemitech.net.cn

================================================================================
来源：http://vt.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lv.shxzskj.cn

================================================================================
来源：http://bs.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://sw.panjiajie.cn

println("Hello")
来源：http://kk.panjiajie.cn

[T02] Kotlin：变量
来源：http://xu.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uj.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://mk.yuntaijiaju.cn

"值: $b"
来源：http://iw.gzmigu.cn

[T04] Kotlin：空安全
来源：http://yx.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://mr.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://az.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://il.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://ff.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sg.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://lz.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cz.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://an.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://lx.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://tb.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://lf.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://kn.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qy.wgjwhj.cn

[T11] Kotlin：协程
来源：http://mj.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ss.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://sj.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://kg.colortex.cn

[T13] Kotlin：只读 Map
来源：http://uc.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://ks.shxzskj.cn

[T14] Kotlin：循环
来源：http://ez.nszjky.cn

for (i in 1..10) println(i)
来源：http://cd.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://pc.521024.cn

interface Shape { fun area(): Double }
来源：http://dg.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://qm.9csxet.cn

print("Hello")
来源：http://yq.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://ce.nicolike.cn

var a = 1;  let b = 2
来源：http://vp.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://ih.huixiangedu.cn

"值: \(b)"
来源：http://hb.9csxet.cn

[T19] Swift：可选绑定
来源：http://ld.yuexingan06.cn

if let n = opt { print(n) }
来源：http://qn.hahajie.cn

[T20] Swift：数组操作
来源：http://xp.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lp.bookmarksfly.cn

[T21] Swift：遍历
来源：http://rp.haigaiapp.cn

for x in a { print(x) }
来源：http://es.huanxung.cn

[T22] Swift：字典
来源：http://na.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zo.lnxyls.cn

[T23] Swift：函数
来源：http://uv.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fz.lnxyls.cn

[T24] Swift：闭包
来源：http://oi.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bg.gzmigu.cn

[T25] Swift：结构体
来源：http://ai.colortex.cn

struct P { var x: Int }
来源：http://nt.hahajie.cn

[T26] Swift：类与重写
来源：http://xm.lnxyls.cn

class A: Base { override func f() {} }
来源：http://lv.szxytkj.cn

[T27] Swift：错误处理
来源：http://jx.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://lq.huanxung.cn

[T28] Swift：枚举
来源：http://td.9csxet.cn

enum Color { case red, green }
来源：http://tp.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://aj.9csxet.cn

guard let x = opt else { return }
来源：http://wj.lnxyls.cn

[T30] Swift：协议
来源：http://ae.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://vu.shxzukj.cn

[T31] Lua：Hello World
来源：http://rj.bookmarksfly.cn

print("Hello")
来源：http://mz.huanxung.cn

[T32] Lua：局部变量
来源：http://vk.jctech888.com.cn

local a = 1
来源：http://ju.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://hg.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wf.gzmigu.cn

[T34] Lua：遍历表
来源：http://ey.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rw.hnjuh.cn

[T35] Lua：字典表
来源：http://ue.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://et.9csxet.cn

[T36] Lua：函数
来源：http://qy.muxihuayi.cn

function add(a, b) return a + b end
来源：http://dv.szsharing.cn

[T37] Lua：字符串拼接
来源：http://wt.nicolike.cn

"a" .. "b"
来源：http://ob.haigaiapp.cn

[T38] Lua：条件
来源：http://qs.muxihuayi.cn

if x > 0 then print("正") end
来源：http://yj.521024.cn

[T39] Lua：模式匹配
来源：http://us.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://jj.huixinmuqiang.cn

[T40] Lua：元表
来源：http://np.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://kk.huixiangedu.cn

[T41] Perl：Hello World
来源：http://pi.shxzukj.cn

print "Hello\n";
来源：http://tw.lnxyls.cn

[T42] Perl：变量类型
来源：http://wq.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ed.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://zu.muxihuayi.cn

"值: $a"
来源：http://ae.hahajie.cn

[T44] Perl：条件
来源：http://se.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://bw.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://jb.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://yd.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://uu.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bw.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://hs.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://in.jctech888.com.cn

[T48] Perl：正则替换
来源：http://xi.newstarts.cn

$s =~ s/old/new/g;
来源：http://ps.huixinmuqiang.cn

[T49] Perl：函数
来源：http://lg.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dl.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://nt.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ak.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://lu.nicolike.cn

[T51] Scala：Hello World
来源：http://fo.lnxyls.cn

println("Hello")
来源：http://bm.szxytkj.cn

[T52] Scala：变量
来源：http://tw.huixiangedu.cn

val a = 1;  var b = 2
来源：http://pb.newstarts.cn

[T53] Scala：字符串插值
来源：http://vr.nicolike.cn

s"值: $b"
来源：http://hy.chemitech.net.cn

[T54] Scala：集合映射
来源：http://ud.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vp.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://ar.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fk.szxytkj.cn

[T56] Scala：样例类
来源：http://lo.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://ze.hahajie.cn

[T57] Scala：模式匹配
来源：http://cg.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iu.shtwfgs.cn

[T58] Scala：函数定义
来源：http://sr.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gw.hnjuh.cn

[T59] Scala：循环
来源：http://jr.521024.cn

for (i <- 1 to 10) println(i)
来源：http://wb.panjiajie.cn

[T60] Scala：折叠
来源：http://gr.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uq.bjjhwx.cn

================================================================================
来源：http://sl.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pe.lnxyls.cn

================================================================================
来源：http://yk.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://ea.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jx.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://ek.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lp.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://de.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vr.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://vd.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jj.asd995.cn

[U05] Py：列表去重且保序
来源：http://ew.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://hc.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://fd.huixiangedu.cn

{**a, **b}
来源：http://zp.newstarts.cn

[U07] Py：反转字典键值
来源：http://za.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://tu.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://oi.muxihuayi.cn

[y for x in nested for y in x]
来源：http://ke.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://hf.521024.cn

max(d, key=d.get)
来源：http://wa.gzmigu.cn

[U10] Py：按值排序字典
来源：http://ke.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aj.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://wz.hnjuh.cn

(x * 2 for x in arr)
来源：http://qs.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ij.colortex.cn

Counter(arr).most_common(3)
来源：http://kz.gzmigu.cn

[U13] Py：固定长度队列
来源：http://wp.wgjwhj.cn

deque(maxlen=10)
来源：http://ui.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://in.lnxyls.cn

defaultdict(list)
来源：http://kc.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://jl.hnjuh.cn

t = time.perf_counter()
来源：http://no.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://kr.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cd.shxzskj.cn

[U17] Py：初始化日志
来源：http://ow.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://fp.chemitech.net.cn

[U18] Py：预编译正则
来源：http://bz.9csxet.cn

pat = re.compile(r"\d+")
来源：http://tk.nszjky.cn


<!-- 参考信息 -->