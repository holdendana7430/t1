代发 wailian999

openssl rand -hex 16
来源：http://io.newstarts.cn

[R68] 计算文件校验值
来源：http://eh.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ua.nszjky.cn

[R69] 生成随机密码
来源：http://ll.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://qd.haigaiapp.cn

[R70] 时间戳与互转
来源：http://ox.szsharing.cn

date +%s;  date -d @1700000000
来源：http://uf.szsharing.cn

[R71] 日期格式化
来源：http://jz.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yt.yuexingan06.cn

[R72] 等待端口就绪
来源：http://us.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fx.hnjuh.cn

[R73] 分割大日志
来源：http://yr.nicolike.cn

split -l 1000 big.log part_
来源：http://jp.panjiajie.cn

[R74] 批量重命名
来源：http://jm.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zo.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://eu.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://iv.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://cw.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vs.muxihuayi.cn

[R77] 读取用户输入
来源：http://ox.szsharing.cn

read -rp "请输入: " ans
来源：http://ub.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://pu.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yb.muxihuayi.cn

[R79] 解析命令行选项
来源：http://ao.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fy.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://dr.jianghongdianzi.cn

time ./run.sh
来源：http://vd.huixinmuqiang.cn

================================================================================
来源：http://zn.muxihuayi.cn

S. C / C++ 专题
来源：http://dj.panjiajie.cn

================================================================================
来源：http://if.muxihuayi.cn

[S01] C：Hello World
来源：http://ue.chemitech.net.cn

#include <stdio.h>
来源：http://gr.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zc.szsharing.cn

[S02] C：变量与格式化输出
来源：http://tf.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://fq.newstarts.cn

[S03] C：读入整数
来源：http://jr.szxytkj.cn

int x; scanf("%d", &x);
来源：http://gn.wgjwhj.cn

[S04] C：字符串复制
来源：http://jm.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gz.szxytkj.cn

[S05] C：字符串长度
来源：http://wa.hahajie.cn

strlen(s)
来源：http://lg.yuexingan06.cn

[S06] C：字符串比较
来源：http://df.wgjwhj.cn

strcmp(a, b) == 0
来源：http://zu.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://ow.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ty.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://sq.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ko.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://rh.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://da.shxzukj.cn

[S10] C：指针与解引用
来源：http://ia.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://db.huanxung.cn

[S11] C：逐行读文件
来源：http://zl.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://mi.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wd.yuexingan06.cn

fclose(f);
来源：http://qn.bjjhwx.cn

[S12] C：写文件
来源：http://oh.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ra.yuntaijiaju.cn

[S13] C：宏定义
来源：http://nt.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lm.lnxyls.cn

[S14] C：枚举
来源：http://cj.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://nm.lnxyls.cn

[S15] C：类型转换
来源：http://oy.lnxyls.cn

(double) a / b
来源：http://bg.panjiajie.cn

[S16] C：位操作置位
来源：http://re.bjjhwx.cn

x |= (1 << 3);
来源：http://qb.newstarts.cn

[S17] C：安全拼接字符串
来源：http://bh.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ht.huixiangedu.cn

[S18] C：命令行参数
来源：http://db.nicolike.cn

int main(int argc, char **argv)
来源：http://tn.muxihuayi.cn

[S19] C：快速排序
来源：http://tb.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lq.lnxyls.cn

[S20] C：二分查找
来源：http://bp.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://do.huixiangedu.cn

[S21] C：字符类别判断
来源：http://hr.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eh.chemitech.net.cn

[S22] C：字符串转数字
来源：http://cv.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oj.huixiangedu.cn

[S23] C：随机数
来源：http://qd.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fz.szsharing.cn

[S24] C：获取本地时间
来源：http://ex.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tq.lnxyls.cn

[S25] C：内存拷贝
来源：http://us.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://dp.gzmigu.cn

[S26] C：内存清零
来源：http://ew.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://eh.lnxyls.cn

[S27] C：定义常量
来源：http://gw.jctech888.com.cn

const double PI = 3.14159;
来源：http://hf.shxzukj.cn

[S28] C：静态变量
来源：http://ut.jctech888.com.cn

static int counter = 0;
来源：http://xd.9csxet.cn

[S29] C：变参函数
来源：http://ua.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cq.huanxung.cn

[S30] C：头文件保护
来源：http://ga.shxzukj.cn

#ifndef X_H
来源：http://ib.521024.cn

#define X_H
来源：http://yq.hahajie.cn

#endif
来源：http://gu.yuexingan06.cn

[S31] C++：Hello World
来源：http://df.yuntaijiaju.cn

#include <iostream>
来源：http://od.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://lu.shtwfgs.cn

[S32] C++：字符串
来源：http://at.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://gb.521024.cn

[S33] C++：vector 增删
来源：http://ic.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ns.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://hp.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://at.wgjwhj.cn

[S35] C++：map
来源：http://nl.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zv.shtwfgs.cn

[S36] C++：unordered_map
来源：http://kr.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://je.szsharing.cn

[S37] C++：set
来源：http://su.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sz.wgjwhj.cn

[S38] C++：排序
来源：http://fr.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://ol.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://xi.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vu.lnxyls.cn

[S40] C++：查找元素
来源：http://de.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gx.gzmigu.cn

[S41] C++：类与构造函数
来源：http://du.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oy.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://xq.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://lk.colortex.cn

[S43] C++：智能指针
来源：http://cg.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://ma.shxzukj.cn

[S44] C++：引用传参
来源：http://om.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://es.gzmigu.cn

[S45] C++：lambda
来源：http://fv.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gs.shtwfgs.cn

[S46] C++：函数模板
来源：http://pb.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fn.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://vd.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jb.szxytkj.cn

[S48] C++：逐行读文件
来源：http://bn.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jj.hahajie.cn

while (std::getline(in, line)) { }
来源：http://de.panjiajie.cn

[S49] C++：写文件
来源：http://bd.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mv.huanxung.cn

[S50] C++：格式化数字
来源：http://nq.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eq.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://kg.panjiajie.cn

static_cast<double>(a) / b
来源：http://vr.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://cj.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://gs.521024.cn

[S53] C++：移动语义
来源：http://rw.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://dq.colortex.cn

[S54] C++：异常处理
来源：http://tg.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ka.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://er.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ig.yuexingan06.cn

[S56] C++：optional
来源：http://ag.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iy.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://er.wgjwhj.cn

constexpr int N = 10;
来源：http://vd.wgjwhj.cn

[S58] C++：命名空间
来源：http://kr.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://wp.chemitech.net.cn

[S59] C++：静态断言
来源：http://kx.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nh.asd995.cn

[S60] C++：遍历并删除元素
来源：http://ik.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zt.nicolike.cn

================================================================================
来源：http://ct.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lc.jctech888.com.cn

================================================================================
来源：http://xd.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://fh.panjiajie.cn

println("Hello")
来源：http://qu.9csxet.cn

[T02] Kotlin：变量
来源：http://ji.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://je.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://nq.shxzskj.cn

"值: $b"
来源：http://zg.gzmigu.cn

[T04] Kotlin：空安全
来源：http://ye.9csxet.cn

val n: String? = null;  n?.length
来源：http://ge.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://qc.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kv.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://pu.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bm.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://ut.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oj.asd995.cn

[T08] Kotlin：数据类
来源：http://go.colortex.cn

data class User(val name: String, val age: Int)
来源：http://zf.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://ci.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://yd.szsharing.cn

[T10] Kotlin：默认参数
来源：http://yh.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nf.bjjhwx.cn

[T11] Kotlin：协程
来源：http://bl.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oo.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://kd.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://yi.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://ua.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://dy.nszjky.cn

[T14] Kotlin：循环
来源：http://yf.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://iz.nicolike.cn

[T15] Kotlin：接口
来源：http://qk.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://rr.chemitech.net.cn

[T16] Swift：Hello World
来源：http://uq.521024.cn

print("Hello")
来源：http://hc.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://pa.panjiajie.cn

var a = 1;  let b = 2
来源：http://ev.hahajie.cn

[T18] Swift：字符串插值
来源：http://hs.bjjhwx.cn

"值: \(b)"
来源：http://ey.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://bu.haigaiapp.cn

if let n = opt { print(n) }
来源：http://ox.panjiajie.cn

[T20] Swift：数组操作
来源：http://om.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ms.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://wn.9csxet.cn

for x in a { print(x) }
来源：http://ur.jctech888.com.cn

[T22] Swift：字典
来源：http://io.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tl.521024.cn

[T23] Swift：函数
来源：http://se.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mg.haigaiapp.cn

[T24] Swift：闭包
来源：http://wi.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ih.lnxyls.cn

[T25] Swift：结构体
来源：http://wr.haigaiapp.cn

struct P { var x: Int }
来源：http://qd.szxytkj.cn

[T26] Swift：类与重写
来源：http://lr.lnxyls.cn

class A: Base { override func f() {} }
来源：http://wc.muxihuayi.cn

[T27] Swift：错误处理
来源：http://ga.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://yr.shtwfgs.cn

[T28] Swift：枚举
来源：http://jp.yuexingan06.cn

enum Color { case red, green }
来源：http://eq.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://lk.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://na.bjjhwx.cn

[T30] Swift：协议
来源：http://gi.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://wy.9csxet.cn

[T31] Lua：Hello World
来源：http://oi.nicolike.cn

print("Hello")
来源：http://ik.bjjhwx.cn

[T32] Lua：局部变量
来源：http://po.bookmarksfly.cn

local a = 1
来源：http://qj.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://fr.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mc.haigaiapp.cn

[T34] Lua：遍历表
来源：http://oe.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://te.lnxyls.cn

[T35] Lua：字典表
来源：http://mt.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://ih.szxytkj.cn

[T36] Lua：函数
来源：http://it.chemitech.net.cn

function add(a, b) return a + b end
来源：http://rf.hahajie.cn

[T37] Lua：字符串拼接
来源：http://xp.jianghongdianzi.cn

"a" .. "b"
来源：http://qp.asd995.cn

[T38] Lua：条件
来源：http://lc.shtwfgs.cn

if x > 0 then print("正") end
来源：http://mw.hnjuh.cn

[T39] Lua：模式匹配
来源：http://yh.hnjuh.cn

string.find(s, "%d+")
来源：http://uw.panjiajie.cn

[T40] Lua：元表
来源：http://al.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://ca.haigaiapp.cn

[T41] Perl：Hello World
来源：http://fw.shxzskj.cn

print "Hello\n";
来源：http://sm.shtwfgs.cn

[T42] Perl：变量类型
来源：http://sl.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zr.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://gw.asd995.cn

"值: $a"
来源：http://bj.szxytkj.cn

[T44] Perl：条件
来源：http://kt.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://fp.521024.cn

[T45] Perl：数组遍历
来源：http://ub.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://iq.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://zo.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gk.panjiajie.cn

[T47] Perl：正则捕获
来源：http://jo.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zp.panjiajie.cn

[T48] Perl：正则替换
来源：http://jp.lnxyls.cn

$s =~ s/old/new/g;
来源：http://sh.bjjhwx.cn

[T49] Perl：函数
来源：http://wk.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ez.asd995.cn

[T50] Perl：逐行读文件
来源：http://ak.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sf.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ks.hnjuh.cn

[T51] Scala：Hello World
来源：http://fn.shxzukj.cn

println("Hello")
来源：http://ob.jianghongdianzi.cn

[T52] Scala：变量
来源：http://nq.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://vh.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://iw.chemitech.net.cn

s"值: $b"
来源：http://bp.shxzskj.cn

[T54] Scala：集合映射
来源：http://xr.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://hj.szsharing.cn

[T55] Scala：集合过滤
来源：http://cp.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qv.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://dd.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://sl.newstarts.cn

[T57] Scala：模式匹配
来源：http://dx.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zu.newstarts.cn

[T58] Scala：函数定义
来源：http://mr.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ap.yuexingan06.cn

[T59] Scala：循环
来源：http://hj.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://rz.shtwfgs.cn

[T60] Scala：折叠
来源：http://jj.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mg.9csxet.cn

================================================================================
来源：http://sm.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ia.bookmarksfly.cn

================================================================================
来源：http://ln.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://gh.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hr.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://jb.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vl.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://nc.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oc.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://gd.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://st.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://im.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://hp.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://vh.szxytkj.cn

{**a, **b}
来源：http://bg.hnjuh.cn

[U07] Py：反转字典键值
来源：http://df.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://ya.9csxet.cn

[U08] Py：展平二维列表
来源：http://pv.shxzskj.cn

[y for x in nested for y in x]
来源：http://yu.lnxyls.cn


<!-- 参考信息 -->