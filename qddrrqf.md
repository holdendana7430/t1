代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://nr.bjjhwx.cn

[R70] 时间戳与互转
来源：http://ea.hahajie.cn

date +%s;  date -d @1700000000
来源：http://tw.jctech888.com.cn

[R71] 日期格式化
来源：http://fh.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eo.szxytkj.cn

[R72] 等待端口就绪
来源：http://ih.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nx.szxytkj.cn

[R73] 分割大日志
来源：http://kx.lnxyls.cn

split -l 1000 big.log part_
来源：http://ho.huixinmuqiang.cn

[R74] 批量重命名
来源：http://nw.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wp.bookmarksfly.cn

[R75] 导出环境变量
来源：http://px.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://pr.newstarts.cn

[R76] 使用临时文件
来源：http://cz.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sv.colortex.cn

[R77] 读取用户输入
来源：http://kq.9csxet.cn

read -rp "请输入: " ans
来源：http://ur.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://qg.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dj.huanxung.cn

[R79] 解析命令行选项
来源：http://jk.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yy.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://tp.9csxet.cn

time ./run.sh
来源：http://tb.colortex.cn

================================================================================
来源：http://ef.jctech888.com.cn

S. C / C++ 专题
来源：http://cd.huanxung.cn

================================================================================
来源：http://xm.hnjuh.cn

[S01] C：Hello World
来源：http://le.nicolike.cn

#include <stdio.h>
来源：http://cq.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fi.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://av.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://hw.jianghongdianzi.cn

[S03] C：读入整数
来源：http://kf.521024.cn

int x; scanf("%d", &x);
来源：http://qv.bookmarksfly.cn

[S04] C：字符串复制
来源：http://wd.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mg.hnjuh.cn

[S05] C：字符串长度
来源：http://fo.colortex.cn

strlen(s)
来源：http://ji.panjiajie.cn

[S06] C：字符串比较
来源：http://eb.bjjhwx.cn

strcmp(a, b) == 0
来源：http://dd.szsharing.cn

[S07] C：数组遍历求和
来源：http://un.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rb.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://bq.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cl.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://wc.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mx.wgjwhj.cn

[S10] C：指针与解引用
来源：http://iu.szsharing.cn

int *p = &a;  *p = 5;
来源：http://zp.nicolike.cn

[S11] C：逐行读文件
来源：http://iw.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ij.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oq.szsharing.cn

fclose(f);
来源：http://ut.huixiangedu.cn

[S12] C：写文件
来源：http://ul.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vw.huixinmuqiang.cn

[S13] C：宏定义
来源：http://tl.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tc.asd995.cn

[S14] C：枚举
来源：http://pw.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://mg.shxzskj.cn

[S15] C：类型转换
来源：http://dn.shxzukj.cn

(double) a / b
来源：http://dy.shxzskj.cn

[S16] C：位操作置位
来源：http://qv.nszjky.cn

x |= (1 << 3);
来源：http://gd.asd995.cn

[S17] C：安全拼接字符串
来源：http://tk.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kq.panjiajie.cn

[S18] C：命令行参数
来源：http://cw.9csxet.cn

int main(int argc, char **argv)
来源：http://lx.nszjky.cn

[S19] C：快速排序
来源：http://qd.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kr.szsharing.cn

[S20] C：二分查找
来源：http://km.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qo.gzmigu.cn

[S21] C：字符类别判断
来源：http://dl.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ss.521024.cn

[S22] C：字符串转数字
来源：http://ar.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kh.521024.cn

[S23] C：随机数
来源：http://uu.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://st.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://sp.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cx.haigaiapp.cn

[S25] C：内存拷贝
来源：http://ia.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://fl.muxihuayi.cn

[S26] C：内存清零
来源：http://pl.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://na.hnjuh.cn

[S27] C：定义常量
来源：http://fg.hahajie.cn

const double PI = 3.14159;
来源：http://qv.shtwfgs.cn

[S28] C：静态变量
来源：http://yx.hahajie.cn

static int counter = 0;
来源：http://jg.muxihuayi.cn

[S29] C：变参函数
来源：http://dx.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vh.asd995.cn

[S30] C：头文件保护
来源：http://jq.huixiangedu.cn

#ifndef X_H
来源：http://oe.hnjuh.cn

#define X_H
来源：http://lo.chemitech.net.cn

#endif
来源：http://xt.panjiajie.cn

[S31] C++：Hello World
来源：http://km.szxytkj.cn

#include <iostream>
来源：http://ir.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://bl.bookmarksfly.cn

[S32] C++：字符串
来源：http://rw.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://wr.shtwfgs.cn

[S33] C++：vector 增删
来源：http://td.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hu.szsharing.cn

[S34] C++：遍历 vector
来源：http://eh.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ow.shtwfgs.cn

[S35] C++：map
来源：http://rt.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ob.huanxung.cn

[S36] C++：unordered_map
来源：http://aa.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pp.lnxyls.cn

[S37] C++：set
来源：http://ac.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eu.nszjky.cn

[S38] C++：排序
来源：http://sv.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://ge.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://vq.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kr.huixiangedu.cn

[S40] C++：查找元素
来源：http://ad.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ja.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://yz.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pb.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://gm.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://am.muxihuayi.cn

[S43] C++：智能指针
来源：http://ej.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://nu.9csxet.cn

[S44] C++：引用传参
来源：http://qz.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://ku.haigaiapp.cn

[S45] C++：lambda
来源：http://ks.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://po.521024.cn

[S46] C++：函数模板
来源：http://jw.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pa.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://go.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cn.newstarts.cn

[S48] C++：逐行读文件
来源：http://im.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eq.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://cu.nicolike.cn

[S49] C++：写文件
来源：http://kx.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ge.colortex.cn

[S50] C++：格式化数字
来源：http://ll.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://la.colortex.cn

[S51] C++：显式类型转换
来源：http://oq.jctech888.com.cn

static_cast<double>(a) / b
来源：http://px.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://sg.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://gk.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://wk.colortex.cn

std::vector<int> w = std::move(v);
来源：http://nw.szxytkj.cn

[S54] C++：异常处理
来源：http://qn.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gi.nszjky.cn

[S55] C++：结构化绑定
来源：http://ze.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hf.gzmigu.cn

[S56] C++：optional
来源：http://lz.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zi.haigaiapp.cn

[S57] C++：编译期常量
来源：http://vr.asd995.cn

constexpr int N = 10;
来源：http://pv.lnxyls.cn

[S58] C++：命名空间
来源：http://mq.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://iq.muxihuayi.cn

[S59] C++：静态断言
来源：http://bu.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rb.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://uv.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ww.nicolike.cn

================================================================================
来源：http://wq.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iq.asd995.cn

================================================================================
来源：http://bt.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://gf.jianghongdianzi.cn

println("Hello")
来源：http://wn.yuexingan06.cn

[T02] Kotlin：变量
来源：http://bk.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ah.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://ia.shtwfgs.cn

"值: $b"
来源：http://vv.nicolike.cn

[T04] Kotlin：空安全
来源：http://pk.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://pl.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://xt.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ab.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ub.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xo.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://gn.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jr.szxytkj.cn

[T08] Kotlin：数据类
来源：http://qk.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://gg.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://uh.asd995.cn

fun String.exclaim() = this + "!"
来源：http://ka.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://sd.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jy.chemitech.net.cn

[T11] Kotlin：协程
来源：http://az.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fn.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://cp.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://if.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://ms.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://zt.szxytkj.cn

[T14] Kotlin：循环
来源：http://sg.nicolike.cn

for (i in 1..10) println(i)
来源：http://rm.chemitech.net.cn

[T15] Kotlin：接口
来源：http://cf.521024.cn

interface Shape { fun area(): Double }
来源：http://zs.yuexingan06.cn

[T16] Swift：Hello World
来源：http://ir.newstarts.cn

print("Hello")
来源：http://zl.hnjuh.cn

[T17] Swift：变量与常量
来源：http://bs.chemitech.net.cn

var a = 1;  let b = 2
来源：http://nf.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://zy.nicolike.cn

"值: \(b)"
来源：http://ph.gzmigu.cn

[T19] Swift：可选绑定
来源：http://zt.colortex.cn

if let n = opt { print(n) }
来源：http://jq.shtwfgs.cn

[T20] Swift：数组操作
来源：http://zr.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ja.lnxyls.cn

[T21] Swift：遍历
来源：http://sl.nicolike.cn

for x in a { print(x) }
来源：http://rc.panjiajie.cn

[T22] Swift：字典
来源：http://ci.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://px.hnjuh.cn

[T23] Swift：函数
来源：http://ep.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ky.nszjky.cn

[T24] Swift：闭包
来源：http://pp.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://il.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://qu.gzmigu.cn

struct P { var x: Int }
来源：http://pb.haigaiapp.cn

[T26] Swift：类与重写
来源：http://my.newstarts.cn

class A: Base { override func f() {} }
来源：http://mr.asd995.cn

[T27] Swift：错误处理
来源：http://jv.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://fd.bjjhwx.cn

[T28] Swift：枚举
来源：http://bh.szxytkj.cn

enum Color { case red, green }
来源：http://fc.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://hh.hnjuh.cn

guard let x = opt else { return }
来源：http://cb.huanxung.cn

[T30] Swift：协议
来源：http://fb.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://je.wgjwhj.cn

[T31] Lua：Hello World
来源：http://dd.asd995.cn

print("Hello")
来源：http://bu.521024.cn

[T32] Lua：局部变量
来源：http://nd.szxytkj.cn

local a = 1
来源：http://gy.9csxet.cn

[T33] Lua：表（数组）
来源：http://dr.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zm.shxzukj.cn

[T34] Lua：遍历表
来源：http://yf.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jm.bjjhwx.cn

[T35] Lua：字典表
来源：http://mc.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://wx.nicolike.cn

[T36] Lua：函数
来源：http://xc.521024.cn

function add(a, b) return a + b end
来源：http://rf.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://ru.hahajie.cn

"a" .. "b"
来源：http://yw.huixinmuqiang.cn

[T38] Lua：条件
来源：http://eu.gzmigu.cn

if x > 0 then print("正") end
来源：http://oi.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://pd.colortex.cn

string.find(s, "%d+")
来源：http://gk.nicolike.cn

[T40] Lua：元表
来源：http://hq.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://zj.haigaiapp.cn

[T41] Perl：Hello World
来源：http://gx.huanxung.cn

print "Hello\n";
来源：http://sz.asd995.cn

[T42] Perl：变量类型
来源：http://gj.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mg.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://vr.521024.cn

"值: $a"
来源：http://kd.asd995.cn

[T44] Perl：条件
来源：http://dt.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://aj.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://dj.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://mf.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://we.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hb.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ay.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hu.shxzukj.cn

[T48] Perl：正则替换
来源：http://jt.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://hr.shxzskj.cn

[T49] Perl：函数
来源：http://df.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xv.9csxet.cn

[T50] Perl：逐行读文件
来源：http://zp.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cu.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://lo.wgjwhj.cn

[T51] Scala：Hello World
来源：http://qu.yuntaijiaju.cn

println("Hello")
来源：http://ky.yuntaijiaju.cn

[T52] Scala：变量
来源：http://fg.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ut.newstarts.cn

[T53] Scala：字符串插值
来源：http://cv.huixiangedu.cn

s"值: $b"
来源：http://mo.bjjhwx.cn

[T54] Scala：集合映射
来源：http://vm.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://bd.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://ge.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ik.muxihuayi.cn

[T56] Scala：样例类
来源：http://er.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://xc.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://hb.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ra.chemitech.net.cn

[T58] Scala：函数定义
来源：http://ve.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rh.asd995.cn

[T59] Scala：循环
来源：http://lj.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://va.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://uv.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fc.bookmarksfly.cn

================================================================================
来源：http://qe.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ty.shxzskj.cn

================================================================================
来源：http://pl.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://fl.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pq.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://fh.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://br.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://gz.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qj.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://nv.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jn.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://hv.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://nu.panjiajie.cn

[U06] Py：合并两个字典
来源：http://nb.nicolike.cn

{**a, **b}
来源：http://ut.panjiajie.cn

[U07] Py：反转字典键值
来源：http://eb.hahajie.cn

{v: k for k, v in d.items()}
来源：http://da.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://af.shxzukj.cn

[y for x in nested for y in x]
来源：http://zd.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://pl.lnxyls.cn

max(d, key=d.get)
来源：http://qy.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://pp.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gt.huixiangedu.cn


<!-- 参考信息 -->