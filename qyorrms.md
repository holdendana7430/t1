代发 wailian999

openssl rand -hex 16
来源：http://lm.chemitech.net.cn

[R68] 计算文件校验值
来源：http://pm.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pj.gzmigu.cn

[R69] 生成随机密码
来源：http://gn.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://hx.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://rw.szsharing.cn

date +%s;  date -d @1700000000
来源：http://go.muxihuayi.cn

[R71] 日期格式化
来源：http://pa.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rv.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://xr.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ud.shtwfgs.cn

[R73] 分割大日志
来源：http://hb.szsharing.cn

split -l 1000 big.log part_
来源：http://fj.huixiangedu.cn

[R74] 批量重命名
来源：http://jv.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ll.bjjhwx.cn

[R75] 导出环境变量
来源：http://mf.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://eu.panjiajie.cn

[R76] 使用临时文件
来源：http://uh.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bx.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://ly.nszjky.cn

read -rp "请输入: " ans
来源：http://vw.huanxung.cn

[R78] 交互式菜单
来源：http://xi.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mk.nicolike.cn

[R79] 解析命令行选项
来源：http://vt.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kx.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://ox.nszjky.cn

time ./run.sh
来源：http://oh.hnjuh.cn

================================================================================
来源：http://rx.wgjwhj.cn

S. C / C++ 专题
来源：http://sr.shxzskj.cn

================================================================================
来源：http://ks.gzmigu.cn

[S01] C：Hello World
来源：http://wv.shtwfgs.cn

#include <stdio.h>
来源：http://sz.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cr.521024.cn

[S02] C：变量与格式化输出
来源：http://af.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://kx.gzmigu.cn

[S03] C：读入整数
来源：http://qk.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://rk.asd995.cn

[S04] C：字符串复制
来源：http://ex.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ql.shtwfgs.cn

[S05] C：字符串长度
来源：http://dg.newstarts.cn

strlen(s)
来源：http://yp.colortex.cn

[S06] C：字符串比较
来源：http://lj.nicolike.cn

strcmp(a, b) == 0
来源：http://zh.szsharing.cn

[S07] C：数组遍历求和
来源：http://ht.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hk.asd995.cn

[S08] C：动态内存分配与释放
来源：http://pm.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fe.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://fi.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xr.haigaiapp.cn

[S10] C：指针与解引用
来源：http://pl.9csxet.cn

int *p = &a;  *p = 5;
来源：http://ve.szsharing.cn

[S11] C：逐行读文件
来源：http://ux.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://uw.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pj.yuntaijiaju.cn

fclose(f);
来源：http://ca.huixiangedu.cn

[S12] C：写文件
来源：http://vr.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ij.bookmarksfly.cn

[S13] C：宏定义
来源：http://zh.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://om.lnxyls.cn

[S14] C：枚举
来源：http://tw.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://dh.hahajie.cn

[S15] C：类型转换
来源：http://bd.gzmigu.cn

(double) a / b
来源：http://md.wgjwhj.cn

[S16] C：位操作置位
来源：http://xe.lnxyls.cn

x |= (1 << 3);
来源：http://vl.szsharing.cn

[S17] C：安全拼接字符串
来源：http://jm.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dw.nicolike.cn

[S18] C：命令行参数
来源：http://jn.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ly.szxytkj.cn

[S19] C：快速排序
来源：http://ze.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ji.9csxet.cn

[S20] C：二分查找
来源：http://et.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cr.nszjky.cn

[S21] C：字符类别判断
来源：http://my.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cg.chemitech.net.cn

[S22] C：字符串转数字
来源：http://kk.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qk.szxytkj.cn

[S23] C：随机数
来源：http://uz.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nj.muxihuayi.cn

[S24] C：获取本地时间
来源：http://ft.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vb.szsharing.cn

[S25] C：内存拷贝
来源：http://ns.hahajie.cn

memcpy(dst, src, n);
来源：http://bd.wgjwhj.cn

[S26] C：内存清零
来源：http://og.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://ki.szsharing.cn

[S27] C：定义常量
来源：http://lh.szsharing.cn

const double PI = 3.14159;
来源：http://ni.newstarts.cn

[S28] C：静态变量
来源：http://ix.haigaiapp.cn

static int counter = 0;
来源：http://yp.nszjky.cn

[S29] C：变参函数
来源：http://xg.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ob.hahajie.cn

[S30] C：头文件保护
来源：http://qu.9csxet.cn

#ifndef X_H
来源：http://mq.yuexingan06.cn

#define X_H
来源：http://ds.nicolike.cn

#endif
来源：http://mh.chemitech.net.cn

[S31] C++：Hello World
来源：http://zy.szsharing.cn

#include <iostream>
来源：http://hw.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://fc.nszjky.cn

[S32] C++：字符串
来源：http://zc.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://uz.asd995.cn

[S33] C++：vector 增删
来源：http://ni.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sa.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://in.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ao.jctech888.com.cn

[S35] C++：map
来源：http://lu.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://no.muxihuayi.cn

[S36] C++：unordered_map
来源：http://vs.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yb.szsharing.cn

[S37] C++：set
来源：http://ka.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ns.jctech888.com.cn

[S38] C++：排序
来源：http://fo.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://uo.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://ga.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nx.shxzukj.cn

[S40] C++：查找元素
来源：http://vt.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xh.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ud.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://if.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://ls.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://wy.bjjhwx.cn

[S43] C++：智能指针
来源：http://tj.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://la.yuexingan06.cn

[S44] C++：引用传参
来源：http://al.nicolike.cn

void inc(int &x) { ++x; }
来源：http://mo.huanxung.cn

[S45] C++：lambda
来源：http://if.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tm.lnxyls.cn

[S46] C++：函数模板
来源：http://rs.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rv.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://ut.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qs.lnxyls.cn

[S48] C++：逐行读文件
来源：http://ta.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dl.nicolike.cn

while (std::getline(in, line)) { }
来源：http://hh.huanxung.cn

[S49] C++：写文件
来源：http://qp.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fo.szxytkj.cn

[S50] C++：格式化数字
来源：http://wj.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mx.nszjky.cn

[S51] C++：显式类型转换
来源：http://ko.shxzukj.cn

static_cast<double>(a) / b
来源：http://dv.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://nd.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ne.haigaiapp.cn

[S53] C++：移动语义
来源：http://ud.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://iv.521024.cn

[S54] C++：异常处理
来源：http://lf.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pk.shxzskj.cn

[S55] C++：结构化绑定
来源：http://kq.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wy.shxzskj.cn

[S56] C++：optional
来源：http://mb.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://te.9csxet.cn

[S57] C++：编译期常量
来源：http://gj.shxzukj.cn

constexpr int N = 10;
来源：http://jt.yuexingan06.cn

[S58] C++：命名空间
来源：http://qv.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://wl.nszjky.cn

[S59] C++：静态断言
来源：http://mf.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://be.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://rg.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oh.lnxyls.cn

================================================================================
来源：http://gj.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lx.wgjwhj.cn

================================================================================
来源：http://bv.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ur.shxzskj.cn

println("Hello")
来源：http://ao.521024.cn

[T02] Kotlin：变量
来源：http://do.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fp.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://ak.asd995.cn

"值: $b"
来源：http://io.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://sv.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://ax.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://hl.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ft.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://zs.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://or.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://jp.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uh.hnjuh.cn

[T08] Kotlin：数据类
来源：http://ra.521024.cn

data class User(val name: String, val age: Int)
来源：http://bk.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://gx.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://gz.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://as.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ur.chemitech.net.cn

[T11] Kotlin：协程
来源：http://vw.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ui.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://ae.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://ts.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://zk.colortex.cn

val m = mapOf("a" to 1)
来源：http://uv.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://ca.shxzukj.cn

for (i in 1..10) println(i)
来源：http://zu.panjiajie.cn

[T15] Kotlin：接口
来源：http://is.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://ma.colortex.cn

[T16] Swift：Hello World
来源：http://fb.yuexingan06.cn

print("Hello")
来源：http://oe.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://zc.colortex.cn

var a = 1;  let b = 2
来源：http://rb.shxzskj.cn

[T18] Swift：字符串插值
来源：http://kf.chemitech.net.cn

"值: \(b)"
来源：http://ve.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://gc.gzmigu.cn

if let n = opt { print(n) }
来源：http://bu.shtwfgs.cn

[T20] Swift：数组操作
来源：http://we.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mq.hahajie.cn

[T21] Swift：遍历
来源：http://fv.bjjhwx.cn

for x in a { print(x) }
来源：http://ey.gzmigu.cn

[T22] Swift：字典
来源：http://uk.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pr.nicolike.cn

[T23] Swift：函数
来源：http://ew.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bg.wgjwhj.cn

[T24] Swift：闭包
来源：http://gl.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zd.yuexingan06.cn

[T25] Swift：结构体
来源：http://kz.panjiajie.cn

struct P { var x: Int }
来源：http://xv.huanxung.cn

[T26] Swift：类与重写
来源：http://oi.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://id.newstarts.cn

[T27] Swift：错误处理
来源：http://js.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://me.szxytkj.cn

[T28] Swift：枚举
来源：http://ab.muxihuayi.cn

enum Color { case red, green }
来源：http://ks.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://gs.asd995.cn

guard let x = opt else { return }
来源：http://pe.gzmigu.cn

[T30] Swift：协议
来源：http://oo.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://fn.chemitech.net.cn

[T31] Lua：Hello World
来源：http://ks.9csxet.cn

print("Hello")
来源：http://ya.huixiangedu.cn

[T32] Lua：局部变量
来源：http://fm.hnjuh.cn

local a = 1
来源：http://ay.szsharing.cn

[T33] Lua：表（数组）
来源：http://lt.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rc.nszjky.cn

[T34] Lua：遍历表
来源：http://is.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yf.szxytkj.cn

[T35] Lua：字典表
来源：http://rx.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://tp.shxzukj.cn

[T36] Lua：函数
来源：http://xr.shxzskj.cn

function add(a, b) return a + b end
来源：http://ee.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://mt.shxzukj.cn

"a" .. "b"
来源：http://dx.szxytkj.cn

[T38] Lua：条件
来源：http://aw.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://vt.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://sg.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://kd.bookmarksfly.cn

[T40] Lua：元表
来源：http://ds.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://vu.haigaiapp.cn

[T41] Perl：Hello World
来源：http://hq.huixiangedu.cn

print "Hello\n";
来源：http://pt.shxzukj.cn

[T42] Perl：变量类型
来源：http://fg.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gv.shxzukj.cn

[T43] Perl：字符串插值
来源：http://sn.521024.cn

"值: $a"
来源：http://za.shtwfgs.cn

[T44] Perl：条件
来源：http://gi.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://am.hnjuh.cn

[T45] Perl：数组遍历
来源：http://zm.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://im.asd995.cn

[T46] Perl：哈希操作
来源：http://yx.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qx.shxzukj.cn

[T47] Perl：正则捕获
来源：http://nr.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dy.shxzukj.cn

[T48] Perl：正则替换
来源：http://wm.gzmigu.cn

$s =~ s/old/new/g;
来源：http://cy.newstarts.cn

[T49] Perl：函数
来源：http://gz.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qs.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://wq.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://se.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://di.jctech888.com.cn

[T51] Scala：Hello World
来源：http://fs.huixiangedu.cn

println("Hello")
来源：http://tp.newstarts.cn

[T52] Scala：变量
来源：http://fi.nicolike.cn

val a = 1;  var b = 2
来源：http://er.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://oz.muxihuayi.cn

s"值: $b"
来源：http://dm.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://gw.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://er.panjiajie.cn

[T55] Scala：集合过滤
来源：http://lv.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bw.colortex.cn

[T56] Scala：样例类
来源：http://te.shxzskj.cn

case class User(name: String, age: Int)
来源：http://yn.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://lp.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fp.jctech888.com.cn

[T58] Scala：函数定义
来源：http://xq.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ba.wgjwhj.cn

[T59] Scala：循环
来源：http://kt.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://uh.szsharing.cn

[T60] Scala：折叠
来源：http://aw.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zg.nicolike.cn

================================================================================
来源：http://ep.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vt.nicolike.cn

================================================================================
来源：http://tq.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://gm.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jc.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://lc.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ni.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://gl.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lu.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ic.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fx.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://zt.szsharing.cn

list(dict.fromkeys(arr))
来源：http://sg.newstarts.cn

[U06] Py：合并两个字典
来源：http://tt.panjiajie.cn

{**a, **b}
来源：http://gn.panjiajie.cn

[U07] Py：反转字典键值
来源：http://tk.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://cq.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://au.bjjhwx.cn

[y for x in nested for y in x]
来源：http://fj.521024.cn


<!-- 参考信息 -->