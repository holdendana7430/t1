代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://yp.nszjky.cn

[R70] 时间戳与互转
来源：http://uo.szsharing.cn

date +%s;  date -d @1700000000
来源：http://vj.panjiajie.cn

[R71] 日期格式化
来源：http://bu.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sa.hahajie.cn

[R72] 等待端口就绪
来源：http://ly.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ad.hnjuh.cn

[R73] 分割大日志
来源：http://wn.nicolike.cn

split -l 1000 big.log part_
来源：http://uq.huixinmuqiang.cn

[R74] 批量重命名
来源：http://ko.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gj.bjjhwx.cn

[R75] 导出环境变量
来源：http://zt.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://vs.nicolike.cn

[R76] 使用临时文件
来源：http://ns.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jn.gzmigu.cn

[R77] 读取用户输入
来源：http://vp.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://xg.szsharing.cn

[R78] 交互式菜单
来源：http://aa.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://du.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://un.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uf.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://kv.521024.cn

time ./run.sh
来源：http://uk.shxzskj.cn

================================================================================
来源：http://yg.yuexingan06.cn

S. C / C++ 专题
来源：http://wf.nszjky.cn

================================================================================
来源：http://nw.nicolike.cn

[S01] C：Hello World
来源：http://cv.bjjhwx.cn

#include <stdio.h>
来源：http://wh.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jn.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://an.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://lu.lnxyls.cn

[S03] C：读入整数
来源：http://vq.colortex.cn

int x; scanf("%d", &x);
来源：http://nh.szxytkj.cn

[S04] C：字符串复制
来源：http://bt.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ds.newstarts.cn

[S05] C：字符串长度
来源：http://sg.yuexingan06.cn

strlen(s)
来源：http://wz.hnjuh.cn

[S06] C：字符串比较
来源：http://ve.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://kr.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://ok.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yk.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://kq.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://su.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://ik.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ew.shxzukj.cn

[S10] C：指针与解引用
来源：http://ct.nicolike.cn

int *p = &a;  *p = 5;
来源：http://ox.521024.cn

[S11] C：逐行读文件
来源：http://js.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://rj.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pu.shxzskj.cn

fclose(f);
来源：http://zv.szsharing.cn

[S12] C：写文件
来源：http://wg.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rq.nicolike.cn

[S13] C：宏定义
来源：http://eo.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ry.wgjwhj.cn

[S14] C：枚举
来源：http://fc.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://vk.muxihuayi.cn

[S15] C：类型转换
来源：http://fq.hahajie.cn

(double) a / b
来源：http://ws.521024.cn

[S16] C：位操作置位
来源：http://vq.jctech888.com.cn

x |= (1 << 3);
来源：http://qq.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://av.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sv.lnxyls.cn

[S18] C：命令行参数
来源：http://bm.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://ud.szxytkj.cn

[S19] C：快速排序
来源：http://xi.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ei.nszjky.cn

[S20] C：二分查找
来源：http://jy.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.szsharing.cn

[S21] C：字符类别判断
来源：http://fv.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dq.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://ds.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sd.szsharing.cn

[S23] C：随机数
来源：http://vj.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://io.chemitech.net.cn

[S24] C：获取本地时间
来源：http://xu.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dk.yuexingan06.cn

[S25] C：内存拷贝
来源：http://us.nicolike.cn

memcpy(dst, src, n);
来源：http://eo.nicolike.cn

[S26] C：内存清零
来源：http://rw.hahajie.cn

memset(a, 0, sizeof a);
来源：http://cc.yuexingan06.cn

[S27] C：定义常量
来源：http://ei.huixiangedu.cn

const double PI = 3.14159;
来源：http://ds.yuexingan06.cn

[S28] C：静态变量
来源：http://vp.wgjwhj.cn

static int counter = 0;
来源：http://pe.szxytkj.cn

[S29] C：变参函数
来源：http://uy.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nk.521024.cn

[S30] C：头文件保护
来源：http://ji.shxzukj.cn

#ifndef X_H
来源：http://nj.shxzskj.cn

#define X_H
来源：http://qs.haigaiapp.cn

#endif
来源：http://df.bookmarksfly.cn

[S31] C++：Hello World
来源：http://dx.lnxyls.cn

#include <iostream>
来源：http://bo.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ak.muxihuayi.cn

[S32] C++：字符串
来源：http://ba.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://xh.nszjky.cn

[S33] C++：vector 增删
来源：http://tr.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lw.szsharing.cn

[S34] C++：遍历 vector
来源：http://mi.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://et.nszjky.cn

[S35] C++：map
来源：http://zn.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ti.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://oh.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qs.shxzukj.cn

[S37] C++：set
来源：http://tb.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ui.hahajie.cn

[S38] C++：排序
来源：http://pt.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://af.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://cl.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qy.muxihuayi.cn

[S40] C++：查找元素
来源：http://xk.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qp.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://pg.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kw.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://ri.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://rv.huanxung.cn

[S43] C++：智能指针
来源：http://hn.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ha.bjjhwx.cn

[S44] C++：引用传参
来源：http://gc.szsharing.cn

void inc(int &x) { ++x; }
来源：http://qb.asd995.cn

[S45] C++：lambda
来源：http://gx.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fh.panjiajie.cn

[S46] C++：函数模板
来源：http://ta.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uw.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://fp.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jh.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://gr.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ew.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://vd.bookmarksfly.cn

[S49] C++：写文件
来源：http://kf.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ya.nszjky.cn

[S50] C++：格式化数字
来源：http://gf.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zt.szxytkj.cn

[S51] C++：显式类型转换
来源：http://oa.yuexingan06.cn

static_cast<double>(a) / b
来源：http://kx.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://lh.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://ml.gzmigu.cn

[S53] C++：移动语义
来源：http://jp.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://cd.szxytkj.cn

[S54] C++：异常处理
来源：http://zo.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cn.gzmigu.cn

[S55] C++：结构化绑定
来源：http://ym.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fj.szsharing.cn

[S56] C++：optional
来源：http://it.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ie.hahajie.cn

[S57] C++：编译期常量
来源：http://sy.jctech888.com.cn

constexpr int N = 10;
来源：http://vi.shxzukj.cn

[S58] C++：命名空间
来源：http://nr.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://ok.colortex.cn

[S59] C++：静态断言
来源：http://fe.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yx.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://ra.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://id.bjjhwx.cn

================================================================================
来源：http://ko.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dm.chemitech.net.cn

================================================================================
来源：http://ms.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://cn.9csxet.cn

println("Hello")
来源：http://bm.shxzukj.cn

[T02] Kotlin：变量
来源：http://gx.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ax.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://ly.chemitech.net.cn

"值: $b"
来源：http://ce.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://wo.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://nn.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://qz.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lk.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://rx.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ur.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://im.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lx.gzmigu.cn

[T08] Kotlin：数据类
来源：http://ts.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://nk.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://jj.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://du.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://rv.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tc.panjiajie.cn

[T11] Kotlin：协程
来源：http://ek.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hu.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://rk.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://do.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://sm.9csxet.cn

val m = mapOf("a" to 1)
来源：http://mw.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://lx.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://wy.panjiajie.cn

[T15] Kotlin：接口
来源：http://bi.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://qr.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://hj.lnxyls.cn

print("Hello")
来源：http://iu.szxytkj.cn

[T17] Swift：变量与常量
来源：http://dl.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://ly.nszjky.cn

[T18] Swift：字符串插值
来源：http://ul.shtwfgs.cn

"值: \(b)"
来源：http://oa.521024.cn

[T19] Swift：可选绑定
来源：http://ul.newstarts.cn

if let n = opt { print(n) }
来源：http://ul.shxzskj.cn

[T20] Swift：数组操作
来源：http://iw.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ye.shtwfgs.cn

[T21] Swift：遍历
来源：http://dz.gzmigu.cn

for x in a { print(x) }
来源：http://qn.bjjhwx.cn

[T22] Swift：字典
来源：http://if.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yf.lnxyls.cn

[T23] Swift：函数
来源：http://il.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tr.chemitech.net.cn

[T24] Swift：闭包
来源：http://ri.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vz.huixiangedu.cn

[T25] Swift：结构体
来源：http://pg.bookmarksfly.cn

struct P { var x: Int }
来源：http://jb.huixiangedu.cn

[T26] Swift：类与重写
来源：http://gj.lnxyls.cn

class A: Base { override func f() {} }
来源：http://cs.lnxyls.cn

[T27] Swift：错误处理
来源：http://aw.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://ny.asd995.cn

[T28] Swift：枚举
来源：http://wg.shxzskj.cn

enum Color { case red, green }
来源：http://er.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://ij.shxzskj.cn

guard let x = opt else { return }
来源：http://zn.gzmigu.cn

[T30] Swift：协议
来源：http://be.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://ec.colortex.cn

[T31] Lua：Hello World
来源：http://wf.hnjuh.cn

print("Hello")
来源：http://pu.521024.cn

[T32] Lua：局部变量
来源：http://xg.hahajie.cn

local a = 1
来源：http://nj.hnjuh.cn

[T33] Lua：表（数组）
来源：http://xf.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xc.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://ue.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gi.panjiajie.cn

[T35] Lua：字典表
来源：http://bm.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://hb.huixinmuqiang.cn

[T36] Lua：函数
来源：http://kb.jctech888.com.cn

function add(a, b) return a + b end
来源：http://lt.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://tk.hnjuh.cn

"a" .. "b"
来源：http://xu.bookmarksfly.cn

[T38] Lua：条件
来源：http://ie.haigaiapp.cn

if x > 0 then print("正") end
来源：http://mh.shxzskj.cn

[T39] Lua：模式匹配
来源：http://ld.newstarts.cn

string.find(s, "%d+")
来源：http://wt.szxytkj.cn

[T40] Lua：元表
来源：http://mj.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://gq.gzmigu.cn

[T41] Perl：Hello World
来源：http://ps.asd995.cn

print "Hello\n";
来源：http://ko.bjjhwx.cn

[T42] Perl：变量类型
来源：http://mg.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sb.panjiajie.cn

[T43] Perl：字符串插值
来源：http://mf.shxzukj.cn

"值: $a"
来源：http://ua.yuntaijiaju.cn

[T44] Perl：条件
来源：http://lz.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://nr.gzmigu.cn

[T45] Perl：数组遍历
来源：http://dg.asd995.cn

for my $x (@arr) { print $x; }
来源：http://tf.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://ac.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mj.9csxet.cn

[T47] Perl：正则捕获
来源：http://ni.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://it.shxzskj.cn

[T48] Perl：正则替换
来源：http://fp.hnjuh.cn

$s =~ s/old/new/g;
来源：http://yn.colortex.cn

[T49] Perl：函数
来源：http://xz.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cg.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://ca.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zg.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://jm.lnxyls.cn

[T51] Scala：Hello World
来源：http://jp.hnjuh.cn

println("Hello")
来源：http://nb.nicolike.cn

[T52] Scala：变量
来源：http://rn.521024.cn

val a = 1;  var b = 2
来源：http://qd.szsharing.cn

[T53] Scala：字符串插值
来源：http://qk.nszjky.cn

s"值: $b"
来源：http://yh.lnxyls.cn

[T54] Scala：集合映射
来源：http://zo.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://af.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://dc.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gg.9csxet.cn

[T56] Scala：样例类
来源：http://uy.521024.cn

case class User(name: String, age: Int)
来源：http://ua.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://zt.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://te.szxytkj.cn

[T58] Scala：函数定义
来源：http://kn.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dx.hahajie.cn

[T59] Scala：循环
来源：http://es.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://kw.huanxung.cn

[T60] Scala：折叠
来源：http://va.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rj.newstarts.cn

================================================================================
来源：http://du.jianghongdianzi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://in.haigaiapp.cn

================================================================================
来源：http://gq.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://xg.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://co.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://iq.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gk.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://sw.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yu.shxzskj.cn

[U04] Py：变量调试打印
来源：http://uh.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bn.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://gk.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://fn.huanxung.cn

[U06] Py：合并两个字典
来源：http://sc.521024.cn

{**a, **b}
来源：http://fb.huanxung.cn

[U07] Py：反转字典键值
来源：http://xe.asd995.cn

{v: k for k, v in d.items()}
来源：http://vb.panjiajie.cn

[U08] Py：展平二维列表
来源：http://hg.szxytkj.cn

[y for x in nested for y in x]
来源：http://ga.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://kg.muxihuayi.cn

max(d, key=d.get)
来源：http://dd.asd995.cn

[U10] Py：按值排序字典
来源：http://lg.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qa.panjiajie.cn


<!-- 参考信息 -->