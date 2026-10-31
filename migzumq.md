代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kc.shxzskj.cn

[R66] 定时任务
来源：http://wt.chemitech.net.cn

crontab -e;  crontab -l
来源：http://vi.9csxet.cn

[R67] 生成随机十六进制串
来源：http://um.szxytkj.cn

openssl rand -hex 16
来源：http://wb.521024.cn

[R68] 计算文件校验值
来源：http://fd.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xi.muxihuayi.cn

[R69] 生成随机密码
来源：http://ud.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://cy.shxzukj.cn

[R70] 时间戳与互转
来源：http://du.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://pj.yuntaijiaju.cn

[R71] 日期格式化
来源：http://jt.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ty.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://qa.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aa.bookmarksfly.cn

[R73] 分割大日志
来源：http://hh.bjjhwx.cn

split -l 1000 big.log part_
来源：http://qu.shtwfgs.cn

[R74] 批量重命名
来源：http://lq.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zz.muxihuayi.cn

[R75] 导出环境变量
来源：http://cj.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://oc.nicolike.cn

[R76] 使用临时文件
来源：http://hl.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gs.newstarts.cn

[R77] 读取用户输入
来源：http://rx.haigaiapp.cn

read -rp "请输入: " ans
来源：http://ym.yuexingan06.cn

[R78] 交互式菜单
来源：http://yq.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sr.9csxet.cn

[R79] 解析命令行选项
来源：http://yd.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jo.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://ch.shxzskj.cn

time ./run.sh
来源：http://ie.shxzukj.cn

================================================================================
来源：http://fb.nicolike.cn

S. C / C++ 专题
来源：http://wb.chemitech.net.cn

================================================================================
来源：http://pf.huixinmuqiang.cn

[S01] C：Hello World
来源：http://ma.shtwfgs.cn

#include <stdio.h>
来源：http://cu.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dg.521024.cn

[S02] C：变量与格式化输出
来源：http://gu.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://gb.nszjky.cn

[S03] C：读入整数
来源：http://jl.panjiajie.cn

int x; scanf("%d", &x);
来源：http://sm.colortex.cn

[S04] C：字符串复制
来源：http://qh.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oe.huanxung.cn

[S05] C：字符串长度
来源：http://fm.huixiangedu.cn

strlen(s)
来源：http://no.nicolike.cn

[S06] C：字符串比较
来源：http://rb.szxytkj.cn

strcmp(a, b) == 0
来源：http://ad.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://bg.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://of.521024.cn

[S08] C：动态内存分配与释放
来源：http://mu.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dr.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://er.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wx.hnjuh.cn

[S10] C：指针与解引用
来源：http://pz.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://as.shxzskj.cn

[S11] C：逐行读文件
来源：http://bv.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://ur.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cf.huixinmuqiang.cn

fclose(f);
来源：http://ik.yuexingan06.cn

[S12] C：写文件
来源：http://er.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://md.muxihuayi.cn

[S13] C：宏定义
来源：http://qh.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fn.yuexingan06.cn

[S14] C：枚举
来源：http://ph.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://nw.huanxung.cn

[S15] C：类型转换
来源：http://rp.szxytkj.cn

(double) a / b
来源：http://yc.colortex.cn

[S16] C：位操作置位
来源：http://th.chemitech.net.cn

x |= (1 << 3);
来源：http://xs.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://up.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qh.szxytkj.cn

[S18] C：命令行参数
来源：http://dd.wgjwhj.cn

int main(int argc, char **argv)
来源：http://zq.huixinmuqiang.cn

[S19] C：快速排序
来源：http://yt.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lf.521024.cn

[S20] C：二分查找
来源：http://kl.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ek.9csxet.cn

[S21] C：字符类别判断
来源：http://gn.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yp.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://mw.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ey.jctech888.com.cn

[S23] C：随机数
来源：http://el.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qo.huanxung.cn

[S24] C：获取本地时间
来源：http://ju.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qw.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://tr.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ct.shxzskj.cn

[S26] C：内存清零
来源：http://xo.nicolike.cn

memset(a, 0, sizeof a);
来源：http://ej.panjiajie.cn

[S27] C：定义常量
来源：http://zj.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://kk.chemitech.net.cn

[S28] C：静态变量
来源：http://nr.wgjwhj.cn

static int counter = 0;
来源：http://nd.shxzskj.cn

[S29] C：变参函数
来源：http://yv.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ms.muxihuayi.cn

[S30] C：头文件保护
来源：http://fq.asd995.cn

#ifndef X_H
来源：http://pe.521024.cn

#define X_H
来源：http://jy.jctech888.com.cn

#endif
来源：http://pn.yuexingan06.cn

[S31] C++：Hello World
来源：http://xi.yuexingan06.cn

#include <iostream>
来源：http://an.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://qb.yuntaijiaju.cn

[S32] C++：字符串
来源：http://lr.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://ys.panjiajie.cn

[S33] C++：vector 增删
来源：http://iv.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gh.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://kf.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://nx.jctech888.com.cn

[S35] C++：map
来源：http://ku.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://em.nicolike.cn

[S36] C++：unordered_map
来源：http://dh.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gn.huanxung.cn

[S37] C++：set
来源：http://xe.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ku.9csxet.cn

[S38] C++：排序
来源：http://wu.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://uo.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://gz.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dc.gzmigu.cn

[S40] C++：查找元素
来源：http://qn.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zj.colortex.cn

[S41] C++：类与构造函数
来源：http://ek.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oe.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://sj.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://lh.newstarts.cn

[S43] C++：智能指针
来源：http://yg.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://hs.nicolike.cn

[S44] C++：引用传参
来源：http://mr.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://dg.yuexingan06.cn

[S45] C++：lambda
来源：http://tt.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xt.panjiajie.cn

[S46] C++：函数模板
来源：http://fx.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uh.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://js.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zz.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://tf.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dz.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://ul.muxihuayi.cn

[S49] C++：写文件
来源：http://cz.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fy.shxzukj.cn

[S50] C++：格式化数字
来源：http://uv.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rn.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://gt.nicolike.cn

static_cast<double>(a) / b
来源：http://xi.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://bk.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://jf.521024.cn

[S53] C++：移动语义
来源：http://fl.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://ns.shxzskj.cn

[S54] C++：异常处理
来源：http://tn.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nr.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://or.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qp.shtwfgs.cn

[S56] C++：optional
来源：http://aw.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kq.wgjwhj.cn

[S57] C++：编译期常量
来源：http://lr.nszjky.cn

constexpr int N = 10;
来源：http://ny.lnxyls.cn

[S58] C++：命名空间
来源：http://dg.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://yr.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://vs.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kf.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://bd.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bc.bookmarksfly.cn

================================================================================
来源：http://uk.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tr.gzmigu.cn

================================================================================
来源：http://fz.nicolike.cn

[T01] Kotlin：Hello World
来源：http://wn.yuexingan06.cn

println("Hello")
来源：http://ac.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://kg.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://js.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://uz.bookmarksfly.cn

"值: $b"
来源：http://ti.gzmigu.cn

[T04] Kotlin：空安全
来源：http://xk.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://yu.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://zu.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aw.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://cc.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jw.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://jp.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aj.shxzskj.cn

[T08] Kotlin：数据类
来源：http://fs.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://fe.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://at.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://ee.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://sc.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://en.lnxyls.cn

[T11] Kotlin：协程
来源：http://qe.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kq.szsharing.cn

[T12] Kotlin：解构声明
来源：http://zh.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://lj.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://sn.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://ec.521024.cn

[T14] Kotlin：循环
来源：http://gz.szsharing.cn

for (i in 1..10) println(i)
来源：http://sl.nszjky.cn

[T15] Kotlin：接口
来源：http://qy.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://sd.jctech888.com.cn

[T16] Swift：Hello World
来源：http://ri.newstarts.cn

print("Hello")
来源：http://xt.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://qi.nszjky.cn

var a = 1;  let b = 2
来源：http://aq.nicolike.cn

[T18] Swift：字符串插值
来源：http://un.yuexingan06.cn

"值: \(b)"
来源：http://qw.hnjuh.cn

[T19] Swift：可选绑定
来源：http://ae.asd995.cn

if let n = opt { print(n) }
来源：http://qs.shxzskj.cn

[T20] Swift：数组操作
来源：http://gu.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hr.nszjky.cn

[T21] Swift：遍历
来源：http://wi.521024.cn

for x in a { print(x) }
来源：http://kk.nszjky.cn

[T22] Swift：字典
来源：http://qr.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ho.huixiangedu.cn

[T23] Swift：函数
来源：http://sk.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xw.wgjwhj.cn

[T24] Swift：闭包
来源：http://sk.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oq.nszjky.cn

[T25] Swift：结构体
来源：http://fn.haigaiapp.cn

struct P { var x: Int }
来源：http://ay.shtwfgs.cn

[T26] Swift：类与重写
来源：http://vl.521024.cn

class A: Base { override func f() {} }
来源：http://gu.shtwfgs.cn

[T27] Swift：错误处理
来源：http://mr.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://cq.szxytkj.cn

[T28] Swift：枚举
来源：http://zp.9csxet.cn

enum Color { case red, green }
来源：http://ar.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://tj.shxzukj.cn

guard let x = opt else { return }
来源：http://xf.lnxyls.cn

[T30] Swift：协议
来源：http://oz.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://fq.gzmigu.cn

[T31] Lua：Hello World
来源：http://aa.nszjky.cn

print("Hello")
来源：http://jy.haigaiapp.cn

[T32] Lua：局部变量
来源：http://ia.nszjky.cn

local a = 1
来源：http://ua.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://wy.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hv.nicolike.cn

[T34] Lua：遍历表
来源：http://gp.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xr.newstarts.cn

[T35] Lua：字典表
来源：http://bp.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://mk.bookmarksfly.cn

[T36] Lua：函数
来源：http://gx.panjiajie.cn

function add(a, b) return a + b end
来源：http://ff.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://tw.yuexingan06.cn

"a" .. "b"
来源：http://ag.nszjky.cn

[T38] Lua：条件
来源：http://vd.yuexingan06.cn

if x > 0 then print("正") end
来源：http://di.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://kv.haigaiapp.cn

string.find(s, "%d+")
来源：http://pn.gzmigu.cn

[T40] Lua：元表
来源：http://fo.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://uj.haigaiapp.cn

[T41] Perl：Hello World
来源：http://ln.shxzukj.cn

print "Hello\n";
来源：http://cv.jctech888.com.cn

[T42] Perl：变量类型
来源：http://tt.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qx.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://cc.wgjwhj.cn

"值: $a"
来源：http://wk.panjiajie.cn

[T44] Perl：条件
来源：http://ih.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://sw.colortex.cn

[T45] Perl：数组遍历
来源：http://la.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://mp.9csxet.cn

[T46] Perl：哈希操作
来源：http://hl.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xr.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://db.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yt.521024.cn

[T48] Perl：正则替换
来源：http://oy.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://ti.szsharing.cn

[T49] Perl：函数
来源：http://lz.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sm.newstarts.cn

[T50] Perl：逐行读文件
来源：http://hx.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nb.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://if.asd995.cn

[T51] Scala：Hello World
来源：http://zi.gzmigu.cn

println("Hello")
来源：http://ng.shtwfgs.cn

[T52] Scala：变量
来源：http://wg.newstarts.cn

val a = 1;  var b = 2
来源：http://fv.9csxet.cn

[T53] Scala：字符串插值
来源：http://ua.szxytkj.cn

s"值: $b"
来源：http://ft.nicolike.cn

[T54] Scala：集合映射
来源：http://gl.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://us.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://pm.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mh.521024.cn

[T56] Scala：样例类
来源：http://lg.lnxyls.cn

case class User(name: String, age: Int)
来源：http://wd.hnjuh.cn

[T57] Scala：模式匹配
来源：http://kt.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nx.gzmigu.cn

[T58] Scala：函数定义
来源：http://zf.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jx.colortex.cn

[T59] Scala：循环
来源：http://dk.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://jm.newstarts.cn

[T60] Scala：折叠
来源：http://zt.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qs.haigaiapp.cn

================================================================================
来源：http://ut.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ue.shxzukj.cn

================================================================================
来源：http://gb.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://zg.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zp.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://cv.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lb.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://cd.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://su.szsharing.cn

[U04] Py：变量调试打印
来源：http://kg.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xo.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://er.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://hl.nicolike.cn

[U06] Py：合并两个字典
来源：http://hy.colortex.cn

{**a, **b}
来源：http://gp.jianghongdianzi.cn


<!-- 参考信息 -->