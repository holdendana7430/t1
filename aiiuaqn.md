代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://vx.gzmigu.cn

[R72] 等待端口就绪
来源：http://ib.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ss.yuexingan06.cn

[R73] 分割大日志
来源：http://eg.shtwfgs.cn

split -l 1000 big.log part_
来源：http://dz.bjjhwx.cn

[R74] 批量重命名
来源：http://tn.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tk.huixiangedu.cn

[R75] 导出环境变量
来源：http://ox.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://op.shtwfgs.cn

[R76] 使用临时文件
来源：http://kd.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ps.nszjky.cn

[R77] 读取用户输入
来源：http://kp.asd995.cn

read -rp "请输入: " ans
来源：http://ch.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://lp.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ox.huanxung.cn

[R79] 解析命令行选项
来源：http://wc.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aj.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://eh.haigaiapp.cn

time ./run.sh
来源：http://yn.yuexingan06.cn

================================================================================
来源：http://mq.nszjky.cn

S. C / C++ 专题
来源：http://ux.bjjhwx.cn

================================================================================
来源：http://ao.shtwfgs.cn

[S01] C：Hello World
来源：http://mq.colortex.cn

#include <stdio.h>
来源：http://kz.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vv.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://qw.521024.cn

int a = 10; printf("%d\n", a);
来源：http://ql.nicolike.cn

[S03] C：读入整数
来源：http://jg.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://li.lnxyls.cn

[S04] C：字符串复制
来源：http://mo.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wz.haigaiapp.cn

[S05] C：字符串长度
来源：http://cw.yuexingan06.cn

strlen(s)
来源：http://cm.nszjky.cn

[S06] C：字符串比较
来源：http://vs.jctech888.com.cn

strcmp(a, b) == 0
来源：http://lo.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://bu.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ad.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://ve.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zz.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://go.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mo.chemitech.net.cn

[S10] C：指针与解引用
来源：http://mu.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://od.9csxet.cn

[S11] C：逐行读文件
来源：http://bi.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://fc.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pe.hahajie.cn

fclose(f);
来源：http://ul.szsharing.cn

[S12] C：写文件
来源：http://fa.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kq.huixiangedu.cn

[S13] C：宏定义
来源：http://zj.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ak.jianghongdianzi.cn

[S14] C：枚举
来源：http://zg.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://mg.huanxung.cn

[S15] C：类型转换
来源：http://sy.jianghongdianzi.cn

(double) a / b
来源：http://de.szxytkj.cn

[S16] C：位操作置位
来源：http://lp.huixiangedu.cn

x |= (1 << 3);
来源：http://dl.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://gd.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pd.hahajie.cn

[S18] C：命令行参数
来源：http://dv.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://sx.gzmigu.cn

[S19] C：快速排序
来源：http://tz.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ns.yuntaijiaju.cn

[S20] C：二分查找
来源：http://cu.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jctech888.com.cn

[S21] C：字符类别判断
来源：http://sv.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mt.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://rn.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ns.haigaiapp.cn

[S23] C：随机数
来源：http://hd.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gc.colortex.cn

[S24] C：获取本地时间
来源：http://us.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gg.shtwfgs.cn

[S25] C：内存拷贝
来源：http://nx.huanxung.cn

memcpy(dst, src, n);
来源：http://gq.colortex.cn

[S26] C：内存清零
来源：http://ce.9csxet.cn

memset(a, 0, sizeof a);
来源：http://jx.9csxet.cn

[S27] C：定义常量
来源：http://ky.hnjuh.cn

const double PI = 3.14159;
来源：http://xr.jctech888.com.cn

[S28] C：静态变量
来源：http://ps.jianghongdianzi.cn

static int counter = 0;
来源：http://ut.yuntaijiaju.cn

[S29] C：变参函数
来源：http://lf.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yk.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://ha.wgjwhj.cn

#ifndef X_H
来源：http://wp.yuntaijiaju.cn

#define X_H
来源：http://xt.jianghongdianzi.cn

#endif
来源：http://po.szxytkj.cn

[S31] C++：Hello World
来源：http://jq.huixinmuqiang.cn

#include <iostream>
来源：http://sl.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://wz.hnjuh.cn

[S32] C++：字符串
来源：http://vk.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://iw.huixiangedu.cn

[S33] C++：vector 增删
来源：http://bs.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zc.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ye.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://ni.newstarts.cn

[S35] C++：map
来源：http://vh.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yj.asd995.cn

[S36] C++：unordered_map
来源：http://xc.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xl.shxzskj.cn

[S37] C++：set
来源：http://zz.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yv.jianghongdianzi.cn

[S38] C++：排序
来源：http://zj.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://fc.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://bm.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pd.szsharing.cn

[S40] C++：查找元素
来源：http://jw.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xy.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://wl.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iw.colortex.cn

[S42] C++：继承与虚函数
来源：http://bs.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://be.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://fj.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://sa.chemitech.net.cn

[S44] C++：引用传参
来源：http://lj.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://of.nszjky.cn

[S45] C++：lambda
来源：http://xa.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cb.muxihuayi.cn

[S46] C++：函数模板
来源：http://zz.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sm.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://gz.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jq.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://jh.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ep.9csxet.cn

while (std::getline(in, line)) { }
来源：http://sw.chemitech.net.cn

[S49] C++：写文件
来源：http://fs.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hg.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://ch.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yd.huanxung.cn

[S51] C++：显式类型转换
来源：http://ti.asd995.cn

static_cast<double>(a) / b
来源：http://fb.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://jj.szsharing.cn

int size() const noexcept { return n_; }
来源：http://ld.nszjky.cn

[S53] C++：移动语义
来源：http://iw.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://zn.newstarts.cn

[S54] C++：异常处理
来源：http://pc.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mg.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://wg.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ik.muxihuayi.cn

[S56] C++：optional
来源：http://ox.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uf.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://po.newstarts.cn

constexpr int N = 10;
来源：http://hc.hnjuh.cn

[S58] C++：命名空间
来源：http://fb.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://zt.colortex.cn

[S59] C++：静态断言
来源：http://sd.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kp.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://yt.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://co.newstarts.cn

================================================================================
来源：http://dr.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fu.nicolike.cn

================================================================================
来源：http://ie.szsharing.cn

[T01] Kotlin：Hello World
来源：http://mb.yuexingan06.cn

println("Hello")
来源：http://je.colortex.cn

[T02] Kotlin：变量
来源：http://qo.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wm.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://dt.chemitech.net.cn

"值: $b"
来源：http://ti.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://pi.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://nr.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://dt.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xh.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://fn.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xb.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://op.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://md.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://es.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://vt.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://sz.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://oj.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://ye.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vs.9csxet.cn

[T11] Kotlin：协程
来源：http://fg.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ck.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://pn.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://na.521024.cn

[T13] Kotlin：只读 Map
来源：http://hk.521024.cn

val m = mapOf("a" to 1)
来源：http://hu.szxytkj.cn

[T14] Kotlin：循环
来源：http://kp.hnjuh.cn

for (i in 1..10) println(i)
来源：http://dy.huixiangedu.cn

[T15] Kotlin：接口
来源：http://dv.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://cc.wgjwhj.cn

[T16] Swift：Hello World
来源：http://zz.huixinmuqiang.cn

print("Hello")
来源：http://hq.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://fl.szxytkj.cn

var a = 1;  let b = 2
来源：http://qz.panjiajie.cn

[T18] Swift：字符串插值
来源：http://ja.gzmigu.cn

"值: \(b)"
来源：http://ao.9csxet.cn

[T19] Swift：可选绑定
来源：http://od.hnjuh.cn

if let n = opt { print(n) }
来源：http://cm.shxzskj.cn

[T20] Swift：数组操作
来源：http://mu.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://an.newstarts.cn

[T21] Swift：遍历
来源：http://hj.jctech888.com.cn

for x in a { print(x) }
来源：http://eo.yuntaijiaju.cn

[T22] Swift：字典
来源：http://uv.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gc.wgjwhj.cn

[T23] Swift：函数
来源：http://vk.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mk.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ce.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zp.gzmigu.cn

[T25] Swift：结构体
来源：http://ic.huanxung.cn

struct P { var x: Int }
来源：http://gv.newstarts.cn

[T26] Swift：类与重写
来源：http://fz.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://bu.chemitech.net.cn

[T27] Swift：错误处理
来源：http://qk.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://pi.szxytkj.cn

[T28] Swift：枚举
来源：http://od.lnxyls.cn

enum Color { case red, green }
来源：http://jo.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://kn.newstarts.cn

guard let x = opt else { return }
来源：http://ec.521024.cn

[T30] Swift：协议
来源：http://ro.521024.cn

protocol Shape { func area() -> Double }
来源：http://hd.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://vn.9csxet.cn

print("Hello")
来源：http://ov.jctech888.com.cn

[T32] Lua：局部变量
来源：http://be.szsharing.cn

local a = 1
来源：http://vx.huanxung.cn

[T33] Lua：表（数组）
来源：http://ya.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pd.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://yx.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hg.panjiajie.cn

[T35] Lua：字典表
来源：http://ik.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://ep.haigaiapp.cn

[T36] Lua：函数
来源：http://io.haigaiapp.cn

function add(a, b) return a + b end
来源：http://mr.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://zk.jianghongdianzi.cn

"a" .. "b"
来源：http://ro.gzmigu.cn

[T38] Lua：条件
来源：http://gn.huanxung.cn

if x > 0 then print("正") end
来源：http://mb.hahajie.cn

[T39] Lua：模式匹配
来源：http://tw.jctech888.com.cn

string.find(s, "%d+")
来源：http://ju.lnxyls.cn

[T40] Lua：元表
来源：http://rw.9csxet.cn

setmetatable({}, { __index = base })
来源：http://jp.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://bl.jctech888.com.cn

print "Hello\n";
来源：http://bw.muxihuayi.cn

[T42] Perl：变量类型
来源：http://yw.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ly.9csxet.cn

[T43] Perl：字符串插值
来源：http://us.hnjuh.cn

"值: $a"
来源：http://ar.shxzukj.cn

[T44] Perl：条件
来源：http://px.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://ox.bjjhwx.cn

[T45] Perl：数组遍历
来源：http://fw.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://lg.szxytkj.cn

[T46] Perl：哈希操作
来源：http://it.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bt.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://tv.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kp.yuexingan06.cn

[T48] Perl：正则替换
来源：http://wv.9csxet.cn

$s =~ s/old/new/g;
来源：http://yb.asd995.cn

[T49] Perl：函数
来源：http://cj.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rv.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://cz.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pg.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ff.colortex.cn

[T51] Scala：Hello World
来源：http://ez.muxihuayi.cn

println("Hello")
来源：http://yg.nszjky.cn

[T52] Scala：变量
来源：http://na.nicolike.cn

val a = 1;  var b = 2
来源：http://ii.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://qp.shxzukj.cn

s"值: $b"
来源：http://bw.chemitech.net.cn

[T54] Scala：集合映射
来源：http://js.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://pl.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://cq.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dq.shtwfgs.cn

[T56] Scala：样例类
来源：http://fk.panjiajie.cn

case class User(name: String, age: Int)
来源：http://oq.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://lt.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wf.muxihuayi.cn

[T58] Scala：函数定义
来源：http://pf.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ok.nicolike.cn

[T59] Scala：循环
来源：http://mk.szxytkj.cn

for (i <- 1 to 10) println(i)
来源：http://jx.yuexingan06.cn

[T60] Scala：折叠
来源：http://pl.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yw.panjiajie.cn

================================================================================
来源：http://ub.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vv.jianghongdianzi.cn

================================================================================
来源：http://yy.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://sv.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://es.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://do.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://az.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://ee.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vz.nszjky.cn

[U04] Py：变量调试打印
来源：http://fj.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qr.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://qy.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://du.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://vl.wgjwhj.cn

{**a, **b}
来源：http://fs.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://zy.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://sn.asd995.cn

[U08] Py：展平二维列表
来源：http://au.asd995.cn

[y for x in nested for y in x]
来源：http://dn.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ev.asd995.cn

max(d, key=d.get)
来源：http://hh.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://ef.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nn.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://dk.szsharing.cn

(x * 2 for x in arr)
来源：http://xw.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dt.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://ly.panjiajie.cn


<!-- 参考信息 -->