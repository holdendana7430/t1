代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://op.9csxet.cn

[R72] 等待端口就绪
来源：http://bi.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gd.shxzukj.cn

[R73] 分割大日志
来源：http://ys.hnjuh.cn

split -l 1000 big.log part_
来源：http://il.szsharing.cn

[R74] 批量重命名
来源：http://qd.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ac.newstarts.cn

[R75] 导出环境变量
来源：http://dx.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://au.haigaiapp.cn

[R76] 使用临时文件
来源：http://uw.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qm.shtwfgs.cn

[R77] 读取用户输入
来源：http://el.huanxung.cn

read -rp "请输入: " ans
来源：http://lf.szxytkj.cn

[R78] 交互式菜单
来源：http://pr.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tz.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ba.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vi.colortex.cn

[R80] 查看脚本执行耗时
来源：http://ll.gzmigu.cn

time ./run.sh
来源：http://zu.gzmigu.cn

================================================================================
来源：http://bk.newstarts.cn

S. C / C++ 专题
来源：http://xg.bookmarksfly.cn

================================================================================
来源：http://mr.hnjuh.cn

[S01] C：Hello World
来源：http://tr.huixinmuqiang.cn

#include <stdio.h>
来源：http://aa.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dr.hahajie.cn

[S02] C：变量与格式化输出
来源：http://ax.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://qm.huixinmuqiang.cn

[S03] C：读入整数
来源：http://yh.nicolike.cn

int x; scanf("%d", &x);
来源：http://el.asd995.cn

[S04] C：字符串复制
来源：http://qk.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kk.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://dq.shtwfgs.cn

strlen(s)
来源：http://zg.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://sg.huanxung.cn

strcmp(a, b) == 0
来源：http://vt.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://rc.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hu.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://tq.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vv.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://rd.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ig.chemitech.net.cn

[S10] C：指针与解引用
来源：http://go.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://qb.panjiajie.cn

[S11] C：逐行读文件
来源：http://ct.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://li.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xh.gzmigu.cn

fclose(f);
来源：http://eh.shxzukj.cn

[S12] C：写文件
来源：http://gv.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ge.colortex.cn

[S13] C：宏定义
来源：http://ts.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kk.newstarts.cn

[S14] C：枚举
来源：http://of.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://pc.asd995.cn

[S15] C：类型转换
来源：http://dy.colortex.cn

(double) a / b
来源：http://la.bookmarksfly.cn

[S16] C：位操作置位
来源：http://vv.chemitech.net.cn

x |= (1 << 3);
来源：http://ot.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://yd.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ur.bookmarksfly.cn

[S18] C：命令行参数
来源：http://wk.shxzukj.cn

int main(int argc, char **argv)
来源：http://vr.yuexingan06.cn

[S19] C：快速排序
来源：http://hg.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yz.jctech888.com.cn

[S20] C：二分查找
来源：http://sy.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gh.panjiajie.cn

[S21] C：字符类别判断
来源：http://dr.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iq.huixiangedu.cn

[S22] C：字符串转数字
来源：http://sw.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yu.szxytkj.cn

[S23] C：随机数
来源：http://bn.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kz.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://pe.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qu.shxzukj.cn

[S25] C：内存拷贝
来源：http://yv.haigaiapp.cn

memcpy(dst, src, n);
来源：http://ba.nicolike.cn

[S26] C：内存清零
来源：http://nr.szsharing.cn

memset(a, 0, sizeof a);
来源：http://kg.9csxet.cn

[S27] C：定义常量
来源：http://dr.colortex.cn

const double PI = 3.14159;
来源：http://kt.yuntaijiaju.cn

[S28] C：静态变量
来源：http://cj.hahajie.cn

static int counter = 0;
来源：http://wq.muxihuayi.cn

[S29] C：变参函数
来源：http://op.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kk.haigaiapp.cn

[S30] C：头文件保护
来源：http://ny.huanxung.cn

#ifndef X_H
来源：http://sz.chemitech.net.cn

#define X_H
来源：http://vj.yuexingan06.cn

#endif
来源：http://dd.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://hi.haigaiapp.cn

#include <iostream>
来源：http://hv.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://bt.haigaiapp.cn

[S32] C++：字符串
来源：http://ob.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://rp.gzmigu.cn

[S33] C++：vector 增删
来源：http://yp.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ys.hahajie.cn

[S34] C++：遍历 vector
来源：http://gs.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://px.yuntaijiaju.cn

[S35] C++：map
来源：http://ls.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://an.521024.cn

[S36] C++：unordered_map
来源：http://av.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jb.shtwfgs.cn

[S37] C++：set
来源：http://xd.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ww.shxzskj.cn

[S38] C++：排序
来源：http://jk.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://tv.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://bp.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ny.asd995.cn

[S40] C++：查找元素
来源：http://hn.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gp.521024.cn

[S41] C++：类与构造函数
来源：http://uu.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cu.huanxung.cn

[S42] C++：继承与虚函数
来源：http://ld.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ql.muxihuayi.cn

[S43] C++：智能指针
来源：http://wk.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://xz.bjjhwx.cn

[S44] C++：引用传参
来源：http://uc.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://xo.jctech888.com.cn

[S45] C++：lambda
来源：http://tw.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wb.shxzskj.cn

[S46] C++：函数模板
来源：http://do.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hi.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://lw.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nq.nszjky.cn

[S48] C++：逐行读文件
来源：http://fi.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fd.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://qo.muxihuayi.cn

[S49] C++：写文件
来源：http://cl.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dn.newstarts.cn

[S50] C++：格式化数字
来源：http://gq.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oj.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://ai.jctech888.com.cn

static_cast<double>(a) / b
来源：http://ey.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://mi.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://wn.colortex.cn

[S53] C++：移动语义
来源：http://pq.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://fw.gzmigu.cn

[S54] C++：异常处理
来源：http://ba.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kc.nszjky.cn

[S55] C++：结构化绑定
来源：http://zs.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jy.shxzukj.cn

[S56] C++：optional
来源：http://in.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mb.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://jt.jianghongdianzi.cn

constexpr int N = 10;
来源：http://ar.asd995.cn

[S58] C++：命名空间
来源：http://kd.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://yz.huanxung.cn

[S59] C++：静态断言
来源：http://yc.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dj.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://at.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nr.nszjky.cn

================================================================================
来源：http://rz.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ou.shxzskj.cn

================================================================================
来源：http://pz.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://ss.huixinmuqiang.cn

println("Hello")
来源：http://bg.newstarts.cn

[T02] Kotlin：变量
来源：http://xw.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rt.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://xk.yuntaijiaju.cn

"值: $b"
来源：http://vx.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://cf.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://wb.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://gv.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ul.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://cg.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nu.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://dj.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ul.hnjuh.cn

[T08] Kotlin：数据类
来源：http://fv.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://fi.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://oq.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://hy.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://mg.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ie.shxzukj.cn

[T11] Kotlin：协程
来源：http://sr.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fn.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://sa.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://la.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://or.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://zl.shxzukj.cn

[T14] Kotlin：循环
来源：http://eq.nszjky.cn

for (i in 1..10) println(i)
来源：http://vq.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://zf.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://sr.chemitech.net.cn

[T16] Swift：Hello World
来源：http://pc.jianghongdianzi.cn

print("Hello")
来源：http://ju.szxytkj.cn

[T17] Swift：变量与常量
来源：http://uf.hnjuh.cn

var a = 1;  let b = 2
来源：http://sd.szxytkj.cn

[T18] Swift：字符串插值
来源：http://wk.huanxung.cn

"值: \(b)"
来源：http://an.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://jk.521024.cn

if let n = opt { print(n) }
来源：http://mu.shtwfgs.cn

[T20] Swift：数组操作
来源：http://bu.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ux.huanxung.cn

[T21] Swift：遍历
来源：http://fa.9csxet.cn

for x in a { print(x) }
来源：http://lu.nicolike.cn

[T22] Swift：字典
来源：http://kw.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nf.huixiangedu.cn

[T23] Swift：函数
来源：http://em.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pb.chemitech.net.cn

[T24] Swift：闭包
来源：http://bz.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ui.colortex.cn

[T25] Swift：结构体
来源：http://bm.panjiajie.cn

struct P { var x: Int }
来源：http://ox.9csxet.cn

[T26] Swift：类与重写
来源：http://vf.521024.cn

class A: Base { override func f() {} }
来源：http://lp.nszjky.cn

[T27] Swift：错误处理
来源：http://de.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://up.9csxet.cn

[T28] Swift：枚举
来源：http://rw.colortex.cn

enum Color { case red, green }
来源：http://sl.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://ii.bookmarksfly.cn

guard let x = opt else { return }
来源：http://mr.gzmigu.cn

[T30] Swift：协议
来源：http://zs.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://ph.panjiajie.cn

[T31] Lua：Hello World
来源：http://xg.shxzskj.cn

print("Hello")
来源：http://cu.szxytkj.cn

[T32] Lua：局部变量
来源：http://vr.shxzukj.cn

local a = 1
来源：http://xq.521024.cn

[T33] Lua：表（数组）
来源：http://ds.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dr.521024.cn

[T34] Lua：遍历表
来源：http://nm.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xn.hahajie.cn

[T35] Lua：字典表
来源：http://gd.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://iu.jianghongdianzi.cn

[T36] Lua：函数
来源：http://wc.muxihuayi.cn

function add(a, b) return a + b end
来源：http://mo.colortex.cn

[T37] Lua：字符串拼接
来源：http://ge.szxytkj.cn

"a" .. "b"
来源：http://yr.huixiangedu.cn

[T38] Lua：条件
来源：http://ot.haigaiapp.cn

if x > 0 then print("正") end
来源：http://rz.newstarts.cn

[T39] Lua：模式匹配
来源：http://ve.nszjky.cn

string.find(s, "%d+")
来源：http://hy.newstarts.cn

[T40] Lua：元表
来源：http://rp.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://ph.haigaiapp.cn

[T41] Perl：Hello World
来源：http://hl.szsharing.cn

print "Hello\n";
来源：http://we.szxytkj.cn

[T42] Perl：变量类型
来源：http://dj.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ss.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://xa.huanxung.cn

"值: $a"
来源：http://bz.hahajie.cn

[T44] Perl：条件
来源：http://jk.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://oz.hnjuh.cn

[T45] Perl：数组遍历
来源：http://ha.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://oa.newstarts.cn

[T46] Perl：哈希操作
来源：http://pp.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jm.521024.cn

[T47] Perl：正则捕获
来源：http://zh.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tw.szxytkj.cn

[T48] Perl：正则替换
来源：http://lv.nicolike.cn

$s =~ s/old/new/g;
来源：http://qu.521024.cn

[T49] Perl：函数
来源：http://hj.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fs.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://kx.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fr.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://uo.szsharing.cn

[T51] Scala：Hello World
来源：http://xv.yuntaijiaju.cn

println("Hello")
来源：http://jp.muxihuayi.cn

[T52] Scala：变量
来源：http://xn.bjjhwx.cn

val a = 1;  var b = 2
来源：http://kf.nszjky.cn

[T53] Scala：字符串插值
来源：http://sw.hahajie.cn

s"值: $b"
来源：http://xi.shtwfgs.cn

[T54] Scala：集合映射
来源：http://ee.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://bw.shxzukj.cn

[T55] Scala：集合过滤
来源：http://zw.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ga.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://xa.szxytkj.cn

case class User(name: String, age: Int)
来源：http://me.shxzukj.cn

[T57] Scala：模式匹配
来源：http://wa.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pf.nicolike.cn

[T58] Scala：函数定义
来源：http://cb.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ij.shtwfgs.cn

[T59] Scala：循环
来源：http://mu.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://io.shxzukj.cn

[T60] Scala：折叠
来源：http://oo.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yk.shxzukj.cn

================================================================================
来源：http://qx.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aq.yuntaijiaju.cn

================================================================================
来源：http://vz.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://em.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yf.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://tj.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://id.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://vs.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dv.newstarts.cn

[U04] Py：变量调试打印
来源：http://eh.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ug.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://gb.nszjky.cn

list(dict.fromkeys(arr))
来源：http://hh.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://kx.szxytkj.cn

{**a, **b}
来源：http://xz.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://jk.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://uy.newstarts.cn

[U08] Py：展平二维列表
来源：http://tg.lnxyls.cn

[y for x in nested for y in x]
来源：http://ds.521024.cn

[U09] Py：字典取最大值的键
来源：http://iu.shtwfgs.cn

max(d, key=d.get)
来源：http://wr.szsharing.cn

[U10] Py：按值排序字典
来源：http://fc.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hu.szsharing.cn

[U11] Py：生成器表达式
来源：http://tj.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://pk.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dz.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://qa.9csxet.cn


<!-- 参考信息 -->