代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://yv.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://bn.newstarts.cn

date +%s;  date -d @1700000000
来源：http://lr.szsharing.cn

[R71] 日期格式化
来源：http://lh.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ms.nszjky.cn

[R72] 等待端口就绪
来源：http://an.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ab.szsharing.cn

[R73] 分割大日志
来源：http://aw.chemitech.net.cn

split -l 1000 big.log part_
来源：http://bj.hnjuh.cn

[R74] 批量重命名
来源：http://tl.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wp.muxihuayi.cn

[R75] 导出环境变量
来源：http://nt.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://xl.bjjhwx.cn

[R76] 使用临时文件
来源：http://tg.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lx.gzmigu.cn

[R77] 读取用户输入
来源：http://ia.asd995.cn

read -rp "请输入: " ans
来源：http://bs.gzmigu.cn

[R78] 交互式菜单
来源：http://cg.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dq.muxihuayi.cn

[R79] 解析命令行选项
来源：http://te.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wm.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://cr.shxzskj.cn

time ./run.sh
来源：http://hf.jianghongdianzi.cn

================================================================================
来源：http://ue.gzmigu.cn

S. C / C++ 专题
来源：http://ag.panjiajie.cn

================================================================================
来源：http://cr.jianghongdianzi.cn

[S01] C：Hello World
来源：http://cp.huanxung.cn

#include <stdio.h>
来源：http://uh.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://za.hahajie.cn

[S02] C：变量与格式化输出
来源：http://nf.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://ge.shxzukj.cn

[S03] C：读入整数
来源：http://pg.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://qr.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://se.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ke.szsharing.cn

[S05] C：字符串长度
来源：http://xg.newstarts.cn

strlen(s)
来源：http://or.yuexingan06.cn

[S06] C：字符串比较
来源：http://ue.panjiajie.cn

strcmp(a, b) == 0
来源：http://un.newstarts.cn

[S07] C：数组遍历求和
来源：http://sd.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yw.colortex.cn

[S08] C：动态内存分配与释放
来源：http://nf.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oq.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://mz.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sw.wgjwhj.cn

[S10] C：指针与解引用
来源：http://js.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://wn.9csxet.cn

[S11] C：逐行读文件
来源：http://cv.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://lp.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://to.wgjwhj.cn

fclose(f);
来源：http://ql.gzmigu.cn

[S12] C：写文件
来源：http://ls.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://je.nicolike.cn

[S13] C：宏定义
来源：http://se.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dt.hahajie.cn

[S14] C：枚举
来源：http://mc.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://fv.shxzukj.cn

[S15] C：类型转换
来源：http://bi.bookmarksfly.cn

(double) a / b
来源：http://ai.huanxung.cn

[S16] C：位操作置位
来源：http://uh.nszjky.cn

x |= (1 << 3);
来源：http://tt.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://wl.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ox.asd995.cn

[S18] C：命令行参数
来源：http://mz.jctech888.com.cn

int main(int argc, char **argv)
来源：http://ia.newstarts.cn

[S19] C：快速排序
来源：http://ps.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bx.bookmarksfly.cn

[S20] C：二分查找
来源：http://fz.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ue.shxzukj.cn

[S21] C：字符类别判断
来源：http://hg.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bf.asd995.cn

[S22] C：字符串转数字
来源：http://ch.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tc.wgjwhj.cn

[S23] C：随机数
来源：http://sg.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tl.colortex.cn

[S24] C：获取本地时间
来源：http://bs.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fi.shtwfgs.cn

[S25] C：内存拷贝
来源：http://of.chemitech.net.cn

memcpy(dst, src, n);
来源：http://hf.haigaiapp.cn

[S26] C：内存清零
来源：http://rv.szsharing.cn

memset(a, 0, sizeof a);
来源：http://ui.shxzskj.cn

[S27] C：定义常量
来源：http://pg.yuexingan06.cn

const double PI = 3.14159;
来源：http://yg.chemitech.net.cn

[S28] C：静态变量
来源：http://uc.9csxet.cn

static int counter = 0;
来源：http://at.wgjwhj.cn

[S29] C：变参函数
来源：http://dn.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dh.wgjwhj.cn

[S30] C：头文件保护
来源：http://fj.jctech888.com.cn

#ifndef X_H
来源：http://pz.yuntaijiaju.cn

#define X_H
来源：http://kw.9csxet.cn

#endif
来源：http://js.nszjky.cn

[S31] C++：Hello World
来源：http://qn.nszjky.cn

#include <iostream>
来源：http://vr.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://jj.lnxyls.cn

[S32] C++：字符串
来源：http://hv.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://qy.hnjuh.cn

[S33] C++：vector 增删
来源：http://yh.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mk.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://vj.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://tr.nicolike.cn

[S35] C++：map
来源：http://se.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wx.asd995.cn

[S36] C++：unordered_map
来源：http://vs.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kp.gzmigu.cn

[S37] C++：set
来源：http://ft.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hj.jianghongdianzi.cn

[S38] C++：排序
来源：http://wx.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://sc.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://xn.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kb.szsharing.cn

[S40] C++：查找元素
来源：http://en.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jy.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://ve.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oq.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://ti.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://iv.521024.cn

[S43] C++：智能指针
来源：http://qz.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://kg.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://wb.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://ys.shxzskj.cn

[S45] C++：lambda
来源：http://ij.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jo.huanxung.cn

[S46] C++：函数模板
来源：http://hm.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ir.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://tq.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qf.shxzskj.cn

[S48] C++：逐行读文件
来源：http://ic.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kb.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://ei.gzmigu.cn

[S49] C++：写文件
来源：http://vg.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ym.jctech888.com.cn

[S50] C++：格式化数字
来源：http://hf.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ke.nicolike.cn

[S51] C++：显式类型转换
来源：http://mv.shtwfgs.cn

static_cast<double>(a) / b
来源：http://el.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ea.nszjky.cn

int size() const noexcept { return n_; }
来源：http://vd.lnxyls.cn

[S53] C++：移动语义
来源：http://pe.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://nn.huanxung.cn

[S54] C++：异常处理
来源：http://rj.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jj.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://tr.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bh.wgjwhj.cn

[S56] C++：optional
来源：http://ah.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qp.shxzskj.cn

[S57] C++：编译期常量
来源：http://an.nicolike.cn

constexpr int N = 10;
来源：http://bb.yuexingan06.cn

[S58] C++：命名空间
来源：http://km.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://sq.wgjwhj.cn

[S59] C++：静态断言
来源：http://ji.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ex.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://zl.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://er.colortex.cn

================================================================================
来源：http://hs.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yl.bookmarksfly.cn

================================================================================
来源：http://ps.asd995.cn

[T01] Kotlin：Hello World
来源：http://nq.gzmigu.cn

println("Hello")
来源：http://pd.nicolike.cn

[T02] Kotlin：变量
来源：http://cq.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dn.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://bz.wgjwhj.cn

"值: $b"
来源：http://yp.panjiajie.cn

[T04] Kotlin：空安全
来源：http://ah.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://ve.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://hp.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ps.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://np.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eu.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://ne.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://er.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://pn.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://wl.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://zf.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://tk.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://mi.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jz.haigaiapp.cn

[T11] Kotlin：协程
来源：http://gt.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rj.szsharing.cn

[T12] Kotlin：解构声明
来源：http://xw.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://ld.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://mt.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://mv.wgjwhj.cn

[T14] Kotlin：循环
来源：http://jn.huanxung.cn

for (i in 1..10) println(i)
来源：http://kq.haigaiapp.cn

[T15] Kotlin：接口
来源：http://dq.nszjky.cn

interface Shape { fun area(): Double }
来源：http://kc.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://cm.haigaiapp.cn

print("Hello")
来源：http://jl.521024.cn

[T17] Swift：变量与常量
来源：http://gl.9csxet.cn

var a = 1;  let b = 2
来源：http://as.9csxet.cn

[T18] Swift：字符串插值
来源：http://fk.shtwfgs.cn

"值: \(b)"
来源：http://yf.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://gr.521024.cn

if let n = opt { print(n) }
来源：http://hy.haigaiapp.cn

[T20] Swift：数组操作
来源：http://bd.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ag.shtwfgs.cn

[T21] Swift：遍历
来源：http://hj.shtwfgs.cn

for x in a { print(x) }
来源：http://tx.huixinmuqiang.cn

[T22] Swift：字典
来源：http://ti.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sd.jctech888.com.cn

[T23] Swift：函数
来源：http://ir.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cz.szsharing.cn

[T24] Swift：闭包
来源：http://el.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cz.colortex.cn

[T25] Swift：结构体
来源：http://jl.szsharing.cn

struct P { var x: Int }
来源：http://gj.shxzukj.cn

[T26] Swift：类与重写
来源：http://fx.9csxet.cn

class A: Base { override func f() {} }
来源：http://my.bjjhwx.cn

[T27] Swift：错误处理
来源：http://xm.colortex.cn

do { try f() } catch { print(error) }
来源：http://gt.shxzskj.cn

[T28] Swift：枚举
来源：http://rp.huixinmuqiang.cn

enum Color { case red, green }
来源：http://sb.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://ax.hahajie.cn

guard let x = opt else { return }
来源：http://jt.yuntaijiaju.cn

[T30] Swift：协议
来源：http://my.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://bi.gzmigu.cn

[T31] Lua：Hello World
来源：http://fs.bookmarksfly.cn

print("Hello")
来源：http://fj.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://pb.nszjky.cn

local a = 1
来源：http://vj.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://xo.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vh.szxytkj.cn

[T34] Lua：遍历表
来源：http://qf.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xa.hahajie.cn

[T35] Lua：字典表
来源：http://gg.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://nr.nszjky.cn

[T36] Lua：函数
来源：http://sr.huanxung.cn

function add(a, b) return a + b end
来源：http://lr.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://su.haigaiapp.cn

"a" .. "b"
来源：http://hl.huixinmuqiang.cn

[T38] Lua：条件
来源：http://vq.haigaiapp.cn

if x > 0 then print("正") end
来源：http://lv.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://nw.bookmarksfly.cn

string.find(s, "%d+")
来源：http://ww.szsharing.cn

[T40] Lua：元表
来源：http://ld.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://vf.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://ww.gzmigu.cn

print "Hello\n";
来源：http://ik.muxihuayi.cn

[T42] Perl：变量类型
来源：http://ae.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uw.newstarts.cn

[T43] Perl：字符串插值
来源：http://by.yuntaijiaju.cn

"值: $a"
来源：http://av.521024.cn

[T44] Perl：条件
来源：http://dk.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://vg.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://er.asd995.cn

for my $x (@arr) { print $x; }
来源：http://rc.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://qc.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qx.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://lf.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qm.muxihuayi.cn

[T48] Perl：正则替换
来源：http://ca.hahajie.cn

$s =~ s/old/new/g;
来源：http://lw.jctech888.com.cn

[T49] Perl：函数
来源：http://my.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ik.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://vr.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lz.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://nd.shtwfgs.cn

[T51] Scala：Hello World
来源：http://fl.521024.cn

println("Hello")
来源：http://il.gzmigu.cn

[T52] Scala：变量
来源：http://qo.shtwfgs.cn

val a = 1;  var b = 2
来源：http://rr.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://he.9csxet.cn

s"值: $b"
来源：http://is.nicolike.cn

[T54] Scala：集合映射
来源：http://mh.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://ch.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://ev.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sg.hnjuh.cn

[T56] Scala：样例类
来源：http://pb.panjiajie.cn

case class User(name: String, age: Int)
来源：http://fu.hahajie.cn

[T57] Scala：模式匹配
来源：http://ur.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gn.chemitech.net.cn

[T58] Scala：函数定义
来源：http://bd.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nc.shxzskj.cn

[T59] Scala：循环
来源：http://ln.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://bx.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://et.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ak.shtwfgs.cn

================================================================================
来源：http://kl.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://em.szxytkj.cn

================================================================================
来源：http://gi.panjiajie.cn

[U01] Py：创建虚拟环境
来源：http://cd.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iq.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://ir.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ug.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://mk.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sa.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://xx.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sa.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://mn.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://pr.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://ma.shxzskj.cn

{**a, **b}
来源：http://rc.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://oe.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://ai.shxzskj.cn

[U08] Py：展平二维列表
来源：http://pi.huixiangedu.cn

[y for x in nested for y in x]
来源：http://ml.521024.cn

[U09] Py：字典取最大值的键
来源：http://sv.colortex.cn

max(d, key=d.get)
来源：http://hs.huanxung.cn

[U10] Py：按值排序字典
来源：http://wn.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nz.shtwfgs.cn


<!-- 参考信息 -->