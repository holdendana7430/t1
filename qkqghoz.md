代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://eq.hahajie.cn

[R76] 使用临时文件
来源：http://nk.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ks.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://fz.shxzukj.cn

read -rp "请输入: " ans
来源：http://li.huixiangedu.cn

[R78] 交互式菜单
来源：http://zt.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jw.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://hj.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tz.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://bt.hnjuh.cn

time ./run.sh
来源：http://wp.panjiajie.cn

================================================================================
来源：http://lw.yuexingan06.cn

S. C / C++ 专题
来源：http://kt.newstarts.cn

================================================================================
来源：http://kg.huixiangedu.cn

[S01] C：Hello World
来源：http://ij.nicolike.cn

#include <stdio.h>
来源：http://sw.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://em.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://zo.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://sg.chemitech.net.cn

[S03] C：读入整数
来源：http://vc.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://br.shxzukj.cn

[S04] C：字符串复制
来源：http://ec.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jk.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://ax.szsharing.cn

strlen(s)
来源：http://hq.shxzukj.cn

[S06] C：字符串比较
来源：http://pa.muxihuayi.cn

strcmp(a, b) == 0
来源：http://nd.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://yn.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://la.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://ge.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mu.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://im.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ok.hahajie.cn

[S10] C：指针与解引用
来源：http://ow.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ya.asd995.cn

[S11] C：逐行读文件
来源：http://op.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://vo.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jh.panjiajie.cn

fclose(f);
来源：http://rm.colortex.cn

[S12] C：写文件
来源：http://xb.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ms.yuntaijiaju.cn

[S13] C：宏定义
来源：http://rw.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qp.muxihuayi.cn

[S14] C：枚举
来源：http://pa.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://mr.yuntaijiaju.cn

[S15] C：类型转换
来源：http://rh.jianghongdianzi.cn

(double) a / b
来源：http://zg.szxytkj.cn

[S16] C：位操作置位
来源：http://fl.wgjwhj.cn

x |= (1 << 3);
来源：http://eq.newstarts.cn

[S17] C：安全拼接字符串
来源：http://bs.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yv.hahajie.cn

[S18] C：命令行参数
来源：http://ve.wgjwhj.cn

int main(int argc, char **argv)
来源：http://mk.panjiajie.cn

[S19] C：快速排序
来源：http://jt.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yo.jctech888.com.cn

[S20] C：二分查找
来源：http://zw.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ye.shxzskj.cn

[S21] C：字符类别判断
来源：http://rq.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://le.jctech888.com.cn

[S22] C：字符串转数字
来源：http://ag.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rd.colortex.cn

[S23] C：随机数
来源：http://dz.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hm.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://bw.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dj.hahajie.cn

[S25] C：内存拷贝
来源：http://we.nicolike.cn

memcpy(dst, src, n);
来源：http://vg.shxzukj.cn

[S26] C：内存清零
来源：http://zt.521024.cn

memset(a, 0, sizeof a);
来源：http://ig.jctech888.com.cn

[S27] C：定义常量
来源：http://rj.shtwfgs.cn

const double PI = 3.14159;
来源：http://si.asd995.cn

[S28] C：静态变量
来源：http://nj.shtwfgs.cn

static int counter = 0;
来源：http://ej.szsharing.cn

[S29] C：变参函数
来源：http://xx.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fq.hahajie.cn

[S30] C：头文件保护
来源：http://tk.9csxet.cn

#ifndef X_H
来源：http://bn.shxzukj.cn

#define X_H
来源：http://ug.yuexingan06.cn

#endif
来源：http://qo.newstarts.cn

[S31] C++：Hello World
来源：http://dz.521024.cn

#include <iostream>
来源：http://wt.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://rc.muxihuayi.cn

[S32] C++：字符串
来源：http://md.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://rz.szxytkj.cn

[S33] C++：vector 增删
来源：http://gd.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zr.szxytkj.cn

[S34] C++：遍历 vector
来源：http://di.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://xv.gzmigu.cn

[S35] C++：map
来源：http://hs.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ul.gzmigu.cn

[S36] C++：unordered_map
来源：http://ro.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yy.hahajie.cn

[S37] C++：set
来源：http://un.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nu.muxihuayi.cn

[S38] C++：排序
来源：http://ht.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://qh.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://sm.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bl.9csxet.cn

[S40] C++：查找元素
来源：http://nn.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qu.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://gv.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hd.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://lr.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://ck.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://hq.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://mk.huanxung.cn

[S44] C++：引用传参
来源：http://pv.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://jb.hnjuh.cn

[S45] C++：lambda
来源：http://wc.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rt.wgjwhj.cn

[S46] C++：函数模板
来源：http://yx.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fa.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://zb.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wo.gzmigu.cn

[S48] C++：逐行读文件
来源：http://pf.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ax.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://hn.huixiangedu.cn

[S49] C++：写文件
来源：http://rl.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pp.chemitech.net.cn

[S50] C++：格式化数字
来源：http://aw.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lo.panjiajie.cn

[S51] C++：显式类型转换
来源：http://yg.hnjuh.cn

static_cast<double>(a) / b
来源：http://wx.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://ba.colortex.cn

int size() const noexcept { return n_; }
来源：http://tj.szsharing.cn

[S53] C++：移动语义
来源：http://hc.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://np.bjjhwx.cn

[S54] C++：异常处理
来源：http://jj.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mt.newstarts.cn

[S55] C++：结构化绑定
来源：http://ep.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tp.bookmarksfly.cn

[S56] C++：optional
来源：http://ov.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zf.panjiajie.cn

[S57] C++：编译期常量
来源：http://rf.huixinmuqiang.cn

constexpr int N = 10;
来源：http://hf.wgjwhj.cn

[S58] C++：命名空间
来源：http://wj.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://he.shxzukj.cn

[S59] C++：静态断言
来源：http://kx.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yz.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://ij.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ro.newstarts.cn

================================================================================
来源：http://wf.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bp.nicolike.cn

================================================================================
来源：http://ir.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://qu.chemitech.net.cn

println("Hello")
来源：http://xq.szxytkj.cn

[T02] Kotlin：变量
来源：http://cm.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tk.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://tx.521024.cn

"值: $b"
来源：http://by.nicolike.cn

[T04] Kotlin：空安全
来源：http://os.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ro.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://wy.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://va.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://vs.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nq.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://rs.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zc.9csxet.cn

[T08] Kotlin：数据类
来源：http://bc.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://zl.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://uu.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://xv.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ok.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qc.hahajie.cn

[T11] Kotlin：协程
来源：http://qy.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oq.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://wz.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://fr.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://zs.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://iv.hnjuh.cn

[T14] Kotlin：循环
来源：http://df.szsharing.cn

for (i in 1..10) println(i)
来源：http://ft.newstarts.cn

[T15] Kotlin：接口
来源：http://mv.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://no.chemitech.net.cn

[T16] Swift：Hello World
来源：http://ww.asd995.cn

print("Hello")
来源：http://df.szxytkj.cn

[T17] Swift：变量与常量
来源：http://kn.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://qk.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://la.hnjuh.cn

"值: \(b)"
来源：http://yi.gzmigu.cn

[T19] Swift：可选绑定
来源：http://yz.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://qu.hnjuh.cn

[T20] Swift：数组操作
来源：http://nj.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hd.szxytkj.cn

[T21] Swift：遍历
来源：http://kj.bjjhwx.cn

for x in a { print(x) }
来源：http://hj.huixinmuqiang.cn

[T22] Swift：字典
来源：http://iy.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nx.nszjky.cn

[T23] Swift：函数
来源：http://kg.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tt.shxzskj.cn

[T24] Swift：闭包
来源：http://gc.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wh.bookmarksfly.cn

[T25] Swift：结构体
来源：http://lk.shxzukj.cn

struct P { var x: Int }
来源：http://bn.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://fn.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://zg.wgjwhj.cn

[T27] Swift：错误处理
来源：http://bf.asd995.cn

do { try f() } catch { print(error) }
来源：http://fy.chemitech.net.cn

[T28] Swift：枚举
来源：http://wf.wgjwhj.cn

enum Color { case red, green }
来源：http://sy.asd995.cn

[T29] Swift：guard 提前返回
来源：http://io.huixiangedu.cn

guard let x = opt else { return }
来源：http://ry.nicolike.cn

[T30] Swift：协议
来源：http://zy.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://vj.szxytkj.cn

[T31] Lua：Hello World
来源：http://re.asd995.cn

print("Hello")
来源：http://pu.huixiangedu.cn

[T32] Lua：局部变量
来源：http://xf.jianghongdianzi.cn

local a = 1
来源：http://oa.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://hz.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://er.szsharing.cn

[T34] Lua：遍历表
来源：http://ph.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mn.521024.cn

[T35] Lua：字典表
来源：http://oa.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://yy.nicolike.cn

[T36] Lua：函数
来源：http://eg.panjiajie.cn

function add(a, b) return a + b end
来源：http://sx.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://lp.hnjuh.cn

"a" .. "b"
来源：http://pj.nszjky.cn

[T38] Lua：条件
来源：http://bb.521024.cn

if x > 0 then print("正") end
来源：http://em.shxzukj.cn

[T39] Lua：模式匹配
来源：http://ic.jctech888.com.cn

string.find(s, "%d+")
来源：http://nh.szxytkj.cn

[T40] Lua：元表
来源：http://em.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://is.hahajie.cn

[T41] Perl：Hello World
来源：http://hi.bjjhwx.cn

print "Hello\n";
来源：http://lu.shxzskj.cn

[T42] Perl：变量类型
来源：http://kx.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sy.hahajie.cn

[T43] Perl：字符串插值
来源：http://pb.colortex.cn

"值: $a"
来源：http://sd.huixiangedu.cn

[T44] Perl：条件
来源：http://fr.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://ay.shxzskj.cn

[T45] Perl：数组遍历
来源：http://jk.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://tm.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://os.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ru.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://zr.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gp.shxzskj.cn

[T48] Perl：正则替换
来源：http://kr.szxytkj.cn

$s =~ s/old/new/g;
来源：http://nm.hnjuh.cn

[T49] Perl：函数
来源：http://hu.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zx.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://it.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jd.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://hj.jctech888.com.cn

[T51] Scala：Hello World
来源：http://xq.huixiangedu.cn

println("Hello")
来源：http://rc.shxzukj.cn

[T52] Scala：变量
来源：http://lp.lnxyls.cn

val a = 1;  var b = 2
来源：http://fe.szsharing.cn

[T53] Scala：字符串插值
来源：http://fw.bookmarksfly.cn

s"值: $b"
来源：http://gp.hahajie.cn

[T54] Scala：集合映射
来源：http://gi.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://ic.newstarts.cn

[T55] Scala：集合过滤
来源：http://px.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wq.huixiangedu.cn

[T56] Scala：样例类
来源：http://tp.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://gi.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ls.521024.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pu.lnxyls.cn

[T58] Scala：函数定义
来源：http://cl.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hu.yuexingan06.cn

[T59] Scala：循环
来源：http://jn.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://hl.gzmigu.cn

[T60] Scala：折叠
来源：http://jx.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oz.hahajie.cn

================================================================================
来源：http://xk.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bx.szsharing.cn

================================================================================
来源：http://ou.521024.cn

[U01] Py：创建虚拟环境
来源：http://uu.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yv.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://pv.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sf.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://sh.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sj.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://vz.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mk.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://fd.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://jc.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://wp.521024.cn

{**a, **b}
来源：http://ab.colortex.cn

[U07] Py：反转字典键值
来源：http://ce.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://tb.nicolike.cn

[U08] Py：展平二维列表
来源：http://hf.jctech888.com.cn

[y for x in nested for y in x]
来源：http://bv.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://qh.gzmigu.cn

max(d, key=d.get)
来源：http://dm.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://dk.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gs.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://kq.shxzskj.cn

(x * 2 for x in arr)
来源：http://kn.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rv.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://zg.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://vu.bookmarksfly.cn

deque(maxlen=10)
来源：http://hx.nszjky.cn

[U14] Py：分组收集到列表
来源：http://nr.521024.cn

defaultdict(list)
来源：http://kq.nicolike.cn

[U15] Py：高精度计时
来源：http://rw.9csxet.cn

t = time.perf_counter()
来源：http://pu.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://py.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ge.hahajie.cn


<!-- 参考信息 -->