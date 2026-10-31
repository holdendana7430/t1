代发 wailian999

openssl rand -hex 16
来源：http://cr.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://tl.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://no.wgjwhj.cn

[R69] 生成随机密码
来源：http://ln.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://hq.szxytkj.cn

[R70] 时间戳与互转
来源：http://ih.colortex.cn

date +%s;  date -d @1700000000
来源：http://lu.jianghongdianzi.cn

[R71] 日期格式化
来源：http://pf.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nr.nszjky.cn

[R72] 等待端口就绪
来源：http://kf.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ft.nszjky.cn

[R73] 分割大日志
来源：http://bj.chemitech.net.cn

split -l 1000 big.log part_
来源：http://ey.szxytkj.cn

[R74] 批量重命名
来源：http://xk.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://co.panjiajie.cn

[R75] 导出环境变量
来源：http://vq.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://aq.nszjky.cn

[R76] 使用临时文件
来源：http://wm.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cy.shxzskj.cn

[R77] 读取用户输入
来源：http://zw.shxzukj.cn

read -rp "请输入: " ans
来源：http://eh.9csxet.cn

[R78] 交互式菜单
来源：http://wg.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yv.asd995.cn

[R79] 解析命令行选项
来源：http://kx.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bi.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://tq.colortex.cn

time ./run.sh
来源：http://wx.9csxet.cn

================================================================================
来源：http://pq.gzmigu.cn

S. C / C++ 专题
来源：http://li.colortex.cn

================================================================================
来源：http://or.nicolike.cn

[S01] C：Hello World
来源：http://dn.bjjhwx.cn

#include <stdio.h>
来源：http://yg.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oh.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://qd.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://jt.szsharing.cn

[S03] C：读入整数
来源：http://rh.gzmigu.cn

int x; scanf("%d", &x);
来源：http://bh.shtwfgs.cn

[S04] C：字符串复制
来源：http://yz.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://io.szsharing.cn

[S05] C：字符串长度
来源：http://qy.yuexingan06.cn

strlen(s)
来源：http://gz.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://kn.shxzskj.cn

strcmp(a, b) == 0
来源：http://ul.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://cd.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eo.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://gu.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ny.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://hr.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wy.huixiangedu.cn

[S10] C：指针与解引用
来源：http://vh.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://sp.panjiajie.cn

[S11] C：逐行读文件
来源：http://nm.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://vn.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://va.haigaiapp.cn

fclose(f);
来源：http://vx.shtwfgs.cn

[S12] C：写文件
来源：http://ge.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yt.nszjky.cn

[S13] C：宏定义
来源：http://nb.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sh.hahajie.cn

[S14] C：枚举
来源：http://at.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://aj.gzmigu.cn

[S15] C：类型转换
来源：http://xo.panjiajie.cn

(double) a / b
来源：http://ij.hahajie.cn

[S16] C：位操作置位
来源：http://qi.huanxung.cn

x |= (1 << 3);
来源：http://fj.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://nf.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kg.szxytkj.cn

[S18] C：命令行参数
来源：http://ka.asd995.cn

int main(int argc, char **argv)
来源：http://fp.huanxung.cn

[S19] C：快速排序
来源：http://ka.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mr.bookmarksfly.cn

[S20] C：二分查找
来源：http://us.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jl.shxzskj.cn

[S21] C：字符类别判断
来源：http://fa.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hm.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://dv.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wi.szsharing.cn

[S23] C：随机数
来源：http://eh.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ox.newstarts.cn

[S24] C：获取本地时间
来源：http://hz.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qx.asd995.cn

[S25] C：内存拷贝
来源：http://de.muxihuayi.cn

memcpy(dst, src, n);
来源：http://tn.9csxet.cn

[S26] C：内存清零
来源：http://qb.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://ku.jianghongdianzi.cn

[S27] C：定义常量
来源：http://cj.szxytkj.cn

const double PI = 3.14159;
来源：http://xk.hnjuh.cn

[S28] C：静态变量
来源：http://hj.hahajie.cn

static int counter = 0;
来源：http://pz.nszjky.cn

[S29] C：变参函数
来源：http://dg.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ot.shxzukj.cn

[S30] C：头文件保护
来源：http://sp.lnxyls.cn

#ifndef X_H
来源：http://lm.szxytkj.cn

#define X_H
来源：http://ot.huixinmuqiang.cn

#endif
来源：http://sg.szsharing.cn

[S31] C++：Hello World
来源：http://zo.chemitech.net.cn

#include <iostream>
来源：http://pc.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ca.wgjwhj.cn

[S32] C++：字符串
来源：http://pp.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://pt.haigaiapp.cn

[S33] C++：vector 增删
来源：http://ve.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uu.huanxung.cn

[S34] C++：遍历 vector
来源：http://tw.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://sa.jianghongdianzi.cn

[S35] C++：map
来源：http://fo.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lp.haigaiapp.cn

[S36] C++：unordered_map
来源：http://pl.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ua.hahajie.cn

[S37] C++：set
来源：http://pk.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jn.huanxung.cn

[S38] C++：排序
来源：http://ux.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://fl.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://al.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ka.huixiangedu.cn

[S40] C++：查找元素
来源：http://pt.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cx.shxzskj.cn

[S41] C++：类与构造函数
来源：http://pm.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://or.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ea.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://bw.huanxung.cn

[S43] C++：智能指针
来源：http://sy.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://yb.hnjuh.cn

[S44] C++：引用传参
来源：http://gq.asd995.cn

void inc(int &x) { ++x; }
来源：http://xz.wgjwhj.cn

[S45] C++：lambda
来源：http://zc.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wn.huixiangedu.cn

[S46] C++：函数模板
来源：http://tp.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hy.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://el.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ie.hahajie.cn

[S48] C++：逐行读文件
来源：http://eg.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qz.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://yg.bjjhwx.cn

[S49] C++：写文件
来源：http://ak.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oa.shxzskj.cn

[S50] C++：格式化数字
来源：http://es.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kx.szxytkj.cn

[S51] C++：显式类型转换
来源：http://io.9csxet.cn

static_cast<double>(a) / b
来源：http://du.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://ps.colortex.cn

int size() const noexcept { return n_; }
来源：http://is.nicolike.cn

[S53] C++：移动语义
来源：http://xn.521024.cn

std::vector<int> w = std::move(v);
来源：http://cs.521024.cn

[S54] C++：异常处理
来源：http://cr.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ov.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://up.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dw.lnxyls.cn

[S56] C++：optional
来源：http://bi.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pr.nszjky.cn

[S57] C++：编译期常量
来源：http://da.nicolike.cn

constexpr int N = 10;
来源：http://mc.nicolike.cn

[S58] C++：命名空间
来源：http://wm.521024.cn

namespace ns { int f() { return 1; } }
来源：http://fa.szsharing.cn

[S59] C++：静态断言
来源：http://wg.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fd.521024.cn

[S60] C++：遍历并删除元素
来源：http://kf.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ce.huixiangedu.cn

================================================================================
来源：http://gm.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mb.shxzukj.cn

================================================================================
来源：http://kw.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://dy.panjiajie.cn

println("Hello")
来源：http://pz.szsharing.cn

[T02] Kotlin：变量
来源：http://fw.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ze.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://se.hahajie.cn

"值: $b"
来源：http://na.panjiajie.cn

[T04] Kotlin：空安全
来源：http://vk.hahajie.cn

val n: String? = null;  n?.length
来源：http://ez.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://cu.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://by.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://yl.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://se.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://fp.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yn.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://dd.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://vy.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://dl.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://lm.nszjky.cn

[T10] Kotlin：默认参数
来源：http://ll.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mp.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://yh.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cn.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://hx.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://eb.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://ur.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://lh.yuexingan06.cn

[T14] Kotlin：循环
来源：http://ft.panjiajie.cn

for (i in 1..10) println(i)
来源：http://rt.szxytkj.cn

[T15] Kotlin：接口
来源：http://jp.hahajie.cn

interface Shape { fun area(): Double }
来源：http://wb.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://ly.lnxyls.cn

print("Hello")
来源：http://ko.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://ak.shtwfgs.cn

var a = 1;  let b = 2
来源：http://vg.nicolike.cn

[T18] Swift：字符串插值
来源：http://he.muxihuayi.cn

"值: \(b)"
来源：http://qv.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://xh.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://oy.huanxung.cn

[T20] Swift：数组操作
来源：http://cb.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dq.chemitech.net.cn

[T21] Swift：遍历
来源：http://pd.bjjhwx.cn

for x in a { print(x) }
来源：http://fc.bookmarksfly.cn

[T22] Swift：字典
来源：http://la.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://po.wgjwhj.cn

[T23] Swift：函数
来源：http://vp.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tb.huixiangedu.cn

[T24] Swift：闭包
来源：http://mg.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fu.szsharing.cn

[T25] Swift：结构体
来源：http://uy.bjjhwx.cn

struct P { var x: Int }
来源：http://ka.yuexingan06.cn

[T26] Swift：类与重写
来源：http://ve.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://tj.huixiangedu.cn

[T27] Swift：错误处理
来源：http://pk.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://lg.muxihuayi.cn

[T28] Swift：枚举
来源：http://vx.chemitech.net.cn

enum Color { case red, green }
来源：http://co.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://mx.szxytkj.cn

guard let x = opt else { return }
来源：http://qy.jianghongdianzi.cn

[T30] Swift：协议
来源：http://hh.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://io.hnjuh.cn

[T31] Lua：Hello World
来源：http://hp.shxzukj.cn

print("Hello")
来源：http://th.bjjhwx.cn

[T32] Lua：局部变量
来源：http://fh.shxzukj.cn

local a = 1
来源：http://za.huanxung.cn

[T33] Lua：表（数组）
来源：http://lk.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ie.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://yq.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rh.panjiajie.cn

[T35] Lua：字典表
来源：http://dm.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://om.huixinmuqiang.cn

[T36] Lua：函数
来源：http://lu.nicolike.cn

function add(a, b) return a + b end
来源：http://vf.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://wd.huanxung.cn

"a" .. "b"
来源：http://kk.hahajie.cn

[T38] Lua：条件
来源：http://kx.bjjhwx.cn

if x > 0 then print("正") end
来源：http://ff.9csxet.cn

[T39] Lua：模式匹配
来源：http://cz.521024.cn

string.find(s, "%d+")
来源：http://ot.hahajie.cn

[T40] Lua：元表
来源：http://ao.asd995.cn

setmetatable({}, { __index = base })
来源：http://vj.521024.cn

[T41] Perl：Hello World
来源：http://xp.muxihuayi.cn

print "Hello\n";
来源：http://fs.gzmigu.cn

[T42] Perl：变量类型
来源：http://df.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wx.szxytkj.cn

[T43] Perl：字符串插值
来源：http://jh.newstarts.cn

"值: $a"
来源：http://xk.521024.cn

[T44] Perl：条件
来源：http://dc.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://oa.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://uv.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://go.nszjky.cn

[T46] Perl：哈希操作
来源：http://jt.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gi.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ss.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pi.hnjuh.cn

[T48] Perl：正则替换
来源：http://gh.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://vh.chemitech.net.cn

[T49] Perl：函数
来源：http://ws.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dv.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://si.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pl.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://xu.9csxet.cn

[T51] Scala：Hello World
来源：http://le.hahajie.cn

println("Hello")
来源：http://ih.haigaiapp.cn

[T52] Scala：变量
来源：http://xr.huixiangedu.cn

val a = 1;  var b = 2
来源：http://mj.521024.cn

[T53] Scala：字符串插值
来源：http://eq.9csxet.cn

s"值: $b"
来源：http://ba.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://fc.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://vw.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://pw.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bz.asd995.cn

[T56] Scala：样例类
来源：http://tv.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://qm.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://uz.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bv.jctech888.com.cn

[T58] Scala：函数定义
来源：http://ng.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wp.szsharing.cn

[T59] Scala：循环
来源：http://yd.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://wn.nicolike.cn

[T60] Scala：折叠
来源：http://lb.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cc.huixiangedu.cn

================================================================================
来源：http://ll.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qz.panjiajie.cn

================================================================================
来源：http://zi.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://nv.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uj.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://wm.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vk.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://jv.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uh.huanxung.cn

[U04] Py：变量调试打印
来源：http://wn.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ej.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://cv.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://bj.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://ph.huanxung.cn

{**a, **b}
来源：http://wj.asd995.cn

[U07] Py：反转字典键值
来源：http://ut.colortex.cn

{v: k for k, v in d.items()}
来源：http://iu.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://hn.newstarts.cn

[y for x in nested for y in x]
来源：http://lv.shxzskj.cn


<!-- 参考信息 -->