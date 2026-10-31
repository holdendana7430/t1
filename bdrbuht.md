代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zn.haigaiapp.cn

[R66] 定时任务
来源：http://qd.jctech888.com.cn

crontab -e;  crontab -l
来源：http://gq.nszjky.cn

[R67] 生成随机十六进制串
来源：http://wd.huixinmuqiang.cn

openssl rand -hex 16
来源：http://ix.shxzukj.cn

[R68] 计算文件校验值
来源：http://ow.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cr.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://jl.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://qn.hahajie.cn

[R70] 时间戳与互转
来源：http://gt.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://pq.haigaiapp.cn

[R71] 日期格式化
来源：http://yt.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uj.bjjhwx.cn

[R72] 等待端口就绪
来源：http://xo.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iw.panjiajie.cn

[R73] 分割大日志
来源：http://gd.hnjuh.cn

split -l 1000 big.log part_
来源：http://ji.nicolike.cn

[R74] 批量重命名
来源：http://fj.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gu.chemitech.net.cn

[R75] 导出环境变量
来源：http://md.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://po.huixiangedu.cn

[R76] 使用临时文件
来源：http://cs.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://av.muxihuayi.cn

[R77] 读取用户输入
来源：http://ly.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://zv.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://qh.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ut.huixiangedu.cn

[R79] 解析命令行选项
来源：http://lp.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gz.521024.cn

[R80] 查看脚本执行耗时
来源：http://qu.gzmigu.cn

time ./run.sh
来源：http://za.muxihuayi.cn

================================================================================
来源：http://jy.szxytkj.cn

S. C / C++ 专题
来源：http://rg.colortex.cn

================================================================================
来源：http://nu.bookmarksfly.cn

[S01] C：Hello World
来源：http://dr.jianghongdianzi.cn

#include <stdio.h>
来源：http://fv.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fg.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://bw.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://oh.gzmigu.cn

[S03] C：读入整数
来源：http://kh.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://zg.asd995.cn

[S04] C：字符串复制
来源：http://sd.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cu.shtwfgs.cn

[S05] C：字符串长度
来源：http://fq.haigaiapp.cn

strlen(s)
来源：http://ff.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://lr.shxzukj.cn

strcmp(a, b) == 0
来源：http://on.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://wy.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gi.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://wf.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kx.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://yz.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jo.521024.cn

[S10] C：指针与解引用
来源：http://oo.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ee.jctech888.com.cn

[S11] C：逐行读文件
来源：http://ao.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://pu.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rb.haigaiapp.cn

fclose(f);
来源：http://fi.yuntaijiaju.cn

[S12] C：写文件
来源：http://mm.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dl.wgjwhj.cn

[S13] C：宏定义
来源：http://le.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uh.haigaiapp.cn

[S14] C：枚举
来源：http://fc.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://ip.nicolike.cn

[S15] C：类型转换
来源：http://ug.jianghongdianzi.cn

(double) a / b
来源：http://pj.huixiangedu.cn

[S16] C：位操作置位
来源：http://ba.nszjky.cn

x |= (1 << 3);
来源：http://cw.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ho.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://he.chemitech.net.cn

[S18] C：命令行参数
来源：http://yi.panjiajie.cn

int main(int argc, char **argv)
来源：http://hh.asd995.cn

[S19] C：快速排序
来源：http://rg.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://un.szsharing.cn

[S20] C：二分查找
来源：http://vh.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sw.gzmigu.cn

[S21] C：字符类别判断
来源：http://tg.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nq.chemitech.net.cn

[S22] C：字符串转数字
来源：http://vx.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oi.huanxung.cn

[S23] C：随机数
来源：http://nz.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ox.lnxyls.cn

[S24] C：获取本地时间
来源：http://jw.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ag.wgjwhj.cn

[S25] C：内存拷贝
来源：http://gs.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://yv.bookmarksfly.cn

[S26] C：内存清零
来源：http://dl.nszjky.cn

memset(a, 0, sizeof a);
来源：http://zm.szsharing.cn

[S27] C：定义常量
来源：http://si.shxzukj.cn

const double PI = 3.14159;
来源：http://lj.huixiangedu.cn

[S28] C：静态变量
来源：http://gi.shxzukj.cn

static int counter = 0;
来源：http://cv.newstarts.cn

[S29] C：变参函数
来源：http://bp.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bk.szsharing.cn

[S30] C：头文件保护
来源：http://fj.muxihuayi.cn

#ifndef X_H
来源：http://bq.bjjhwx.cn

#define X_H
来源：http://ow.muxihuayi.cn

#endif
来源：http://su.newstarts.cn

[S31] C++：Hello World
来源：http://dd.szxytkj.cn

#include <iostream>
来源：http://hf.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ou.hnjuh.cn

[S32] C++：字符串
来源：http://lf.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://up.hnjuh.cn

[S33] C++：vector 增删
来源：http://rx.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fl.asd995.cn

[S34] C++：遍历 vector
来源：http://ey.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://sm.bjjhwx.cn

[S35] C++：map
来源：http://ae.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wr.panjiajie.cn

[S36] C++：unordered_map
来源：http://ou.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tn.bjjhwx.cn

[S37] C++：set
来源：http://za.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://np.521024.cn

[S38] C++：排序
来源：http://sj.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://qc.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ps.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oj.bookmarksfly.cn

[S40] C++：查找元素
来源：http://lo.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pm.nszjky.cn

[S41] C++：类与构造函数
来源：http://gk.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qs.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://xc.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://ro.yuexingan06.cn

[S43] C++：智能指针
来源：http://rv.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://pj.huanxung.cn

[S44] C++：引用传参
来源：http://xd.newstarts.cn

void inc(int &x) { ++x; }
来源：http://ut.bookmarksfly.cn

[S45] C++：lambda
来源：http://pl.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aa.asd995.cn

[S46] C++：函数模板
来源：http://dr.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dc.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://bn.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qn.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://mn.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wg.szsharing.cn

while (std::getline(in, line)) { }
来源：http://bd.hnjuh.cn

[S49] C++：写文件
来源：http://am.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rg.szxytkj.cn

[S50] C++：格式化数字
来源：http://qn.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fj.huanxung.cn

[S51] C++：显式类型转换
来源：http://wm.asd995.cn

static_cast<double>(a) / b
来源：http://ia.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://yb.521024.cn

int size() const noexcept { return n_; }
来源：http://ck.yuexingan06.cn

[S53] C++：移动语义
来源：http://ww.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://gn.szxytkj.cn

[S54] C++：异常处理
来源：http://hk.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oc.shxzskj.cn

[S55] C++：结构化绑定
来源：http://mm.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mr.hahajie.cn

[S56] C++：optional
来源：http://no.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://am.szxytkj.cn

[S57] C++：编译期常量
来源：http://vh.lnxyls.cn

constexpr int N = 10;
来源：http://pg.bjjhwx.cn

[S58] C++：命名空间
来源：http://mt.521024.cn

namespace ns { int f() { return 1; } }
来源：http://io.bjjhwx.cn

[S59] C++：静态断言
来源：http://qu.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://br.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://vc.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bo.haigaiapp.cn

================================================================================
来源：http://bh.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jz.muxihuayi.cn

================================================================================
来源：http://aq.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://cc.bjjhwx.cn

println("Hello")
来源：http://ig.lnxyls.cn

[T02] Kotlin：变量
来源：http://ae.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rj.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://cp.szsharing.cn

"值: $b"
来源：http://zo.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://se.hahajie.cn

val n: String? = null;  n?.length
来源：http://qt.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://rx.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://at.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://uy.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yo.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://vy.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xi.colortex.cn

[T08] Kotlin：数据类
来源：http://np.asd995.cn

data class User(val name: String, val age: Int)
来源：http://nt.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://oa.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://kr.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://nz.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oi.yuexingan06.cn

[T11] Kotlin：协程
来源：http://mg.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fx.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://rh.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://yz.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://ba.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://xk.521024.cn

[T14] Kotlin：循环
来源：http://jn.shxzskj.cn

for (i in 1..10) println(i)
来源：http://cw.asd995.cn

[T15] Kotlin：接口
来源：http://qa.9csxet.cn

interface Shape { fun area(): Double }
来源：http://yj.chemitech.net.cn

[T16] Swift：Hello World
来源：http://iv.huixinmuqiang.cn

print("Hello")
来源：http://vw.szsharing.cn

[T17] Swift：变量与常量
来源：http://ob.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://dr.asd995.cn

[T18] Swift：字符串插值
来源：http://yx.jctech888.com.cn

"值: \(b)"
来源：http://fo.hnjuh.cn

[T19] Swift：可选绑定
来源：http://pz.bjjhwx.cn

if let n = opt { print(n) }
来源：http://kj.newstarts.cn

[T20] Swift：数组操作
来源：http://yg.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qm.hnjuh.cn

[T21] Swift：遍历
来源：http://qw.jctech888.com.cn

for x in a { print(x) }
来源：http://it.shxzukj.cn

[T22] Swift：字典
来源：http://xi.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fe.yuexingan06.cn

[T23] Swift：函数
来源：http://jy.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nh.shxzskj.cn

[T24] Swift：闭包
来源：http://ip.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ee.haigaiapp.cn

[T25] Swift：结构体
来源：http://gf.huixinmuqiang.cn

struct P { var x: Int }
来源：http://ho.nszjky.cn

[T26] Swift：类与重写
来源：http://mq.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://mf.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://gz.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://nw.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://na.huixiangedu.cn

enum Color { case red, green }
来源：http://rf.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://pd.gzmigu.cn

guard let x = opt else { return }
来源：http://pd.colortex.cn

[T30] Swift：协议
来源：http://ga.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://ru.szxytkj.cn

[T31] Lua：Hello World
来源：http://ao.lnxyls.cn

print("Hello")
来源：http://ur.asd995.cn

[T32] Lua：局部变量
来源：http://yu.haigaiapp.cn

local a = 1
来源：http://me.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://jp.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bd.jctech888.com.cn

[T34] Lua：遍历表
来源：http://ev.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yx.gzmigu.cn

[T35] Lua：字典表
来源：http://ut.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://pk.521024.cn

[T36] Lua：函数
来源：http://iy.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://gr.nicolike.cn

[T37] Lua：字符串拼接
来源：http://hj.yuexingan06.cn

"a" .. "b"
来源：http://jv.shtwfgs.cn

[T38] Lua：条件
来源：http://on.panjiajie.cn

if x > 0 then print("正") end
来源：http://ne.nszjky.cn

[T39] Lua：模式匹配
来源：http://xv.hahajie.cn

string.find(s, "%d+")
来源：http://yr.haigaiapp.cn

[T40] Lua：元表
来源：http://ou.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://zy.hnjuh.cn

[T41] Perl：Hello World
来源：http://oh.szxytkj.cn

print "Hello\n";
来源：http://gw.szxytkj.cn

[T42] Perl：变量类型
来源：http://bw.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://do.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://qj.nicolike.cn

"值: $a"
来源：http://iy.panjiajie.cn

[T44] Perl：条件
来源：http://ws.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://lt.shxzukj.cn

[T45] Perl：数组遍历
来源：http://hk.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://rt.hahajie.cn

[T46] Perl：哈希操作
来源：http://ri.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zm.shxzskj.cn

[T47] Perl：正则捕获
来源：http://af.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mu.colortex.cn

[T48] Perl：正则替换
来源：http://et.hahajie.cn

$s =~ s/old/new/g;
来源：http://ln.shtwfgs.cn

[T49] Perl：函数
来源：http://tq.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://au.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://hg.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://je.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://dn.chemitech.net.cn

[T51] Scala：Hello World
来源：http://xf.gzmigu.cn

println("Hello")
来源：http://aa.wgjwhj.cn

[T52] Scala：变量
来源：http://uj.huanxung.cn

val a = 1;  var b = 2
来源：http://hp.colortex.cn

[T53] Scala：字符串插值
来源：http://fg.shxzukj.cn

s"值: $b"
来源：http://fc.lnxyls.cn

[T54] Scala：集合映射
来源：http://pq.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://qd.nszjky.cn

[T55] Scala：集合过滤
来源：http://mb.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gh.shtwfgs.cn

[T56] Scala：样例类
来源：http://tr.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://sq.nszjky.cn

[T57] Scala：模式匹配
来源：http://tt.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://if.szxytkj.cn

[T58] Scala：函数定义
来源：http://yj.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sr.hahajie.cn

[T59] Scala：循环
来源：http://xz.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://rb.huanxung.cn

[T60] Scala：折叠
来源：http://bd.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cz.shxzskj.cn

================================================================================
来源：http://po.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zl.chemitech.net.cn

================================================================================
来源：http://na.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://fs.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xo.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://vx.asd995.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kp.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://xd.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mj.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://pv.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uf.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://im.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://vr.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://gj.521024.cn

{**a, **b}
来源：http://me.szsharing.cn


<!-- 参考信息 -->