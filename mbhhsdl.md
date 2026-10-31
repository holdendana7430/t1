代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pr.yuntaijiaju.cn

[R66] 定时任务
来源：http://oz.shxzskj.cn

crontab -e;  crontab -l
来源：http://nv.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://lh.9csxet.cn

openssl rand -hex 16
来源：http://uc.huanxung.cn

[R68] 计算文件校验值
来源：http://lb.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lr.muxihuayi.cn

[R69] 生成随机密码
来源：http://op.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://xm.shxzukj.cn

[R70] 时间戳与互转
来源：http://ih.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://eg.asd995.cn

[R71] 日期格式化
来源：http://ad.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://of.muxihuayi.cn

[R72] 等待端口就绪
来源：http://xe.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://et.muxihuayi.cn

[R73] 分割大日志
来源：http://ca.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ud.521024.cn

[R74] 批量重命名
来源：http://xm.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lv.9csxet.cn

[R75] 导出环境变量
来源：http://cz.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://ve.nszjky.cn

[R76] 使用临时文件
来源：http://cy.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xa.hnjuh.cn

[R77] 读取用户输入
来源：http://bf.asd995.cn

read -rp "请输入: " ans
来源：http://ev.shxzskj.cn

[R78] 交互式菜单
来源：http://zo.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fr.wgjwhj.cn

[R79] 解析命令行选项
来源：http://gu.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ai.colortex.cn

[R80] 查看脚本执行耗时
来源：http://ey.haigaiapp.cn

time ./run.sh
来源：http://rc.muxihuayi.cn

================================================================================
来源：http://ln.jianghongdianzi.cn

S. C / C++ 专题
来源：http://wz.hahajie.cn

================================================================================
来源：http://bt.9csxet.cn

[S01] C：Hello World
来源：http://wa.huanxung.cn

#include <stdio.h>
来源：http://ls.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nz.huanxung.cn

[S02] C：变量与格式化输出
来源：http://qh.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://wp.shtwfgs.cn

[S03] C：读入整数
来源：http://ld.huanxung.cn

int x; scanf("%d", &x);
来源：http://lc.gzmigu.cn

[S04] C：字符串复制
来源：http://pt.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gq.muxihuayi.cn

[S05] C：字符串长度
来源：http://na.bookmarksfly.cn

strlen(s)
来源：http://zq.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://rk.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://bc.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://ke.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jh.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://ew.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eq.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://au.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rm.colortex.cn

[S10] C：指针与解引用
来源：http://hg.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://sl.yuexingan06.cn

[S11] C：逐行读文件
来源：http://oc.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ya.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bf.panjiajie.cn

fclose(f);
来源：http://gy.lnxyls.cn

[S12] C：写文件
来源：http://ht.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zs.bjjhwx.cn

[S13] C：宏定义
来源：http://xy.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yi.lnxyls.cn

[S14] C：枚举
来源：http://ty.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://mx.asd995.cn

[S15] C：类型转换
来源：http://jx.szxytkj.cn

(double) a / b
来源：http://vf.hahajie.cn

[S16] C：位操作置位
来源：http://so.panjiajie.cn

x |= (1 << 3);
来源：http://hz.newstarts.cn

[S17] C：安全拼接字符串
来源：http://tz.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lw.bookmarksfly.cn

[S18] C：命令行参数
来源：http://rs.huixiangedu.cn

int main(int argc, char **argv)
来源：http://gg.bookmarksfly.cn

[S19] C：快速排序
来源：http://up.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ix.jianghongdianzi.cn

[S20] C：二分查找
来源：http://ix.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vr.hahajie.cn

[S21] C：字符类别判断
来源：http://hu.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bh.newstarts.cn

[S22] C：字符串转数字
来源：http://wi.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zg.jianghongdianzi.cn

[S23] C：随机数
来源：http://gx.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bm.shxzukj.cn

[S24] C：获取本地时间
来源：http://yo.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cf.wgjwhj.cn

[S25] C：内存拷贝
来源：http://ar.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://mx.szxytkj.cn

[S26] C：内存清零
来源：http://tc.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://ur.yuexingan06.cn

[S27] C：定义常量
来源：http://kx.wgjwhj.cn

const double PI = 3.14159;
来源：http://dw.shxzskj.cn

[S28] C：静态变量
来源：http://zo.521024.cn

static int counter = 0;
来源：http://ix.bookmarksfly.cn

[S29] C：变参函数
来源：http://pz.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://go.haigaiapp.cn

[S30] C：头文件保护
来源：http://md.521024.cn

#ifndef X_H
来源：http://ch.hahajie.cn

#define X_H
来源：http://gf.nicolike.cn

#endif
来源：http://zq.szxytkj.cn

[S31] C++：Hello World
来源：http://iq.newstarts.cn

#include <iostream>
来源：http://ix.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://aa.haigaiapp.cn

[S32] C++：字符串
来源：http://ln.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://cw.yuexingan06.cn

[S33] C++：vector 增删
来源：http://ag.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://he.gzmigu.cn

[S34] C++：遍历 vector
来源：http://op.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://it.wgjwhj.cn

[S35] C++：map
来源：http://fb.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qs.gzmigu.cn

[S36] C++：unordered_map
来源：http://mp.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ek.nszjky.cn

[S37] C++：set
来源：http://ek.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vi.colortex.cn

[S38] C++：排序
来源：http://qb.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://zk.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://up.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vx.huixiangedu.cn

[S40] C++：查找元素
来源：http://jn.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zn.521024.cn

[S41] C++：类与构造函数
来源：http://lm.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fk.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://uw.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://mk.newstarts.cn

[S43] C++：智能指针
来源：http://aj.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://vp.newstarts.cn

[S44] C++：引用传参
来源：http://wt.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://mx.newstarts.cn

[S45] C++：lambda
来源：http://ey.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ct.hahajie.cn

[S46] C++：函数模板
来源：http://he.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sy.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://xm.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tf.colortex.cn

[S48] C++：逐行读文件
来源：http://ef.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qy.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://qc.asd995.cn

[S49] C++：写文件
来源：http://qr.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ip.nicolike.cn

[S50] C++：格式化数字
来源：http://tb.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lr.9csxet.cn

[S51] C++：显式类型转换
来源：http://jb.hnjuh.cn

static_cast<double>(a) / b
来源：http://io.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://qp.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://ft.newstarts.cn

[S53] C++：移动语义
来源：http://cr.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://in.shxzukj.cn

[S54] C++：异常处理
来源：http://ce.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://np.panjiajie.cn

[S55] C++：结构化绑定
来源：http://ux.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xn.yuntaijiaju.cn

[S56] C++：optional
来源：http://un.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tz.newstarts.cn

[S57] C++：编译期常量
来源：http://gn.huixiangedu.cn

constexpr int N = 10;
来源：http://sr.shxzukj.cn

[S58] C++：命名空间
来源：http://tf.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://zp.gzmigu.cn

[S59] C++：静态断言
来源：http://bl.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ou.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://ad.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rs.hahajie.cn

================================================================================
来源：http://lo.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://je.bjjhwx.cn

================================================================================
来源：http://aa.521024.cn

[T01] Kotlin：Hello World
来源：http://so.nszjky.cn

println("Hello")
来源：http://ep.haigaiapp.cn

[T02] Kotlin：变量
来源：http://lx.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jz.colortex.cn

[T03] Kotlin：字符串模板
来源：http://ba.bjjhwx.cn

"值: $b"
来源：http://nn.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://tz.hahajie.cn

val n: String? = null;  n?.length
来源：http://om.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://kh.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oz.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://mw.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nz.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ja.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mu.gzmigu.cn

[T08] Kotlin：数据类
来源：http://jx.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://ix.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://yq.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://ij.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://cv.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ay.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://mk.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ee.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://op.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://kp.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://mv.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://mn.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://fo.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://qn.nicolike.cn

[T15] Kotlin：接口
来源：http://rc.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://xe.yuexingan06.cn

[T16] Swift：Hello World
来源：http://nz.yuexingan06.cn

print("Hello")
来源：http://al.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://qs.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://qb.521024.cn

[T18] Swift：字符串插值
来源：http://ax.huixinmuqiang.cn

"值: \(b)"
来源：http://fg.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://de.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://bk.lnxyls.cn

[T20] Swift：数组操作
来源：http://ja.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aq.asd995.cn

[T21] Swift：遍历
来源：http://jg.newstarts.cn

for x in a { print(x) }
来源：http://at.gzmigu.cn

[T22] Swift：字典
来源：http://na.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qx.colortex.cn

[T23] Swift：函数
来源：http://bf.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://px.wgjwhj.cn

[T24] Swift：闭包
来源：http://ig.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://th.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://hc.hnjuh.cn

struct P { var x: Int }
来源：http://jo.nicolike.cn

[T26] Swift：类与重写
来源：http://yv.lnxyls.cn

class A: Base { override func f() {} }
来源：http://au.yuexingan06.cn

[T27] Swift：错误处理
来源：http://cr.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ys.shxzukj.cn

[T28] Swift：枚举
来源：http://wk.shtwfgs.cn

enum Color { case red, green }
来源：http://hc.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://rk.shxzukj.cn

guard let x = opt else { return }
来源：http://yt.muxihuayi.cn

[T30] Swift：协议
来源：http://qa.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://tg.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://ox.gzmigu.cn

print("Hello")
来源：http://iq.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://ys.panjiajie.cn

local a = 1
来源：http://ff.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://np.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fx.9csxet.cn

[T34] Lua：遍历表
来源：http://lq.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pw.lnxyls.cn

[T35] Lua：字典表
来源：http://eh.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://rt.521024.cn

[T36] Lua：函数
来源：http://me.chemitech.net.cn

function add(a, b) return a + b end
来源：http://xk.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://uj.lnxyls.cn

"a" .. "b"
来源：http://iu.huanxung.cn

[T38] Lua：条件
来源：http://fl.gzmigu.cn

if x > 0 then print("正") end
来源：http://ly.lnxyls.cn

[T39] Lua：模式匹配
来源：http://hi.gzmigu.cn

string.find(s, "%d+")
来源：http://ex.9csxet.cn

[T40] Lua：元表
来源：http://pk.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://ew.colortex.cn

[T41] Perl：Hello World
来源：http://rm.yuexingan06.cn

print "Hello\n";
来源：http://ol.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://kn.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lh.szxytkj.cn

[T43] Perl：字符串插值
来源：http://vp.muxihuayi.cn

"值: $a"
来源：http://th.szxytkj.cn

[T44] Perl：条件
来源：http://qh.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://fz.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://fu.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://jc.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://cp.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vh.hnjuh.cn

[T47] Perl：正则捕获
来源：http://cr.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kn.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://ch.hnjuh.cn

$s =~ s/old/new/g;
来源：http://rl.szxytkj.cn

[T49] Perl：函数
来源：http://ia.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pt.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://ju.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yg.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://nu.nicolike.cn

[T51] Scala：Hello World
来源：http://qg.wgjwhj.cn

println("Hello")
来源：http://cj.huixiangedu.cn

[T52] Scala：变量
来源：http://yh.chemitech.net.cn

val a = 1;  var b = 2
来源：http://wy.hahajie.cn

[T53] Scala：字符串插值
来源：http://pr.huixinmuqiang.cn

s"值: $b"
来源：http://xp.chemitech.net.cn

[T54] Scala：集合映射
来源：http://fs.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ae.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://al.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tr.nicolike.cn

[T56] Scala：样例类
来源：http://ym.szsharing.cn

case class User(name: String, age: Int)
来源：http://ml.huanxung.cn

[T57] Scala：模式匹配
来源：http://mv.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hi.chemitech.net.cn

[T58] Scala：函数定义
来源：http://kx.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xt.nicolike.cn

[T59] Scala：循环
来源：http://jk.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://ac.shxzukj.cn

[T60] Scala：折叠
来源：http://gq.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mi.nszjky.cn

================================================================================
来源：http://cx.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jw.huixinmuqiang.cn

================================================================================
来源：http://xg.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://mi.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tk.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://jc.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jr.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://oz.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lo.shxzskj.cn

[U04] Py：变量调试打印
来源：http://cy.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yx.nicolike.cn

[U05] Py：列表去重且保序
来源：http://bh.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://nl.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://tb.hnjuh.cn

{**a, **b}
来源：http://hd.hnjuh.cn


<!-- 参考信息 -->