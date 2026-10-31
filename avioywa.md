代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://xs.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://ju.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oi.muxihuayi.cn

[R73] 分割大日志
来源：http://cn.shtwfgs.cn

split -l 1000 big.log part_
来源：http://up.jianghongdianzi.cn

[R74] 批量重命名
来源：http://de.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oa.bookmarksfly.cn

[R75] 导出环境变量
来源：http://le.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://po.shtwfgs.cn

[R76] 使用临时文件
来源：http://jg.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ox.szxytkj.cn

[R77] 读取用户输入
来源：http://ln.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://iy.lnxyls.cn

[R78] 交互式菜单
来源：http://su.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lp.lnxyls.cn

[R79] 解析命令行选项
来源：http://hs.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qa.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://eq.nszjky.cn

time ./run.sh
来源：http://xp.jctech888.com.cn

================================================================================
来源：http://ni.asd995.cn

S. C / C++ 专题
来源：http://oz.nicolike.cn

================================================================================
来源：http://rw.shxzskj.cn

[S01] C：Hello World
来源：http://wr.szxytkj.cn

#include <stdio.h>
来源：http://tn.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gt.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://av.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://yw.nicolike.cn

[S03] C：读入整数
来源：http://bm.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://dt.gzmigu.cn

[S04] C：字符串复制
来源：http://bj.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ga.haigaiapp.cn

[S05] C：字符串长度
来源：http://mq.gzmigu.cn

strlen(s)
来源：http://nu.asd995.cn

[S06] C：字符串比较
来源：http://gb.chemitech.net.cn

strcmp(a, b) == 0
来源：http://dg.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://jc.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hr.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://rl.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ik.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://th.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://na.9csxet.cn

[S10] C：指针与解引用
来源：http://bd.colortex.cn

int *p = &a;  *p = 5;
来源：http://mw.nicolike.cn

[S11] C：逐行读文件
来源：http://bu.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ej.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ih.521024.cn

fclose(f);
来源：http://zr.9csxet.cn

[S12] C：写文件
来源：http://ni.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cw.nicolike.cn

[S13] C：宏定义
来源：http://ed.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pp.yuexingan06.cn

[S14] C：枚举
来源：http://oi.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://ce.lnxyls.cn

[S15] C：类型转换
来源：http://vw.szsharing.cn

(double) a / b
来源：http://ak.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://ql.jianghongdianzi.cn

x |= (1 << 3);
来源：http://qp.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://ek.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sb.yuexingan06.cn

[S18] C：命令行参数
来源：http://iz.shtwfgs.cn

int main(int argc, char **argv)
来源：http://py.lnxyls.cn

[S19] C：快速排序
来源：http://lt.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sd.huixiangedu.cn

[S20] C：二分查找
来源：http://wl.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yw.huixiangedu.cn

[S21] C：字符类别判断
来源：http://gv.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ya.jctech888.com.cn

[S22] C：字符串转数字
来源：http://fb.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oe.muxihuayi.cn

[S23] C：随机数
来源：http://zm.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xl.shxzukj.cn

[S24] C：获取本地时间
来源：http://kp.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rz.colortex.cn

[S25] C：内存拷贝
来源：http://dt.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://im.521024.cn

[S26] C：内存清零
来源：http://ah.szsharing.cn

memset(a, 0, sizeof a);
来源：http://fu.shtwfgs.cn

[S27] C：定义常量
来源：http://dc.bjjhwx.cn

const double PI = 3.14159;
来源：http://iu.haigaiapp.cn

[S28] C：静态变量
来源：http://no.colortex.cn

static int counter = 0;
来源：http://vq.newstarts.cn

[S29] C：变参函数
来源：http://li.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hu.colortex.cn

[S30] C：头文件保护
来源：http://ct.nicolike.cn

#ifndef X_H
来源：http://xj.gzmigu.cn

#define X_H
来源：http://kr.521024.cn

#endif
来源：http://ct.newstarts.cn

[S31] C++：Hello World
来源：http://pn.szxytkj.cn

#include <iostream>
来源：http://yl.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://fy.chemitech.net.cn

[S32] C++：字符串
来源：http://ma.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://wf.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ip.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ee.nszjky.cn

[S34] C++：遍历 vector
来源：http://jc.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://wv.jctech888.com.cn

[S35] C++：map
来源：http://yi.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cn.521024.cn

[S36] C++：unordered_map
来源：http://gd.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bp.newstarts.cn

[S37] C++：set
来源：http://ot.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qs.shxzukj.cn

[S38] C++：排序
来源：http://we.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://gz.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://ij.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dk.colortex.cn

[S40] C++：查找元素
来源：http://ql.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ll.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://km.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oo.asd995.cn

[S42] C++：继承与虚函数
来源：http://nm.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://gm.haigaiapp.cn

[S43] C++：智能指针
来源：http://ga.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://au.panjiajie.cn

[S44] C++：引用传参
来源：http://on.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://vw.asd995.cn

[S45] C++：lambda
来源：http://sc.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rw.szxytkj.cn

[S46] C++：函数模板
来源：http://kl.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xn.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://vl.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hv.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://jz.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mp.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://sd.nicolike.cn

[S49] C++：写文件
来源：http://ug.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://up.colortex.cn

[S50] C++：格式化数字
来源：http://en.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gy.szxytkj.cn

[S51] C++：显式类型转换
来源：http://vg.nicolike.cn

static_cast<double>(a) / b
来源：http://vp.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://ti.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://fq.shtwfgs.cn

[S53] C++：移动语义
来源：http://ly.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://pi.nszjky.cn

[S54] C++：异常处理
来源：http://zo.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zv.nicolike.cn

[S55] C++：结构化绑定
来源：http://ha.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ib.yuntaijiaju.cn

[S56] C++：optional
来源：http://tw.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mk.huanxung.cn

[S57] C++：编译期常量
来源：http://jk.huixinmuqiang.cn

constexpr int N = 10;
来源：http://hm.jctech888.com.cn

[S58] C++：命名空间
来源：http://ne.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://ey.newstarts.cn

[S59] C++：静态断言
来源：http://mk.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ef.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://vd.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://am.bookmarksfly.cn

================================================================================
来源：http://nx.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qa.hnjuh.cn

================================================================================
来源：http://zx.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://se.yuntaijiaju.cn

println("Hello")
来源：http://pi.shxzukj.cn

[T02] Kotlin：变量
来源：http://xy.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://it.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://uj.bjjhwx.cn

"值: $b"
来源：http://uk.shxzskj.cn

[T04] Kotlin：空安全
来源：http://xn.nszjky.cn

val n: String? = null;  n?.length
来源：http://td.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://ws.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mv.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://oj.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eg.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://nt.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lf.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://zu.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://qn.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://hm.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://ng.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://bz.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://th.shtwfgs.cn

[T11] Kotlin：协程
来源：http://zo.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ru.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://yt.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://ee.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://zj.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://rh.bjjhwx.cn

[T14] Kotlin：循环
来源：http://ju.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://ch.9csxet.cn

[T15] Kotlin：接口
来源：http://na.9csxet.cn

interface Shape { fun area(): Double }
来源：http://ie.wgjwhj.cn

[T16] Swift：Hello World
来源：http://kg.wgjwhj.cn

print("Hello")
来源：http://af.shxzukj.cn

[T17] Swift：变量与常量
来源：http://dn.shtwfgs.cn

var a = 1;  let b = 2
来源：http://xu.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://ck.wgjwhj.cn

"值: \(b)"
来源：http://un.asd995.cn

[T19] Swift：可选绑定
来源：http://rs.shxzukj.cn

if let n = opt { print(n) }
来源：http://kp.shtwfgs.cn

[T20] Swift：数组操作
来源：http://yh.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wy.muxihuayi.cn

[T21] Swift：遍历
来源：http://tr.newstarts.cn

for x in a { print(x) }
来源：http://cg.nszjky.cn

[T22] Swift：字典
来源：http://lw.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://td.521024.cn

[T23] Swift：函数
来源：http://zt.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bc.wgjwhj.cn

[T24] Swift：闭包
来源：http://nq.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uj.shxzskj.cn

[T25] Swift：结构体
来源：http://du.asd995.cn

struct P { var x: Int }
来源：http://hm.panjiajie.cn

[T26] Swift：类与重写
来源：http://ec.panjiajie.cn

class A: Base { override func f() {} }
来源：http://rd.szxytkj.cn

[T27] Swift：错误处理
来源：http://jh.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://jy.yuexingan06.cn

[T28] Swift：枚举
来源：http://px.jianghongdianzi.cn

enum Color { case red, green }
来源：http://jx.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://ci.panjiajie.cn

guard let x = opt else { return }
来源：http://om.shtwfgs.cn

[T30] Swift：协议
来源：http://ql.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://mc.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://yy.panjiajie.cn

print("Hello")
来源：http://zs.huanxung.cn

[T32] Lua：局部变量
来源：http://ly.huixiangedu.cn

local a = 1
来源：http://qp.szxytkj.cn

[T33] Lua：表（数组）
来源：http://np.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dk.asd995.cn

[T34] Lua：遍历表
来源：http://iu.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xs.huixiangedu.cn

[T35] Lua：字典表
来源：http://kd.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://ly.colortex.cn

[T36] Lua：函数
来源：http://vv.asd995.cn

function add(a, b) return a + b end
来源：http://um.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://ic.chemitech.net.cn

"a" .. "b"
来源：http://mi.jctech888.com.cn

[T38] Lua：条件
来源：http://qq.huanxung.cn

if x > 0 then print("正") end
来源：http://zh.nicolike.cn

[T39] Lua：模式匹配
来源：http://ny.shxzskj.cn

string.find(s, "%d+")
来源：http://fl.szsharing.cn

[T40] Lua：元表
来源：http://dl.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://aq.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://fy.521024.cn

print "Hello\n";
来源：http://xc.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://tq.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ca.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://zx.shtwfgs.cn

"值: $a"
来源：http://hj.9csxet.cn

[T44] Perl：条件
来源：http://oa.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://zg.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://ah.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://xg.gzmigu.cn

[T46] Perl：哈希操作
来源：http://yt.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://te.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://ce.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sl.hnjuh.cn

[T48] Perl：正则替换
来源：http://be.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://ga.huixinmuqiang.cn

[T49] Perl：函数
来源：http://pp.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kd.asd995.cn

[T50] Perl：逐行读文件
来源：http://ly.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eb.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://fr.jctech888.com.cn

[T51] Scala：Hello World
来源：http://pb.shxzukj.cn

println("Hello")
来源：http://ne.colortex.cn

[T52] Scala：变量
来源：http://yq.hnjuh.cn

val a = 1;  var b = 2
来源：http://ke.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ax.521024.cn

s"值: $b"
来源：http://nw.szsharing.cn

[T54] Scala：集合映射
来源：http://yi.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://bm.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://tx.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ih.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://iz.hnjuh.cn

case class User(name: String, age: Int)
来源：http://gs.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://mf.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ji.hahajie.cn

[T58] Scala：函数定义
来源：http://kr.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kt.huixiangedu.cn

[T59] Scala：循环
来源：http://lq.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://pa.newstarts.cn

[T60] Scala：折叠
来源：http://re.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mw.shtwfgs.cn

================================================================================
来源：http://zr.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xp.9csxet.cn

================================================================================
来源：http://qy.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://do.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bi.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://vv.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vh.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://zx.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qf.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://oi.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://in.nszjky.cn

[U05] Py：列表去重且保序
来源：http://qe.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://sa.nicolike.cn

[U06] Py：合并两个字典
来源：http://qf.521024.cn

{**a, **b}
来源：http://ph.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://kg.asd995.cn

{v: k for k, v in d.items()}
来源：http://bn.hnjuh.cn

[U08] Py：展平二维列表
来源：http://cd.bjjhwx.cn

[y for x in nested for y in x]
来源：http://kp.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://ao.chemitech.net.cn

max(d, key=d.get)
来源：http://bq.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://xr.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ms.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://rm.bjjhwx.cn

(x * 2 for x in arr)
来源：http://pz.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dp.nicolike.cn

Counter(arr).most_common(3)
来源：http://be.gzmigu.cn


<!-- 参考信息 -->