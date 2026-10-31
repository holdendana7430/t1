代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://bm.chemitech.net.cn

[R70] 时间戳与互转
来源：http://ub.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://lb.shtwfgs.cn

[R71] 日期格式化
来源：http://zu.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jn.szxytkj.cn

[R72] 等待端口就绪
来源：http://ef.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fa.bjjhwx.cn

[R73] 分割大日志
来源：http://eb.hnjuh.cn

split -l 1000 big.log part_
来源：http://sp.colortex.cn

[R74] 批量重命名
来源：http://tq.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ap.chemitech.net.cn

[R75] 导出环境变量
来源：http://yz.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://pd.newstarts.cn

[R76] 使用临时文件
来源：http://vj.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://an.huixiangedu.cn

[R77] 读取用户输入
来源：http://gd.huixiangedu.cn

read -rp "请输入: " ans
来源：http://km.nszjky.cn

[R78] 交互式菜单
来源：http://xl.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ml.nicolike.cn

[R79] 解析命令行选项
来源：http://jo.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fe.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://wk.huixiangedu.cn

time ./run.sh
来源：http://uz.huanxung.cn

================================================================================
来源：http://vd.chemitech.net.cn

S. C / C++ 专题
来源：http://aw.wgjwhj.cn

================================================================================
来源：http://pz.colortex.cn

[S01] C：Hello World
来源：http://tv.jctech888.com.cn

#include <stdio.h>
来源：http://cp.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eb.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://iu.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://nh.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ny.nicolike.cn

int x; scanf("%d", &x);
来源：http://xa.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://by.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xo.colortex.cn

[S05] C：字符串长度
来源：http://qi.huixinmuqiang.cn

strlen(s)
来源：http://lq.lnxyls.cn

[S06] C：字符串比较
来源：http://tn.bjjhwx.cn

strcmp(a, b) == 0
来源：http://qe.hnjuh.cn

[S07] C：数组遍历求和
来源：http://mw.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ud.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://yh.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://om.521024.cn

[S09] C：结构体定义与初始化
来源：http://pa.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sh.shxzukj.cn

[S10] C：指针与解引用
来源：http://mp.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://mk.newstarts.cn

[S11] C：逐行读文件
来源：http://iv.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://qt.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pr.521024.cn

fclose(f);
来源：http://fx.bookmarksfly.cn

[S12] C：写文件
来源：http://ok.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qn.shxzukj.cn

[S13] C：宏定义
来源：http://to.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lc.colortex.cn

[S14] C：枚举
来源：http://fd.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://wl.haigaiapp.cn

[S15] C：类型转换
来源：http://tn.hahajie.cn

(double) a / b
来源：http://wv.nszjky.cn

[S16] C：位操作置位
来源：http://yq.asd995.cn

x |= (1 << 3);
来源：http://jd.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://ao.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xr.yuexingan06.cn

[S18] C：命令行参数
来源：http://km.szsharing.cn

int main(int argc, char **argv)
来源：http://kd.nszjky.cn

[S19] C：快速排序
来源：http://ew.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tl.huixiangedu.cn

[S20] C：二分查找
来源：http://ft.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ya.huixiangedu.cn

[S21] C：字符类别判断
来源：http://ml.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sg.wgjwhj.cn

[S22] C：字符串转数字
来源：http://db.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tk.521024.cn

[S23] C：随机数
来源：http://sr.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mk.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://gm.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yr.muxihuayi.cn

[S25] C：内存拷贝
来源：http://xa.nicolike.cn

memcpy(dst, src, n);
来源：http://jv.muxihuayi.cn

[S26] C：内存清零
来源：http://nn.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://uq.jianghongdianzi.cn

[S27] C：定义常量
来源：http://hq.asd995.cn

const double PI = 3.14159;
来源：http://kz.bjjhwx.cn

[S28] C：静态变量
来源：http://uq.huixiangedu.cn

static int counter = 0;
来源：http://xi.colortex.cn

[S29] C：变参函数
来源：http://dl.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ir.bookmarksfly.cn

[S30] C：头文件保护
来源：http://sl.hnjuh.cn

#ifndef X_H
来源：http://lh.hahajie.cn

#define X_H
来源：http://zt.muxihuayi.cn

#endif
来源：http://wo.nicolike.cn

[S31] C++：Hello World
来源：http://vq.jctech888.com.cn

#include <iostream>
来源：http://qp.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://ld.colortex.cn

[S32] C++：字符串
来源：http://ci.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://jj.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ss.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sj.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://qr.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://iv.lnxyls.cn

[S35] C++：map
来源：http://kc.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://no.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://bj.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ic.hahajie.cn

[S37] C++：set
来源：http://au.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qg.jctech888.com.cn

[S38] C++：排序
来源：http://eb.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://tp.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://we.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sv.shxzukj.cn

[S40] C++：查找元素
来源：http://nr.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ou.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://we.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zc.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://mn.521024.cn

class B : public Base { public: void f() override {} };
来源：http://lt.panjiajie.cn

[S43] C++：智能指针
来源：http://ec.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://to.shxzukj.cn

[S44] C++：引用传参
来源：http://sc.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://om.gzmigu.cn

[S45] C++：lambda
来源：http://ad.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ha.bjjhwx.cn

[S46] C++：函数模板
来源：http://ne.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://se.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://zl.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ul.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://zz.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hy.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://da.muxihuayi.cn

[S49] C++：写文件
来源：http://wy.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bt.hahajie.cn

[S50] C++：格式化数字
来源：http://yi.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vx.newstarts.cn

[S51] C++：显式类型转换
来源：http://ge.wgjwhj.cn

static_cast<double>(a) / b
来源：http://yo.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://dy.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://sk.9csxet.cn

[S53] C++：移动语义
来源：http://yt.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://us.lnxyls.cn

[S54] C++：异常处理
来源：http://wn.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kr.shxzskj.cn

[S55] C++：结构化绑定
来源：http://hq.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eg.chemitech.net.cn

[S56] C++：optional
来源：http://bv.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yu.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://jo.9csxet.cn

constexpr int N = 10;
来源：http://po.nicolike.cn

[S58] C++：命名空间
来源：http://ul.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ub.hnjuh.cn

[S59] C++：静态断言
来源：http://cf.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qx.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://gb.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nz.nszjky.cn

================================================================================
来源：http://no.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ou.521024.cn

================================================================================
来源：http://xp.nszjky.cn

[T01] Kotlin：Hello World
来源：http://li.521024.cn

println("Hello")
来源：http://lq.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://dv.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xz.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://su.huanxung.cn

"值: $b"
来源：http://xk.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://eo.9csxet.cn

val n: String? = null;  n?.length
来源：http://xe.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://fr.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ju.hahajie.cn

[T06] Kotlin：集合映射
来源：http://fp.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kl.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://cg.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ty.huanxung.cn

[T08] Kotlin：数据类
来源：http://mk.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://fb.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://oh.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://ej.hahajie.cn

[T10] Kotlin：默认参数
来源：http://sx.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vo.asd995.cn

[T11] Kotlin：协程
来源：http://pk.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sw.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://wy.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://tz.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://qe.nszjky.cn

val m = mapOf("a" to 1)
来源：http://yy.nszjky.cn

[T14] Kotlin：循环
来源：http://dg.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://hk.lnxyls.cn

[T15] Kotlin：接口
来源：http://ce.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://mm.9csxet.cn

[T16] Swift：Hello World
来源：http://tk.jianghongdianzi.cn

print("Hello")
来源：http://rr.hahajie.cn

[T17] Swift：变量与常量
来源：http://af.shxzukj.cn

var a = 1;  let b = 2
来源：http://zv.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://vw.shxzskj.cn

"值: \(b)"
来源：http://ol.huanxung.cn

[T19] Swift：可选绑定
来源：http://no.lnxyls.cn

if let n = opt { print(n) }
来源：http://mk.shxzskj.cn

[T20] Swift：数组操作
来源：http://be.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://le.szxytkj.cn

[T21] Swift：遍历
来源：http://yy.hnjuh.cn

for x in a { print(x) }
来源：http://pz.jianghongdianzi.cn

[T22] Swift：字典
来源：http://uq.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tr.jianghongdianzi.cn

[T23] Swift：函数
来源：http://qn.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kt.jctech888.com.cn

[T24] Swift：闭包
来源：http://gl.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sm.newstarts.cn

[T25] Swift：结构体
来源：http://vp.9csxet.cn

struct P { var x: Int }
来源：http://py.colortex.cn

[T26] Swift：类与重写
来源：http://nz.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://nf.yuexingan06.cn

[T27] Swift：错误处理
来源：http://fv.asd995.cn

do { try f() } catch { print(error) }
来源：http://hm.nicolike.cn

[T28] Swift：枚举
来源：http://sb.szxytkj.cn

enum Color { case red, green }
来源：http://ks.colortex.cn

[T29] Swift：guard 提前返回
来源：http://dl.9csxet.cn

guard let x = opt else { return }
来源：http://ll.nszjky.cn

[T30] Swift：协议
来源：http://fk.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://lz.muxihuayi.cn

[T31] Lua：Hello World
来源：http://by.jctech888.com.cn

print("Hello")
来源：http://cw.szxytkj.cn

[T32] Lua：局部变量
来源：http://ou.hnjuh.cn

local a = 1
来源：http://yi.lnxyls.cn

[T33] Lua：表（数组）
来源：http://dg.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zb.bjjhwx.cn

[T34] Lua：遍历表
来源：http://bm.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yw.jctech888.com.cn

[T35] Lua：字典表
来源：http://cq.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://gc.asd995.cn

[T36] Lua：函数
来源：http://oi.9csxet.cn

function add(a, b) return a + b end
来源：http://iv.newstarts.cn

[T37] Lua：字符串拼接
来源：http://vg.shtwfgs.cn

"a" .. "b"
来源：http://lj.hnjuh.cn

[T38] Lua：条件
来源：http://gf.lnxyls.cn

if x > 0 then print("正") end
来源：http://ai.9csxet.cn

[T39] Lua：模式匹配
来源：http://us.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://yz.muxihuayi.cn

[T40] Lua：元表
来源：http://rx.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://tb.asd995.cn

[T41] Perl：Hello World
来源：http://vn.muxihuayi.cn

print "Hello\n";
来源：http://sn.gzmigu.cn

[T42] Perl：变量类型
来源：http://zc.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fk.521024.cn

[T43] Perl：字符串插值
来源：http://qy.jianghongdianzi.cn

"值: $a"
来源：http://gq.newstarts.cn

[T44] Perl：条件
来源：http://lx.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://vi.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://cw.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://sj.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://rq.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fa.nszjky.cn

[T47] Perl：正则捕获
来源：http://dq.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ne.9csxet.cn

[T48] Perl：正则替换
来源：http://jt.gzmigu.cn

$s =~ s/old/new/g;
来源：http://kc.bjjhwx.cn

[T49] Perl：函数
来源：http://if.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oo.newstarts.cn

[T50] Perl：逐行读文件
来源：http://du.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ln.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ja.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ho.nicolike.cn

println("Hello")
来源：http://ik.bjjhwx.cn

[T52] Scala：变量
来源：http://xm.colortex.cn

val a = 1;  var b = 2
来源：http://uz.lnxyls.cn

[T53] Scala：字符串插值
来源：http://fo.szxytkj.cn

s"值: $b"
来源：http://wi.shxzukj.cn

[T54] Scala：集合映射
来源：http://yp.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://nc.hahajie.cn

[T55] Scala：集合过滤
来源：http://kg.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ug.yuexingan06.cn

[T56] Scala：样例类
来源：http://lk.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://qb.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://hd.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gm.bjjhwx.cn

[T58] Scala：函数定义
来源：http://tk.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://io.huanxung.cn

[T59] Scala：循环
来源：http://fc.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://zq.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://cf.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gk.jianghongdianzi.cn

================================================================================
来源：http://lr.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wx.chemitech.net.cn

================================================================================
来源：http://lf.asd995.cn

[U01] Py：创建虚拟环境
来源：http://it.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qx.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://mg.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ol.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://ek.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cc.nicolike.cn

[U04] Py：变量调试打印
来源：http://tr.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xs.huanxung.cn

[U05] Py：列表去重且保序
来源：http://mi.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://lh.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://yc.jctech888.com.cn

{**a, **b}
来源：http://lw.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://yf.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://ot.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://ur.yuntaijiaju.cn

[y for x in nested for y in x]
来源：http://qm.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://ya.szxytkj.cn

max(d, key=d.get)
来源：http://xz.hnjuh.cn

[U10] Py：按值排序字典
来源：http://ls.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oq.hnjuh.cn


<!-- 参考信息 -->