代发 wailian999

split -l 1000 big.log part_
来源：http://le.muxihuayi.cn

[R74] 批量重命名
来源：http://tz.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ly.newstarts.cn

[R75] 导出环境变量
来源：http://ua.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ds.huixiangedu.cn

[R76] 使用临时文件
来源：http://cl.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bc.bookmarksfly.cn

[R77] 读取用户输入
来源：http://vy.huixiangedu.cn

read -rp "请输入: " ans
来源：http://ix.huanxung.cn

[R78] 交互式菜单
来源：http://kf.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://av.hahajie.cn

[R79] 解析命令行选项
来源：http://ty.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vu.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://lt.huanxung.cn

time ./run.sh
来源：http://uq.hahajie.cn

================================================================================
来源：http://aj.haigaiapp.cn

S. C / C++ 专题
来源：http://nq.muxihuayi.cn

================================================================================
来源：http://sm.yuntaijiaju.cn

[S01] C：Hello World
来源：http://dl.shxzukj.cn

#include <stdio.h>
来源：http://jv.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zj.szsharing.cn

[S02] C：变量与格式化输出
来源：http://pe.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://hs.521024.cn

[S03] C：读入整数
来源：http://ht.newstarts.cn

int x; scanf("%d", &x);
来源：http://zv.shtwfgs.cn

[S04] C：字符串复制
来源：http://yj.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rx.chemitech.net.cn

[S05] C：字符串长度
来源：http://zz.yuntaijiaju.cn

strlen(s)
来源：http://dq.nicolike.cn

[S06] C：字符串比较
来源：http://os.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://jk.hahajie.cn

[S07] C：数组遍历求和
来源：http://nx.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ou.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://re.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kr.asd995.cn

[S09] C：结构体定义与初始化
来源：http://ll.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ri.panjiajie.cn

[S10] C：指针与解引用
来源：http://hz.newstarts.cn

int *p = &a;  *p = 5;
来源：http://eb.panjiajie.cn

[S11] C：逐行读文件
来源：http://vj.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://jc.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zk.wgjwhj.cn

fclose(f);
来源：http://av.haigaiapp.cn

[S12] C：写文件
来源：http://na.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oc.chemitech.net.cn

[S13] C：宏定义
来源：http://th.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lm.muxihuayi.cn

[S14] C：枚举
来源：http://dp.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://zj.szxytkj.cn

[S15] C：类型转换
来源：http://ph.chemitech.net.cn

(double) a / b
来源：http://eh.hahajie.cn

[S16] C：位操作置位
来源：http://ea.yuexingan06.cn

x |= (1 << 3);
来源：http://un.hahajie.cn

[S17] C：安全拼接字符串
来源：http://mu.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xn.9csxet.cn

[S18] C：命令行参数
来源：http://hy.huixiangedu.cn

int main(int argc, char **argv)
来源：http://zt.huixinmuqiang.cn

[S19] C：快速排序
来源：http://sx.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hj.bookmarksfly.cn

[S20] C：二分查找
来源：http://mb.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ei.bjjhwx.cn

[S21] C：字符类别判断
来源：http://sj.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qj.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://ln.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fd.asd995.cn

[S23] C：随机数
来源：http://dw.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ix.shtwfgs.cn

[S24] C：获取本地时间
来源：http://ov.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gq.muxihuayi.cn

[S25] C：内存拷贝
来源：http://lz.521024.cn

memcpy(dst, src, n);
来源：http://em.chemitech.net.cn

[S26] C：内存清零
来源：http://om.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://nv.jianghongdianzi.cn

[S27] C：定义常量
来源：http://uj.lnxyls.cn

const double PI = 3.14159;
来源：http://et.muxihuayi.cn

[S28] C：静态变量
来源：http://ii.huanxung.cn

static int counter = 0;
来源：http://jj.bookmarksfly.cn

[S29] C：变参函数
来源：http://ih.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ul.nszjky.cn

[S30] C：头文件保护
来源：http://jx.bjjhwx.cn

#ifndef X_H
来源：http://th.newstarts.cn

#define X_H
来源：http://fd.szxytkj.cn

#endif
来源：http://wq.newstarts.cn

[S31] C++：Hello World
来源：http://bd.huixinmuqiang.cn

#include <iostream>
来源：http://dd.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://nt.haigaiapp.cn

[S32] C++：字符串
来源：http://lu.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://od.jctech888.com.cn

[S33] C++：vector 增删
来源：http://lw.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dq.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://qs.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ne.wgjwhj.cn

[S35] C++：map
来源：http://rh.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ja.shxzukj.cn

[S36] C++：unordered_map
来源：http://xl.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vm.bookmarksfly.cn

[S37] C++：set
来源：http://mi.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ey.muxihuayi.cn

[S38] C++：排序
来源：http://ar.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://mc.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://td.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uo.huixiangedu.cn

[S40] C++：查找元素
来源：http://fz.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ul.nicolike.cn

[S41] C++：类与构造函数
来源：http://bp.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vm.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://qr.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://df.muxihuayi.cn

[S43] C++：智能指针
来源：http://yn.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://kj.gzmigu.cn

[S44] C++：引用传参
来源：http://dl.nszjky.cn

void inc(int &x) { ++x; }
来源：http://ax.hahajie.cn

[S45] C++：lambda
来源：http://bn.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://to.newstarts.cn

[S46] C++：函数模板
来源：http://ml.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xb.521024.cn

[S47] C++：结构化绑定遍历
来源：http://li.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ro.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://nd.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yg.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://qr.asd995.cn

[S49] C++：写文件
来源：http://it.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oh.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://hy.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ln.shxzukj.cn

[S51] C++：显式类型转换
来源：http://hi.szxytkj.cn

static_cast<double>(a) / b
来源：http://zb.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://ua.newstarts.cn

int size() const noexcept { return n_; }
来源：http://kv.muxihuayi.cn

[S53] C++：移动语义
来源：http://pm.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://uk.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://wj.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yw.9csxet.cn

[S55] C++：结构化绑定
来源：http://eg.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vc.yuntaijiaju.cn

[S56] C++：optional
来源：http://nh.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gb.shxzskj.cn

[S57] C++：编译期常量
来源：http://eo.9csxet.cn

constexpr int N = 10;
来源：http://nu.huanxung.cn

[S58] C++：命名空间
来源：http://cq.521024.cn

namespace ns { int f() { return 1; } }
来源：http://cg.nicolike.cn

[S59] C++：静态断言
来源：http://nd.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vi.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://wi.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ot.wgjwhj.cn

================================================================================
来源：http://ox.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ny.521024.cn

================================================================================
来源：http://co.szsharing.cn

[T01] Kotlin：Hello World
来源：http://ol.wgjwhj.cn

println("Hello")
来源：http://zk.jctech888.com.cn

[T02] Kotlin：变量
来源：http://js.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dp.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://wx.nicolike.cn

"值: $b"
来源：http://la.hahajie.cn

[T04] Kotlin：空安全
来源：http://at.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://rz.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://ms.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rk.asd995.cn

[T06] Kotlin：集合映射
来源：http://uh.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jl.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://ju.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bg.9csxet.cn

[T08] Kotlin：数据类
来源：http://ou.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://fc.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://rn.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://mn.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://qy.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oh.shxzskj.cn

[T11] Kotlin：协程
来源：http://xk.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mu.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://ub.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://nb.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://je.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://nc.shxzukj.cn

[T14] Kotlin：循环
来源：http://pt.szsharing.cn

for (i in 1..10) println(i)
来源：http://fm.hahajie.cn

[T15] Kotlin：接口
来源：http://lf.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ug.haigaiapp.cn

[T16] Swift：Hello World
来源：http://nq.hnjuh.cn

print("Hello")
来源：http://av.gzmigu.cn

[T17] Swift：变量与常量
来源：http://fe.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ma.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://iw.jctech888.com.cn

"值: \(b)"
来源：http://lc.colortex.cn

[T19] Swift：可选绑定
来源：http://vw.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://zi.wgjwhj.cn

[T20] Swift：数组操作
来源：http://gw.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ba.szsharing.cn

[T21] Swift：遍历
来源：http://oh.chemitech.net.cn

for x in a { print(x) }
来源：http://rn.bjjhwx.cn

[T22] Swift：字典
来源：http://jk.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ct.colortex.cn

[T23] Swift：函数
来源：http://fd.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://je.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://rt.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wn.nszjky.cn

[T25] Swift：结构体
来源：http://ee.bookmarksfly.cn

struct P { var x: Int }
来源：http://tf.asd995.cn

[T26] Swift：类与重写
来源：http://wy.lnxyls.cn

class A: Base { override func f() {} }
来源：http://fp.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://mw.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://kp.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://sn.muxihuayi.cn

enum Color { case red, green }
来源：http://dk.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://tb.wgjwhj.cn

guard let x = opt else { return }
来源：http://ii.haigaiapp.cn

[T30] Swift：协议
来源：http://ex.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://ks.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://zj.jianghongdianzi.cn

print("Hello")
来源：http://un.szsharing.cn

[T32] Lua：局部变量
来源：http://xg.yuexingan06.cn

local a = 1
来源：http://bk.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://ts.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lt.szxytkj.cn

[T34] Lua：遍历表
来源：http://yq.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://da.szsharing.cn

[T35] Lua：字典表
来源：http://nu.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://ax.wgjwhj.cn

[T36] Lua：函数
来源：http://qd.hahajie.cn

function add(a, b) return a + b end
来源：http://st.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://zy.colortex.cn

"a" .. "b"
来源：http://zg.nicolike.cn

[T38] Lua：条件
来源：http://mw.szsharing.cn

if x > 0 then print("正") end
来源：http://dm.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://lv.haigaiapp.cn

string.find(s, "%d+")
来源：http://zm.bjjhwx.cn

[T40] Lua：元表
来源：http://wj.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://kd.yuexingan06.cn

[T41] Perl：Hello World
来源：http://uh.521024.cn

print "Hello\n";
来源：http://co.521024.cn

[T42] Perl：变量类型
来源：http://ke.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vl.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://be.9csxet.cn

"值: $a"
来源：http://nw.wgjwhj.cn

[T44] Perl：条件
来源：http://jl.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://qf.szsharing.cn

[T45] Perl：数组遍历
来源：http://rq.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://zc.shxzukj.cn

[T46] Perl：哈希操作
来源：http://xp.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://su.gzmigu.cn

[T47] Perl：正则捕获
来源：http://fq.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kf.colortex.cn

[T48] Perl：正则替换
来源：http://ag.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://pa.hahajie.cn

[T49] Perl：函数
来源：http://ld.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fb.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://cm.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wk.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://mv.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://bw.huixiangedu.cn

println("Hello")
来源：http://dt.szxytkj.cn

[T52] Scala：变量
来源：http://fy.asd995.cn

val a = 1;  var b = 2
来源：http://dm.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ew.nicolike.cn

s"值: $b"
来源：http://ue.panjiajie.cn

[T54] Scala：集合映射
来源：http://yg.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://fc.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ra.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ra.9csxet.cn

[T56] Scala：样例类
来源：http://ji.nicolike.cn

case class User(name: String, age: Int)
来源：http://oe.asd995.cn

[T57] Scala：模式匹配
来源：http://bb.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aq.haigaiapp.cn

[T58] Scala：函数定义
来源：http://zu.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ea.shxzskj.cn

[T59] Scala：循环
来源：http://ri.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://xn.hahajie.cn

[T60] Scala：折叠
来源：http://gm.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ok.yuexingan06.cn

================================================================================
来源：http://uq.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://on.panjiajie.cn

================================================================================
来源：http://oi.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://ih.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ws.bjjhwx.cn

[U02] Py：导出 / 安装依赖
来源：http://oe.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hq.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://qc.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gx.szsharing.cn

[U04] Py：变量调试打印
来源：http://xr.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mt.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://de.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://cf.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://sz.bjjhwx.cn

{**a, **b}
来源：http://ic.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ys.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://ik.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://xg.huanxung.cn

[y for x in nested for y in x]
来源：http://ny.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://di.jctech888.com.cn

max(d, key=d.get)
来源：http://lt.asd995.cn

[U10] Py：按值排序字典
来源：http://yu.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fd.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://wp.nszjky.cn

(x * 2 for x in arr)
来源：http://tm.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://em.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://mv.lnxyls.cn

[U13] Py：固定长度队列
来源：http://cr.9csxet.cn

deque(maxlen=10)
来源：http://fw.nicolike.cn

[U14] Py：分组收集到列表
来源：http://ue.hahajie.cn

defaultdict(list)
来源：http://ww.nszjky.cn


<!-- 参考信息 -->