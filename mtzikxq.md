代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cg.yuntaijiaju.cn

[R66] 定时任务
来源：http://gv.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://va.521024.cn

[R67] 生成随机十六进制串
来源：http://dq.huanxung.cn

openssl rand -hex 16
来源：http://kz.nicolike.cn

[R68] 计算文件校验值
来源：http://ih.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fi.yuexingan06.cn

[R69] 生成随机密码
来源：http://yz.521024.cn

head -c 16 /dev/urandom | base64
来源：http://eo.nszjky.cn

[R70] 时间戳与互转
来源：http://hj.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://pj.newstarts.cn

[R71] 日期格式化
来源：http://iy.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gj.haigaiapp.cn

[R72] 等待端口就绪
来源：http://ku.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jy.jianghongdianzi.cn

[R73] 分割大日志
来源：http://xq.asd995.cn

split -l 1000 big.log part_
来源：http://nv.bookmarksfly.cn

[R74] 批量重命名
来源：http://hb.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qd.chemitech.net.cn

[R75] 导出环境变量
来源：http://ix.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://jk.nicolike.cn

[R76] 使用临时文件
来源：http://cd.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ed.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://jn.lnxyls.cn

read -rp "请输入: " ans
来源：http://ol.haigaiapp.cn

[R78] 交互式菜单
来源：http://vb.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zs.colortex.cn

[R79] 解析命令行选项
来源：http://qp.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vk.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://do.szsharing.cn

time ./run.sh
来源：http://ax.newstarts.cn

================================================================================
来源：http://ku.muxihuayi.cn

S. C / C++ 专题
来源：http://nw.lnxyls.cn

================================================================================
来源：http://rv.jianghongdianzi.cn

[S01] C：Hello World
来源：http://pp.huanxung.cn

#include <stdio.h>
来源：http://af.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pq.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://cg.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://kn.jianghongdianzi.cn

[S03] C：读入整数
来源：http://pi.lnxyls.cn

int x; scanf("%d", &x);
来源：http://by.szxytkj.cn

[S04] C：字符串复制
来源：http://de.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tb.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ux.huixinmuqiang.cn

strlen(s)
来源：http://ci.colortex.cn

[S06] C：字符串比较
来源：http://uv.hahajie.cn

strcmp(a, b) == 0
来源：http://vx.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://se.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qi.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://gg.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bw.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://wq.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mh.yuexingan06.cn

[S10] C：指针与解引用
来源：http://vw.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://pn.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://es.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://xw.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ib.haigaiapp.cn

fclose(f);
来源：http://of.bookmarksfly.cn

[S12] C：写文件
来源：http://vf.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wb.shxzskj.cn

[S13] C：宏定义
来源：http://to.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wq.muxihuayi.cn

[S14] C：枚举
来源：http://kn.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://hy.9csxet.cn

[S15] C：类型转换
来源：http://oj.bjjhwx.cn

(double) a / b
来源：http://rh.panjiajie.cn

[S16] C：位操作置位
来源：http://xn.jianghongdianzi.cn

x |= (1 << 3);
来源：http://an.huanxung.cn

[S17] C：安全拼接字符串
来源：http://fj.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dp.szsharing.cn

[S18] C：命令行参数
来源：http://un.9csxet.cn

int main(int argc, char **argv)
来源：http://sg.szxytkj.cn

[S19] C：快速排序
来源：http://nh.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://no.shxzukj.cn

[S20] C：二分查找
来源：http://oh.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yl.hahajie.cn

[S21] C：字符类别判断
来源：http://hz.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gf.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://om.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gt.jctech888.com.cn

[S23] C：随机数
来源：http://wg.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bv.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://mp.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ob.521024.cn

[S25] C：内存拷贝
来源：http://ip.newstarts.cn

memcpy(dst, src, n);
来源：http://an.521024.cn

[S26] C：内存清零
来源：http://lt.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://ol.asd995.cn

[S27] C：定义常量
来源：http://qz.panjiajie.cn

const double PI = 3.14159;
来源：http://dw.9csxet.cn

[S28] C：静态变量
来源：http://cd.szxytkj.cn

static int counter = 0;
来源：http://js.haigaiapp.cn

[S29] C：变参函数
来源：http://gd.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ct.nszjky.cn

[S30] C：头文件保护
来源：http://ps.hahajie.cn

#ifndef X_H
来源：http://en.szsharing.cn

#define X_H
来源：http://ag.muxihuayi.cn

#endif
来源：http://cp.shxzukj.cn

[S31] C++：Hello World
来源：http://jr.haigaiapp.cn

#include <iostream>
来源：http://tb.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://bj.asd995.cn

[S32] C++：字符串
来源：http://hv.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://am.colortex.cn

[S33] C++：vector 增删
来源：http://iw.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lx.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://ir.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://yt.nszjky.cn

[S35] C++：map
来源：http://wd.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ie.chemitech.net.cn

[S36] C++：unordered_map
来源：http://zo.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tk.panjiajie.cn

[S37] C++：set
来源：http://hh.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vu.shxzukj.cn

[S38] C++：排序
来源：http://am.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://bz.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://jv.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pv.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://bz.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://be.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://nr.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bd.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://cd.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://vz.wgjwhj.cn

[S43] C++：智能指针
来源：http://cg.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://ae.521024.cn

[S44] C++：引用传参
来源：http://dm.nszjky.cn

void inc(int &x) { ++x; }
来源：http://fp.jianghongdianzi.cn

[S45] C++：lambda
来源：http://ha.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bu.haigaiapp.cn

[S46] C++：函数模板
来源：http://ri.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gd.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ob.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rb.newstarts.cn

[S48] C++：逐行读文件
来源：http://uw.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lz.newstarts.cn

while (std::getline(in, line)) { }
来源：http://ke.9csxet.cn

[S49] C++：写文件
来源：http://cm.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bn.hahajie.cn

[S50] C++：格式化数字
来源：http://lv.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xj.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://ov.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://td.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://gy.nszjky.cn

int size() const noexcept { return n_; }
来源：http://ga.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://qe.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://ro.yuexingan06.cn

[S54] C++：异常处理
来源：http://bc.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ip.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://xl.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dl.huixinmuqiang.cn

[S56] C++：optional
来源：http://yn.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ac.9csxet.cn

[S57] C++：编译期常量
来源：http://av.huixinmuqiang.cn

constexpr int N = 10;
来源：http://bj.hnjuh.cn

[S58] C++：命名空间
来源：http://tj.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://zx.panjiajie.cn

[S59] C++：静态断言
来源：http://el.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mu.asd995.cn

[S60] C++：遍历并删除元素
来源：http://wa.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vo.hnjuh.cn

================================================================================
来源：http://qk.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dj.wgjwhj.cn

================================================================================
来源：http://od.newstarts.cn

[T01] Kotlin：Hello World
来源：http://vr.shxzukj.cn

println("Hello")
来源：http://qh.521024.cn

[T02] Kotlin：变量
来源：http://xm.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nl.colortex.cn

[T03] Kotlin：字符串模板
来源：http://hf.wgjwhj.cn

"值: $b"
来源：http://la.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://kx.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://gw.521024.cn

[T05] Kotlin：when 表达式
来源：http://cc.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xv.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://qm.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fh.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://gf.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cq.szxytkj.cn

[T08] Kotlin：数据类
来源：http://xp.colortex.cn

data class User(val name: String, val age: Int)
来源：http://nt.521024.cn

[T09] Kotlin：扩展函数
来源：http://jj.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://le.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://zx.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wt.asd995.cn

[T11] Kotlin：协程
来源：http://lc.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qz.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://fa.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://do.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://jn.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://ku.newstarts.cn

[T14] Kotlin：循环
来源：http://hq.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://ui.newstarts.cn

[T15] Kotlin：接口
来源：http://wk.nszjky.cn

interface Shape { fun area(): Double }
来源：http://fx.shtwfgs.cn

[T16] Swift：Hello World
来源：http://zi.shxzskj.cn

print("Hello")
来源：http://ty.shxzukj.cn

[T17] Swift：变量与常量
来源：http://df.asd995.cn

var a = 1;  let b = 2
来源：http://us.nszjky.cn

[T18] Swift：字符串插值
来源：http://gi.szxytkj.cn

"值: \(b)"
来源：http://an.gzmigu.cn

[T19] Swift：可选绑定
来源：http://bz.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://ax.colortex.cn

[T20] Swift：数组操作
来源：http://th.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hd.bookmarksfly.cn

[T21] Swift：遍历
来源：http://jj.panjiajie.cn

for x in a { print(x) }
来源：http://oz.newstarts.cn

[T22] Swift：字典
来源：http://ny.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fy.jctech888.com.cn

[T23] Swift：函数
来源：http://qk.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rn.521024.cn

[T24] Swift：闭包
来源：http://ng.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://so.bjjhwx.cn

[T25] Swift：结构体
来源：http://jr.huanxung.cn

struct P { var x: Int }
来源：http://db.gzmigu.cn

[T26] Swift：类与重写
来源：http://kk.szsharing.cn

class A: Base { override func f() {} }
来源：http://pu.lnxyls.cn

[T27] Swift：错误处理
来源：http://tb.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://hk.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://gf.yuexingan06.cn

enum Color { case red, green }
来源：http://ag.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://yz.haigaiapp.cn

guard let x = opt else { return }
来源：http://eo.huixinmuqiang.cn

[T30] Swift：协议
来源：http://lr.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://gf.9csxet.cn

[T31] Lua：Hello World
来源：http://us.hnjuh.cn

print("Hello")
来源：http://mu.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://mv.jctech888.com.cn

local a = 1
来源：http://ry.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://rd.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dj.gzmigu.cn

[T34] Lua：遍历表
来源：http://ie.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sq.nicolike.cn

[T35] Lua：字典表
来源：http://km.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://tj.muxihuayi.cn

[T36] Lua：函数
来源：http://hg.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://bj.521024.cn

[T37] Lua：字符串拼接
来源：http://mb.szxytkj.cn

"a" .. "b"
来源：http://ni.jctech888.com.cn

[T38] Lua：条件
来源：http://te.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://ha.panjiajie.cn

[T39] Lua：模式匹配
来源：http://up.gzmigu.cn

string.find(s, "%d+")
来源：http://qc.newstarts.cn

[T40] Lua：元表
来源：http://jf.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://gx.hahajie.cn

[T41] Perl：Hello World
来源：http://tv.asd995.cn

print "Hello\n";
来源：http://bg.hnjuh.cn

[T42] Perl：变量类型
来源：http://dh.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uj.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://xd.szxytkj.cn

"值: $a"
来源：http://cq.huixinmuqiang.cn

[T44] Perl：条件
来源：http://wn.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://jy.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ja.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://ut.newstarts.cn

[T46] Perl：哈希操作
来源：http://wx.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bu.9csxet.cn

[T47] Perl：正则捕获
来源：http://fb.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pk.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://tc.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://bh.asd995.cn

[T49] Perl：函数
来源：http://an.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ee.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://rn.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nh.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://rl.bjjhwx.cn

[T51] Scala：Hello World
来源：http://kd.jctech888.com.cn

println("Hello")
来源：http://oj.yuexingan06.cn

[T52] Scala：变量
来源：http://kq.szsharing.cn

val a = 1;  var b = 2
来源：http://nu.huanxung.cn

[T53] Scala：字符串插值
来源：http://ox.yuexingan06.cn

s"值: $b"
来源：http://dj.chemitech.net.cn

[T54] Scala：集合映射
来源：http://pd.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://jf.hnjuh.cn

[T55] Scala：集合过滤
来源：http://la.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gh.asd995.cn

[T56] Scala：样例类
来源：http://jv.9csxet.cn

case class User(name: String, age: Int)
来源：http://og.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://kw.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ko.hahajie.cn

[T58] Scala：函数定义
来源：http://sv.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ao.muxihuayi.cn

[T59] Scala：循环
来源：http://fw.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://ge.9csxet.cn

[T60] Scala：折叠
来源：http://rm.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sf.yuexingan06.cn

================================================================================
来源：http://zb.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nl.bjjhwx.cn

================================================================================
来源：http://ve.521024.cn

[U01] Py：创建虚拟环境
来源：http://nx.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cd.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://tj.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xh.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://yc.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mt.huanxung.cn

[U04] Py：变量调试打印
来源：http://kn.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mx.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://ul.nicolike.cn

list(dict.fromkeys(arr))
来源：http://zo.huanxung.cn

[U06] Py：合并两个字典
来源：http://kf.colortex.cn

{**a, **b}
来源：http://fr.huixinmuqiang.cn


<!-- 参考信息 -->