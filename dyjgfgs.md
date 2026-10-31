代发 wailian999

free -h;  ps aux | grep nginx
来源：http://zn.yuexingan06.cn

[R64] 结束进程
来源：http://qc.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://lm.szxytkj.cn

[R65] 查看端口占用
来源：http://sr.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ru.chemitech.net.cn

[R66] 定时任务
来源：http://zm.gzmigu.cn

crontab -e;  crontab -l
来源：http://bx.nszjky.cn

[R67] 生成随机十六进制串
来源：http://bp.chemitech.net.cn

openssl rand -hex 16
来源：http://fr.521024.cn

[R68] 计算文件校验值
来源：http://fi.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zx.9csxet.cn

[R69] 生成随机密码
来源：http://vl.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://md.huanxung.cn

[R70] 时间戳与互转
来源：http://yt.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://io.nszjky.cn

[R71] 日期格式化
来源：http://ka.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lb.panjiajie.cn

[R72] 等待端口就绪
来源：http://qi.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bp.shtwfgs.cn

[R73] 分割大日志
来源：http://nt.huixiangedu.cn

split -l 1000 big.log part_
来源：http://gc.panjiajie.cn

[R74] 批量重命名
来源：http://ek.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rl.bookmarksfly.cn

[R75] 导出环境变量
来源：http://dp.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://kc.yuexingan06.cn

[R76] 使用临时文件
来源：http://wb.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kf.lnxyls.cn

[R77] 读取用户输入
来源：http://cd.9csxet.cn

read -rp "请输入: " ans
来源：http://qn.shxzukj.cn

[R78] 交互式菜单
来源：http://mm.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ag.asd995.cn

[R79] 解析命令行选项
来源：http://bb.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ut.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://zq.muxihuayi.cn

time ./run.sh
来源：http://ho.huixiangedu.cn

================================================================================
来源：http://tj.asd995.cn

S. C / C++ 专题
来源：http://rg.panjiajie.cn

================================================================================
来源：http://ka.9csxet.cn

[S01] C：Hello World
来源：http://ga.yuexingan06.cn

#include <stdio.h>
来源：http://jc.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yr.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://mc.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://yp.lnxyls.cn

[S03] C：读入整数
来源：http://uc.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://gi.wgjwhj.cn

[S04] C：字符串复制
来源：http://vc.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oz.gzmigu.cn

[S05] C：字符串长度
来源：http://xi.huixinmuqiang.cn

strlen(s)
来源：http://vd.huixiangedu.cn

[S06] C：字符串比较
来源：http://sm.colortex.cn

strcmp(a, b) == 0
来源：http://ux.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://bj.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mv.colortex.cn

[S08] C：动态内存分配与释放
来源：http://es.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hy.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://kx.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cs.panjiajie.cn

[S10] C：指针与解引用
来源：http://sx.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://pv.szxytkj.cn

[S11] C：逐行读文件
来源：http://fa.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ij.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jd.jctech888.com.cn

fclose(f);
来源：http://at.colortex.cn

[S12] C：写文件
来源：http://ho.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nt.lnxyls.cn

[S13] C：宏定义
来源：http://xl.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bo.bookmarksfly.cn

[S14] C：枚举
来源：http://oz.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://ya.szsharing.cn

[S15] C：类型转换
来源：http://ow.nszjky.cn

(double) a / b
来源：http://wv.muxihuayi.cn

[S16] C：位操作置位
来源：http://vm.gzmigu.cn

x |= (1 << 3);
来源：http://di.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://jc.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wz.521024.cn

[S18] C：命令行参数
来源：http://zi.szxytkj.cn

int main(int argc, char **argv)
来源：http://qd.bookmarksfly.cn

[S19] C：快速排序
来源：http://fv.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yb.lnxyls.cn

[S20] C：二分查找
来源：http://iv.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qn.wgjwhj.cn

[S21] C：字符类别判断
来源：http://ze.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://et.hnjuh.cn

[S22] C：字符串转数字
来源：http://er.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jf.panjiajie.cn

[S23] C：随机数
来源：http://xv.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bg.szxytkj.cn

[S24] C：获取本地时间
来源：http://jx.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mo.lnxyls.cn

[S25] C：内存拷贝
来源：http://jr.shxzskj.cn

memcpy(dst, src, n);
来源：http://op.huixiangedu.cn

[S26] C：内存清零
来源：http://jy.9csxet.cn

memset(a, 0, sizeof a);
来源：http://nr.colortex.cn

[S27] C：定义常量
来源：http://mu.bookmarksfly.cn

const double PI = 3.14159;
来源：http://pp.jianghongdianzi.cn

[S28] C：静态变量
来源：http://sv.gzmigu.cn

static int counter = 0;
来源：http://ns.hahajie.cn

[S29] C：变参函数
来源：http://xy.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rc.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://wm.bookmarksfly.cn

#ifndef X_H
来源：http://nh.jianghongdianzi.cn

#define X_H
来源：http://tr.lnxyls.cn

#endif
来源：http://iz.chemitech.net.cn

[S31] C++：Hello World
来源：http://eq.bookmarksfly.cn

#include <iostream>
来源：http://ka.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://mq.bookmarksfly.cn

[S32] C++：字符串
来源：http://bj.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://oh.jctech888.com.cn

[S33] C++：vector 增删
来源：http://eq.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jp.gzmigu.cn

[S34] C++：遍历 vector
来源：http://sb.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://gk.newstarts.cn

[S35] C++：map
来源：http://kj.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gn.newstarts.cn

[S36] C++：unordered_map
来源：http://zh.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uj.521024.cn

[S37] C++：set
来源：http://vm.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zj.muxihuayi.cn

[S38] C++：排序
来源：http://so.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://xy.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://ax.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xg.521024.cn

[S40] C++：查找元素
来源：http://rf.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zd.shxzukj.cn

[S41] C++：类与构造函数
来源：http://oh.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ou.huanxung.cn

[S42] C++：继承与虚函数
来源：http://un.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://gs.gzmigu.cn

[S43] C++：智能指针
来源：http://nj.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://ye.szxytkj.cn

[S44] C++：引用传参
来源：http://qj.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ek.yuexingan06.cn

[S45] C++：lambda
来源：http://vt.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ud.gzmigu.cn

[S46] C++：函数模板
来源：http://wa.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nz.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://pv.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ls.colortex.cn

[S48] C++：逐行读文件
来源：http://ar.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mj.nicolike.cn

while (std::getline(in, line)) { }
来源：http://bj.yuntaijiaju.cn

[S49] C++：写文件
来源：http://wb.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ry.lnxyls.cn

[S50] C++：格式化数字
来源：http://dn.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pa.shxzskj.cn

[S51] C++：显式类型转换
来源：http://qu.muxihuayi.cn

static_cast<double>(a) / b
来源：http://nk.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://cf.colortex.cn

int size() const noexcept { return n_; }
来源：http://da.bjjhwx.cn

[S53] C++：移动语义
来源：http://qa.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://br.shtwfgs.cn

[S54] C++：异常处理
来源：http://gu.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bl.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://un.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xu.yuntaijiaju.cn

[S56] C++：optional
来源：http://hk.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qq.shtwfgs.cn

[S57] C++：编译期常量
来源：http://gi.jianghongdianzi.cn

constexpr int N = 10;
来源：http://mq.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://gi.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://tu.hahajie.cn

[S59] C++：静态断言
来源：http://jq.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://un.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://xg.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ok.yuexingan06.cn

================================================================================
来源：http://wt.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://in.nicolike.cn

================================================================================
来源：http://eo.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://eg.szsharing.cn

println("Hello")
来源：http://xx.9csxet.cn

[T02] Kotlin：变量
来源：http://pj.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ve.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://va.lnxyls.cn

"值: $b"
来源：http://dv.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://gw.szsharing.cn

val n: String? = null;  n?.length
来源：http://xk.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://uz.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vj.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://og.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bk.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://vs.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dy.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://fh.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://mf.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://td.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://vt.hahajie.cn

[T10] Kotlin：默认参数
来源：http://da.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vm.panjiajie.cn

[T11] Kotlin：协程
来源：http://zz.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yh.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://dm.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://yg.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://id.newstarts.cn

val m = mapOf("a" to 1)
来源：http://fq.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://nk.hnjuh.cn

for (i in 1..10) println(i)
来源：http://tq.wgjwhj.cn

[T15] Kotlin：接口
来源：http://dr.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://de.shxzskj.cn

[T16] Swift：Hello World
来源：http://uy.shxzskj.cn

print("Hello")
来源：http://yf.shxzskj.cn

[T17] Swift：变量与常量
来源：http://ey.hahajie.cn

var a = 1;  let b = 2
来源：http://tz.szsharing.cn

[T18] Swift：字符串插值
来源：http://fl.huixiangedu.cn

"值: \(b)"
来源：http://ty.lnxyls.cn

[T19] Swift：可选绑定
来源：http://qd.nszjky.cn

if let n = opt { print(n) }
来源：http://yn.haigaiapp.cn

[T20] Swift：数组操作
来源：http://ga.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xy.huixiangedu.cn

[T21] Swift：遍历
来源：http://mh.wgjwhj.cn

for x in a { print(x) }
来源：http://la.huixiangedu.cn

[T22] Swift：字典
来源：http://er.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xa.nicolike.cn

[T23] Swift：函数
来源：http://xq.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zx.9csxet.cn

[T24] Swift：闭包
来源：http://xy.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bv.shtwfgs.cn

[T25] Swift：结构体
来源：http://up.huixiangedu.cn

struct P { var x: Int }
来源：http://ja.nszjky.cn

[T26] Swift：类与重写
来源：http://pw.9csxet.cn

class A: Base { override func f() {} }
来源：http://lr.yuexingan06.cn

[T27] Swift：错误处理
来源：http://ot.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://ei.shtwfgs.cn

[T28] Swift：枚举
来源：http://sq.colortex.cn

enum Color { case red, green }
来源：http://lq.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://ug.9csxet.cn

guard let x = opt else { return }
来源：http://xf.szsharing.cn

[T30] Swift：协议
来源：http://uz.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://kz.asd995.cn

[T31] Lua：Hello World
来源：http://lm.nszjky.cn

print("Hello")
来源：http://xc.shtwfgs.cn

[T32] Lua：局部变量
来源：http://zw.colortex.cn

local a = 1
来源：http://hw.colortex.cn

[T33] Lua：表（数组）
来源：http://dl.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fc.nszjky.cn

[T34] Lua：遍历表
来源：http://hx.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ij.9csxet.cn

[T35] Lua：字典表
来源：http://un.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://lu.huixiangedu.cn

[T36] Lua：函数
来源：http://js.chemitech.net.cn

function add(a, b) return a + b end
来源：http://dc.9csxet.cn

[T37] Lua：字符串拼接
来源：http://am.nszjky.cn

"a" .. "b"
来源：http://zr.gzmigu.cn

[T38] Lua：条件
来源：http://sa.haigaiapp.cn

if x > 0 then print("正") end
来源：http://ud.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://mq.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://oe.9csxet.cn

[T40] Lua：元表
来源：http://rp.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://kt.newstarts.cn

[T41] Perl：Hello World
来源：http://md.nszjky.cn

print "Hello\n";
来源：http://pz.9csxet.cn

[T42] Perl：变量类型
来源：http://dn.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vw.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://pu.shxzukj.cn

"值: $a"
来源：http://fq.nszjky.cn

[T44] Perl：条件
来源：http://cu.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://on.nicolike.cn

[T45] Perl：数组遍历
来源：http://mr.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://wv.shxzskj.cn

[T46] Perl：哈希操作
来源：http://ly.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bp.szsharing.cn

[T47] Perl：正则捕获
来源：http://yn.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jw.bjjhwx.cn

[T48] Perl：正则替换
来源：http://ue.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://nk.jianghongdianzi.cn

[T49] Perl：函数
来源：http://vo.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rv.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://cq.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oa.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://pu.colortex.cn

[T51] Scala：Hello World
来源：http://dd.colortex.cn

println("Hello")
来源：http://ch.yuexingan06.cn

[T52] Scala：变量
来源：http://vu.szsharing.cn

val a = 1;  var b = 2
来源：http://ae.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://id.wgjwhj.cn

s"值: $b"
来源：http://uf.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://rt.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://fk.lnxyls.cn

[T55] Scala：集合过滤
来源：http://dc.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://na.bjjhwx.cn

[T56] Scala：样例类
来源：http://vy.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://wt.shxzukj.cn

[T57] Scala：模式匹配
来源：http://zq.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bk.szxytkj.cn

[T58] Scala：函数定义
来源：http://ei.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://as.szsharing.cn

[T59] Scala：循环
来源：http://bu.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://al.newstarts.cn

[T60] Scala：折叠
来源：http://tx.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ja.lnxyls.cn

================================================================================
来源：http://fc.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kz.muxihuayi.cn

================================================================================
来源：http://vd.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://lf.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lh.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://vr.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ku.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://od.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bc.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://mx.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tl.nicolike.cn


<!-- 参考信息 -->