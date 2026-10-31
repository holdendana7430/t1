代发 wailian999

openssl rand -hex 16
来源：http://aw.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://ft.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mp.nszjky.cn

[R69] 生成随机密码
来源：http://cr.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://kx.lnxyls.cn

[R70] 时间戳与互转
来源：http://rx.nicolike.cn

date +%s;  date -d @1700000000
来源：http://in.nicolike.cn

[R71] 日期格式化
来源：http://hc.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yv.nicolike.cn

[R72] 等待端口就绪
来源：http://bw.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://he.yuexingan06.cn

[R73] 分割大日志
来源：http://tu.nszjky.cn

split -l 1000 big.log part_
来源：http://bo.lnxyls.cn

[R74] 批量重命名
来源：http://tq.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hu.haigaiapp.cn

[R75] 导出环境变量
来源：http://wc.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://cu.asd995.cn

[R76] 使用临时文件
来源：http://zq.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pw.nicolike.cn

[R77] 读取用户输入
来源：http://uj.shxzskj.cn

read -rp "请输入: " ans
来源：http://rz.hnjuh.cn

[R78] 交互式菜单
来源：http://yx.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nr.wgjwhj.cn

[R79] 解析命令行选项
来源：http://tu.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yh.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://ny.asd995.cn

time ./run.sh
来源：http://ay.nszjky.cn

================================================================================
来源：http://qv.hnjuh.cn

S. C / C++ 专题
来源：http://en.jctech888.com.cn

================================================================================
来源：http://oq.jianghongdianzi.cn

[S01] C：Hello World
来源：http://ts.lnxyls.cn

#include <stdio.h>
来源：http://kz.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rv.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://vd.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://or.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ms.huanxung.cn

int x; scanf("%d", &x);
来源：http://sn.newstarts.cn

[S04] C：字符串复制
来源：http://ug.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bv.muxihuayi.cn

[S05] C：字符串长度
来源：http://oi.nicolike.cn

strlen(s)
来源：http://gf.hnjuh.cn

[S06] C：字符串比较
来源：http://zv.panjiajie.cn

strcmp(a, b) == 0
来源：http://wl.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://oz.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bj.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://ci.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tz.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://te.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oi.gzmigu.cn

[S10] C：指针与解引用
来源：http://nw.hahajie.cn

int *p = &a;  *p = 5;
来源：http://nf.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://cf.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ti.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yt.hahajie.cn

fclose(f);
来源：http://iy.nicolike.cn

[S12] C：写文件
来源：http://at.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://er.wgjwhj.cn

[S13] C：宏定义
来源：http://cf.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zc.yuexingan06.cn

[S14] C：枚举
来源：http://cl.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://fb.shxzskj.cn

[S15] C：类型转换
来源：http://ak.shxzukj.cn

(double) a / b
来源：http://jq.colortex.cn

[S16] C：位操作置位
来源：http://ug.yuntaijiaju.cn

x |= (1 << 3);
来源：http://am.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://jv.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pk.chemitech.net.cn

[S18] C：命令行参数
来源：http://tc.gzmigu.cn

int main(int argc, char **argv)
来源：http://fv.szsharing.cn

[S19] C：快速排序
来源：http://no.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://op.shtwfgs.cn

[S20] C：二分查找
来源：http://za.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ni.nszjky.cn

[S21] C：字符类别判断
来源：http://iq.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qv.nszjky.cn

[S22] C：字符串转数字
来源：http://jd.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uy.hahajie.cn

[S23] C：随机数
来源：http://fb.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iy.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://tw.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iv.asd995.cn

[S25] C：内存拷贝
来源：http://dg.colortex.cn

memcpy(dst, src, n);
来源：http://oy.nszjky.cn

[S26] C：内存清零
来源：http://pg.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://ei.bookmarksfly.cn

[S27] C：定义常量
来源：http://fb.bjjhwx.cn

const double PI = 3.14159;
来源：http://wl.gzmigu.cn

[S28] C：静态变量
来源：http://ga.shxzskj.cn

static int counter = 0;
来源：http://pu.wgjwhj.cn

[S29] C：变参函数
来源：http://yu.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ed.wgjwhj.cn

[S30] C：头文件保护
来源：http://ee.gzmigu.cn

#ifndef X_H
来源：http://aq.asd995.cn

#define X_H
来源：http://mu.jianghongdianzi.cn

#endif
来源：http://tz.nszjky.cn

[S31] C++：Hello World
来源：http://jj.gzmigu.cn

#include <iostream>
来源：http://qt.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://sd.haigaiapp.cn

[S32] C++：字符串
来源：http://fr.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://qm.szxytkj.cn

[S33] C++：vector 增删
来源：http://cb.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ap.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://uo.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://fi.panjiajie.cn

[S35] C++：map
来源：http://ix.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gr.huixiangedu.cn

[S36] C++：unordered_map
来源：http://sh.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dm.9csxet.cn

[S37] C++：set
来源：http://cq.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zg.yuntaijiaju.cn

[S38] C++：排序
来源：http://we.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://di.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://xs.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ha.newstarts.cn

[S40] C++：查找元素
来源：http://hm.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uw.nicolike.cn

[S41] C++：类与构造函数
来源：http://ii.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pj.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://gz.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://zy.lnxyls.cn

[S43] C++：智能指针
来源：http://yb.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ou.nicolike.cn

[S44] C++：引用传参
来源：http://vj.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://xp.yuntaijiaju.cn

[S45] C++：lambda
来源：http://gv.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://md.huanxung.cn

[S46] C++：函数模板
来源：http://jk.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bt.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://ws.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pl.szxytkj.cn

[S48] C++：逐行读文件
来源：http://za.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kg.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://ee.muxihuayi.cn

[S49] C++：写文件
来源：http://uy.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vv.shxzukj.cn

[S50] C++：格式化数字
来源：http://zb.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lz.nszjky.cn

[S51] C++：显式类型转换
来源：http://yb.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://ib.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://ba.newstarts.cn

int size() const noexcept { return n_; }
来源：http://cv.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://jl.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://xj.gzmigu.cn

[S54] C++：异常处理
来源：http://ba.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aj.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://kv.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ak.jctech888.com.cn

[S56] C++：optional
来源：http://vn.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pq.nszjky.cn

[S57] C++：编译期常量
来源：http://cu.521024.cn

constexpr int N = 10;
来源：http://fw.bookmarksfly.cn

[S58] C++：命名空间
来源：http://eb.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://dm.hnjuh.cn

[S59] C++：静态断言
来源：http://ko.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://th.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://lr.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kc.lnxyls.cn

================================================================================
来源：http://mj.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://np.shtwfgs.cn

================================================================================
来源：http://bf.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://wl.huixiangedu.cn

println("Hello")
来源：http://zf.9csxet.cn

[T02] Kotlin：变量
来源：http://wk.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://td.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://sr.huixinmuqiang.cn

"值: $b"
来源：http://eb.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://fu.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://gb.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://ot.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ac.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://mf.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wk.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://sf.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iq.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://sm.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://lg.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://nz.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://nb.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://cq.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rx.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://fu.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hq.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://li.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://ut.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://lr.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://wx.9csxet.cn

[T14] Kotlin：循环
来源：http://ao.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://dz.9csxet.cn

[T15] Kotlin：接口
来源：http://sg.newstarts.cn

interface Shape { fun area(): Double }
来源：http://jh.muxihuayi.cn

[T16] Swift：Hello World
来源：http://kk.shxzskj.cn

print("Hello")
来源：http://pr.huanxung.cn

[T17] Swift：变量与常量
来源：http://ud.gzmigu.cn

var a = 1;  let b = 2
来源：http://rx.panjiajie.cn

[T18] Swift：字符串插值
来源：http://sp.nicolike.cn

"值: \(b)"
来源：http://ij.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://yc.nszjky.cn

if let n = opt { print(n) }
来源：http://vm.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://io.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mm.haigaiapp.cn

[T21] Swift：遍历
来源：http://ri.szsharing.cn

for x in a { print(x) }
来源：http://bp.nicolike.cn

[T22] Swift：字典
来源：http://pl.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vq.szsharing.cn

[T23] Swift：函数
来源：http://hy.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://we.szxytkj.cn

[T24] Swift：闭包
来源：http://uo.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jw.panjiajie.cn

[T25] Swift：结构体
来源：http://ho.shxzskj.cn

struct P { var x: Int }
来源：http://tq.colortex.cn

[T26] Swift：类与重写
来源：http://zd.asd995.cn

class A: Base { override func f() {} }
来源：http://un.bjjhwx.cn

[T27] Swift：错误处理
来源：http://fq.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://bk.gzmigu.cn

[T28] Swift：枚举
来源：http://bi.szsharing.cn

enum Color { case red, green }
来源：http://vy.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://dg.szsharing.cn

guard let x = opt else { return }
来源：http://qf.colortex.cn

[T30] Swift：协议
来源：http://as.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://ai.szxytkj.cn

[T31] Lua：Hello World
来源：http://xt.wgjwhj.cn

print("Hello")
来源：http://um.shxzukj.cn

[T32] Lua：局部变量
来源：http://aw.nicolike.cn

local a = 1
来源：http://am.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://ob.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fi.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://li.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nv.shtwfgs.cn

[T35] Lua：字典表
来源：http://hu.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://nf.szsharing.cn

[T36] Lua：函数
来源：http://ci.szxytkj.cn

function add(a, b) return a + b end
来源：http://pm.huanxung.cn

[T37] Lua：字符串拼接
来源：http://jm.521024.cn

"a" .. "b"
来源：http://ws.shxzskj.cn

[T38] Lua：条件
来源：http://sy.wgjwhj.cn

if x > 0 then print("正") end
来源：http://fj.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://ab.chemitech.net.cn

string.find(s, "%d+")
来源：http://qp.colortex.cn

[T40] Lua：元表
来源：http://ri.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://fb.muxihuayi.cn

[T41] Perl：Hello World
来源：http://zz.bookmarksfly.cn

print "Hello\n";
来源：http://ht.szxytkj.cn

[T42] Perl：变量类型
来源：http://wq.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cx.szsharing.cn

[T43] Perl：字符串插值
来源：http://dr.9csxet.cn

"值: $a"
来源：http://bz.jianghongdianzi.cn

[T44] Perl：条件
来源：http://gm.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://uo.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://bv.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://fe.lnxyls.cn

[T46] Perl：哈希操作
来源：http://qo.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vz.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ez.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kx.colortex.cn

[T48] Perl：正则替换
来源：http://hb.gzmigu.cn

$s =~ s/old/new/g;
来源：http://xt.521024.cn

[T49] Perl：函数
来源：http://ug.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fo.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://hf.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ch.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://cd.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://se.panjiajie.cn

println("Hello")
来源：http://tu.nicolike.cn

[T52] Scala：变量
来源：http://pk.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://ms.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://pc.521024.cn

s"值: $b"
来源：http://nu.shxzskj.cn

[T54] Scala：集合映射
来源：http://ae.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://dh.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://lg.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sm.asd995.cn

[T56] Scala：样例类
来源：http://co.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://vj.shxzskj.cn

[T57] Scala：模式匹配
来源：http://aq.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iw.jctech888.com.cn

[T58] Scala：函数定义
来源：http://hn.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ml.shxzukj.cn

[T59] Scala：循环
来源：http://oi.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://tb.wgjwhj.cn

[T60] Scala：折叠
来源：http://eg.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://br.bjjhwx.cn

================================================================================
来源：http://ki.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zp.jianghongdianzi.cn

================================================================================
来源：http://dw.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://yw.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wh.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://xv.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uj.colortex.cn

[U03] Py：加载 .env 配置
来源：http://oc.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wj.hnjuh.cn

[U04] Py：变量调试打印
来源：http://as.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tm.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://hd.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://jf.gzmigu.cn

[U06] Py：合并两个字典
来源：http://yn.bookmarksfly.cn

{**a, **b}
来源：http://az.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://uz.szsharing.cn

{v: k for k, v in d.items()}
来源：http://ks.newstarts.cn

[U08] Py：展平二维列表
来源：http://zl.521024.cn

[y for x in nested for y in x]
来源：http://ii.521024.cn


<!-- 参考信息 -->