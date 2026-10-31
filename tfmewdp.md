代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://wy.huanxung.cn

[R76] 使用临时文件
来源：http://et.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uh.bookmarksfly.cn

[R77] 读取用户输入
来源：http://iw.asd995.cn

read -rp "请输入: " ans
来源：http://bi.huixiangedu.cn

[R78] 交互式菜单
来源：http://be.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gd.huixiangedu.cn

[R79] 解析命令行选项
来源：http://cf.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wi.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://ql.gzmigu.cn

time ./run.sh
来源：http://cu.hnjuh.cn

================================================================================
来源：http://pz.huixiangedu.cn

S. C / C++ 专题
来源：http://yh.szxytkj.cn

================================================================================
来源：http://po.521024.cn

[S01] C：Hello World
来源：http://re.colortex.cn

#include <stdio.h>
来源：http://gi.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rg.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://ce.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://rb.chemitech.net.cn

[S03] C：读入整数
来源：http://ii.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://vy.nszjky.cn

[S04] C：字符串复制
来源：http://st.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pr.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://mf.panjiajie.cn

strlen(s)
来源：http://go.chemitech.net.cn

[S06] C：字符串比较
来源：http://vv.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://vk.gzmigu.cn

[S07] C：数组遍历求和
来源：http://jh.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ng.521024.cn

[S08] C：动态内存分配与释放
来源：http://bw.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://up.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://zz.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oy.colortex.cn

[S10] C：指针与解引用
来源：http://ek.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ut.newstarts.cn

[S11] C：逐行读文件
来源：http://oy.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://mj.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ri.bookmarksfly.cn

fclose(f);
来源：http://vf.newstarts.cn

[S12] C：写文件
来源：http://zt.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vf.yuexingan06.cn

[S13] C：宏定义
来源：http://sn.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vd.hahajie.cn

[S14] C：枚举
来源：http://tb.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://zo.yuntaijiaju.cn

[S15] C：类型转换
来源：http://yy.haigaiapp.cn

(double) a / b
来源：http://rn.bookmarksfly.cn

[S16] C：位操作置位
来源：http://do.nszjky.cn

x |= (1 << 3);
来源：http://ex.asd995.cn

[S17] C：安全拼接字符串
来源：http://lz.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qj.lnxyls.cn

[S18] C：命令行参数
来源：http://sg.muxihuayi.cn

int main(int argc, char **argv)
来源：http://dv.chemitech.net.cn

[S19] C：快速排序
来源：http://ru.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fy.9csxet.cn

[S20] C：二分查找
来源：http://tq.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://af.nicolike.cn

[S21] C：字符类别判断
来源：http://gh.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dx.asd995.cn

[S22] C：字符串转数字
来源：http://ss.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sz.shxzukj.cn

[S23] C：随机数
来源：http://ab.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://so.shxzskj.cn

[S24] C：获取本地时间
来源：http://cr.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xw.bjjhwx.cn

[S25] C：内存拷贝
来源：http://qa.shtwfgs.cn

memcpy(dst, src, n);
来源：http://ti.jctech888.com.cn

[S26] C：内存清零
来源：http://fo.szsharing.cn

memset(a, 0, sizeof a);
来源：http://go.hahajie.cn

[S27] C：定义常量
来源：http://qq.huixiangedu.cn

const double PI = 3.14159;
来源：http://qg.shtwfgs.cn

[S28] C：静态变量
来源：http://wi.huanxung.cn

static int counter = 0;
来源：http://vi.asd995.cn

[S29] C：变参函数
来源：http://th.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hx.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://jv.shxzukj.cn

#ifndef X_H
来源：http://on.huanxung.cn

#define X_H
来源：http://bq.yuexingan06.cn

#endif
来源：http://kx.jctech888.com.cn

[S31] C++：Hello World
来源：http://mb.newstarts.cn

#include <iostream>
来源：http://yd.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://tw.muxihuayi.cn

[S32] C++：字符串
来源：http://fq.colortex.cn

std::string s = "hi";  s += "!";
来源：http://az.gzmigu.cn

[S33] C++：vector 增删
来源：http://xy.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://le.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://gj.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ks.asd995.cn

[S35] C++：map
来源：http://qo.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fr.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://nn.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jz.jctech888.com.cn

[S37] C++：set
来源：http://mh.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nv.bjjhwx.cn

[S38] C++：排序
来源：http://xf.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://cn.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://dn.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://td.hahajie.cn

[S40] C++：查找元素
来源：http://da.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zs.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://pt.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ng.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://bi.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://yz.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://zs.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://jx.huixiangedu.cn

[S44] C++：引用传参
来源：http://lf.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://on.521024.cn

[S45] C++：lambda
来源：http://gg.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xw.nszjky.cn

[S46] C++：函数模板
来源：http://ax.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uf.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://jx.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ob.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://zo.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tp.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ak.jctech888.com.cn

[S49] C++：写文件
来源：http://tx.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bm.shxzskj.cn

[S50] C++：格式化数字
来源：http://ve.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vo.szxytkj.cn

[S51] C++：显式类型转换
来源：http://cp.panjiajie.cn

static_cast<double>(a) / b
来源：http://gk.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://uz.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://tw.bookmarksfly.cn

[S53] C++：移动语义
来源：http://nl.asd995.cn

std::vector<int> w = std::move(v);
来源：http://nm.yuexingan06.cn

[S54] C++：异常处理
来源：http://ut.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nv.hahajie.cn

[S55] C++：结构化绑定
来源：http://nn.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tm.nicolike.cn

[S56] C++：optional
来源：http://gx.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://we.shxzskj.cn

[S57] C++：编译期常量
来源：http://zi.521024.cn

constexpr int N = 10;
来源：http://sj.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://rg.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://cu.hahajie.cn

[S59] C++：静态断言
来源：http://ys.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://np.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://fc.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zu.lnxyls.cn

================================================================================
来源：http://vd.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xy.9csxet.cn

================================================================================
来源：http://nr.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://ji.hahajie.cn

println("Hello")
来源：http://pd.521024.cn

[T02] Kotlin：变量
来源：http://zw.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cd.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://fz.gzmigu.cn

"值: $b"
来源：http://zf.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://jq.521024.cn

val n: String? = null;  n?.length
来源：http://ks.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://mq.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ct.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://kn.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://px.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://gr.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vh.colortex.cn

[T08] Kotlin：数据类
来源：http://wm.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://au.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://he.colortex.cn

fun String.exclaim() = this + "!"
来源：http://vo.asd995.cn

[T10] Kotlin：默认参数
来源：http://yf.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://px.bjjhwx.cn

[T11] Kotlin：协程
来源：http://wj.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fj.9csxet.cn

[T12] Kotlin：解构声明
来源：http://ak.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://av.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://hi.nszjky.cn

val m = mapOf("a" to 1)
来源：http://gp.nicolike.cn

[T14] Kotlin：循环
来源：http://wu.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://hf.panjiajie.cn

[T15] Kotlin：接口
来源：http://ib.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://re.huixiangedu.cn

[T16] Swift：Hello World
来源：http://td.jctech888.com.cn

print("Hello")
来源：http://hn.shxzukj.cn

[T17] Swift：变量与常量
来源：http://hy.hahajie.cn

var a = 1;  let b = 2
来源：http://rl.huanxung.cn

[T18] Swift：字符串插值
来源：http://kx.muxihuayi.cn

"值: \(b)"
来源：http://fr.nicolike.cn

[T19] Swift：可选绑定
来源：http://ob.chemitech.net.cn

if let n = opt { print(n) }
来源：http://nm.hnjuh.cn

[T20] Swift：数组操作
来源：http://ja.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cn.yuexingan06.cn

[T21] Swift：遍历
来源：http://ls.nszjky.cn

for x in a { print(x) }
来源：http://qp.asd995.cn

[T22] Swift：字典
来源：http://un.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oj.szxytkj.cn

[T23] Swift：函数
来源：http://jq.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oz.szsharing.cn

[T24] Swift：闭包
来源：http://vu.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tf.lnxyls.cn

[T25] Swift：结构体
来源：http://ln.nszjky.cn

struct P { var x: Int }
来源：http://ss.haigaiapp.cn

[T26] Swift：类与重写
来源：http://pz.shxzskj.cn

class A: Base { override func f() {} }
来源：http://oh.colortex.cn

[T27] Swift：错误处理
来源：http://sz.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://zf.9csxet.cn

[T28] Swift：枚举
来源：http://rc.huixinmuqiang.cn

enum Color { case red, green }
来源：http://ni.asd995.cn

[T29] Swift：guard 提前返回
来源：http://ef.szsharing.cn

guard let x = opt else { return }
来源：http://kq.9csxet.cn

[T30] Swift：协议
来源：http://hy.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://mk.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://qn.521024.cn

print("Hello")
来源：http://wf.panjiajie.cn

[T32] Lua：局部变量
来源：http://xd.jianghongdianzi.cn

local a = 1
来源：http://cp.gzmigu.cn

[T33] Lua：表（数组）
来源：http://rv.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xn.yuexingan06.cn

[T34] Lua：遍历表
来源：http://gv.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fo.bjjhwx.cn

[T35] Lua：字典表
来源：http://sn.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://bn.yuntaijiaju.cn

[T36] Lua：函数
来源：http://fr.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://ki.szsharing.cn

[T37] Lua：字符串拼接
来源：http://qg.huixiangedu.cn

"a" .. "b"
来源：http://wf.panjiajie.cn

[T38] Lua：条件
来源：http://fy.hnjuh.cn

if x > 0 then print("正") end
来源：http://tp.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://zm.chemitech.net.cn

string.find(s, "%d+")
来源：http://wh.bookmarksfly.cn

[T40] Lua：元表
来源：http://pf.9csxet.cn

setmetatable({}, { __index = base })
来源：http://wb.shtwfgs.cn

[T41] Perl：Hello World
来源：http://dz.huixiangedu.cn

print "Hello\n";
来源：http://jn.bjjhwx.cn

[T42] Perl：变量类型
来源：http://yl.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://am.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://kl.bjjhwx.cn

"值: $a"
来源：http://lp.muxihuayi.cn

[T44] Perl：条件
来源：http://xp.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://ux.521024.cn

[T45] Perl：数组遍历
来源：http://ln.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://ko.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://ag.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hu.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://an.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pg.muxihuayi.cn

[T48] Perl：正则替换
来源：http://jo.newstarts.cn

$s =~ s/old/new/g;
来源：http://sv.hahajie.cn

[T49] Perl：函数
来源：http://mb.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vf.nicolike.cn

[T50] Perl：逐行读文件
来源：http://xy.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vs.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://if.yuexingan06.cn

[T51] Scala：Hello World
来源：http://bi.colortex.cn

println("Hello")
来源：http://pz.newstarts.cn

[T52] Scala：变量
来源：http://lf.yuexingan06.cn

val a = 1;  var b = 2
来源：http://yx.nicolike.cn

[T53] Scala：字符串插值
来源：http://vy.haigaiapp.cn

s"值: $b"
来源：http://wb.haigaiapp.cn

[T54] Scala：集合映射
来源：http://in.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://fj.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://tu.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vk.shtwfgs.cn

[T56] Scala：样例类
来源：http://ug.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://et.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://zy.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kq.shxzskj.cn

[T58] Scala：函数定义
来源：http://gk.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yh.bookmarksfly.cn

[T59] Scala：循环
来源：http://us.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://gc.jctech888.com.cn

[T60] Scala：折叠
来源：http://fm.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xb.jianghongdianzi.cn

================================================================================
来源：http://gr.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gm.jianghongdianzi.cn

================================================================================
来源：http://ui.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://zj.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jy.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://hh.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mw.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://jp.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sb.nicolike.cn

[U04] Py：变量调试打印
来源：http://ig.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gy.hahajie.cn

[U05] Py：列表去重且保序
来源：http://ve.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://cp.shxzukj.cn

[U06] Py：合并两个字典
来源：http://dy.bjjhwx.cn

{**a, **b}
来源：http://ax.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://ym.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://di.szsharing.cn

[U08] Py：展平二维列表
来源：http://nx.chemitech.net.cn

[y for x in nested for y in x]
来源：http://xu.521024.cn

[U09] Py：字典取最大值的键
来源：http://km.jianghongdianzi.cn

max(d, key=d.get)
来源：http://lp.asd995.cn

[U10] Py：按值排序字典
来源：http://zh.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jk.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://jt.haigaiapp.cn

(x * 2 for x in arr)
来源：http://fd.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fz.9csxet.cn

Counter(arr).most_common(3)
来源：http://op.gzmigu.cn

[U13] Py：固定长度队列
来源：http://su.hnjuh.cn

deque(maxlen=10)
来源：http://lu.521024.cn

[U14] Py：分组收集到列表
来源：http://fx.shxzskj.cn

defaultdict(list)
来源：http://ov.9csxet.cn

[U15] Py：高精度计时
来源：http://jh.asd995.cn

t = time.perf_counter()
来源：http://bb.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://yg.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xr.gzmigu.cn


<!-- 参考信息 -->