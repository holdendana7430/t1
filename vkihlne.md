代发 wailian999

read -rp "请输入: " ans
来源：http://zz.huanxung.cn

[R78] 交互式菜单
来源：http://fm.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ug.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://ix.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hh.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://xh.huixinmuqiang.cn

time ./run.sh
来源：http://jf.huixiangedu.cn

================================================================================
来源：http://hf.szsharing.cn

S. C / C++ 专题
来源：http://jw.bookmarksfly.cn

================================================================================
来源：http://az.muxihuayi.cn

[S01] C：Hello World
来源：http://fg.haigaiapp.cn

#include <stdio.h>
来源：http://um.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qx.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://nz.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://eq.yuntaijiaju.cn

[S03] C：读入整数
来源：http://fo.shxzskj.cn

int x; scanf("%d", &x);
来源：http://qz.newstarts.cn

[S04] C：字符串复制
来源：http://yu.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ze.shtwfgs.cn

[S05] C：字符串长度
来源：http://ut.szxytkj.cn

strlen(s)
来源：http://pc.bjjhwx.cn

[S06] C：字符串比较
来源：http://ad.wgjwhj.cn

strcmp(a, b) == 0
来源：http://ya.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://mh.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ok.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://hk.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hc.colortex.cn

[S09] C：结构体定义与初始化
来源：http://at.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mq.muxihuayi.cn

[S10] C：指针与解引用
来源：http://eu.colortex.cn

int *p = &a;  *p = 5;
来源：http://br.bjjhwx.cn

[S11] C：逐行读文件
来源：http://xy.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://ey.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hf.hahajie.cn

fclose(f);
来源：http://nl.asd995.cn

[S12] C：写文件
来源：http://ht.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gn.huixiangedu.cn

[S13] C：宏定义
来源：http://ay.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://up.panjiajie.cn

[S14] C：枚举
来源：http://cc.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://nb.lnxyls.cn

[S15] C：类型转换
来源：http://jr.muxihuayi.cn

(double) a / b
来源：http://ry.nicolike.cn

[S16] C：位操作置位
来源：http://dy.yuexingan06.cn

x |= (1 << 3);
来源：http://oe.newstarts.cn

[S17] C：安全拼接字符串
来源：http://vj.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jg.gzmigu.cn

[S18] C：命令行参数
来源：http://pe.yuexingan06.cn

int main(int argc, char **argv)
来源：http://uz.colortex.cn

[S19] C：快速排序
来源：http://kq.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fa.shtwfgs.cn

[S20] C：二分查找
来源：http://da.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pc.newstarts.cn

[S21] C：字符类别判断
来源：http://tt.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qp.chemitech.net.cn

[S22] C：字符串转数字
来源：http://ua.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lc.521024.cn

[S23] C：随机数
来源：http://zz.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tc.newstarts.cn

[S24] C：获取本地时间
来源：http://wp.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://os.bjjhwx.cn

[S25] C：内存拷贝
来源：http://wo.muxihuayi.cn

memcpy(dst, src, n);
来源：http://sl.shtwfgs.cn

[S26] C：内存清零
来源：http://jp.hahajie.cn

memset(a, 0, sizeof a);
来源：http://ar.jctech888.com.cn

[S27] C：定义常量
来源：http://cs.shxzskj.cn

const double PI = 3.14159;
来源：http://gg.hahajie.cn

[S28] C：静态变量
来源：http://yf.newstarts.cn

static int counter = 0;
来源：http://ua.asd995.cn

[S29] C：变参函数
来源：http://aa.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fq.9csxet.cn

[S30] C：头文件保护
来源：http://ij.bjjhwx.cn

#ifndef X_H
来源：http://lh.bjjhwx.cn

#define X_H
来源：http://xy.huanxung.cn

#endif
来源：http://tu.521024.cn

[S31] C++：Hello World
来源：http://tk.newstarts.cn

#include <iostream>
来源：http://ie.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://hf.9csxet.cn

[S32] C++：字符串
来源：http://wo.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://hw.asd995.cn

[S33] C++：vector 增删
来源：http://bp.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hd.lnxyls.cn

[S34] C++：遍历 vector
来源：http://yz.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://vt.wgjwhj.cn

[S35] C++：map
来源：http://ax.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ln.szsharing.cn

[S36] C++：unordered_map
来源：http://cn.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qi.nszjky.cn

[S37] C++：set
来源：http://nr.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://na.muxihuayi.cn

[S38] C++：排序
来源：http://mk.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://jl.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://mi.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://js.huanxung.cn

[S40] C++：查找元素
来源：http://mp.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bb.nszjky.cn

[S41] C++：类与构造函数
来源：http://on.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fq.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://ea.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://vg.lnxyls.cn

[S43] C++：智能指针
来源：http://gg.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://tq.9csxet.cn

[S44] C++：引用传参
来源：http://gb.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://uv.nszjky.cn

[S45] C++：lambda
来源：http://yy.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qq.bookmarksfly.cn

[S46] C++：函数模板
来源：http://ai.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jo.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://gc.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dp.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://dj.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bj.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://go.nicolike.cn

[S49] C++：写文件
来源：http://yt.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uf.asd995.cn

[S50] C++：格式化数字
来源：http://if.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ol.shxzskj.cn

[S51] C++：显式类型转换
来源：http://fs.nicolike.cn

static_cast<double>(a) / b
来源：http://fy.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://ho.9csxet.cn

int size() const noexcept { return n_; }
来源：http://va.shxzskj.cn

[S53] C++：移动语义
来源：http://nt.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://lq.szsharing.cn

[S54] C++：异常处理
来源：http://md.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://av.panjiajie.cn

[S55] C++：结构化绑定
来源：http://yq.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nd.chemitech.net.cn

[S56] C++：optional
来源：http://wu.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xn.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://iy.shxzskj.cn

constexpr int N = 10;
来源：http://qa.hahajie.cn

[S58] C++：命名空间
来源：http://vw.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://we.newstarts.cn

[S59] C++：静态断言
来源：http://vw.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fo.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://tp.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ds.hnjuh.cn

================================================================================
来源：http://li.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gd.colortex.cn

================================================================================
来源：http://on.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://jb.shtwfgs.cn

println("Hello")
来源：http://sn.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://ig.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jt.521024.cn

[T03] Kotlin：字符串模板
来源：http://bf.yuexingan06.cn

"值: $b"
来源：http://fx.gzmigu.cn

[T04] Kotlin：空安全
来源：http://aq.newstarts.cn

val n: String? = null;  n?.length
来源：http://bl.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://tr.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iv.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://br.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zy.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://zi.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://be.asd995.cn

[T08] Kotlin：数据类
来源：http://vs.521024.cn

data class User(val name: String, val age: Int)
来源：http://of.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://jq.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://ys.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ge.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bz.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ti.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hq.colortex.cn

[T12] Kotlin：解构声明
来源：http://tb.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://cw.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://is.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://et.yuexingan06.cn

[T14] Kotlin：循环
来源：http://jq.lnxyls.cn

for (i in 1..10) println(i)
来源：http://dw.9csxet.cn

[T15] Kotlin：接口
来源：http://jf.hahajie.cn

interface Shape { fun area(): Double }
来源：http://ej.521024.cn

[T16] Swift：Hello World
来源：http://mn.hnjuh.cn

print("Hello")
来源：http://mi.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://ov.asd995.cn

var a = 1;  let b = 2
来源：http://gj.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://ck.huixinmuqiang.cn

"值: \(b)"
来源：http://hq.asd995.cn

[T19] Swift：可选绑定
来源：http://zs.shxzukj.cn

if let n = opt { print(n) }
来源：http://ya.huanxung.cn

[T20] Swift：数组操作
来源：http://wc.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ki.muxihuayi.cn

[T21] Swift：遍历
来源：http://pc.521024.cn

for x in a { print(x) }
来源：http://qd.bookmarksfly.cn

[T22] Swift：字典
来源：http://iz.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sq.asd995.cn

[T23] Swift：函数
来源：http://sh.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yf.hnjuh.cn

[T24] Swift：闭包
来源：http://wu.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://re.szsharing.cn

[T25] Swift：结构体
来源：http://ig.szxytkj.cn

struct P { var x: Int }
来源：http://st.521024.cn

[T26] Swift：类与重写
来源：http://tu.newstarts.cn

class A: Base { override func f() {} }
来源：http://ll.haigaiapp.cn

[T27] Swift：错误处理
来源：http://ym.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://md.wgjwhj.cn

[T28] Swift：枚举
来源：http://yg.huixinmuqiang.cn

enum Color { case red, green }
来源：http://dk.colortex.cn

[T29] Swift：guard 提前返回
来源：http://ae.bjjhwx.cn

guard let x = opt else { return }
来源：http://xv.jianghongdianzi.cn

[T30] Swift：协议
来源：http://bi.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://gc.colortex.cn

[T31] Lua：Hello World
来源：http://ut.huixinmuqiang.cn

print("Hello")
来源：http://gl.haigaiapp.cn

[T32] Lua：局部变量
来源：http://ue.bjjhwx.cn

local a = 1
来源：http://ql.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://ge.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vv.huanxung.cn

[T34] Lua：遍历表
来源：http://si.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ms.hnjuh.cn

[T35] Lua：字典表
来源：http://xv.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://mq.haigaiapp.cn

[T36] Lua：函数
来源：http://jx.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://ar.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://io.9csxet.cn

"a" .. "b"
来源：http://jn.bjjhwx.cn

[T38] Lua：条件
来源：http://qx.shxzskj.cn

if x > 0 then print("正") end
来源：http://ku.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://rs.bjjhwx.cn

string.find(s, "%d+")
来源：http://kz.haigaiapp.cn

[T40] Lua：元表
来源：http://iu.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://kw.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://yd.bjjhwx.cn

print "Hello\n";
来源：http://lt.huanxung.cn

[T42] Perl：变量类型
来源：http://fu.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vt.hnjuh.cn

[T43] Perl：字符串插值
来源：http://hn.panjiajie.cn

"值: $a"
来源：http://xr.nszjky.cn

[T44] Perl：条件
来源：http://ga.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://fh.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://so.asd995.cn

for my $x (@arr) { print $x; }
来源：http://ky.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://cs.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rz.szsharing.cn

[T47] Perl：正则捕获
来源：http://in.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sd.hahajie.cn

[T48] Perl：正则替换
来源：http://xj.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://wl.newstarts.cn

[T49] Perl：函数
来源：http://tf.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ie.hahajie.cn

[T50] Perl：逐行读文件
来源：http://yv.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tm.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://cb.shtwfgs.cn

[T51] Scala：Hello World
来源：http://rl.shxzukj.cn

println("Hello")
来源：http://fd.hnjuh.cn

[T52] Scala：变量
来源：http://ud.muxihuayi.cn

val a = 1;  var b = 2
来源：http://mv.hnjuh.cn

[T53] Scala：字符串插值
来源：http://mp.nszjky.cn

s"值: $b"
来源：http://pf.521024.cn

[T54] Scala：集合映射
来源：http://pz.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://gg.szsharing.cn

[T55] Scala：集合过滤
来源：http://uc.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cg.szxytkj.cn

[T56] Scala：样例类
来源：http://ba.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://cs.shxzskj.cn

[T57] Scala：模式匹配
来源：http://tt.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vr.shxzukj.cn

[T58] Scala：函数定义
来源：http://ko.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ku.nicolike.cn

[T59] Scala：循环
来源：http://jr.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ku.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://ti.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tv.chemitech.net.cn

================================================================================
来源：http://rn.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xk.521024.cn

================================================================================
来源：http://ct.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://ew.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tz.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://al.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vg.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://jm.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ca.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://rq.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rw.huanxung.cn

[U05] Py：列表去重且保序
来源：http://ax.nicolike.cn

list(dict.fromkeys(arr))
来源：http://tr.szsharing.cn

[U06] Py：合并两个字典
来源：http://db.chemitech.net.cn

{**a, **b}
来源：http://bo.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://xq.colortex.cn

{v: k for k, v in d.items()}
来源：http://oo.colortex.cn

[U08] Py：展平二维列表
来源：http://sh.shtwfgs.cn

[y for x in nested for y in x]
来源：http://tt.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://br.muxihuayi.cn

max(d, key=d.get)
来源：http://at.huanxung.cn

[U10] Py：按值排序字典
来源：http://ur.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bl.9csxet.cn

[U11] Py：生成器表达式
来源：http://ng.gzmigu.cn

(x * 2 for x in arr)
来源：http://iw.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ak.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://ob.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://rz.jctech888.com.cn

deque(maxlen=10)
来源：http://nr.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://wt.nszjky.cn

defaultdict(list)
来源：http://pl.jctech888.com.cn

[U15] Py：高精度计时
来源：http://tc.chemitech.net.cn

t = time.perf_counter()
来源：http://xu.gzmigu.cn

[U16] Py：命令行参数解析
来源：http://bw.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yn.shxzukj.cn

[U17] Py：初始化日志
来源：http://xu.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://vy.huanxung.cn

[U18] Py：预编译正则
来源：http://xk.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://ty.bjjhwx.cn


<!-- 参考信息 -->