代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ts.muxihuayi.cn

[R66] 定时任务
来源：http://iz.colortex.cn

crontab -e;  crontab -l
来源：http://eg.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://cv.colortex.cn

openssl rand -hex 16
来源：http://ni.szsharing.cn

[R68] 计算文件校验值
来源：http://gz.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vg.nszjky.cn

[R69] 生成随机密码
来源：http://ys.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://vo.chemitech.net.cn

[R70] 时间戳与互转
来源：http://su.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://mb.muxihuayi.cn

[R71] 日期格式化
来源：http://cx.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wg.szxytkj.cn

[R72] 等待端口就绪
来源：http://ak.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sf.huanxung.cn

[R73] 分割大日志
来源：http://st.chemitech.net.cn

split -l 1000 big.log part_
来源：http://sx.bjjhwx.cn

[R74] 批量重命名
来源：http://it.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hf.asd995.cn

[R75] 导出环境变量
来源：http://qc.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://ay.asd995.cn

[R76] 使用临时文件
来源：http://mf.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rw.bjjhwx.cn

[R77] 读取用户输入
来源：http://jp.panjiajie.cn

read -rp "请输入: " ans
来源：http://ve.huanxung.cn

[R78] 交互式菜单
来源：http://gl.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fy.huanxung.cn

[R79] 解析命令行选项
来源：http://dr.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vf.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://rd.haigaiapp.cn

time ./run.sh
来源：http://gq.bjjhwx.cn

================================================================================
来源：http://kd.gzmigu.cn

S. C / C++ 专题
来源：http://ze.huanxung.cn

================================================================================
来源：http://gf.nszjky.cn

[S01] C：Hello World
来源：http://ia.nicolike.cn

#include <stdio.h>
来源：http://ar.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gc.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://wp.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://aq.jianghongdianzi.cn

[S03] C：读入整数
来源：http://ux.lnxyls.cn

int x; scanf("%d", &x);
来源：http://cl.bookmarksfly.cn

[S04] C：字符串复制
来源：http://zq.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ew.chemitech.net.cn

[S05] C：字符串长度
来源：http://lw.huixiangedu.cn

strlen(s)
来源：http://fq.asd995.cn

[S06] C：字符串比较
来源：http://fe.shtwfgs.cn

strcmp(a, b) == 0
来源：http://vn.9csxet.cn

[S07] C：数组遍历求和
来源：http://hi.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xu.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://au.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mj.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://bp.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yr.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://nr.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://qi.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://wq.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://qe.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wh.asd995.cn

fclose(f);
来源：http://qu.newstarts.cn

[S12] C：写文件
来源：http://gt.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zf.colortex.cn

[S13] C：宏定义
来源：http://bf.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bq.newstarts.cn

[S14] C：枚举
来源：http://wh.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://kv.yuntaijiaju.cn

[S15] C：类型转换
来源：http://yz.chemitech.net.cn

(double) a / b
来源：http://no.9csxet.cn

[S16] C：位操作置位
来源：http://wv.shtwfgs.cn

x |= (1 << 3);
来源：http://ag.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://rb.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bg.hnjuh.cn

[S18] C：命令行参数
来源：http://dl.panjiajie.cn

int main(int argc, char **argv)
来源：http://zz.wgjwhj.cn

[S19] C：快速排序
来源：http://il.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tg.nszjky.cn

[S20] C：二分查找
来源：http://qg.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lx.haigaiapp.cn

[S21] C：字符类别判断
来源：http://go.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hs.shxzukj.cn

[S22] C：字符串转数字
来源：http://xk.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cz.shtwfgs.cn

[S23] C：随机数
来源：http://ow.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cj.hnjuh.cn

[S24] C：获取本地时间
来源：http://yw.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://va.jctech888.com.cn

[S25] C：内存拷贝
来源：http://yy.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://cp.asd995.cn

[S26] C：内存清零
来源：http://wv.huanxung.cn

memset(a, 0, sizeof a);
来源：http://dc.jianghongdianzi.cn

[S27] C：定义常量
来源：http://rg.hnjuh.cn

const double PI = 3.14159;
来源：http://oe.521024.cn

[S28] C：静态变量
来源：http://kp.colortex.cn

static int counter = 0;
来源：http://ke.szxytkj.cn

[S29] C：变参函数
来源：http://dd.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uj.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://zy.chemitech.net.cn

#ifndef X_H
来源：http://tg.chemitech.net.cn

#define X_H
来源：http://rw.9csxet.cn

#endif
来源：http://vi.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ul.shtwfgs.cn

#include <iostream>
来源：http://by.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://gr.asd995.cn

[S32] C++：字符串
来源：http://cq.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://cz.shtwfgs.cn

[S33] C++：vector 增删
来源：http://by.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xp.newstarts.cn

[S34] C++：遍历 vector
来源：http://sl.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://gb.bookmarksfly.cn

[S35] C++：map
来源：http://md.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://er.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://fv.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gc.wgjwhj.cn

[S37] C++：set
来源：http://yq.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://at.bookmarksfly.cn

[S38] C++：排序
来源：http://tn.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://zp.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://up.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lr.muxihuayi.cn

[S40] C++：查找元素
来源：http://iu.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ab.hnjuh.cn

[S41] C++：类与构造函数
来源：http://wd.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xw.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://yb.521024.cn

class B : public Base { public: void f() override {} };
来源：http://cv.huixiangedu.cn

[S43] C++：智能指针
来源：http://tc.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://pr.nszjky.cn

[S44] C++：引用传参
来源：http://ei.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://pd.chemitech.net.cn

[S45] C++：lambda
来源：http://ao.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yo.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://bi.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zu.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://xt.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jt.nszjky.cn

[S48] C++：逐行读文件
来源：http://ky.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://da.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://rj.shtwfgs.cn

[S49] C++：写文件
来源：http://zk.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cj.szsharing.cn

[S50] C++：格式化数字
来源：http://ws.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eh.hnjuh.cn

[S51] C++：显式类型转换
来源：http://mi.asd995.cn

static_cast<double>(a) / b
来源：http://wh.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://lc.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://qs.szsharing.cn

[S53] C++：移动语义
来源：http://ch.521024.cn

std::vector<int> w = std::move(v);
来源：http://up.muxihuayi.cn

[S54] C++：异常处理
来源：http://wd.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pk.asd995.cn

[S55] C++：结构化绑定
来源：http://rw.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://er.szsharing.cn

[S56] C++：optional
来源：http://fx.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tz.9csxet.cn

[S57] C++：编译期常量
来源：http://jl.huixiangedu.cn

constexpr int N = 10;
来源：http://nv.newstarts.cn

[S58] C++：命名空间
来源：http://ta.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://cl.huixiangedu.cn

[S59] C++：静态断言
来源：http://hd.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ha.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://jx.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ft.colortex.cn

================================================================================
来源：http://xj.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://re.chemitech.net.cn

================================================================================
来源：http://xu.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://ca.huixiangedu.cn

println("Hello")
来源：http://en.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://dp.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://md.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://vz.shtwfgs.cn

"值: $b"
来源：http://nz.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://uh.huanxung.cn

val n: String? = null;  n?.length
来源：http://uh.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://lw.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mj.nszjky.cn

[T06] Kotlin：集合映射
来源：http://zi.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://og.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://dy.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bn.9csxet.cn

[T08] Kotlin：数据类
来源：http://kx.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://ds.colortex.cn

[T09] Kotlin：扩展函数
来源：http://nx.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://qk.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://md.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bw.gzmigu.cn

[T11] Kotlin：协程
来源：http://hr.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://id.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://nt.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://sw.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://tq.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://yd.bjjhwx.cn

[T14] Kotlin：循环
来源：http://ei.colortex.cn

for (i in 1..10) println(i)
来源：http://ah.nszjky.cn

[T15] Kotlin：接口
来源：http://mo.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://jh.yuexingan06.cn

[T16] Swift：Hello World
来源：http://mp.lnxyls.cn

print("Hello")
来源：http://aj.newstarts.cn

[T17] Swift：变量与常量
来源：http://nb.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ko.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://zg.shtwfgs.cn

"值: \(b)"
来源：http://oo.nszjky.cn

[T19] Swift：可选绑定
来源：http://is.asd995.cn

if let n = opt { print(n) }
来源：http://ej.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://qp.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jj.yuexingan06.cn

[T21] Swift：遍历
来源：http://hj.huanxung.cn

for x in a { print(x) }
来源：http://pc.nicolike.cn

[T22] Swift：字典
来源：http://kq.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wf.jianghongdianzi.cn

[T23] Swift：函数
来源：http://rr.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ng.yuexingan06.cn

[T24] Swift：闭包
来源：http://ip.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gi.bookmarksfly.cn

[T25] Swift：结构体
来源：http://ge.lnxyls.cn

struct P { var x: Int }
来源：http://ti.newstarts.cn

[T26] Swift：类与重写
来源：http://sz.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://ep.szsharing.cn

[T27] Swift：错误处理
来源：http://ts.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://ve.huanxung.cn

[T28] Swift：枚举
来源：http://ag.nszjky.cn

enum Color { case red, green }
来源：http://pm.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://ba.szxytkj.cn

guard let x = opt else { return }
来源：http://ao.9csxet.cn

[T30] Swift：协议
来源：http://io.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://nd.hnjuh.cn

[T31] Lua：Hello World
来源：http://bg.hahajie.cn

print("Hello")
来源：http://ee.szxytkj.cn

[T32] Lua：局部变量
来源：http://wr.huixinmuqiang.cn

local a = 1
来源：http://sw.szxytkj.cn

[T33] Lua：表（数组）
来源：http://rs.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rs.hahajie.cn

[T34] Lua：遍历表
来源：http://oe.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lt.9csxet.cn

[T35] Lua：字典表
来源：http://ce.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://md.colortex.cn

[T36] Lua：函数
来源：http://jh.muxihuayi.cn

function add(a, b) return a + b end
来源：http://ap.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://zm.asd995.cn

"a" .. "b"
来源：http://mt.panjiajie.cn

[T38] Lua：条件
来源：http://ol.shxzskj.cn

if x > 0 then print("正") end
来源：http://qx.lnxyls.cn

[T39] Lua：模式匹配
来源：http://qk.newstarts.cn

string.find(s, "%d+")
来源：http://gu.9csxet.cn

[T40] Lua：元表
来源：http://fi.newstarts.cn

setmetatable({}, { __index = base })
来源：http://gv.shtwfgs.cn

[T41] Perl：Hello World
来源：http://hk.muxihuayi.cn

print "Hello\n";
来源：http://mz.hahajie.cn

[T42] Perl：变量类型
来源：http://kg.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vf.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://wk.nszjky.cn

"值: $a"
来源：http://sq.yuntaijiaju.cn

[T44] Perl：条件
来源：http://dd.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://be.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://ct.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://hk.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://rh.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fb.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://na.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lt.colortex.cn

[T48] Perl：正则替换
来源：http://uv.colortex.cn

$s =~ s/old/new/g;
来源：http://bj.gzmigu.cn

[T49] Perl：函数
来源：http://cq.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://de.521024.cn

[T50] Perl：逐行读文件
来源：http://pm.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://te.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://bh.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://hv.bookmarksfly.cn

println("Hello")
来源：http://wq.yuexingan06.cn

[T52] Scala：变量
来源：http://dx.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://hk.hahajie.cn

[T53] Scala：字符串插值
来源：http://ro.hahajie.cn

s"值: $b"
来源：http://dw.huixiangedu.cn

[T54] Scala：集合映射
来源：http://nu.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://in.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://ay.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ue.521024.cn

[T56] Scala：样例类
来源：http://wm.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://xt.szsharing.cn

[T57] Scala：模式匹配
来源：http://pk.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xe.colortex.cn

[T58] Scala：函数定义
来源：http://xd.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ul.9csxet.cn

[T59] Scala：循环
来源：http://yc.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://jl.newstarts.cn

[T60] Scala：折叠
来源：http://ip.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hh.hnjuh.cn

================================================================================
来源：http://zh.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://na.yuexingan06.cn

================================================================================
来源：http://dj.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://xp.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rd.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://lz.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nn.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://ru.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nj.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://wk.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://av.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://bk.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://vt.asd995.cn

[U06] Py：合并两个字典
来源：http://bj.lnxyls.cn

{**a, **b}
来源：http://uo.shtwfgs.cn


<!-- 参考信息 -->