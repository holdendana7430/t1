代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qw.asd995.cn

[R66] 定时任务
来源：http://sj.hnjuh.cn

crontab -e;  crontab -l
来源：http://kv.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ac.shtwfgs.cn

openssl rand -hex 16
来源：http://zj.huanxung.cn

[R68] 计算文件校验值
来源：http://je.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yr.wgjwhj.cn

[R69] 生成随机密码
来源：http://cb.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://yy.gzmigu.cn

[R70] 时间戳与互转
来源：http://of.huanxung.cn

date +%s;  date -d @1700000000
来源：http://lf.yuntaijiaju.cn

[R71] 日期格式化
来源：http://xi.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ps.colortex.cn

[R72] 等待端口就绪
来源：http://mf.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qn.bookmarksfly.cn

[R73] 分割大日志
来源：http://az.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://nx.muxihuayi.cn

[R74] 批量重命名
来源：http://pz.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ib.haigaiapp.cn

[R75] 导出环境变量
来源：http://jw.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://nk.haigaiapp.cn

[R76] 使用临时文件
来源：http://br.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gy.colortex.cn

[R77] 读取用户输入
来源：http://zx.szsharing.cn

read -rp "请输入: " ans
来源：http://ky.shtwfgs.cn

[R78] 交互式菜单
来源：http://rp.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rc.huanxung.cn

[R79] 解析命令行选项
来源：http://vs.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://co.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://mp.nicolike.cn

time ./run.sh
来源：http://sz.szsharing.cn

================================================================================
来源：http://ni.nicolike.cn

S. C / C++ 专题
来源：http://jp.muxihuayi.cn

================================================================================
来源：http://sk.haigaiapp.cn

[S01] C：Hello World
来源：http://ig.hahajie.cn

#include <stdio.h>
来源：http://nq.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yk.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://cm.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://ub.muxihuayi.cn

[S03] C：读入整数
来源：http://vw.shxzskj.cn

int x; scanf("%d", &x);
来源：http://jb.hahajie.cn

[S04] C：字符串复制
来源：http://dq.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ye.bjjhwx.cn

[S05] C：字符串长度
来源：http://xi.huixinmuqiang.cn

strlen(s)
来源：http://fl.chemitech.net.cn

[S06] C：字符串比较
来源：http://ui.asd995.cn

strcmp(a, b) == 0
来源：http://qc.hahajie.cn

[S07] C：数组遍历求和
来源：http://kw.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dj.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://yj.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nb.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://ua.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://po.shxzskj.cn

[S10] C：指针与解引用
来源：http://qp.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ss.hnjuh.cn

[S11] C：逐行读文件
来源：http://si.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://sv.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nx.gzmigu.cn

fclose(f);
来源：http://nj.yuexingan06.cn

[S12] C：写文件
来源：http://st.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wy.yuntaijiaju.cn

[S13] C：宏定义
来源：http://cu.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vs.shxzskj.cn

[S14] C：枚举
来源：http://mn.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://rm.yuntaijiaju.cn

[S15] C：类型转换
来源：http://dl.shxzskj.cn

(double) a / b
来源：http://nn.nszjky.cn

[S16] C：位操作置位
来源：http://ji.nszjky.cn

x |= (1 << 3);
来源：http://eg.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://zm.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://em.huixiangedu.cn

[S18] C：命令行参数
来源：http://pw.huanxung.cn

int main(int argc, char **argv)
来源：http://uv.lnxyls.cn

[S19] C：快速排序
来源：http://vq.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gl.muxihuayi.cn

[S20] C：二分查找
来源：http://jr.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://he.wgjwhj.cn

[S21] C：字符类别判断
来源：http://fs.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sj.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://wa.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ob.yuntaijiaju.cn

[S23] C：随机数
来源：http://oc.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://km.nicolike.cn

[S24] C：获取本地时间
来源：http://aj.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oz.szxytkj.cn

[S25] C：内存拷贝
来源：http://la.huixiangedu.cn

memcpy(dst, src, n);
来源：http://em.jctech888.com.cn

[S26] C：内存清零
来源：http://ci.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://ke.hnjuh.cn

[S27] C：定义常量
来源：http://em.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://yk.nicolike.cn

[S28] C：静态变量
来源：http://cx.bjjhwx.cn

static int counter = 0;
来源：http://jb.521024.cn

[S29] C：变参函数
来源：http://gx.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wg.wgjwhj.cn

[S30] C：头文件保护
来源：http://br.colortex.cn

#ifndef X_H
来源：http://ys.yuntaijiaju.cn

#define X_H
来源：http://cx.chemitech.net.cn

#endif
来源：http://yp.hahajie.cn

[S31] C++：Hello World
来源：http://hc.shxzukj.cn

#include <iostream>
来源：http://vz.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://ro.bookmarksfly.cn

[S32] C++：字符串
来源：http://ja.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://cw.nszjky.cn

[S33] C++：vector 增删
来源：http://hz.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ni.shxzskj.cn

[S34] C++：遍历 vector
来源：http://sw.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://xm.huanxung.cn

[S35] C++：map
来源：http://sv.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ag.haigaiapp.cn

[S36] C++：unordered_map
来源：http://iy.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jf.yuntaijiaju.cn

[S37] C++：set
来源：http://it.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://br.lnxyls.cn

[S38] C++：排序
来源：http://qp.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://mb.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://kz.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qp.asd995.cn

[S40] C++：查找元素
来源：http://th.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eu.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://nk.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nc.nicolike.cn

[S42] C++：继承与虚函数
来源：http://ki.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://rh.shxzukj.cn

[S43] C++：智能指针
来源：http://vb.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://xk.shtwfgs.cn

[S44] C++：引用传参
来源：http://il.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://er.jctech888.com.cn

[S45] C++：lambda
来源：http://eo.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ph.nszjky.cn

[S46] C++：函数模板
来源：http://zz.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mm.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://rd.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dt.panjiajie.cn

[S48] C++：逐行读文件
来源：http://ck.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pb.nicolike.cn

while (std::getline(in, line)) { }
来源：http://sv.jctech888.com.cn

[S49] C++：写文件
来源：http://oz.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hk.nszjky.cn

[S50] C++：格式化数字
来源：http://lx.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://et.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://te.gzmigu.cn

static_cast<double>(a) / b
来源：http://xc.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://sv.huanxung.cn

int size() const noexcept { return n_; }
来源：http://cr.gzmigu.cn

[S53] C++：移动语义
来源：http://bs.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://he.shtwfgs.cn

[S54] C++：异常处理
来源：http://ul.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bs.521024.cn

[S55] C++：结构化绑定
来源：http://jl.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vm.gzmigu.cn

[S56] C++：optional
来源：http://nc.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pm.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://hi.nszjky.cn

constexpr int N = 10;
来源：http://pu.haigaiapp.cn

[S58] C++：命名空间
来源：http://px.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://rk.panjiajie.cn

[S59] C++：静态断言
来源：http://lw.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aq.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://gi.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jn.panjiajie.cn

================================================================================
来源：http://ib.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mu.newstarts.cn

================================================================================
来源：http://ew.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://oq.yuexingan06.cn

println("Hello")
来源：http://ys.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ff.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lo.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://pb.bjjhwx.cn

"值: $b"
来源：http://vp.shxzukj.cn

[T04] Kotlin：空安全
来源：http://dj.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ce.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://gm.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ui.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://xs.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ke.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://sm.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bc.panjiajie.cn

[T08] Kotlin：数据类
来源：http://im.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ju.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://ea.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://dj.huanxung.cn

[T10] Kotlin：默认参数
来源：http://ib.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sh.lnxyls.cn

[T11] Kotlin：协程
来源：http://xm.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nn.nicolike.cn

[T12] Kotlin：解构声明
来源：http://uo.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://oz.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://ul.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://ua.yuexingan06.cn

[T14] Kotlin：循环
来源：http://ih.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://sn.lnxyls.cn

[T15] Kotlin：接口
来源：http://lq.9csxet.cn

interface Shape { fun area(): Double }
来源：http://rl.shxzukj.cn

[T16] Swift：Hello World
来源：http://qx.hnjuh.cn

print("Hello")
来源：http://oq.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://cq.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://kt.szsharing.cn

[T18] Swift：字符串插值
来源：http://wk.szsharing.cn

"值: \(b)"
来源：http://ru.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://er.hahajie.cn

if let n = opt { print(n) }
来源：http://pm.haigaiapp.cn

[T20] Swift：数组操作
来源：http://jh.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ud.muxihuayi.cn

[T21] Swift：遍历
来源：http://la.nszjky.cn

for x in a { print(x) }
来源：http://ch.haigaiapp.cn

[T22] Swift：字典
来源：http://ah.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://no.haigaiapp.cn

[T23] Swift：函数
来源：http://dp.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bq.szsharing.cn

[T24] Swift：闭包
来源：http://lo.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ju.wgjwhj.cn

[T25] Swift：结构体
来源：http://lt.nszjky.cn

struct P { var x: Int }
来源：http://iy.nszjky.cn

[T26] Swift：类与重写
来源：http://mg.shxzskj.cn

class A: Base { override func f() {} }
来源：http://mb.shxzskj.cn

[T27] Swift：错误处理
来源：http://ju.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://pk.huanxung.cn

[T28] Swift：枚举
来源：http://vb.shxzukj.cn

enum Color { case red, green }
来源：http://yy.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://el.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://zm.szsharing.cn

[T30] Swift：协议
来源：http://xu.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://re.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://fi.hnjuh.cn

print("Hello")
来源：http://ub.hnjuh.cn

[T32] Lua：局部变量
来源：http://jy.szsharing.cn

local a = 1
来源：http://jd.gzmigu.cn

[T33] Lua：表（数组）
来源：http://xt.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kn.huanxung.cn

[T34] Lua：遍历表
来源：http://js.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ks.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://sp.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://tq.huanxung.cn

[T36] Lua：函数
来源：http://gd.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://zw.521024.cn

[T37] Lua：字符串拼接
来源：http://jd.colortex.cn

"a" .. "b"
来源：http://oi.huixiangedu.cn

[T38] Lua：条件
来源：http://tr.shxzukj.cn

if x > 0 then print("正") end
来源：http://th.9csxet.cn

[T39] Lua：模式匹配
来源：http://rv.lnxyls.cn

string.find(s, "%d+")
来源：http://rw.huixinmuqiang.cn

[T40] Lua：元表
来源：http://oi.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://zw.wgjwhj.cn

[T41] Perl：Hello World
来源：http://th.huanxung.cn

print "Hello\n";
来源：http://sx.colortex.cn

[T42] Perl：变量类型
来源：http://nk.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mk.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://el.bookmarksfly.cn

"值: $a"
来源：http://zi.asd995.cn

[T44] Perl：条件
来源：http://oo.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://ue.lnxyls.cn

[T45] Perl：数组遍历
来源：http://wr.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://fu.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://xt.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zr.nszjky.cn

[T47] Perl：正则捕获
来源：http://kg.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hr.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://fl.szxytkj.cn

$s =~ s/old/new/g;
来源：http://xw.huixinmuqiang.cn

[T49] Perl：函数
来源：http://rb.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gp.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://gx.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://np.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://vv.shxzskj.cn

[T51] Scala：Hello World
来源：http://ms.szsharing.cn

println("Hello")
来源：http://cq.yuexingan06.cn

[T52] Scala：变量
来源：http://ih.shtwfgs.cn

val a = 1;  var b = 2
来源：http://yx.lnxyls.cn

[T53] Scala：字符串插值
来源：http://pa.521024.cn

s"值: $b"
来源：http://zj.szxytkj.cn

[T54] Scala：集合映射
来源：http://mz.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://uw.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://kb.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oy.huanxung.cn

[T56] Scala：样例类
来源：http://se.colortex.cn

case class User(name: String, age: Int)
来源：http://bu.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://mg.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kx.chemitech.net.cn

[T58] Scala：函数定义
来源：http://wb.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mb.shxzukj.cn

[T59] Scala：循环
来源：http://kt.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://gl.chemitech.net.cn

[T60] Scala：折叠
来源：http://wv.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xe.bookmarksfly.cn

================================================================================
来源：http://hs.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ct.9csxet.cn

================================================================================
来源：http://am.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://xy.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lm.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://pr.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hx.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://tz.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dm.521024.cn

[U04] Py：变量调试打印
来源：http://px.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ab.521024.cn

[U05] Py：列表去重且保序
来源：http://ai.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://hb.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://ai.muxihuayi.cn

{**a, **b}
来源：http://lj.huixinmuqiang.cn


<!-- 参考信息 -->