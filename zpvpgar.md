代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://jk.muxihuayi.cn

[R72] 等待端口就绪
来源：http://su.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bo.521024.cn

[R73] 分割大日志
来源：http://ak.nszjky.cn

split -l 1000 big.log part_
来源：http://gs.chemitech.net.cn

[R74] 批量重命名
来源：http://ml.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ii.nicolike.cn

[R75] 导出环境变量
来源：http://me.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://lh.shtwfgs.cn

[R76] 使用临时文件
来源：http://yd.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zo.521024.cn

[R77] 读取用户输入
来源：http://bh.shxzukj.cn

read -rp "请输入: " ans
来源：http://mi.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://pi.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kn.huanxung.cn

[R79] 解析命令行选项
来源：http://ls.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xq.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://vx.bookmarksfly.cn

time ./run.sh
来源：http://st.asd995.cn

================================================================================
来源：http://vc.nszjky.cn

S. C / C++ 专题
来源：http://bu.shxzskj.cn

================================================================================
来源：http://gz.muxihuayi.cn

[S01] C：Hello World
来源：http://mo.nicolike.cn

#include <stdio.h>
来源：http://xc.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bh.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://jq.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://bi.jctech888.com.cn

[S03] C：读入整数
来源：http://tv.asd995.cn

int x; scanf("%d", &x);
来源：http://xz.wgjwhj.cn

[S04] C：字符串复制
来源：http://qi.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://og.jctech888.com.cn

[S05] C：字符串长度
来源：http://yr.bookmarksfly.cn

strlen(s)
来源：http://nd.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://zo.bjjhwx.cn

strcmp(a, b) == 0
来源：http://fk.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://qv.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qd.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://yg.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vr.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://oy.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ja.colortex.cn

[S10] C：指针与解引用
来源：http://jm.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://iw.panjiajie.cn

[S11] C：逐行读文件
来源：http://fh.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://in.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ks.shxzskj.cn

fclose(f);
来源：http://tv.yuexingan06.cn

[S12] C：写文件
来源：http://xj.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tp.nicolike.cn

[S13] C：宏定义
来源：http://fy.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ig.shxzukj.cn

[S14] C：枚举
来源：http://fc.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://qk.jctech888.com.cn

[S15] C：类型转换
来源：http://qa.wgjwhj.cn

(double) a / b
来源：http://md.lnxyls.cn

[S16] C：位操作置位
来源：http://oj.nszjky.cn

x |= (1 << 3);
来源：http://bt.asd995.cn

[S17] C：安全拼接字符串
来源：http://kb.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://py.9csxet.cn

[S18] C：命令行参数
来源：http://qe.lnxyls.cn

int main(int argc, char **argv)
来源：http://jk.panjiajie.cn

[S19] C：快速排序
来源：http://az.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zg.gzmigu.cn

[S20] C：二分查找
来源：http://fx.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oa.szsharing.cn

[S21] C：字符类别判断
来源：http://mk.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cy.jctech888.com.cn

[S22] C：字符串转数字
来源：http://rm.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ib.szxytkj.cn

[S23] C：随机数
来源：http://wh.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gd.jctech888.com.cn

[S24] C：获取本地时间
来源：http://dn.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qr.panjiajie.cn

[S25] C：内存拷贝
来源：http://qo.9csxet.cn

memcpy(dst, src, n);
来源：http://ul.asd995.cn

[S26] C：内存清零
来源：http://we.szsharing.cn

memset(a, 0, sizeof a);
来源：http://pc.yuexingan06.cn

[S27] C：定义常量
来源：http://vo.panjiajie.cn

const double PI = 3.14159;
来源：http://ch.muxihuayi.cn

[S28] C：静态变量
来源：http://hw.haigaiapp.cn

static int counter = 0;
来源：http://ds.shxzukj.cn

[S29] C：变参函数
来源：http://sf.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yd.hahajie.cn

[S30] C：头文件保护
来源：http://tl.haigaiapp.cn

#ifndef X_H
来源：http://ix.9csxet.cn

#define X_H
来源：http://cv.hnjuh.cn

#endif
来源：http://qp.muxihuayi.cn

[S31] C++：Hello World
来源：http://sc.yuntaijiaju.cn

#include <iostream>
来源：http://cd.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://jt.jctech888.com.cn

[S32] C++：字符串
来源：http://zz.521024.cn

std::string s = "hi";  s += "!";
来源：http://bz.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://dx.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bh.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ic.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://oj.gzmigu.cn

[S35] C++：map
来源：http://lu.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ux.gzmigu.cn

[S36] C++：unordered_map
来源：http://li.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lg.szsharing.cn

[S37] C++：set
来源：http://jx.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oc.haigaiapp.cn

[S38] C++：排序
来源：http://gb.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://xm.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://wx.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yy.asd995.cn

[S40] C++：查找元素
来源：http://se.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ho.9csxet.cn

[S41] C++：类与构造函数
来源：http://gc.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qy.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://ur.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://uo.shxzukj.cn

[S43] C++：智能指针
来源：http://kc.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://hw.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://ry.hahajie.cn

void inc(int &x) { ++x; }
来源：http://wa.panjiajie.cn

[S45] C++：lambda
来源：http://ol.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iq.shxzskj.cn

[S46] C++：函数模板
来源：http://hp.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lv.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://al.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yv.szxytkj.cn

[S48] C++：逐行读文件
来源：http://oi.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://de.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://ra.yuntaijiaju.cn

[S49] C++：写文件
来源：http://bn.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bi.colortex.cn

[S50] C++：格式化数字
来源：http://xk.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ah.521024.cn

[S51] C++：显式类型转换
来源：http://as.panjiajie.cn

static_cast<double>(a) / b
来源：http://cf.colortex.cn

[S52] C++：const 与 noexcept
来源：http://hf.521024.cn

int size() const noexcept { return n_; }
来源：http://rm.hnjuh.cn

[S53] C++：移动语义
来源：http://le.asd995.cn

std::vector<int> w = std::move(v);
来源：http://bt.haigaiapp.cn

[S54] C++：异常处理
来源：http://cw.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://je.panjiajie.cn

[S55] C++：结构化绑定
来源：http://ez.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ob.jianghongdianzi.cn

[S56] C++：optional
来源：http://cd.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lo.muxihuayi.cn

[S57] C++：编译期常量
来源：http://zu.colortex.cn

constexpr int N = 10;
来源：http://al.wgjwhj.cn

[S58] C++：命名空间
来源：http://ab.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://xn.9csxet.cn

[S59] C++：静态断言
来源：http://ve.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dc.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://me.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nn.haigaiapp.cn

================================================================================
来源：http://bb.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mu.nszjky.cn

================================================================================
来源：http://uz.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://kl.haigaiapp.cn

println("Hello")
来源：http://lf.9csxet.cn

[T02] Kotlin：变量
来源：http://rv.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zw.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://mh.gzmigu.cn

"值: $b"
来源：http://mw.hahajie.cn

[T04] Kotlin：空安全
来源：http://sy.nszjky.cn

val n: String? = null;  n?.length
来源：http://su.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://vx.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hn.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://gz.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fp.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://wu.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uu.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://pm.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://ns.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://in.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://po.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://pq.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ax.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://qq.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zv.szsharing.cn

[T12] Kotlin：解构声明
来源：http://vs.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://nm.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://ua.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://uz.newstarts.cn

[T14] Kotlin：循环
来源：http://pa.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://kg.9csxet.cn

[T15] Kotlin：接口
来源：http://jz.asd995.cn

interface Shape { fun area(): Double }
来源：http://dx.panjiajie.cn

[T16] Swift：Hello World
来源：http://oz.shxzskj.cn

print("Hello")
来源：http://yf.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://ix.szxytkj.cn

var a = 1;  let b = 2
来源：http://hp.gzmigu.cn

[T18] Swift：字符串插值
来源：http://fx.newstarts.cn

"值: \(b)"
来源：http://do.hnjuh.cn

[T19] Swift：可选绑定
来源：http://xp.huanxung.cn

if let n = opt { print(n) }
来源：http://jt.chemitech.net.cn

[T20] Swift：数组操作
来源：http://dw.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ac.muxihuayi.cn

[T21] Swift：遍历
来源：http://xb.newstarts.cn

for x in a { print(x) }
来源：http://za.yuexingan06.cn

[T22] Swift：字典
来源：http://wv.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vz.yuexingan06.cn

[T23] Swift：函数
来源：http://bl.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mt.newstarts.cn

[T24] Swift：闭包
来源：http://wz.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gq.newstarts.cn

[T25] Swift：结构体
来源：http://pe.nszjky.cn

struct P { var x: Int }
来源：http://nd.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://ny.shxzskj.cn

class A: Base { override func f() {} }
来源：http://au.huixiangedu.cn

[T27] Swift：错误处理
来源：http://gq.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://do.haigaiapp.cn

[T28] Swift：枚举
来源：http://tg.nicolike.cn

enum Color { case red, green }
来源：http://jq.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://gh.shtwfgs.cn

guard let x = opt else { return }
来源：http://gu.gzmigu.cn

[T30] Swift：协议
来源：http://nm.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ha.muxihuayi.cn

[T31] Lua：Hello World
来源：http://yw.lnxyls.cn

print("Hello")
来源：http://cd.huanxung.cn

[T32] Lua：局部变量
来源：http://lb.jctech888.com.cn

local a = 1
来源：http://or.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ug.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yp.szxytkj.cn

[T34] Lua：遍历表
来源：http://eh.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lv.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://mq.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://xe.shxzskj.cn

[T36] Lua：函数
来源：http://xt.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://fg.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://pg.szsharing.cn

"a" .. "b"
来源：http://zi.huixiangedu.cn

[T38] Lua：条件
来源：http://ee.huanxung.cn

if x > 0 then print("正") end
来源：http://kx.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://vr.nicolike.cn

string.find(s, "%d+")
来源：http://ra.gzmigu.cn

[T40] Lua：元表
来源：http://he.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ht.hnjuh.cn

[T41] Perl：Hello World
来源：http://nu.jianghongdianzi.cn

print "Hello\n";
来源：http://mv.jctech888.com.cn

[T42] Perl：变量类型
来源：http://cw.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ic.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://fy.nicolike.cn

"值: $a"
来源：http://ec.huixiangedu.cn

[T44] Perl：条件
来源：http://ur.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://oq.szxytkj.cn

[T45] Perl：数组遍历
来源：http://uy.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://js.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://ff.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rv.9csxet.cn

[T47] Perl：正则捕获
来源：http://oa.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tg.shxzukj.cn

[T48] Perl：正则替换
来源：http://nr.nicolike.cn

$s =~ s/old/new/g;
来源：http://el.huanxung.cn

[T49] Perl：函数
来源：http://mk.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yj.newstarts.cn

[T50] Perl：逐行读文件
来源：http://cx.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cg.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://of.muxihuayi.cn

[T51] Scala：Hello World
来源：http://uq.gzmigu.cn

println("Hello")
来源：http://rx.colortex.cn

[T52] Scala：变量
来源：http://zs.newstarts.cn

val a = 1;  var b = 2
来源：http://pi.lnxyls.cn

[T53] Scala：字符串插值
来源：http://kk.jctech888.com.cn

s"值: $b"
来源：http://fv.shtwfgs.cn

[T54] Scala：集合映射
来源：http://au.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://ql.szxytkj.cn

[T55] Scala：集合过滤
来源：http://ee.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tb.szsharing.cn

[T56] Scala：样例类
来源：http://vi.panjiajie.cn

case class User(name: String, age: Int)
来源：http://nt.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://mg.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yr.muxihuayi.cn

[T58] Scala：函数定义
来源：http://xe.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fq.hahajie.cn

[T59] Scala：循环
来源：http://ev.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://qh.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://ac.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oh.haigaiapp.cn

================================================================================
来源：http://du.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bv.gzmigu.cn

================================================================================
来源：http://sx.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://jb.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xs.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://yi.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tc.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://cd.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ep.panjiajie.cn

[U04] Py：变量调试打印
来源：http://mv.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kg.521024.cn

[U05] Py：列表去重且保序
来源：http://no.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://nn.nszjky.cn

[U06] Py：合并两个字典
来源：http://kj.huanxung.cn

{**a, **b}
来源：http://fr.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ex.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://tr.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://vu.asd995.cn

[y for x in nested for y in x]
来源：http://sg.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://ws.szxytkj.cn

max(d, key=d.get)
来源：http://po.asd995.cn

[U10] Py：按值排序字典
来源：http://ip.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vv.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://rw.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://zm.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sa.huanxung.cn

Counter(arr).most_common(3)
来源：http://es.jctech888.com.cn


<!-- 参考信息 -->