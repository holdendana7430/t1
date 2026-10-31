代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://zq.huixiangedu.cn

[R72] 等待端口就绪
来源：http://vx.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://um.asd995.cn

[R73] 分割大日志
来源：http://pk.huanxung.cn

split -l 1000 big.log part_
来源：http://jv.szxytkj.cn

[R74] 批量重命名
来源：http://yr.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fj.szxytkj.cn

[R75] 导出环境变量
来源：http://vp.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://qc.huixiangedu.cn

[R76] 使用临时文件
来源：http://ph.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://in.jctech888.com.cn

[R77] 读取用户输入
来源：http://gd.colortex.cn

read -rp "请输入: " ans
来源：http://hi.asd995.cn

[R78] 交互式菜单
来源：http://mc.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wo.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ej.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mc.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://qv.bjjhwx.cn

time ./run.sh
来源：http://kt.jianghongdianzi.cn

================================================================================
来源：http://ks.shtwfgs.cn

S. C / C++ 专题
来源：http://we.wgjwhj.cn

================================================================================
来源：http://lb.shxzskj.cn

[S01] C：Hello World
来源：http://za.521024.cn

#include <stdio.h>
来源：http://xk.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jt.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://lf.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://mw.wgjwhj.cn

[S03] C：读入整数
来源：http://hv.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://gx.jctech888.com.cn

[S04] C：字符串复制
来源：http://ui.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yu.colortex.cn

[S05] C：字符串长度
来源：http://jq.haigaiapp.cn

strlen(s)
来源：http://nh.panjiajie.cn

[S06] C：字符串比较
来源：http://nd.newstarts.cn

strcmp(a, b) == 0
来源：http://de.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://ec.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iq.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://me.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rf.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://jo.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xp.szsharing.cn

[S10] C：指针与解引用
来源：http://xy.nicolike.cn

int *p = &a;  *p = 5;
来源：http://mf.9csxet.cn

[S11] C：逐行读文件
来源：http://xm.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://mt.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xo.huixinmuqiang.cn

fclose(f);
来源：http://we.nicolike.cn

[S12] C：写文件
来源：http://zw.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kw.huanxung.cn

[S13] C：宏定义
来源：http://fx.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nz.shxzskj.cn

[S14] C：枚举
来源：http://nm.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://fx.yuntaijiaju.cn

[S15] C：类型转换
来源：http://lj.hnjuh.cn

(double) a / b
来源：http://ha.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://pv.shxzukj.cn

x |= (1 << 3);
来源：http://gl.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://dh.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://og.newstarts.cn

[S18] C：命令行参数
来源：http://du.wgjwhj.cn

int main(int argc, char **argv)
来源：http://dw.huixinmuqiang.cn

[S19] C：快速排序
来源：http://az.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pj.wgjwhj.cn

[S20] C：二分查找
来源：http://ki.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zf.shxzukj.cn

[S21] C：字符类别判断
来源：http://jq.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ew.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://ln.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vf.asd995.cn

[S23] C：随机数
来源：http://ym.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gg.panjiajie.cn

[S24] C：获取本地时间
来源：http://gf.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mv.huixiangedu.cn

[S25] C：内存拷贝
来源：http://cs.huanxung.cn

memcpy(dst, src, n);
来源：http://bb.yuntaijiaju.cn

[S26] C：内存清零
来源：http://fc.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://du.huanxung.cn

[S27] C：定义常量
来源：http://hf.521024.cn

const double PI = 3.14159;
来源：http://kc.shtwfgs.cn

[S28] C：静态变量
来源：http://kz.bjjhwx.cn

static int counter = 0;
来源：http://tz.huanxung.cn

[S29] C：变参函数
来源：http://wt.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ou.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://uj.wgjwhj.cn

#ifndef X_H
来源：http://et.bjjhwx.cn

#define X_H
来源：http://dw.jctech888.com.cn

#endif
来源：http://nb.yuexingan06.cn

[S31] C++：Hello World
来源：http://lf.muxihuayi.cn

#include <iostream>
来源：http://hn.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://cc.huixiangedu.cn

[S32] C++：字符串
来源：http://yy.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://vn.shtwfgs.cn

[S33] C++：vector 增删
来源：http://sb.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ln.521024.cn

[S34] C++：遍历 vector
来源：http://zj.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://zx.haigaiapp.cn

[S35] C++：map
来源：http://wu.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jk.newstarts.cn

[S36] C++：unordered_map
来源：http://kq.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hq.jctech888.com.cn

[S37] C++：set
来源：http://bd.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fd.9csxet.cn

[S38] C++：排序
来源：http://wb.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://pq.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://cw.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ad.9csxet.cn

[S40] C++：查找元素
来源：http://ve.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bl.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://cm.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://di.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://cu.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://ql.szxytkj.cn

[S43] C++：智能指针
来源：http://lx.521024.cn

auto p = std::make_unique<int>(5);
来源：http://dh.bookmarksfly.cn

[S44] C++：引用传参
来源：http://me.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://fm.yuexingan06.cn

[S45] C++：lambda
来源：http://ns.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lp.yuexingan06.cn

[S46] C++：函数模板
来源：http://rd.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ae.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://ta.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xi.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://yg.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ok.nszjky.cn

while (std::getline(in, line)) { }
来源：http://jg.jctech888.com.cn

[S49] C++：写文件
来源：http://yh.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fa.shxzskj.cn

[S50] C++：格式化数字
来源：http://yu.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eu.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://qt.newstarts.cn

static_cast<double>(a) / b
来源：http://tw.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://dp.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://gv.wgjwhj.cn

[S53] C++：移动语义
来源：http://db.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://mz.muxihuayi.cn

[S54] C++：异常处理
来源：http://wt.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://re.shxzukj.cn

[S55] C++：结构化绑定
来源：http://pa.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tq.jctech888.com.cn

[S56] C++：optional
来源：http://ms.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://on.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://ps.huixinmuqiang.cn

constexpr int N = 10;
来源：http://el.huanxung.cn

[S58] C++：命名空间
来源：http://zq.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://wz.bookmarksfly.cn

[S59] C++：静态断言
来源：http://mb.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ke.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://bi.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fy.colortex.cn

================================================================================
来源：http://bz.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nb.haigaiapp.cn

================================================================================
来源：http://bo.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://rb.szsharing.cn

println("Hello")
来源：http://ao.hahajie.cn

[T02] Kotlin：变量
来源：http://dv.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cg.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://lh.521024.cn

"值: $b"
来源：http://zm.gzmigu.cn

[T04] Kotlin：空安全
来源：http://cv.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://wn.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://jc.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hp.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://oh.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bp.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://zr.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yu.521024.cn

[T08] Kotlin：数据类
来源：http://xn.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ux.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://ar.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://bb.szsharing.cn

[T10] Kotlin：默认参数
来源：http://fs.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eg.bjjhwx.cn

[T11] Kotlin：协程
来源：http://rn.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sf.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://xl.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://lf.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://uj.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://ug.gzmigu.cn

[T14] Kotlin：循环
来源：http://yk.9csxet.cn

for (i in 1..10) println(i)
来源：http://sy.lnxyls.cn

[T15] Kotlin：接口
来源：http://gw.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://qm.nszjky.cn

[T16] Swift：Hello World
来源：http://vm.wgjwhj.cn

print("Hello")
来源：http://zn.9csxet.cn

[T17] Swift：变量与常量
来源：http://cj.hahajie.cn

var a = 1;  let b = 2
来源：http://jv.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://zl.shtwfgs.cn

"值: \(b)"
来源：http://iu.huanxung.cn

[T19] Swift：可选绑定
来源：http://ql.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://hs.colortex.cn

[T20] Swift：数组操作
来源：http://by.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dm.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://kw.lnxyls.cn

for x in a { print(x) }
来源：http://tg.hnjuh.cn

[T22] Swift：字典
来源：http://yj.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://td.jianghongdianzi.cn

[T23] Swift：函数
来源：http://dt.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sa.newstarts.cn

[T24] Swift：闭包
来源：http://xx.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ub.asd995.cn

[T25] Swift：结构体
来源：http://dw.bjjhwx.cn

struct P { var x: Int }
来源：http://du.szxytkj.cn

[T26] Swift：类与重写
来源：http://kx.colortex.cn

class A: Base { override func f() {} }
来源：http://fe.huanxung.cn

[T27] Swift：错误处理
来源：http://qv.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://kq.9csxet.cn

[T28] Swift：枚举
来源：http://sf.szsharing.cn

enum Color { case red, green }
来源：http://eq.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://gd.lnxyls.cn

guard let x = opt else { return }
来源：http://pb.9csxet.cn

[T30] Swift：协议
来源：http://zn.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://kk.szxytkj.cn

[T31] Lua：Hello World
来源：http://yw.bookmarksfly.cn

print("Hello")
来源：http://xt.hnjuh.cn

[T32] Lua：局部变量
来源：http://sw.huixinmuqiang.cn

local a = 1
来源：http://gv.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://tf.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fr.nicolike.cn

[T34] Lua：遍历表
来源：http://ll.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dq.lnxyls.cn

[T35] Lua：字典表
来源：http://fr.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://eo.nicolike.cn

[T36] Lua：函数
来源：http://bd.huanxung.cn

function add(a, b) return a + b end
来源：http://wm.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://lo.wgjwhj.cn

"a" .. "b"
来源：http://rr.yuntaijiaju.cn

[T38] Lua：条件
来源：http://vl.asd995.cn

if x > 0 then print("正") end
来源：http://pp.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://cc.shxzskj.cn

string.find(s, "%d+")
来源：http://uq.lnxyls.cn

[T40] Lua：元表
来源：http://ly.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://hu.jctech888.com.cn

[T41] Perl：Hello World
来源：http://ag.shxzskj.cn

print "Hello\n";
来源：http://ot.shxzskj.cn

[T42] Perl：变量类型
来源：http://jc.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hi.hahajie.cn

[T43] Perl：字符串插值
来源：http://qj.9csxet.cn

"值: $a"
来源：http://mi.haigaiapp.cn

[T44] Perl：条件
来源：http://at.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://pf.9csxet.cn

[T45] Perl：数组遍历
来源：http://ht.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://dt.szsharing.cn

[T46] Perl：哈希操作
来源：http://bv.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mc.nszjky.cn

[T47] Perl：正则捕获
来源：http://hr.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gv.nicolike.cn

[T48] Perl：正则替换
来源：http://se.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://bi.521024.cn

[T49] Perl：函数
来源：http://jw.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qc.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://db.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://no.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://fh.9csxet.cn

[T51] Scala：Hello World
来源：http://vm.shxzukj.cn

println("Hello")
来源：http://qb.colortex.cn

[T52] Scala：变量
来源：http://va.lnxyls.cn

val a = 1;  var b = 2
来源：http://vd.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://ac.jctech888.com.cn

s"值: $b"
来源：http://vv.asd995.cn

[T54] Scala：集合映射
来源：http://zt.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://gq.lnxyls.cn

[T55] Scala：集合过滤
来源：http://vm.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ut.nicolike.cn

[T56] Scala：样例类
来源：http://vu.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://yz.colortex.cn

[T57] Scala：模式匹配
来源：http://sc.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wp.9csxet.cn

[T58] Scala：函数定义
来源：http://pj.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mp.yuexingan06.cn

[T59] Scala：循环
来源：http://hk.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://ny.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://gx.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cd.huixiangedu.cn

================================================================================
来源：http://sj.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://un.haigaiapp.cn

================================================================================
来源：http://cr.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://iw.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ss.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://ml.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yk.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://td.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mg.9csxet.cn

[U04] Py：变量调试打印
来源：http://le.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zx.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://oa.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://sj.newstarts.cn

[U06] Py：合并两个字典
来源：http://bm.haigaiapp.cn

{**a, **b}
来源：http://xt.hnjuh.cn

[U07] Py：反转字典键值
来源：http://wq.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://gl.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://qd.yuexingan06.cn

[y for x in nested for y in x]
来源：http://gs.asd995.cn

[U09] Py：字典取最大值的键
来源：http://ub.yuexingan06.cn

max(d, key=d.get)
来源：http://jq.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://zo.chemitech.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://an.hahajie.cn

[U11] Py：生成器表达式
来源：http://xn.hahajie.cn

(x * 2 for x in arr)
来源：http://hg.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ny.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://ob.jctech888.com.cn


<!-- 参考信息 -->