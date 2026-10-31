代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://dq.hahajie.cn

[R70] 时间戳与互转
来源：http://ff.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://hm.huixiangedu.cn

[R71] 日期格式化
来源：http://oq.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wt.panjiajie.cn

[R72] 等待端口就绪
来源：http://dh.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qz.wgjwhj.cn

[R73] 分割大日志
来源：http://sc.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://ei.gzmigu.cn

[R74] 批量重命名
来源：http://sl.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tx.wgjwhj.cn

[R75] 导出环境变量
来源：http://ip.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://zq.nszjky.cn

[R76] 使用临时文件
来源：http://lf.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rd.521024.cn

[R77] 读取用户输入
来源：http://ju.asd995.cn

read -rp "请输入: " ans
来源：http://oy.panjiajie.cn

[R78] 交互式菜单
来源：http://ro.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eg.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://sp.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zj.asd995.cn

[R80] 查看脚本执行耗时
来源：http://xd.yuexingan06.cn

time ./run.sh
来源：http://in.jctech888.com.cn

================================================================================
来源：http://ir.huixiangedu.cn

S. C / C++ 专题
来源：http://ho.jianghongdianzi.cn

================================================================================
来源：http://ll.huixiangedu.cn

[S01] C：Hello World
来源：http://hu.9csxet.cn

#include <stdio.h>
来源：http://yx.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ez.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://qv.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://ci.huixiangedu.cn

[S03] C：读入整数
来源：http://df.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://fg.haigaiapp.cn

[S04] C：字符串复制
来源：http://hz.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fc.hnjuh.cn

[S05] C：字符串长度
来源：http://tf.haigaiapp.cn

strlen(s)
来源：http://dc.asd995.cn

[S06] C：字符串比较
来源：http://ec.521024.cn

strcmp(a, b) == 0
来源：http://jf.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://hz.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cr.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://rw.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nc.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://ad.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jj.muxihuayi.cn

[S10] C：指针与解引用
来源：http://nl.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://id.asd995.cn

[S11] C：逐行读文件
来源：http://ss.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://qo.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nj.hnjuh.cn

fclose(f);
来源：http://wx.lnxyls.cn

[S12] C：写文件
来源：http://wv.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vc.szxytkj.cn

[S13] C：宏定义
来源：http://hz.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://as.huixiangedu.cn

[S14] C：枚举
来源：http://lx.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://tx.yuntaijiaju.cn

[S15] C：类型转换
来源：http://vu.colortex.cn

(double) a / b
来源：http://nx.szxytkj.cn

[S16] C：位操作置位
来源：http://gm.asd995.cn

x |= (1 << 3);
来源：http://co.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://kk.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qv.shxzskj.cn

[S18] C：命令行参数
来源：http://cy.hahajie.cn

int main(int argc, char **argv)
来源：http://di.newstarts.cn

[S19] C：快速排序
来源：http://jc.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mt.shxzukj.cn

[S20] C：二分查找
来源：http://ck.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qi.gzmigu.cn

[S21] C：字符类别判断
来源：http://ll.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hj.lnxyls.cn

[S22] C：字符串转数字
来源：http://ii.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://og.colortex.cn

[S23] C：随机数
来源：http://xy.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rm.hnjuh.cn

[S24] C：获取本地时间
来源：http://dm.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tl.asd995.cn

[S25] C：内存拷贝
来源：http://ng.haigaiapp.cn

memcpy(dst, src, n);
来源：http://nm.bookmarksfly.cn

[S26] C：内存清零
来源：http://li.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ze.szsharing.cn

[S27] C：定义常量
来源：http://sn.haigaiapp.cn

const double PI = 3.14159;
来源：http://sy.newstarts.cn

[S28] C：静态变量
来源：http://mk.asd995.cn

static int counter = 0;
来源：http://fz.szxytkj.cn

[S29] C：变参函数
来源：http://zf.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://op.szxytkj.cn

[S30] C：头文件保护
来源：http://le.haigaiapp.cn

#ifndef X_H
来源：http://ir.wgjwhj.cn

#define X_H
来源：http://fb.newstarts.cn

#endif
来源：http://wb.chemitech.net.cn

[S31] C++：Hello World
来源：http://uj.newstarts.cn

#include <iostream>
来源：http://az.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ax.colortex.cn

[S32] C++：字符串
来源：http://xc.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://cr.jctech888.com.cn

[S33] C++：vector 增删
来源：http://yl.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ln.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://gr.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://dx.yuexingan06.cn

[S35] C++：map
来源：http://rg.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ie.colortex.cn

[S36] C++：unordered_map
来源：http://yq.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sj.bookmarksfly.cn

[S37] C++：set
来源：http://xq.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wr.haigaiapp.cn

[S38] C++：排序
来源：http://ex.521024.cn

std::sort(v.begin(), v.end());
来源：http://yf.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://qe.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bs.yuexingan06.cn

[S40] C++：查找元素
来源：http://sx.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hm.asd995.cn

[S41] C++：类与构造函数
来源：http://bc.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ii.hahajie.cn

[S42] C++：继承与虚函数
来源：http://xs.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://em.asd995.cn

[S43] C++：智能指针
来源：http://cy.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://sr.muxihuayi.cn

[S44] C++：引用传参
来源：http://fm.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://sz.hahajie.cn

[S45] C++：lambda
来源：http://vr.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://av.panjiajie.cn

[S46] C++：函数模板
来源：http://ob.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://je.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://bx.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zj.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://kd.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oh.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://aa.shxzskj.cn

[S49] C++：写文件
来源：http://ww.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ac.nicolike.cn

[S50] C++：格式化数字
来源：http://kn.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cv.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://qt.muxihuayi.cn

static_cast<double>(a) / b
来源：http://zc.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://uk.huanxung.cn

int size() const noexcept { return n_; }
来源：http://rr.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://lv.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://gu.huixiangedu.cn

[S54] C++：异常处理
来源：http://hb.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mx.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://vz.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rc.chemitech.net.cn

[S56] C++：optional
来源：http://rp.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://on.shxzukj.cn

[S57] C++：编译期常量
来源：http://zc.yuexingan06.cn

constexpr int N = 10;
来源：http://jp.muxihuayi.cn

[S58] C++：命名空间
来源：http://hm.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://qm.huanxung.cn

[S59] C++：静态断言
来源：http://xw.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vg.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://so.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://op.bjjhwx.cn

================================================================================
来源：http://fb.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tm.jianghongdianzi.cn

================================================================================
来源：http://al.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://fb.bookmarksfly.cn

println("Hello")
来源：http://en.nszjky.cn

[T02] Kotlin：变量
来源：http://he.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kd.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://ry.newstarts.cn

"值: $b"
来源：http://tv.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://wf.hnjuh.cn

val n: String? = null;  n?.length
来源：http://mn.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://mj.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lr.colortex.cn

[T06] Kotlin：集合映射
来源：http://fl.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eh.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ur.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xg.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://qv.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://bt.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://qh.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://ph.521024.cn

[T10] Kotlin：默认参数
来源：http://qn.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ys.lnxyls.cn

[T11] Kotlin：协程
来源：http://at.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vm.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://tc.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://hw.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://qk.szsharing.cn

val m = mapOf("a" to 1)
来源：http://hw.colortex.cn

[T14] Kotlin：循环
来源：http://yj.lnxyls.cn

for (i in 1..10) println(i)
来源：http://rm.gzmigu.cn

[T15] Kotlin：接口
来源：http://sv.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://mv.nicolike.cn

[T16] Swift：Hello World
来源：http://xb.colortex.cn

print("Hello")
来源：http://vw.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://to.hnjuh.cn

var a = 1;  let b = 2
来源：http://cq.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://vi.521024.cn

"值: \(b)"
来源：http://ls.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://df.lnxyls.cn

if let n = opt { print(n) }
来源：http://bm.colortex.cn

[T20] Swift：数组操作
来源：http://ch.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://km.jctech888.com.cn

[T21] Swift：遍历
来源：http://kf.nszjky.cn

for x in a { print(x) }
来源：http://ur.jianghongdianzi.cn

[T22] Swift：字典
来源：http://vp.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jz.bjjhwx.cn

[T23] Swift：函数
来源：http://ag.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kw.bookmarksfly.cn

[T24] Swift：闭包
来源：http://ap.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iz.szsharing.cn

[T25] Swift：结构体
来源：http://pk.wgjwhj.cn

struct P { var x: Int }
来源：http://jp.gzmigu.cn

[T26] Swift：类与重写
来源：http://ao.521024.cn

class A: Base { override func f() {} }
来源：http://qo.chemitech.net.cn

[T27] Swift：错误处理
来源：http://dg.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://tc.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://cv.lnxyls.cn

enum Color { case red, green }
来源：http://ip.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://om.hahajie.cn

guard let x = opt else { return }
来源：http://pk.huixinmuqiang.cn

[T30] Swift：协议
来源：http://sa.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://aa.shxzukj.cn

[T31] Lua：Hello World
来源：http://ws.nicolike.cn

print("Hello")
来源：http://ff.521024.cn

[T32] Lua：局部变量
来源：http://yr.asd995.cn

local a = 1
来源：http://py.asd995.cn

[T33] Lua：表（数组）
来源：http://mr.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ul.szxytkj.cn

[T34] Lua：遍历表
来源：http://ui.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gm.chemitech.net.cn

[T35] Lua：字典表
来源：http://ji.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://da.shxzukj.cn

[T36] Lua：函数
来源：http://ia.newstarts.cn

function add(a, b) return a + b end
来源：http://cc.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://su.nszjky.cn

"a" .. "b"
来源：http://rt.nicolike.cn

[T38] Lua：条件
来源：http://uz.bjjhwx.cn

if x > 0 then print("正") end
来源：http://yg.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://jp.wgjwhj.cn

string.find(s, "%d+")
来源：http://ao.huixinmuqiang.cn

[T40] Lua：元表
来源：http://ms.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://si.hahajie.cn

[T41] Perl：Hello World
来源：http://kl.gzmigu.cn

print "Hello\n";
来源：http://rs.huixiangedu.cn

[T42] Perl：变量类型
来源：http://by.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mw.lnxyls.cn

[T43] Perl：字符串插值
来源：http://yt.hnjuh.cn

"值: $a"
来源：http://ys.haigaiapp.cn

[T44] Perl：条件
来源：http://mh.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://eg.nicolike.cn

[T45] Perl：数组遍历
来源：http://hi.colortex.cn

for my $x (@arr) { print $x; }
来源：http://hv.hnjuh.cn

[T46] Perl：哈希操作
来源：http://zx.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rx.nszjky.cn

[T47] Perl：正则捕获
来源：http://wl.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ej.yuexingan06.cn

[T48] Perl：正则替换
来源：http://pk.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://jd.asd995.cn

[T49] Perl：函数
来源：http://jl.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ym.521024.cn

[T50] Perl：逐行读文件
来源：http://il.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ku.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://as.hnjuh.cn

[T51] Scala：Hello World
来源：http://fg.gzmigu.cn

println("Hello")
来源：http://bm.muxihuayi.cn

[T52] Scala：变量
来源：http://kn.huixiangedu.cn

val a = 1;  var b = 2
来源：http://by.gzmigu.cn

[T53] Scala：字符串插值
来源：http://zf.szsharing.cn

s"值: $b"
来源：http://yf.huixiangedu.cn

[T54] Scala：集合映射
来源：http://dl.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://qe.szsharing.cn

[T55] Scala：集合过滤
来源：http://jk.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ee.521024.cn

[T56] Scala：样例类
来源：http://jr.shxzskj.cn

case class User(name: String, age: Int)
来源：http://ff.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://hf.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vf.shxzskj.cn

[T58] Scala：函数定义
来源：http://ld.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ld.shxzukj.cn

[T59] Scala：循环
来源：http://oe.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://sx.panjiajie.cn

[T60] Scala：折叠
来源：http://rc.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ng.chemitech.net.cn

================================================================================
来源：http://ze.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sg.huixiangedu.cn

================================================================================
来源：http://gh.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://ud.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wr.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://ra.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qg.colortex.cn

[U03] Py：加载 .env 配置
来源：http://zc.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cv.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://nn.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fv.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://xp.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://pt.521024.cn

[U06] Py：合并两个字典
来源：http://df.lnxyls.cn

{**a, **b}
来源：http://ce.szxytkj.cn

[U07] Py：反转字典键值
来源：http://af.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://wf.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://nl.huanxung.cn

[y for x in nested for y in x]
来源：http://nh.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://rf.huanxung.cn

max(d, key=d.get)
来源：http://yg.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://qr.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vf.521024.cn


<!-- 参考信息 -->