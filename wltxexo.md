代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://ev.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://hb.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yf.haigaiapp.cn

[R73] 分割大日志
来源：http://pp.yuexingan06.cn

split -l 1000 big.log part_
来源：http://op.shxzskj.cn

[R74] 批量重命名
来源：http://aa.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bx.nszjky.cn

[R75] 导出环境变量
来源：http://vw.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://ow.szxytkj.cn

[R76] 使用临时文件
来源：http://rw.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fd.huixiangedu.cn

[R77] 读取用户输入
来源：http://rj.shxzukj.cn

read -rp "请输入: " ans
来源：http://fm.lnxyls.cn

[R78] 交互式菜单
来源：http://jz.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cq.wgjwhj.cn

[R79] 解析命令行选项
来源：http://la.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ng.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://ya.shxzskj.cn

time ./run.sh
来源：http://iq.nszjky.cn

================================================================================
来源：http://hv.shtwfgs.cn

S. C / C++ 专题
来源：http://tg.hahajie.cn

================================================================================
来源：http://pb.muxihuayi.cn

[S01] C：Hello World
来源：http://qs.huixinmuqiang.cn

#include <stdio.h>
来源：http://kk.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gh.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://hq.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://zc.hahajie.cn

[S03] C：读入整数
来源：http://nz.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://ah.bookmarksfly.cn

[S04] C：字符串复制
来源：http://ym.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xq.bookmarksfly.cn

[S05] C：字符串长度
来源：http://zo.521024.cn

strlen(s)
来源：http://vk.nszjky.cn

[S06] C：字符串比较
来源：http://fp.wgjwhj.cn

strcmp(a, b) == 0
来源：http://jn.colortex.cn

[S07] C：数组遍历求和
来源：http://fb.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wu.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://sx.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iv.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://oq.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cp.nszjky.cn

[S10] C：指针与解引用
来源：http://vf.nicolike.cn

int *p = &a;  *p = 5;
来源：http://yb.huixiangedu.cn

[S11] C：逐行读文件
来源：http://fs.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://or.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sy.chemitech.net.cn

fclose(f);
来源：http://zo.bjjhwx.cn

[S12] C：写文件
来源：http://qg.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dx.chemitech.net.cn

[S13] C：宏定义
来源：http://sb.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tr.bookmarksfly.cn

[S14] C：枚举
来源：http://kc.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://it.nicolike.cn

[S15] C：类型转换
来源：http://gk.hnjuh.cn

(double) a / b
来源：http://kn.jctech888.com.cn

[S16] C：位操作置位
来源：http://vz.yuntaijiaju.cn

x |= (1 << 3);
来源：http://ea.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://zk.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xj.huixiangedu.cn

[S18] C：命令行参数
来源：http://qx.nicolike.cn

int main(int argc, char **argv)
来源：http://kj.yuntaijiaju.cn

[S19] C：快速排序
来源：http://xa.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tj.lnxyls.cn

[S20] C：二分查找
来源：http://zh.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://px.asd995.cn

[S21] C：字符类别判断
来源：http://yp.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dv.haigaiapp.cn

[S22] C：字符串转数字
来源：http://rf.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kk.huixinmuqiang.cn

[S23] C：随机数
来源：http://zy.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fs.colortex.cn

[S24] C：获取本地时间
来源：http://fk.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mq.newstarts.cn

[S25] C：内存拷贝
来源：http://bq.szsharing.cn

memcpy(dst, src, n);
来源：http://bw.shxzskj.cn

[S26] C：内存清零
来源：http://zx.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://ff.lnxyls.cn

[S27] C：定义常量
来源：http://ii.lnxyls.cn

const double PI = 3.14159;
来源：http://qp.szsharing.cn

[S28] C：静态变量
来源：http://td.newstarts.cn

static int counter = 0;
来源：http://bn.huixinmuqiang.cn

[S29] C：变参函数
来源：http://kq.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gm.gzmigu.cn

[S30] C：头文件保护
来源：http://ej.nicolike.cn

#ifndef X_H
来源：http://rr.bjjhwx.cn

#define X_H
来源：http://cd.bjjhwx.cn

#endif
来源：http://sd.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://hg.chemitech.net.cn

#include <iostream>
来源：http://qz.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://zw.shxzskj.cn

[S32] C++：字符串
来源：http://af.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://rc.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://zr.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mo.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://za.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://vf.huixinmuqiang.cn

[S35] C++：map
来源：http://oa.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ot.huixiangedu.cn

[S36] C++：unordered_map
来源：http://gn.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sc.gzmigu.cn

[S37] C++：set
来源：http://lw.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yb.9csxet.cn

[S38] C++：排序
来源：http://wr.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://gc.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ug.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ye.wgjwhj.cn

[S40] C++：查找元素
来源：http://pt.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ob.hnjuh.cn

[S41] C++：类与构造函数
来源：http://ok.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tq.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://jf.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ox.hnjuh.cn

[S43] C++：智能指针
来源：http://vz.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://tg.nicolike.cn

[S44] C++：引用传参
来源：http://fp.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://no.colortex.cn

[S45] C++：lambda
来源：http://jz.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ig.wgjwhj.cn

[S46] C++：函数模板
来源：http://kp.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bm.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://gk.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vk.gzmigu.cn

[S48] C++：逐行读文件
来源：http://lb.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kb.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://pp.haigaiapp.cn

[S49] C++：写文件
来源：http://ik.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ch.newstarts.cn

[S50] C++：格式化数字
来源：http://dx.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kb.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://tv.newstarts.cn

static_cast<double>(a) / b
来源：http://jp.colortex.cn

[S52] C++：const 与 noexcept
来源：http://el.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://zh.newstarts.cn

[S53] C++：移动语义
来源：http://pp.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://mt.nicolike.cn

[S54] C++：异常处理
来源：http://bp.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mo.newstarts.cn

[S55] C++：结构化绑定
来源：http://fq.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jw.muxihuayi.cn

[S56] C++：optional
来源：http://tn.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ml.nicolike.cn

[S57] C++：编译期常量
来源：http://km.szsharing.cn

constexpr int N = 10;
来源：http://fi.gzmigu.cn

[S58] C++：命名空间
来源：http://ju.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://ys.chemitech.net.cn

[S59] C++：静态断言
来源：http://en.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rw.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://sq.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zy.hnjuh.cn

================================================================================
来源：http://ol.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ig.hnjuh.cn

================================================================================
来源：http://cs.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://ee.huixinmuqiang.cn

println("Hello")
来源：http://pq.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://zt.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jv.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://bk.yuntaijiaju.cn

"值: $b"
来源：http://om.lnxyls.cn

[T04] Kotlin：空安全
来源：http://wl.shxzskj.cn

val n: String? = null;  n?.length
来源：http://wr.521024.cn

[T05] Kotlin：when 表达式
来源：http://nq.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vy.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://gz.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pf.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://lp.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zf.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://uc.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://ie.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://ni.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://ew.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://lk.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ia.szsharing.cn

[T11] Kotlin：协程
来源：http://zu.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bv.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://uh.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://vh.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://fv.szsharing.cn

val m = mapOf("a" to 1)
来源：http://mp.chemitech.net.cn

[T14] Kotlin：循环
来源：http://um.huanxung.cn

for (i in 1..10) println(i)
来源：http://ox.szxytkj.cn

[T15] Kotlin：接口
来源：http://ch.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://ni.hnjuh.cn

[T16] Swift：Hello World
来源：http://se.9csxet.cn

print("Hello")
来源：http://ze.asd995.cn

[T17] Swift：变量与常量
来源：http://ro.nicolike.cn

var a = 1;  let b = 2
来源：http://qz.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://sd.bookmarksfly.cn

"值: \(b)"
来源：http://la.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://lx.lnxyls.cn

if let n = opt { print(n) }
来源：http://xs.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://xl.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ni.huanxung.cn

[T21] Swift：遍历
来源：http://dx.nicolike.cn

for x in a { print(x) }
来源：http://hj.haigaiapp.cn

[T22] Swift：字典
来源：http://cl.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mk.asd995.cn

[T23] Swift：函数
来源：http://bt.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sn.yuexingan06.cn

[T24] Swift：闭包
来源：http://gb.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://id.lnxyls.cn

[T25] Swift：结构体
来源：http://lh.gzmigu.cn

struct P { var x: Int }
来源：http://fd.jctech888.com.cn

[T26] Swift：类与重写
来源：http://kx.lnxyls.cn

class A: Base { override func f() {} }
来源：http://eh.szsharing.cn

[T27] Swift：错误处理
来源：http://zl.hahajie.cn

do { try f() } catch { print(error) }
来源：http://ej.bookmarksfly.cn

[T28] Swift：枚举
来源：http://ja.shxzukj.cn

enum Color { case red, green }
来源：http://ld.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://mw.bjjhwx.cn

guard let x = opt else { return }
来源：http://eb.yuntaijiaju.cn

[T30] Swift：协议
来源：http://kd.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://ho.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://sp.muxihuayi.cn

print("Hello")
来源：http://rx.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://fg.bookmarksfly.cn

local a = 1
来源：http://dh.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://bl.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wq.huanxung.cn

[T34] Lua：遍历表
来源：http://fx.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://un.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://nq.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://ho.panjiajie.cn

[T36] Lua：函数
来源：http://bm.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://xt.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://zj.nszjky.cn

"a" .. "b"
来源：http://gq.szsharing.cn

[T38] Lua：条件
来源：http://qp.9csxet.cn

if x > 0 then print("正") end
来源：http://jm.szsharing.cn

[T39] Lua：模式匹配
来源：http://by.nicolike.cn

string.find(s, "%d+")
来源：http://eo.hnjuh.cn

[T40] Lua：元表
来源：http://qf.asd995.cn

setmetatable({}, { __index = base })
来源：http://dj.jctech888.com.cn

[T41] Perl：Hello World
来源：http://zl.colortex.cn

print "Hello\n";
来源：http://lt.shxzukj.cn

[T42] Perl：变量类型
来源：http://rn.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cz.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://wq.hnjuh.cn

"值: $a"
来源：http://ur.shxzukj.cn

[T44] Perl：条件
来源：http://tv.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://uo.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://sq.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://ju.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://zt.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tq.newstarts.cn

[T47] Perl：正则捕获
来源：http://xx.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hl.asd995.cn

[T48] Perl：正则替换
来源：http://ln.521024.cn

$s =~ s/old/new/g;
来源：http://vr.9csxet.cn

[T49] Perl：函数
来源：http://cy.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eb.huanxung.cn

[T50] Perl：逐行读文件
来源：http://ak.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ay.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://px.hahajie.cn

[T51] Scala：Hello World
来源：http://vo.szxytkj.cn

println("Hello")
来源：http://gp.hnjuh.cn

[T52] Scala：变量
来源：http://id.wgjwhj.cn

val a = 1;  var b = 2
来源：http://cz.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://qd.panjiajie.cn

s"值: $b"
来源：http://xo.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://pm.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://qj.shxzskj.cn

[T55] Scala：集合过滤
来源：http://sc.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ig.szsharing.cn

[T56] Scala：样例类
来源：http://uw.hahajie.cn

case class User(name: String, age: Int)
来源：http://is.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://jt.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dq.hahajie.cn

[T58] Scala：函数定义
来源：http://uf.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://am.muxihuayi.cn

[T59] Scala：循环
来源：http://ki.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://gv.szxytkj.cn

[T60] Scala：折叠
来源：http://xg.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zs.haigaiapp.cn

================================================================================
来源：http://yy.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cq.shtwfgs.cn

================================================================================
来源：http://oy.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://qu.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mq.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://mv.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dx.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://gw.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oq.panjiajie.cn

[U04] Py：变量调试打印
来源：http://ng.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jd.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://se.nicolike.cn

list(dict.fromkeys(arr))
来源：http://kw.shxzukj.cn

[U06] Py：合并两个字典
来源：http://ya.szxytkj.cn

{**a, **b}
来源：http://qi.panjiajie.cn

[U07] Py：反转字典键值
来源：http://co.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://ro.colortex.cn

[U08] Py：展平二维列表
来源：http://dz.nszjky.cn

[y for x in nested for y in x]
来源：http://mm.asd995.cn

[U09] Py：字典取最大值的键
来源：http://sp.shtwfgs.cn

max(d, key=d.get)
来源：http://jo.shxzukj.cn

[U10] Py：按值排序字典
来源：http://tc.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uu.newstarts.cn

[U11] Py：生成器表达式
来源：http://iw.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://ek.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wf.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://zm.muxihuayi.cn


<!-- 参考信息 -->