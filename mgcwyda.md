代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://nn.lnxyls.cn

[R76] 使用临时文件
来源：http://mk.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cl.huanxung.cn

[R77] 读取用户输入
来源：http://bm.yuexingan06.cn

read -rp "请输入: " ans
来源：http://hj.asd995.cn

[R78] 交互式菜单
来源：http://oy.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bc.gzmigu.cn

[R79] 解析命令行选项
来源：http://ed.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mz.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://yh.wgjwhj.cn

time ./run.sh
来源：http://sk.colortex.cn

================================================================================
来源：http://yj.yuexingan06.cn

S. C / C++ 专题
来源：http://xo.gzmigu.cn

================================================================================
来源：http://ed.gzmigu.cn

[S01] C：Hello World
来源：http://zf.shtwfgs.cn

#include <stdio.h>
来源：http://hx.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tg.asd995.cn

[S02] C：变量与格式化输出
来源：http://wx.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://qg.nicolike.cn

[S03] C：读入整数
来源：http://kz.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://dw.haigaiapp.cn

[S04] C：字符串复制
来源：http://lr.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ep.lnxyls.cn

[S05] C：字符串长度
来源：http://tg.521024.cn

strlen(s)
来源：http://bn.lnxyls.cn

[S06] C：字符串比较
来源：http://iv.nicolike.cn

strcmp(a, b) == 0
来源：http://ry.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://sr.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mb.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://dq.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uo.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://mz.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cf.yuexingan06.cn

[S10] C：指针与解引用
来源：http://ez.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://pd.yuexingan06.cn

[S11] C：逐行读文件
来源：http://br.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://to.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ts.szsharing.cn

fclose(f);
来源：http://cr.jctech888.com.cn

[S12] C：写文件
来源：http://no.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zc.huanxung.cn

[S13] C：宏定义
来源：http://ri.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zn.nicolike.cn

[S14] C：枚举
来源：http://ll.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://st.huixiangedu.cn

[S15] C：类型转换
来源：http://zq.shxzukj.cn

(double) a / b
来源：http://xt.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://ft.panjiajie.cn

x |= (1 << 3);
来源：http://md.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://gy.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sn.shtwfgs.cn

[S18] C：命令行参数
来源：http://hi.shxzukj.cn

int main(int argc, char **argv)
来源：http://po.szxytkj.cn

[S19] C：快速排序
来源：http://jv.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fb.bookmarksfly.cn

[S20] C：二分查找
来源：http://aj.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dl.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://dw.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lh.shxzukj.cn

[S22] C：字符串转数字
来源：http://oe.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://os.nicolike.cn

[S23] C：随机数
来源：http://qo.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ce.521024.cn

[S24] C：获取本地时间
来源：http://ms.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xj.hahajie.cn

[S25] C：内存拷贝
来源：http://mv.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://zp.szxytkj.cn

[S26] C：内存清零
来源：http://if.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://hx.521024.cn

[S27] C：定义常量
来源：http://mx.chemitech.net.cn

const double PI = 3.14159;
来源：http://qc.shxzukj.cn

[S28] C：静态变量
来源：http://xs.9csxet.cn

static int counter = 0;
来源：http://ad.newstarts.cn

[S29] C：变参函数
来源：http://bb.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hx.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://jy.huixiangedu.cn

#ifndef X_H
来源：http://eo.shxzukj.cn

#define X_H
来源：http://rq.colortex.cn

#endif
来源：http://ev.521024.cn

[S31] C++：Hello World
来源：http://jl.huixiangedu.cn

#include <iostream>
来源：http://lg.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://su.szxytkj.cn

[S32] C++：字符串
来源：http://sa.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://wc.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://po.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://db.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ld.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ad.huanxung.cn

[S35] C++：map
来源：http://je.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kp.nszjky.cn

[S36] C++：unordered_map
来源：http://ie.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lf.muxihuayi.cn

[S37] C++：set
来源：http://bm.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ba.9csxet.cn

[S38] C++：排序
来源：http://px.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://ja.colortex.cn

[S39] C++：自定义比较器排序
来源：http://hu.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dm.shxzukj.cn

[S40] C++：查找元素
来源：http://vk.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vx.asd995.cn

[S41] C++：类与构造函数
来源：http://yn.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ni.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://hu.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://qt.nicolike.cn

[S43] C++：智能指针
来源：http://cw.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ih.newstarts.cn

[S44] C++：引用传参
来源：http://dc.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://fz.asd995.cn

[S45] C++：lambda
来源：http://lh.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xl.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://uz.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vj.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://vc.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ul.hnjuh.cn

[S48] C++：逐行读文件
来源：http://mw.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yq.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://bd.huanxung.cn

[S49] C++：写文件
来源：http://os.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dp.nszjky.cn

[S50] C++：格式化数字
来源：http://km.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kg.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://an.hnjuh.cn

static_cast<double>(a) / b
来源：http://bk.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://fj.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://dj.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://tq.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://yl.muxihuayi.cn

[S54] C++：异常处理
来源：http://lw.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hc.shxzukj.cn

[S55] C++：结构化绑定
来源：http://zf.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://up.bjjhwx.cn

[S56] C++：optional
来源：http://yw.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ck.szsharing.cn

[S57] C++：编译期常量
来源：http://yc.gzmigu.cn

constexpr int N = 10;
来源：http://wz.asd995.cn

[S58] C++：命名空间
来源：http://et.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://nc.bjjhwx.cn

[S59] C++：静态断言
来源：http://rf.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ea.colortex.cn

[S60] C++：遍历并删除元素
来源：http://aw.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wn.szsharing.cn

================================================================================
来源：http://ho.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yn.yuexingan06.cn

================================================================================
来源：http://so.newstarts.cn

[T01] Kotlin：Hello World
来源：http://ae.huixinmuqiang.cn

println("Hello")
来源：http://ux.wgjwhj.cn

[T02] Kotlin：变量
来源：http://bf.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jx.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://tc.newstarts.cn

"值: $b"
来源：http://xc.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://wz.hahajie.cn

val n: String? = null;  n?.length
来源：http://qo.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://xf.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wx.colortex.cn

[T06] Kotlin：集合映射
来源：http://bz.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://db.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://iu.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mt.9csxet.cn

[T08] Kotlin：数据类
来源：http://ab.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://ws.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://ep.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://yw.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://vs.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xo.nicolike.cn

[T11] Kotlin：协程
来源：http://ac.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://th.huanxung.cn

[T12] Kotlin：解构声明
来源：http://fv.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://pz.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://ec.hahajie.cn

val m = mapOf("a" to 1)
来源：http://sd.gzmigu.cn

[T14] Kotlin：循环
来源：http://sh.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://en.huixiangedu.cn

[T15] Kotlin：接口
来源：http://kq.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://db.9csxet.cn

[T16] Swift：Hello World
来源：http://fi.colortex.cn

print("Hello")
来源：http://zw.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ow.muxihuayi.cn

var a = 1;  let b = 2
来源：http://wh.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://jo.asd995.cn

"值: \(b)"
来源：http://dd.newstarts.cn

[T19] Swift：可选绑定
来源：http://ql.hnjuh.cn

if let n = opt { print(n) }
来源：http://wf.colortex.cn

[T20] Swift：数组操作
来源：http://jz.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qy.newstarts.cn

[T21] Swift：遍历
来源：http://sl.yuexingan06.cn

for x in a { print(x) }
来源：http://is.jctech888.com.cn

[T22] Swift：字典
来源：http://fw.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pb.hnjuh.cn

[T23] Swift：函数
来源：http://yw.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kp.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://qg.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zx.hahajie.cn

[T25] Swift：结构体
来源：http://zl.haigaiapp.cn

struct P { var x: Int }
来源：http://wf.shxzukj.cn

[T26] Swift：类与重写
来源：http://bt.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://ji.jctech888.com.cn

[T27] Swift：错误处理
来源：http://uy.hahajie.cn

do { try f() } catch { print(error) }
来源：http://mk.bookmarksfly.cn

[T28] Swift：枚举
来源：http://vg.haigaiapp.cn

enum Color { case red, green }
来源：http://tp.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://sa.nszjky.cn

guard let x = opt else { return }
来源：http://lg.yuntaijiaju.cn

[T30] Swift：协议
来源：http://nm.asd995.cn

protocol Shape { func area() -> Double }
来源：http://kd.newstarts.cn

[T31] Lua：Hello World
来源：http://gm.szsharing.cn

print("Hello")
来源：http://vh.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://eb.jctech888.com.cn

local a = 1
来源：http://gt.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://gq.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iq.colortex.cn

[T34] Lua：遍历表
来源：http://wj.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mw.bookmarksfly.cn

[T35] Lua：字典表
来源：http://hf.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://tp.huanxung.cn

[T36] Lua：函数
来源：http://bq.huanxung.cn

function add(a, b) return a + b end
来源：http://if.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://wo.huixiangedu.cn

"a" .. "b"
来源：http://oc.shxzskj.cn

[T38] Lua：条件
来源：http://on.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://cg.shxzskj.cn

[T39] Lua：模式匹配
来源：http://ty.asd995.cn

string.find(s, "%d+")
来源：http://gn.panjiajie.cn

[T40] Lua：元表
来源：http://ku.nicolike.cn

setmetatable({}, { __index = base })
来源：http://am.9csxet.cn

[T41] Perl：Hello World
来源：http://nd.nszjky.cn

print "Hello\n";
来源：http://cy.panjiajie.cn

[T42] Perl：变量类型
来源：http://ci.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xn.szxytkj.cn

[T43] Perl：字符串插值
来源：http://di.panjiajie.cn

"值: $a"
来源：http://rc.bjjhwx.cn

[T44] Perl：条件
来源：http://xn.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://af.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://zo.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://vl.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://fl.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ua.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ut.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://me.shxzskj.cn

[T48] Perl：正则替换
来源：http://ld.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://so.asd995.cn

[T49] Perl：函数
来源：http://ur.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://le.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://mi.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yi.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://yk.nicolike.cn

[T51] Scala：Hello World
来源：http://nl.yuntaijiaju.cn

println("Hello")
来源：http://pd.shtwfgs.cn

[T52] Scala：变量
来源：http://rt.shxzskj.cn

val a = 1;  var b = 2
来源：http://rr.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://lr.lnxyls.cn

s"值: $b"
来源：http://hi.hahajie.cn

[T54] Scala：集合映射
来源：http://sb.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://wt.asd995.cn

[T55] Scala：集合过滤
来源：http://be.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qo.nszjky.cn

[T56] Scala：样例类
来源：http://tr.hahajie.cn

case class User(name: String, age: Int)
来源：http://jy.panjiajie.cn

[T57] Scala：模式匹配
来源：http://ar.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ok.huixiangedu.cn

[T58] Scala：函数定义
来源：http://bx.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yx.huixinmuqiang.cn

[T59] Scala：循环
来源：http://zl.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://fs.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://tg.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fb.hahajie.cn

================================================================================
来源：http://on.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mq.huanxung.cn

================================================================================
来源：http://mt.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://zq.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nv.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://lv.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dv.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://bq.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ll.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://qo.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ix.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://jd.asd995.cn

list(dict.fromkeys(arr))
来源：http://yq.panjiajie.cn

[U06] Py：合并两个字典
来源：http://my.colortex.cn

{**a, **b}
来源：http://wl.panjiajie.cn

[U07] Py：反转字典键值
来源：http://cc.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://jj.shxzskj.cn

[U08] Py：展平二维列表
来源：http://lj.huanxung.cn

[y for x in nested for y in x]
来源：http://yd.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://jc.521024.cn

max(d, key=d.get)
来源：http://rs.hnjuh.cn

[U10] Py：按值排序字典
来源：http://za.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dj.gzmigu.cn

[U11] Py：生成器表达式
来源：http://sq.wgjwhj.cn

(x * 2 for x in arr)
来源：http://hi.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yz.asd995.cn

Counter(arr).most_common(3)
来源：http://ep.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://pm.asd995.cn

deque(maxlen=10)
来源：http://mr.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://so.haigaiapp.cn

defaultdict(list)
来源：http://cf.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://cs.yuntaijiaju.cn

t = time.perf_counter()
来源：http://wf.521024.cn

[U16] Py：命令行参数解析
来源：http://do.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kl.9csxet.cn


<!-- 参考信息 -->