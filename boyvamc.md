代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://tx.lnxyls.cn

[R70] 时间戳与互转
来源：http://ee.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ge.colortex.cn

[R71] 日期格式化
来源：http://cj.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zm.panjiajie.cn

[R72] 等待端口就绪
来源：http://hr.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tx.hahajie.cn

[R73] 分割大日志
来源：http://ia.szxytkj.cn

split -l 1000 big.log part_
来源：http://gp.nszjky.cn

[R74] 批量重命名
来源：http://dx.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sr.haigaiapp.cn

[R75] 导出环境变量
来源：http://bb.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://zl.shtwfgs.cn

[R76] 使用临时文件
来源：http://bn.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ce.nicolike.cn

[R77] 读取用户输入
来源：http://zj.lnxyls.cn

read -rp "请输入: " ans
来源：http://xs.newstarts.cn

[R78] 交互式菜单
来源：http://yd.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jj.asd995.cn

[R79] 解析命令行选项
来源：http://jt.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ye.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://nn.hnjuh.cn

time ./run.sh
来源：http://kh.yuexingan06.cn

================================================================================
来源：http://zq.panjiajie.cn

S. C / C++ 专题
来源：http://oy.jctech888.com.cn

================================================================================
来源：http://cz.hahajie.cn

[S01] C：Hello World
来源：http://ck.shtwfgs.cn

#include <stdio.h>
来源：http://dh.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hb.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://eu.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://pt.yuntaijiaju.cn

[S03] C：读入整数
来源：http://jv.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://wt.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://lr.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qu.9csxet.cn

[S05] C：字符串长度
来源：http://vm.9csxet.cn

strlen(s)
来源：http://rp.shxzukj.cn

[S06] C：字符串比较
来源：http://du.gzmigu.cn

strcmp(a, b) == 0
来源：http://jr.gzmigu.cn

[S07] C：数组遍历求和
来源：http://zl.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://be.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://hd.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dg.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://ec.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bb.wgjwhj.cn

[S10] C：指针与解引用
来源：http://pt.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://aj.shxzskj.cn

[S11] C：逐行读文件
来源：http://fb.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ls.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bm.huanxung.cn

fclose(f);
来源：http://oo.shxzskj.cn

[S12] C：写文件
来源：http://ll.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jn.jctech888.com.cn

[S13] C：宏定义
来源：http://al.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tp.nicolike.cn

[S14] C：枚举
来源：http://dt.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://gh.gzmigu.cn

[S15] C：类型转换
来源：http://ta.huixiangedu.cn

(double) a / b
来源：http://hn.nicolike.cn

[S16] C：位操作置位
来源：http://gj.gzmigu.cn

x |= (1 << 3);
来源：http://bz.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://zz.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wf.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://ju.shxzukj.cn

int main(int argc, char **argv)
来源：http://ii.bjjhwx.cn

[S19] C：快速排序
来源：http://am.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fz.bookmarksfly.cn

[S20] C：二分查找
来源：http://ax.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pr.bjjhwx.cn

[S21] C：字符类别判断
来源：http://ot.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dv.shxzukj.cn

[S22] C：字符串转数字
来源：http://vv.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jr.nicolike.cn

[S23] C：随机数
来源：http://eu.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sf.huixiangedu.cn

[S24] C：获取本地时间
来源：http://eh.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oj.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://wc.asd995.cn

memcpy(dst, src, n);
来源：http://me.colortex.cn

[S26] C：内存清零
来源：http://at.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://rw.szsharing.cn

[S27] C：定义常量
来源：http://gk.shxzukj.cn

const double PI = 3.14159;
来源：http://bn.szxytkj.cn

[S28] C：静态变量
来源：http://pk.521024.cn

static int counter = 0;
来源：http://sa.szsharing.cn

[S29] C：变参函数
来源：http://tj.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zr.hnjuh.cn

[S30] C：头文件保护
来源：http://xk.colortex.cn

#ifndef X_H
来源：http://uq.lnxyls.cn

#define X_H
来源：http://vn.shtwfgs.cn

#endif
来源：http://uc.panjiajie.cn

[S31] C++：Hello World
来源：http://cu.lnxyls.cn

#include <iostream>
来源：http://rb.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://kh.huixiangedu.cn

[S32] C++：字符串
来源：http://bt.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://we.shxzukj.cn

[S33] C++：vector 增删
来源：http://dn.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yr.newstarts.cn

[S34] C++：遍历 vector
来源：http://es.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://em.chemitech.net.cn

[S35] C++：map
来源：http://pu.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ql.lnxyls.cn

[S36] C++：unordered_map
来源：http://go.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mw.shxzukj.cn

[S37] C++：set
来源：http://se.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jd.asd995.cn

[S38] C++：排序
来源：http://xu.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://sk.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://le.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ad.521024.cn

[S40] C++：查找元素
来源：http://bh.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://es.hnjuh.cn

[S41] C++：类与构造函数
来源：http://um.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ov.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://vt.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://cv.newstarts.cn

[S43] C++：智能指针
来源：http://uj.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://ua.colortex.cn

[S44] C++：引用传参
来源：http://lk.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://fi.hahajie.cn

[S45] C++：lambda
来源：http://ce.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://py.shxzukj.cn

[S46] C++：函数模板
来源：http://sk.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rm.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://go.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xe.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://ro.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hx.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://aq.szxytkj.cn

[S49] C++：写文件
来源：http://zo.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ax.huanxung.cn

[S50] C++：格式化数字
来源：http://ok.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://na.hnjuh.cn

[S51] C++：显式类型转换
来源：http://oi.asd995.cn

static_cast<double>(a) / b
来源：http://bl.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://kr.newstarts.cn

int size() const noexcept { return n_; }
来源：http://qo.huixiangedu.cn

[S53] C++：移动语义
来源：http://sl.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://sj.nicolike.cn

[S54] C++：异常处理
来源：http://yi.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dg.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://os.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hy.huanxung.cn

[S56] C++：optional
来源：http://zd.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pl.szxytkj.cn

[S57] C++：编译期常量
来源：http://mn.muxihuayi.cn

constexpr int N = 10;
来源：http://wl.panjiajie.cn

[S58] C++：命名空间
来源：http://zz.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://ea.colortex.cn

[S59] C++：静态断言
来源：http://ww.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yd.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://uj.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jy.huanxung.cn

================================================================================
来源：http://oc.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cx.asd995.cn

================================================================================
来源：http://id.9csxet.cn

[T01] Kotlin：Hello World
来源：http://jl.521024.cn

println("Hello")
来源：http://kh.muxihuayi.cn

[T02] Kotlin：变量
来源：http://fh.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jq.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://ib.asd995.cn

"值: $b"
来源：http://sl.szxytkj.cn

[T04] Kotlin：空安全
来源：http://vy.gzmigu.cn

val n: String? = null;  n?.length
来源：http://ri.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://kq.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dd.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://kb.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ux.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ka.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fr.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://ew.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://vq.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://fs.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://re.521024.cn

[T10] Kotlin：默认参数
来源：http://dd.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mj.shxzukj.cn

[T11] Kotlin：协程
来源：http://ki.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jv.colortex.cn

[T12] Kotlin：解构声明
来源：http://hm.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://by.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://cw.szsharing.cn

val m = mapOf("a" to 1)
来源：http://un.hnjuh.cn

[T14] Kotlin：循环
来源：http://nq.panjiajie.cn

for (i in 1..10) println(i)
来源：http://cv.nicolike.cn

[T15] Kotlin：接口
来源：http://za.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://qi.huanxung.cn

[T16] Swift：Hello World
来源：http://kq.wgjwhj.cn

print("Hello")
来源：http://pl.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://ub.colortex.cn

var a = 1;  let b = 2
来源：http://bg.shxzukj.cn

[T18] Swift：字符串插值
来源：http://ng.asd995.cn

"值: \(b)"
来源：http://zx.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://sz.szxytkj.cn

if let n = opt { print(n) }
来源：http://nf.haigaiapp.cn

[T20] Swift：数组操作
来源：http://vf.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ke.nicolike.cn

[T21] Swift：遍历
来源：http://dp.nszjky.cn

for x in a { print(x) }
来源：http://mo.chemitech.net.cn

[T22] Swift：字典
来源：http://cp.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rr.9csxet.cn

[T23] Swift：函数
来源：http://wo.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://we.newstarts.cn

[T24] Swift：闭包
来源：http://xn.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uw.521024.cn

[T25] Swift：结构体
来源：http://vx.haigaiapp.cn

struct P { var x: Int }
来源：http://jp.colortex.cn

[T26] Swift：类与重写
来源：http://tf.gzmigu.cn

class A: Base { override func f() {} }
来源：http://qf.panjiajie.cn

[T27] Swift：错误处理
来源：http://er.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://lv.asd995.cn

[T28] Swift：枚举
来源：http://ws.hahajie.cn

enum Color { case red, green }
来源：http://rs.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://rk.colortex.cn

guard let x = opt else { return }
来源：http://be.hnjuh.cn

[T30] Swift：协议
来源：http://kh.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://nk.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://ft.yuntaijiaju.cn

print("Hello")
来源：http://pn.newstarts.cn

[T32] Lua：局部变量
来源：http://fw.chemitech.net.cn

local a = 1
来源：http://ah.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://wn.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qq.bjjhwx.cn

[T34] Lua：遍历表
来源：http://vh.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ms.huixiangedu.cn

[T35] Lua：字典表
来源：http://mo.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://ka.szsharing.cn

[T36] Lua：函数
来源：http://il.shxzskj.cn

function add(a, b) return a + b end
来源：http://go.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://rv.muxihuayi.cn

"a" .. "b"
来源：http://bx.wgjwhj.cn

[T38] Lua：条件
来源：http://jr.haigaiapp.cn

if x > 0 then print("正") end
来源：http://pv.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://od.shxzukj.cn

string.find(s, "%d+")
来源：http://hf.lnxyls.cn

[T40] Lua：元表
来源：http://vi.newstarts.cn

setmetatable({}, { __index = base })
来源：http://on.haigaiapp.cn

[T41] Perl：Hello World
来源：http://fh.hahajie.cn

print "Hello\n";
来源：http://dx.yuexingan06.cn

[T42] Perl：变量类型
来源：http://st.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ob.asd995.cn

[T43] Perl：字符串插值
来源：http://zm.shxzukj.cn

"值: $a"
来源：http://gk.newstarts.cn

[T44] Perl：条件
来源：http://lr.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://wo.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://ng.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://ac.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://sw.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dq.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://qk.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gp.shxzukj.cn

[T48] Perl：正则替换
来源：http://wr.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://vf.shxzskj.cn

[T49] Perl：函数
来源：http://zh.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zq.hahajie.cn

[T50] Perl：逐行读文件
来源：http://kf.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bq.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://qh.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://jk.asd995.cn

println("Hello")
来源：http://qp.jianghongdianzi.cn

[T52] Scala：变量
来源：http://zc.asd995.cn

val a = 1;  var b = 2
来源：http://sv.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://bz.panjiajie.cn

s"值: $b"
来源：http://zw.huixiangedu.cn

[T54] Scala：集合映射
来源：http://dq.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://co.lnxyls.cn

[T55] Scala：集合过滤
来源：http://ox.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kc.huixiangedu.cn

[T56] Scala：样例类
来源：http://tu.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://ps.lnxyls.cn

[T57] Scala：模式匹配
来源：http://bk.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://di.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://ff.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ee.yuntaijiaju.cn

[T59] Scala：循环
来源：http://ni.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://qr.bookmarksfly.cn

[T60] Scala：折叠
来源：http://mm.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ig.521024.cn

================================================================================
来源：http://ra.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vw.bjjhwx.cn

================================================================================
来源：http://hz.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://rp.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ew.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://kx.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zg.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://no.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xd.panjiajie.cn

[U04] Py：变量调试打印
来源：http://wv.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pq.huanxung.cn

[U05] Py：列表去重且保序
来源：http://az.hahajie.cn

list(dict.fromkeys(arr))
来源：http://gt.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://qb.nszjky.cn

{**a, **b}
来源：http://vp.asd995.cn

[U07] Py：反转字典键值
来源：http://bb.yuntaijiaju.cn

{v: k for k, v in d.items()}
来源：http://dc.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://oo.nicolike.cn

[y for x in nested for y in x]
来源：http://eq.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://rs.lnxyls.cn

max(d, key=d.get)
来源：http://ca.lnxyls.cn

[U10] Py：按值排序字典
来源：http://gd.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://re.gzmigu.cn


<!-- 参考信息 -->