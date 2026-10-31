代发 wailian999

openssl rand -hex 16
来源：http://qt.521024.cn

[R68] 计算文件校验值
来源：http://mg.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://io.szsharing.cn

[R69] 生成随机密码
来源：http://tf.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://ik.shxzskj.cn

[R70] 时间戳与互转
来源：http://nc.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://rk.jctech888.com.cn

[R71] 日期格式化
来源：http://xi.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lx.nszjky.cn

[R72] 等待端口就绪
来源：http://mu.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ot.nicolike.cn

[R73] 分割大日志
来源：http://ij.gzmigu.cn

split -l 1000 big.log part_
来源：http://au.yuexingan06.cn

[R74] 批量重命名
来源：http://gf.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://il.nszjky.cn

[R75] 导出环境变量
来源：http://sc.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://ik.chemitech.net.cn

[R76] 使用临时文件
来源：http://mk.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ey.shxzskj.cn

[R77] 读取用户输入
来源：http://yl.9csxet.cn

read -rp "请输入: " ans
来源：http://ec.newstarts.cn

[R78] 交互式菜单
来源：http://xv.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ja.muxihuayi.cn

[R79] 解析命令行选项
来源：http://wr.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dv.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://iv.colortex.cn

time ./run.sh
来源：http://mq.nszjky.cn

================================================================================
来源：http://sw.9csxet.cn

S. C / C++ 专题
来源：http://sx.521024.cn

================================================================================
来源：http://jp.shtwfgs.cn

[S01] C：Hello World
来源：http://yb.hnjuh.cn

#include <stdio.h>
来源：http://bf.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tl.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ge.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://zb.shxzukj.cn

[S03] C：读入整数
来源：http://vf.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://lm.szxytkj.cn

[S04] C：字符串复制
来源：http://ko.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nt.huixiangedu.cn

[S05] C：字符串长度
来源：http://er.panjiajie.cn

strlen(s)
来源：http://px.521024.cn

[S06] C：字符串比较
来源：http://fs.9csxet.cn

strcmp(a, b) == 0
来源：http://tr.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://lc.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bm.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://gg.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fz.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://hi.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uw.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://yq.asd995.cn

int *p = &a;  *p = 5;
来源：http://nn.szsharing.cn

[S11] C：逐行读文件
来源：http://jh.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://vc.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rd.huixinmuqiang.cn

fclose(f);
来源：http://xg.521024.cn

[S12] C：写文件
来源：http://vt.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ar.szxytkj.cn

[S13] C：宏定义
来源：http://ye.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yp.9csxet.cn

[S14] C：枚举
来源：http://vr.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://oz.huixiangedu.cn

[S15] C：类型转换
来源：http://oo.huanxung.cn

(double) a / b
来源：http://ry.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://tr.hahajie.cn

x |= (1 << 3);
来源：http://uj.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://vy.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ej.shtwfgs.cn

[S18] C：命令行参数
来源：http://on.haigaiapp.cn

int main(int argc, char **argv)
来源：http://oh.shxzskj.cn

[S19] C：快速排序
来源：http://rx.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ep.muxihuayi.cn

[S20] C：二分查找
来源：http://zt.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lf.asd995.cn

[S21] C：字符类别判断
来源：http://jt.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rd.muxihuayi.cn

[S22] C：字符串转数字
来源：http://to.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iq.yuexingan06.cn

[S23] C：随机数
来源：http://lh.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wh.asd995.cn

[S24] C：获取本地时间
来源：http://yh.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lx.panjiajie.cn

[S25] C：内存拷贝
来源：http://cs.chemitech.net.cn

memcpy(dst, src, n);
来源：http://vu.huanxung.cn

[S26] C：内存清零
来源：http://ib.asd995.cn

memset(a, 0, sizeof a);
来源：http://el.gzmigu.cn

[S27] C：定义常量
来源：http://tq.huanxung.cn

const double PI = 3.14159;
来源：http://ab.hnjuh.cn

[S28] C：静态变量
来源：http://tf.szxytkj.cn

static int counter = 0;
来源：http://rf.bjjhwx.cn

[S29] C：变参函数
来源：http://ys.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ny.nszjky.cn

[S30] C：头文件保护
来源：http://kj.hahajie.cn

#ifndef X_H
来源：http://lf.wgjwhj.cn

#define X_H
来源：http://dn.shxzukj.cn

#endif
来源：http://jx.nicolike.cn

[S31] C++：Hello World
来源：http://dy.huixiangedu.cn

#include <iostream>
来源：http://aj.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://mt.szxytkj.cn

[S32] C++：字符串
来源：http://nk.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://ux.szxytkj.cn

[S33] C++：vector 增删
来源：http://gr.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pw.9csxet.cn

[S34] C++：遍历 vector
来源：http://td.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ib.shxzskj.cn

[S35] C++：map
来源：http://fj.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://so.lnxyls.cn

[S36] C++：unordered_map
来源：http://kf.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cd.yuntaijiaju.cn

[S37] C++：set
来源：http://zf.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mj.muxihuayi.cn

[S38] C++：排序
来源：http://am.colortex.cn

std::sort(v.begin(), v.end());
来源：http://iw.asd995.cn

[S39] C++：自定义比较器排序
来源：http://lj.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wx.9csxet.cn

[S40] C++：查找元素
来源：http://nx.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ja.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://kd.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jg.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://tw.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://tu.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://nc.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://pd.bjjhwx.cn

[S44] C++：引用传参
来源：http://fz.nicolike.cn

void inc(int &x) { ++x; }
来源：http://lp.lnxyls.cn

[S45] C++：lambda
来源：http://yg.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ht.gzmigu.cn

[S46] C++：函数模板
来源：http://jp.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zu.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://bj.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hl.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://xe.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uv.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://el.newstarts.cn

[S49] C++：写文件
来源：http://wg.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://su.nszjky.cn

[S50] C++：格式化数字
来源：http://eb.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qz.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://ky.bjjhwx.cn

static_cast<double>(a) / b
来源：http://sy.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://xh.asd995.cn

int size() const noexcept { return n_; }
来源：http://fh.muxihuayi.cn

[S53] C++：移动语义
来源：http://ba.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://zw.colortex.cn

[S54] C++：异常处理
来源：http://bh.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yt.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://ml.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bi.yuexingan06.cn

[S56] C++：optional
来源：http://hr.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fw.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://gi.huixinmuqiang.cn

constexpr int N = 10;
来源：http://rl.nszjky.cn

[S58] C++：命名空间
来源：http://my.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://ts.shtwfgs.cn

[S59] C++：静态断言
来源：http://gm.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://er.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://lo.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://po.bjjhwx.cn

================================================================================
来源：http://au.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://re.shtwfgs.cn

================================================================================
来源：http://eb.szsharing.cn

[T01] Kotlin：Hello World
来源：http://ts.panjiajie.cn

println("Hello")
来源：http://pk.huixiangedu.cn

[T02] Kotlin：变量
来源：http://xc.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xw.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://gz.szsharing.cn

"值: $b"
来源：http://mp.newstarts.cn

[T04] Kotlin：空安全
来源：http://ks.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://cr.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://fi.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://un.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://ln.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gj.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://wq.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fo.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://si.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://te.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://am.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://pv.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://xz.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oe.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://kx.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ln.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://ux.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://rv.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://yh.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://dw.muxihuayi.cn

[T14] Kotlin：循环
来源：http://yb.asd995.cn

for (i in 1..10) println(i)
来源：http://jz.shxzskj.cn

[T15] Kotlin：接口
来源：http://zc.nszjky.cn

interface Shape { fun area(): Double }
来源：http://pm.szxytkj.cn

[T16] Swift：Hello World
来源：http://gu.nicolike.cn

print("Hello")
来源：http://yl.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://sq.huanxung.cn

var a = 1;  let b = 2
来源：http://ej.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://wt.521024.cn

"值: \(b)"
来源：http://lr.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://ot.521024.cn

if let n = opt { print(n) }
来源：http://wv.9csxet.cn

[T20] Swift：数组操作
来源：http://ul.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ed.bookmarksfly.cn

[T21] Swift：遍历
来源：http://ao.bookmarksfly.cn

for x in a { print(x) }
来源：http://wf.shxzskj.cn

[T22] Swift：字典
来源：http://no.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ws.yuexingan06.cn

[T23] Swift：函数
来源：http://ge.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pl.wgjwhj.cn

[T24] Swift：闭包
来源：http://dg.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ry.lnxyls.cn

[T25] Swift：结构体
来源：http://gz.9csxet.cn

struct P { var x: Int }
来源：http://iw.bjjhwx.cn

[T26] Swift：类与重写
来源：http://jt.shxzskj.cn

class A: Base { override func f() {} }
来源：http://cm.lnxyls.cn

[T27] Swift：错误处理
来源：http://og.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://yg.shxzskj.cn

[T28] Swift：枚举
来源：http://tf.bookmarksfly.cn

enum Color { case red, green }
来源：http://sa.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://kh.nicolike.cn

guard let x = opt else { return }
来源：http://is.shxzskj.cn

[T30] Swift：协议
来源：http://mx.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://nb.jctech888.com.cn

[T31] Lua：Hello World
来源：http://nm.shxzskj.cn

print("Hello")
来源：http://hp.newstarts.cn

[T32] Lua：局部变量
来源：http://tu.szsharing.cn

local a = 1
来源：http://nw.szsharing.cn

[T33] Lua：表（数组）
来源：http://xj.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jl.szsharing.cn

[T34] Lua：遍历表
来源：http://ok.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rm.szxytkj.cn

[T35] Lua：字典表
来源：http://vf.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://zl.szsharing.cn

[T36] Lua：函数
来源：http://cr.muxihuayi.cn

function add(a, b) return a + b end
来源：http://qd.hahajie.cn

[T37] Lua：字符串拼接
来源：http://ht.shxzskj.cn

"a" .. "b"
来源：http://xn.colortex.cn

[T38] Lua：条件
来源：http://fx.huixiangedu.cn

if x > 0 then print("正") end
来源：http://up.shxzukj.cn

[T39] Lua：模式匹配
来源：http://pd.yuexingan06.cn

string.find(s, "%d+")
来源：http://xg.shtwfgs.cn

[T40] Lua：元表
来源：http://jn.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://mz.jctech888.com.cn

[T41] Perl：Hello World
来源：http://yp.wgjwhj.cn

print "Hello\n";
来源：http://pe.newstarts.cn

[T42] Perl：变量类型
来源：http://vk.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://un.newstarts.cn

[T43] Perl：字符串插值
来源：http://qv.bookmarksfly.cn

"值: $a"
来源：http://ir.9csxet.cn

[T44] Perl：条件
来源：http://jy.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://us.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://ob.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://os.9csxet.cn

[T46] Perl：哈希操作
来源：http://df.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nf.hnjuh.cn

[T47] Perl：正则捕获
来源：http://cj.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sv.521024.cn

[T48] Perl：正则替换
来源：http://fw.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://tq.gzmigu.cn

[T49] Perl：函数
来源：http://si.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zn.hahajie.cn

[T50] Perl：逐行读文件
来源：http://au.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ck.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://zz.muxihuayi.cn

[T51] Scala：Hello World
来源：http://vx.szxytkj.cn

println("Hello")
来源：http://mz.huixinmuqiang.cn

[T52] Scala：变量
来源：http://hw.nszjky.cn

val a = 1;  var b = 2
来源：http://yl.colortex.cn

[T53] Scala：字符串插值
来源：http://in.huanxung.cn

s"值: $b"
来源：http://ip.colortex.cn

[T54] Scala：集合映射
来源：http://yo.nszjky.cn

List(1, 2, 3).map(_ * 2)
来源：http://li.huanxung.cn

[T55] Scala：集合过滤
来源：http://mm.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fz.shtwfgs.cn

[T56] Scala：样例类
来源：http://vp.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://ps.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://hp.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yo.shtwfgs.cn

[T58] Scala：函数定义
来源：http://iw.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qo.nicolike.cn

[T59] Scala：循环
来源：http://nk.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://na.yuexingan06.cn

[T60] Scala：折叠
来源：http://at.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pc.bookmarksfly.cn

================================================================================
来源：http://dt.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sq.shxzukj.cn

================================================================================
来源：http://da.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://ke.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ul.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://su.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://js.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://li.chemitech.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xn.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://dy.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ap.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://ai.hnjuh.cn

list(dict.fromkeys(arr))
来源：http://fg.panjiajie.cn

[U06] Py：合并两个字典
来源：http://pj.huixiangedu.cn

{**a, **b}
来源：http://md.szsharing.cn

[U07] Py：反转字典键值
来源：http://up.521024.cn

{v: k for k, v in d.items()}
来源：http://uf.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://bk.jctech888.com.cn

[y for x in nested for y in x]
来源：http://id.shxzskj.cn


<!-- 参考信息 -->