代发 wailian999

read -rp "请输入: " ans
来源：http://hd.muxihuayi.cn

[R78] 交互式菜单
来源：http://wu.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cb.szxytkj.cn

[R79] 解析命令行选项
来源：http://eu.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dy.521024.cn

[R80] 查看脚本执行耗时
来源：http://gg.nicolike.cn

time ./run.sh
来源：http://mu.haigaiapp.cn

================================================================================
来源：http://pe.lnxyls.cn

S. C / C++ 专题
来源：http://op.shxzskj.cn

================================================================================
来源：http://fv.shxzskj.cn

[S01] C：Hello World
来源：http://kt.nicolike.cn

#include <stdio.h>
来源：http://ff.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xg.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://hj.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://ke.yuexingan06.cn

[S03] C：读入整数
来源：http://wu.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://cb.huanxung.cn

[S04] C：字符串复制
来源：http://bi.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jy.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://yr.szsharing.cn

strlen(s)
来源：http://ik.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://vt.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://de.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://oh.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eh.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://we.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ln.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://cy.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lu.521024.cn

[S10] C：指针与解引用
来源：http://jo.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://it.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://us.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://sy.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zj.szsharing.cn

fclose(f);
来源：http://qg.panjiajie.cn

[S12] C：写文件
来源：http://je.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://au.jctech888.com.cn

[S13] C：宏定义
来源：http://qj.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kr.shxzskj.cn

[S14] C：枚举
来源：http://yt.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://uj.hahajie.cn

[S15] C：类型转换
来源：http://mh.hahajie.cn

(double) a / b
来源：http://xq.wgjwhj.cn

[S16] C：位操作置位
来源：http://cx.lnxyls.cn

x |= (1 << 3);
来源：http://oa.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://od.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ya.szxytkj.cn

[S18] C：命令行参数
来源：http://vq.muxihuayi.cn

int main(int argc, char **argv)
来源：http://ym.asd995.cn

[S19] C：快速排序
来源：http://kc.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zl.hnjuh.cn

[S20] C：二分查找
来源：http://sz.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yb.hahajie.cn

[S21] C：字符类别判断
来源：http://ca.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wm.wgjwhj.cn

[S22] C：字符串转数字
来源：http://ek.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zw.yuexingan06.cn

[S23] C：随机数
来源：http://ie.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://up.colortex.cn

[S24] C：获取本地时间
来源：http://nl.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ob.bjjhwx.cn

[S25] C：内存拷贝
来源：http://ga.shxzskj.cn

memcpy(dst, src, n);
来源：http://rw.huixinmuqiang.cn

[S26] C：内存清零
来源：http://kt.colortex.cn

memset(a, 0, sizeof a);
来源：http://vf.haigaiapp.cn

[S27] C：定义常量
来源：http://uh.shxzskj.cn

const double PI = 3.14159;
来源：http://cy.colortex.cn

[S28] C：静态变量
来源：http://at.jianghongdianzi.cn

static int counter = 0;
来源：http://nv.wgjwhj.cn

[S29] C：变参函数
来源：http://as.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://af.521024.cn

[S30] C：头文件保护
来源：http://bg.colortex.cn

#ifndef X_H
来源：http://ma.jctech888.com.cn

#define X_H
来源：http://qn.jctech888.com.cn

#endif
来源：http://hd.muxihuayi.cn

[S31] C++：Hello World
来源：http://pr.haigaiapp.cn

#include <iostream>
来源：http://ly.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ov.newstarts.cn

[S32] C++：字符串
来源：http://ef.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://gq.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://kd.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ot.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://qb.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://ag.lnxyls.cn

[S35] C++：map
来源：http://so.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dc.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://gf.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vf.jctech888.com.cn

[S37] C++：set
来源：http://hy.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nl.szsharing.cn

[S38] C++：排序
来源：http://cb.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://dy.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://kr.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ko.wgjwhj.cn

[S40] C++：查找元素
来源：http://kk.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cu.nszjky.cn

[S41] C++：类与构造函数
来源：http://mi.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://le.szsharing.cn

[S42] C++：继承与虚函数
来源：http://ln.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ae.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://wi.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://jw.muxihuayi.cn

[S44] C++：引用传参
来源：http://sr.nszjky.cn

void inc(int &x) { ++x; }
来源：http://yd.lnxyls.cn

[S45] C++：lambda
来源：http://dg.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuexingan06.cn

[S46] C++：函数模板
来源：http://wn.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ij.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://so.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://og.nicolike.cn

[S48] C++：逐行读文件
来源：http://eh.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pp.newstarts.cn

while (std::getline(in, line)) { }
来源：http://zb.yuexingan06.cn

[S49] C++：写文件
来源：http://jn.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qy.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://bz.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dy.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://wi.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://da.asd995.cn

[S52] C++：const 与 noexcept
来源：http://ca.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://uy.szsharing.cn

[S53] C++：移动语义
来源：http://pg.521024.cn

std::vector<int> w = std::move(v);
来源：http://xr.szxytkj.cn

[S54] C++：异常处理
来源：http://st.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ny.colortex.cn

[S55] C++：结构化绑定
来源：http://js.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vu.colortex.cn

[S56] C++：optional
来源：http://mx.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vg.szsharing.cn

[S57] C++：编译期常量
来源：http://jl.newstarts.cn

constexpr int N = 10;
来源：http://wx.shtwfgs.cn

[S58] C++：命名空间
来源：http://eo.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://kj.huanxung.cn

[S59] C++：静态断言
来源：http://dd.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hq.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://mk.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lv.shxzukj.cn

================================================================================
来源：http://pu.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dq.lnxyls.cn

================================================================================
来源：http://by.hahajie.cn

[T01] Kotlin：Hello World
来源：http://os.nszjky.cn

println("Hello")
来源：http://vk.nszjky.cn

[T02] Kotlin：变量
来源：http://lz.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xj.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://sq.yuntaijiaju.cn

"值: $b"
来源：http://lk.shxzukj.cn

[T04] Kotlin：空安全
来源：http://xb.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://xm.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://wu.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fo.asd995.cn

[T06] Kotlin：集合映射
来源：http://xn.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tm.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://hf.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nd.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://ss.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://xd.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://mh.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://ck.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://gx.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gt.9csxet.cn

[T11] Kotlin：协程
来源：http://ss.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://do.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://gh.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://xk.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://bg.hahajie.cn

val m = mapOf("a" to 1)
来源：http://kt.shtwfgs.cn

[T14] Kotlin：循环
来源：http://sc.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://mx.haigaiapp.cn

[T15] Kotlin：接口
来源：http://vn.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://ri.yuexingan06.cn

[T16] Swift：Hello World
来源：http://bv.nszjky.cn

print("Hello")
来源：http://qd.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://hs.hnjuh.cn

var a = 1;  let b = 2
来源：http://al.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://ga.colortex.cn

"值: \(b)"
来源：http://oc.szxytkj.cn

[T19] Swift：可选绑定
来源：http://eg.haigaiapp.cn

if let n = opt { print(n) }
来源：http://wt.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://pc.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rm.chemitech.net.cn

[T21] Swift：遍历
来源：http://nh.bjjhwx.cn

for x in a { print(x) }
来源：http://ly.gzmigu.cn

[T22] Swift：字典
来源：http://ci.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://py.huixiangedu.cn

[T23] Swift：函数
来源：http://ad.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cc.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://zh.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zn.521024.cn

[T25] Swift：结构体
来源：http://fi.bjjhwx.cn

struct P { var x: Int }
来源：http://oi.haigaiapp.cn

[T26] Swift：类与重写
来源：http://ba.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://pw.nszjky.cn

[T27] Swift：错误处理
来源：http://an.huanxung.cn

do { try f() } catch { print(error) }
来源：http://gt.panjiajie.cn

[T28] Swift：枚举
来源：http://qf.nicolike.cn

enum Color { case red, green }
来源：http://os.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://ja.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://ug.jianghongdianzi.cn

[T30] Swift：协议
来源：http://zk.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://rj.wgjwhj.cn

[T31] Lua：Hello World
来源：http://da.chemitech.net.cn

print("Hello")
来源：http://nc.shxzukj.cn

[T32] Lua：局部变量
来源：http://be.nicolike.cn

local a = 1
来源：http://gr.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://bd.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sn.huanxung.cn

[T34] Lua：遍历表
来源：http://xi.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jd.huixiangedu.cn

[T35] Lua：字典表
来源：http://yt.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://gs.chemitech.net.cn

[T36] Lua：函数
来源：http://bc.chemitech.net.cn

function add(a, b) return a + b end
来源：http://sz.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://ld.shtwfgs.cn

"a" .. "b"
来源：http://el.jianghongdianzi.cn

[T38] Lua：条件
来源：http://su.szsharing.cn

if x > 0 then print("正") end
来源：http://bj.nicolike.cn

[T39] Lua：模式匹配
来源：http://el.panjiajie.cn

string.find(s, "%d+")
来源：http://lt.huixinmuqiang.cn

[T40] Lua：元表
来源：http://xj.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://jp.9csxet.cn

[T41] Perl：Hello World
来源：http://cd.lnxyls.cn

print "Hello\n";
来源：http://mf.nszjky.cn

[T42] Perl：变量类型
来源：http://hh.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nq.nszjky.cn

[T43] Perl：字符串插值
来源：http://bt.yuntaijiaju.cn

"值: $a"
来源：http://bb.gzmigu.cn

[T44] Perl：条件
来源：http://gn.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://hv.szsharing.cn

[T45] Perl：数组遍历
来源：http://sx.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://to.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://oh.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wo.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://ad.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zj.hahajie.cn

[T48] Perl：正则替换
来源：http://ep.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://uk.shxzukj.cn

[T49] Perl：函数
来源：http://lq.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uo.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://aq.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gh.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://sq.colortex.cn

[T51] Scala：Hello World
来源：http://uc.huixinmuqiang.cn

println("Hello")
来源：http://pp.shxzskj.cn

[T52] Scala：变量
来源：http://pu.newstarts.cn

val a = 1;  var b = 2
来源：http://wq.szxytkj.cn

[T53] Scala：字符串插值
来源：http://ov.huanxung.cn

s"值: $b"
来源：http://il.muxihuayi.cn

[T54] Scala：集合映射
来源：http://id.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://nn.521024.cn

[T55] Scala：集合过滤
来源：http://gq.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qd.nicolike.cn

[T56] Scala：样例类
来源：http://re.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://ww.9csxet.cn

[T57] Scala：模式匹配
来源：http://gk.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://df.yuexingan06.cn

[T58] Scala：函数定义
来源：http://op.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vz.lnxyls.cn

[T59] Scala：循环
来源：http://mj.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://dx.shxzukj.cn

[T60] Scala：折叠
来源：http://ug.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pt.nicolike.cn

================================================================================
来源：http://qr.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zu.nszjky.cn

================================================================================
来源：http://oc.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://ce.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://as.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://gj.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dl.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://cp.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vw.panjiajie.cn

[U04] Py：变量调试打印
来源：http://wc.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qi.nszjky.cn

[U05] Py：列表去重且保序
来源：http://tj.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://xg.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://if.huixinmuqiang.cn

{**a, **b}
来源：http://cm.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://he.9csxet.cn

{v: k for k, v in d.items()}
来源：http://vu.lnxyls.cn

[U08] Py：展平二维列表
来源：http://xy.hahajie.cn

[y for x in nested for y in x]
来源：http://mg.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://lo.szxytkj.cn

max(d, key=d.get)
来源：http://hm.newstarts.cn

[U10] Py：按值排序字典
来源：http://fb.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mf.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://ol.521024.cn

(x * 2 for x in arr)
来源：http://tm.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://db.gzmigu.cn

Counter(arr).most_common(3)
来源：http://bc.huanxung.cn

[U13] Py：固定长度队列
来源：http://hq.newstarts.cn

deque(maxlen=10)
来源：http://rs.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://kv.muxihuayi.cn

defaultdict(list)
来源：http://gu.asd995.cn

[U15] Py：高精度计时
来源：http://vp.yuexingan06.cn

t = time.perf_counter()
来源：http://rn.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://vv.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rb.haigaiapp.cn

[U17] Py：初始化日志
来源：http://bk.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://hi.lnxyls.cn

[U18] Py：预编译正则
来源：http://su.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://kt.huixinmuqiang.cn


<!-- 参考信息 -->