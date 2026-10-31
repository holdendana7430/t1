代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://dr.panjiajie.cn

[R70] 时间戳与互转
来源：http://wk.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://fo.shxzukj.cn

[R71] 日期格式化
来源：http://gj.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bg.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://ex.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nw.gzmigu.cn

[R73] 分割大日志
来源：http://qg.szxytkj.cn

split -l 1000 big.log part_
来源：http://li.huixinmuqiang.cn

[R74] 批量重命名
来源：http://nt.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rg.muxihuayi.cn

[R75] 导出环境变量
来源：http://jm.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://gp.asd995.cn

[R76] 使用临时文件
来源：http://rh.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pl.shtwfgs.cn

[R77] 读取用户输入
来源：http://ub.panjiajie.cn

read -rp "请输入: " ans
来源：http://hn.muxihuayi.cn

[R78] 交互式菜单
来源：http://ur.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zq.asd995.cn

[R79] 解析命令行选项
来源：http://dm.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kj.colortex.cn

[R80] 查看脚本执行耗时
来源：http://zo.colortex.cn

time ./run.sh
来源：http://jl.bookmarksfly.cn

================================================================================
来源：http://nz.yuntaijiaju.cn

S. C / C++ 专题
来源：http://yw.lnxyls.cn

================================================================================
来源：http://ja.bjjhwx.cn

[S01] C：Hello World
来源：http://hi.huixiangedu.cn

#include <stdio.h>
来源：http://wl.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ki.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://gu.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://df.shxzskj.cn

[S03] C：读入整数
来源：http://ri.nicolike.cn

int x; scanf("%d", &x);
来源：http://kw.muxihuayi.cn

[S04] C：字符串复制
来源：http://ks.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tc.bookmarksfly.cn

[S05] C：字符串长度
来源：http://mx.nszjky.cn

strlen(s)
来源：http://xd.gzmigu.cn

[S06] C：字符串比较
来源：http://po.chemitech.net.cn

strcmp(a, b) == 0
来源：http://oi.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://dt.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uk.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://bw.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fq.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://py.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tx.shxzskj.cn

[S10] C：指针与解引用
来源：http://xy.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://uv.gzmigu.cn

[S11] C：逐行读文件
来源：http://dw.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://im.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fq.haigaiapp.cn

fclose(f);
来源：http://zf.yuexingan06.cn

[S12] C：写文件
来源：http://mn.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ox.huixinmuqiang.cn

[S13] C：宏定义
来源：http://kd.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nq.chemitech.net.cn

[S14] C：枚举
来源：http://my.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://oh.szsharing.cn

[S15] C：类型转换
来源：http://pg.haigaiapp.cn

(double) a / b
来源：http://yg.haigaiapp.cn

[S16] C：位操作置位
来源：http://ab.nicolike.cn

x |= (1 << 3);
来源：http://ny.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://or.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fk.muxihuayi.cn

[S18] C：命令行参数
来源：http://ci.huanxung.cn

int main(int argc, char **argv)
来源：http://ty.nszjky.cn

[S19] C：快速排序
来源：http://wr.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hl.521024.cn

[S20] C：二分查找
来源：http://wm.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://op.shxzskj.cn

[S21] C：字符类别判断
来源：http://aw.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yj.bjjhwx.cn

[S22] C：字符串转数字
来源：http://nl.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vm.9csxet.cn

[S23] C：随机数
来源：http://ru.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wg.huanxung.cn

[S24] C：获取本地时间
来源：http://kz.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nw.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://gf.jctech888.com.cn

memcpy(dst, src, n);
来源：http://jl.jianghongdianzi.cn

[S26] C：内存清零
来源：http://zd.newstarts.cn

memset(a, 0, sizeof a);
来源：http://aq.colortex.cn

[S27] C：定义常量
来源：http://je.hnjuh.cn

const double PI = 3.14159;
来源：http://bc.haigaiapp.cn

[S28] C：静态变量
来源：http://mh.huanxung.cn

static int counter = 0;
来源：http://cl.muxihuayi.cn

[S29] C：变参函数
来源：http://rk.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vq.shxzskj.cn

[S30] C：头文件保护
来源：http://fe.yuexingan06.cn

#ifndef X_H
来源：http://co.chemitech.net.cn

#define X_H
来源：http://te.haigaiapp.cn

#endif
来源：http://mf.521024.cn

[S31] C++：Hello World
来源：http://rr.asd995.cn

#include <iostream>
来源：http://up.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://za.nicolike.cn

[S32] C++：字符串
来源：http://ms.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://fq.lnxyls.cn

[S33] C++：vector 增删
来源：http://sa.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vu.huanxung.cn

[S34] C++：遍历 vector
来源：http://uz.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://zs.szxytkj.cn

[S35] C++：map
来源：http://xe.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qv.hahajie.cn

[S36] C++：unordered_map
来源：http://yb.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ma.wgjwhj.cn

[S37] C++：set
来源：http://jg.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://da.bjjhwx.cn

[S38] C++：排序
来源：http://iw.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://gv.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://tb.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tv.szsharing.cn

[S40] C++：查找元素
来源：http://gz.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ix.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://dy.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xw.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://qh.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://gd.huixiangedu.cn

[S43] C++：智能指针
来源：http://tl.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://yi.shxzukj.cn

[S44] C++：引用传参
来源：http://vt.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://az.szxytkj.cn

[S45] C++：lambda
来源：http://xf.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kl.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://ll.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qu.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://pa.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cb.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://km.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ze.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://rt.asd995.cn

[S49] C++：写文件
来源：http://yw.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gv.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://mz.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zn.hnjuh.cn

[S51] C++：显式类型转换
来源：http://iq.huixiangedu.cn

static_cast<double>(a) / b
来源：http://wo.huanxung.cn

[S52] C++：const 与 noexcept
来源：http://pg.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://dn.shtwfgs.cn

[S53] C++：移动语义
来源：http://oj.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://vb.hnjuh.cn

[S54] C++：异常处理
来源：http://sj.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gc.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://ur.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://up.szsharing.cn

[S56] C++：optional
来源：http://nv.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sl.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://hb.hahajie.cn

constexpr int N = 10;
来源：http://jx.yuexingan06.cn

[S58] C++：命名空间
来源：http://ft.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://wa.nszjky.cn

[S59] C++：静态断言
来源：http://ah.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hu.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://sd.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rf.panjiajie.cn

================================================================================
来源：http://hp.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://be.huixiangedu.cn

================================================================================
来源：http://vw.asd995.cn

[T01] Kotlin：Hello World
来源：http://gv.shtwfgs.cn

println("Hello")
来源：http://cy.hnjuh.cn

[T02] Kotlin：变量
来源：http://xx.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qg.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://ns.chemitech.net.cn

"值: $b"
来源：http://dz.hahajie.cn

[T04] Kotlin：空安全
来源：http://hf.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://xb.colortex.cn

[T05] Kotlin：when 表达式
来源：http://wz.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zb.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://ww.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vc.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://rb.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uz.newstarts.cn

[T08] Kotlin：数据类
来源：http://jj.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://lu.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ih.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://dc.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://kl.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tv.gzmigu.cn

[T11] Kotlin：协程
来源：http://ga.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ql.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://zc.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://jl.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://ax.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://lb.huanxung.cn

[T14] Kotlin：循环
来源：http://wv.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://jd.szsharing.cn

[T15] Kotlin：接口
来源：http://rc.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://oz.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://ru.jianghongdianzi.cn

print("Hello")
来源：http://dc.nszjky.cn

[T17] Swift：变量与常量
来源：http://sx.wgjwhj.cn

var a = 1;  let b = 2
来源：http://cf.hahajie.cn

[T18] Swift：字符串插值
来源：http://ez.haigaiapp.cn

"值: \(b)"
来源：http://qb.hnjuh.cn

[T19] Swift：可选绑定
来源：http://wv.newstarts.cn

if let n = opt { print(n) }
来源：http://ka.hahajie.cn

[T20] Swift：数组操作
来源：http://lm.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rd.wgjwhj.cn

[T21] Swift：遍历
来源：http://of.szsharing.cn

for x in a { print(x) }
来源：http://wg.chemitech.net.cn

[T22] Swift：字典
来源：http://dc.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nm.huixinmuqiang.cn

[T23] Swift：函数
来源：http://hu.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://au.521024.cn

[T24] Swift：闭包
来源：http://by.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cq.chemitech.net.cn

[T25] Swift：结构体
来源：http://do.chemitech.net.cn

struct P { var x: Int }
来源：http://xv.szxytkj.cn

[T26] Swift：类与重写
来源：http://np.gzmigu.cn

class A: Base { override func f() {} }
来源：http://jf.hahajie.cn

[T27] Swift：错误处理
来源：http://nu.nicolike.cn

do { try f() } catch { print(error) }
来源：http://zq.wgjwhj.cn

[T28] Swift：枚举
来源：http://kv.shxzskj.cn

enum Color { case red, green }
来源：http://ok.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://ei.huanxung.cn

guard let x = opt else { return }
来源：http://ew.hahajie.cn

[T30] Swift：协议
来源：http://xf.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://ay.9csxet.cn

[T31] Lua：Hello World
来源：http://pd.colortex.cn

print("Hello")
来源：http://ls.szsharing.cn

[T32] Lua：局部变量
来源：http://ot.huixinmuqiang.cn

local a = 1
来源：http://vc.hnjuh.cn

[T33] Lua：表（数组）
来源：http://xb.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xn.shxzukj.cn

[T34] Lua：遍历表
来源：http://kl.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bb.muxihuayi.cn

[T35] Lua：字典表
来源：http://xj.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://sm.shxzukj.cn

[T36] Lua：函数
来源：http://ny.haigaiapp.cn

function add(a, b) return a + b end
来源：http://xg.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://dq.9csxet.cn

"a" .. "b"
来源：http://py.shxzukj.cn

[T38] Lua：条件
来源：http://bt.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://hi.lnxyls.cn

[T39] Lua：模式匹配
来源：http://kn.huixiangedu.cn

string.find(s, "%d+")
来源：http://cx.jctech888.com.cn

[T40] Lua：元表
来源：http://qk.nicolike.cn

setmetatable({}, { __index = base })
来源：http://mv.9csxet.cn

[T41] Perl：Hello World
来源：http://ph.bjjhwx.cn

print "Hello\n";
来源：http://bu.9csxet.cn

[T42] Perl：变量类型
来源：http://ee.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qw.hnjuh.cn

[T43] Perl：字符串插值
来源：http://al.wgjwhj.cn

"值: $a"
来源：http://pm.huixiangedu.cn

[T44] Perl：条件
来源：http://kf.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://xu.nicolike.cn

[T45] Perl：数组遍历
来源：http://mz.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://ft.9csxet.cn

[T46] Perl：哈希操作
来源：http://gq.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iv.gzmigu.cn

[T47] Perl：正则捕获
来源：http://ta.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ul.nicolike.cn

[T48] Perl：正则替换
来源：http://pe.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://wq.szsharing.cn

[T49] Perl：函数
来源：http://ry.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://el.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://qk.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vr.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://bv.huanxung.cn

[T51] Scala：Hello World
来源：http://td.huixinmuqiang.cn

println("Hello")
来源：http://uq.huanxung.cn

[T52] Scala：变量
来源：http://fb.9csxet.cn

val a = 1;  var b = 2
来源：http://yv.huanxung.cn

[T53] Scala：字符串插值
来源：http://ak.szxytkj.cn

s"值: $b"
来源：http://wn.szxytkj.cn

[T54] Scala：集合映射
来源：http://lx.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://vx.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://ya.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bz.colortex.cn

[T56] Scala：样例类
来源：http://ip.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://cu.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://lr.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eg.shtwfgs.cn

[T58] Scala：函数定义
来源：http://wl.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ao.muxihuayi.cn

[T59] Scala：循环
来源：http://xp.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://jz.shtwfgs.cn

[T60] Scala：折叠
来源：http://xr.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vq.yuntaijiaju.cn

================================================================================
来源：http://xj.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qb.521024.cn

================================================================================
来源：http://ha.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://xg.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wj.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://ca.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gz.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://dc.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tm.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://ha.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ph.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://gg.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://xp.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://oc.hahajie.cn

{**a, **b}
来源：http://xr.hnjuh.cn

[U07] Py：反转字典键值
来源：http://iv.huanxung.cn

{v: k for k, v in d.items()}
来源：http://nm.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://dt.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://qd.shxzukj.cn

[U09] Py：字典取最大值的键
来源：http://ah.nszjky.cn

max(d, key=d.get)
来源：http://ad.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://so.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nr.shtwfgs.cn


<!-- 参考信息 -->