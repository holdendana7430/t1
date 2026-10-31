代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://ei.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://kv.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://ny.shxzukj.cn

[R71] 日期格式化
来源：http://mx.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ia.bjjhwx.cn

[R72] 等待端口就绪
来源：http://ep.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pi.9csxet.cn

[R73] 分割大日志
来源：http://ih.jctech888.com.cn

split -l 1000 big.log part_
来源：http://lm.shxzskj.cn

[R74] 批量重命名
来源：http://ax.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fc.jctech888.com.cn

[R75] 导出环境变量
来源：http://qp.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://uy.chemitech.net.cn

[R76] 使用临时文件
来源：http://et.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kj.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ja.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://ys.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://oq.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ht.panjiajie.cn

[R79] 解析命令行选项
来源：http://fg.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://no.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://za.yuexingan06.cn

time ./run.sh
来源：http://zr.wgjwhj.cn

================================================================================
来源：http://je.9csxet.cn

S. C / C++ 专题
来源：http://bk.chemitech.net.cn

================================================================================
来源：http://ru.lnxyls.cn

[S01] C：Hello World
来源：http://uj.muxihuayi.cn

#include <stdio.h>
来源：http://zl.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hp.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://ut.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://ya.hnjuh.cn

[S03] C：读入整数
来源：http://tx.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://to.haigaiapp.cn

[S04] C：字符串复制
来源：http://nw.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ob.shxzukj.cn

[S05] C：字符串长度
来源：http://yk.shxzukj.cn

strlen(s)
来源：http://wi.gzmigu.cn

[S06] C：字符串比较
来源：http://dw.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://nu.panjiajie.cn

[S07] C：数组遍历求和
来源：http://wz.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ax.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://cg.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fm.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://os.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://no.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://un.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://rh.colortex.cn

[S11] C：逐行读文件
来源：http://tr.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://hv.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rh.lnxyls.cn

fclose(f);
来源：http://ao.szxytkj.cn

[S12] C：写文件
来源：http://mz.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xx.yuntaijiaju.cn

[S13] C：宏定义
来源：http://yf.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://et.huixinmuqiang.cn

[S14] C：枚举
来源：http://or.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://cr.lnxyls.cn

[S15] C：类型转换
来源：http://pg.bjjhwx.cn

(double) a / b
来源：http://am.asd995.cn

[S16] C：位操作置位
来源：http://pj.gzmigu.cn

x |= (1 << 3);
来源：http://yv.newstarts.cn

[S17] C：安全拼接字符串
来源：http://zl.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bh.bookmarksfly.cn

[S18] C：命令行参数
来源：http://lh.hnjuh.cn

int main(int argc, char **argv)
来源：http://ne.hnjuh.cn

[S19] C：快速排序
来源：http://iw.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ep.gzmigu.cn

[S20] C：二分查找
来源：http://ci.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pf.gzmigu.cn

[S21] C：字符类别判断
来源：http://hc.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ck.gzmigu.cn

[S22] C：字符串转数字
来源：http://zy.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fj.yuexingan06.cn

[S23] C：随机数
来源：http://fp.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ss.yuexingan06.cn

[S24] C：获取本地时间
来源：http://fk.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ut.yuexingan06.cn

[S25] C：内存拷贝
来源：http://rq.nszjky.cn

memcpy(dst, src, n);
来源：http://qn.haigaiapp.cn

[S26] C：内存清零
来源：http://dj.hahajie.cn

memset(a, 0, sizeof a);
来源：http://dm.haigaiapp.cn

[S27] C：定义常量
来源：http://di.huixiangedu.cn

const double PI = 3.14159;
来源：http://hf.jctech888.com.cn

[S28] C：静态变量
来源：http://wp.hnjuh.cn

static int counter = 0;
来源：http://py.newstarts.cn

[S29] C：变参函数
来源：http://or.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ns.colortex.cn

[S30] C：头文件保护
来源：http://jh.colortex.cn

#ifndef X_H
来源：http://lb.jctech888.com.cn

#define X_H
来源：http://dj.hnjuh.cn

#endif
来源：http://dc.jctech888.com.cn

[S31] C++：Hello World
来源：http://qn.jctech888.com.cn

#include <iostream>
来源：http://xr.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://lq.muxihuayi.cn

[S32] C++：字符串
来源：http://ar.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://bz.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://tm.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sf.shxzukj.cn

[S34] C++：遍历 vector
来源：http://qg.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://dz.newstarts.cn

[S35] C++：map
来源：http://nn.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dq.nicolike.cn

[S36] C++：unordered_map
来源：http://tx.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ri.muxihuayi.cn

[S37] C++：set
来源：http://yy.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lb.szxytkj.cn

[S38] C++：排序
来源：http://ci.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://va.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://km.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sa.jctech888.com.cn

[S40] C++：查找元素
来源：http://un.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oh.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://kp.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://co.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://oq.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://gw.newstarts.cn

[S43] C++：智能指针
来源：http://qn.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://kk.hahajie.cn

[S44] C++：引用传参
来源：http://bm.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://sk.wgjwhj.cn

[S45] C++：lambda
来源：http://wa.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dk.shtwfgs.cn

[S46] C++：函数模板
来源：http://pr.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dg.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://uw.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sz.newstarts.cn

[S48] C++：逐行读文件
来源：http://ay.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mt.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://yp.shxzskj.cn

[S49] C++：写文件
来源：http://nk.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ld.gzmigu.cn

[S50] C++：格式化数字
来源：http://ul.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fg.nszjky.cn

[S51] C++：显式类型转换
来源：http://ut.nszjky.cn

static_cast<double>(a) / b
来源：http://rf.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://xc.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://aj.muxihuayi.cn

[S53] C++：移动语义
来源：http://mg.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://wy.szsharing.cn

[S54] C++：异常处理
来源：http://ke.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nd.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://hk.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rc.bookmarksfly.cn

[S56] C++：optional
来源：http://ib.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ue.shxzukj.cn

[S57] C++：编译期常量
来源：http://mu.szsharing.cn

constexpr int N = 10;
来源：http://iq.nszjky.cn

[S58] C++：命名空间
来源：http://nk.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://qz.jctech888.com.cn

[S59] C++：静态断言
来源：http://ol.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yl.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://tk.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vv.asd995.cn

================================================================================
来源：http://cl.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nb.yuexingan06.cn

================================================================================
来源：http://mr.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://ge.yuntaijiaju.cn

println("Hello")
来源：http://dj.shxzskj.cn

[T02] Kotlin：变量
来源：http://qk.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hu.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://di.chemitech.net.cn

"值: $b"
来源：http://pm.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://in.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://vc.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://dp.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bl.9csxet.cn

[T06] Kotlin：集合映射
来源：http://wd.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mf.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://gs.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ou.521024.cn

[T08] Kotlin：数据类
来源：http://wy.colortex.cn

data class User(val name: String, val age: Int)
来源：http://bx.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://un.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://rs.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://od.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gn.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://yy.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sm.nicolike.cn

[T12] Kotlin：解构声明
来源：http://rf.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://lw.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://il.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://hk.asd995.cn

[T14] Kotlin：循环
来源：http://gy.gzmigu.cn

for (i in 1..10) println(i)
来源：http://wp.huixiangedu.cn

[T15] Kotlin：接口
来源：http://xe.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://ee.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://tc.colortex.cn

print("Hello")
来源：http://es.szxytkj.cn

[T17] Swift：变量与常量
来源：http://gq.hnjuh.cn

var a = 1;  let b = 2
来源：http://wq.szsharing.cn

[T18] Swift：字符串插值
来源：http://ao.huixiangedu.cn

"值: \(b)"
来源：http://bt.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://zn.nicolike.cn

if let n = opt { print(n) }
来源：http://pg.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://jl.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cb.lnxyls.cn

[T21] Swift：遍历
来源：http://mx.muxihuayi.cn

for x in a { print(x) }
来源：http://nu.nicolike.cn

[T22] Swift：字典
来源：http://ce.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oi.wgjwhj.cn

[T23] Swift：函数
来源：http://qg.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ll.gzmigu.cn

[T24] Swift：闭包
来源：http://rw.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fy.hahajie.cn

[T25] Swift：结构体
来源：http://xf.newstarts.cn

struct P { var x: Int }
来源：http://mt.colortex.cn

[T26] Swift：类与重写
来源：http://cl.gzmigu.cn

class A: Base { override func f() {} }
来源：http://xs.yuexingan06.cn

[T27] Swift：错误处理
来源：http://nk.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://of.shxzskj.cn

[T28] Swift：枚举
来源：http://ry.szxytkj.cn

enum Color { case red, green }
来源：http://nw.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://xp.bookmarksfly.cn

guard let x = opt else { return }
来源：http://im.bjjhwx.cn

[T30] Swift：协议
来源：http://qs.asd995.cn

protocol Shape { func area() -> Double }
来源：http://mz.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://ov.yuntaijiaju.cn

print("Hello")
来源：http://vh.521024.cn

[T32] Lua：局部变量
来源：http://kk.chemitech.net.cn

local a = 1
来源：http://to.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://al.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uk.shxzukj.cn

[T34] Lua：遍历表
来源：http://bk.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://px.521024.cn

[T35] Lua：字典表
来源：http://bu.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://ix.gzmigu.cn

[T36] Lua：函数
来源：http://wu.9csxet.cn

function add(a, b) return a + b end
来源：http://mt.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://fu.szxytkj.cn

"a" .. "b"
来源：http://xi.colortex.cn

[T38] Lua：条件
来源：http://lb.haigaiapp.cn

if x > 0 then print("正") end
来源：http://zq.panjiajie.cn

[T39] Lua：模式匹配
来源：http://yt.szxytkj.cn

string.find(s, "%d+")
来源：http://tu.chemitech.net.cn

[T40] Lua：元表
来源：http://hj.hahajie.cn

setmetatable({}, { __index = base })
来源：http://wy.521024.cn

[T41] Perl：Hello World
来源：http://an.yuntaijiaju.cn

print "Hello\n";
来源：http://gh.hahajie.cn

[T42] Perl：变量类型
来源：http://co.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pv.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://xo.huixiangedu.cn

"值: $a"
来源：http://ak.szsharing.cn

[T44] Perl：条件
来源：http://gt.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://pa.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://ul.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://wr.szxytkj.cn

[T46] Perl：哈希操作
来源：http://zh.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://za.shxzukj.cn

[T47] Perl：正则捕获
来源：http://np.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sv.shxzukj.cn

[T48] Perl：正则替换
来源：http://ul.shxzukj.cn

$s =~ s/old/new/g;
来源：http://wp.yuexingan06.cn

[T49] Perl：函数
来源：http://ni.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dh.szsharing.cn

[T50] Perl：逐行读文件
来源：http://cf.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ba.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://gw.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://pg.521024.cn

println("Hello")
来源：http://wv.wgjwhj.cn

[T52] Scala：变量
来源：http://cm.szsharing.cn

val a = 1;  var b = 2
来源：http://xf.lnxyls.cn

[T53] Scala：字符串插值
来源：http://wv.521024.cn

s"值: $b"
来源：http://ve.nszjky.cn

[T54] Scala：集合映射
来源：http://uj.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://ie.szxytkj.cn

[T55] Scala：集合过滤
来源：http://ha.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://le.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://hg.lnxyls.cn

case class User(name: String, age: Int)
来源：http://ze.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://lu.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ja.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://hy.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ja.bookmarksfly.cn

[T59] Scala：循环
来源：http://zw.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://eu.huanxung.cn

[T60] Scala：折叠
来源：http://zl.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ld.521024.cn

================================================================================
来源：http://jt.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gu.muxihuayi.cn

================================================================================
来源：http://be.asd995.cn

[U01] Py：创建虚拟环境
来源：http://zw.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qp.chemitech.net.cn

[U02] Py：导出 / 安装依赖
来源：http://vi.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://un.asd995.cn

[U03] Py：加载 .env 配置
来源：http://qo.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vq.9csxet.cn

[U04] Py：变量调试打印
来源：http://ub.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ks.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://od.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ef.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://wt.wgjwhj.cn

{**a, **b}
来源：http://sk.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://vp.lnxyls.cn

{v: k for k, v in d.items()}
来源：http://oi.szxytkj.cn

[U08] Py：展平二维列表
来源：http://mz.lnxyls.cn

[y for x in nested for y in x]
来源：http://fm.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://ji.newstarts.cn

max(d, key=d.get)
来源：http://no.lnxyls.cn

[U10] Py：按值排序字典
来源：http://ja.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gd.shxzukj.cn


<!-- 参考信息 -->