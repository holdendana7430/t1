代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://uk.szxytkj.cn

[R72] 等待端口就绪
来源：http://il.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tp.shxzukj.cn

[R73] 分割大日志
来源：http://vm.asd995.cn

split -l 1000 big.log part_
来源：http://fu.szsharing.cn

[R74] 批量重命名
来源：http://yo.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nf.9csxet.cn

[R75] 导出环境变量
来源：http://yd.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://ya.newstarts.cn

[R76] 使用临时文件
来源：http://ts.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tj.chemitech.net.cn

[R77] 读取用户输入
来源：http://wm.haigaiapp.cn

read -rp "请输入: " ans
来源：http://rn.shxzukj.cn

[R78] 交互式菜单
来源：http://hq.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://an.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://lw.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yd.asd995.cn

[R80] 查看脚本执行耗时
来源：http://tv.chemitech.net.cn

time ./run.sh
来源：http://uo.bookmarksfly.cn

================================================================================
来源：http://gn.panjiajie.cn

S. C / C++ 专题
来源：http://ku.yuntaijiaju.cn

================================================================================
来源：http://jw.colortex.cn

[S01] C：Hello World
来源：http://uv.shxzukj.cn

#include <stdio.h>
来源：http://qu.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xm.hahajie.cn

[S02] C：变量与格式化输出
来源：http://qn.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://kz.szsharing.cn

[S03] C：读入整数
来源：http://lj.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://lr.521024.cn

[S04] C：字符串复制
来源：http://ac.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vx.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://ts.bookmarksfly.cn

strlen(s)
来源：http://ju.9csxet.cn

[S06] C：字符串比较
来源：http://yn.haigaiapp.cn

strcmp(a, b) == 0
来源：http://zl.huanxung.cn

[S07] C：数组遍历求和
来源：http://tl.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lz.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://vd.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gk.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://jn.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oj.lnxyls.cn

[S10] C：指针与解引用
来源：http://ac.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://yv.colortex.cn

[S11] C：逐行读文件
来源：http://mx.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://jl.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tk.9csxet.cn

fclose(f);
来源：http://vx.hnjuh.cn

[S12] C：写文件
来源：http://zc.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ee.bjjhwx.cn

[S13] C：宏定义
来源：http://wd.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sn.huixiangedu.cn

[S14] C：枚举
来源：http://se.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://uf.huixiangedu.cn

[S15] C：类型转换
来源：http://uc.yuntaijiaju.cn

(double) a / b
来源：http://id.muxihuayi.cn

[S16] C：位操作置位
来源：http://il.lnxyls.cn

x |= (1 << 3);
来源：http://tg.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://ss.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gl.9csxet.cn

[S18] C：命令行参数
来源：http://sl.panjiajie.cn

int main(int argc, char **argv)
来源：http://un.newstarts.cn

[S19] C：快速排序
来源：http://ql.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jh.huanxung.cn

[S20] C：二分查找
来源：http://pp.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://da.haigaiapp.cn

[S21] C：字符类别判断
来源：http://fy.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rb.huanxung.cn

[S22] C：字符串转数字
来源：http://ut.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ls.newstarts.cn

[S23] C：随机数
来源：http://kl.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iy.huanxung.cn

[S24] C：获取本地时间
来源：http://wd.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jb.newstarts.cn

[S25] C：内存拷贝
来源：http://ku.szxytkj.cn

memcpy(dst, src, n);
来源：http://xh.shtwfgs.cn

[S26] C：内存清零
来源：http://gj.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://sb.yuexingan06.cn

[S27] C：定义常量
来源：http://kq.chemitech.net.cn

const double PI = 3.14159;
来源：http://at.huixinmuqiang.cn

[S28] C：静态变量
来源：http://gz.lnxyls.cn

static int counter = 0;
来源：http://gk.huixinmuqiang.cn

[S29] C：变参函数
来源：http://bf.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ev.9csxet.cn

[S30] C：头文件保护
来源：http://mu.huixiangedu.cn

#ifndef X_H
来源：http://jh.huixinmuqiang.cn

#define X_H
来源：http://yt.yuntaijiaju.cn

#endif
来源：http://jv.newstarts.cn

[S31] C++：Hello World
来源：http://tb.chemitech.net.cn

#include <iostream>
来源：http://dr.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://mh.panjiajie.cn

[S32] C++：字符串
来源：http://ya.521024.cn

std::string s = "hi";  s += "!";
来源：http://qn.muxihuayi.cn

[S33] C++：vector 增删
来源：http://qg.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bv.colortex.cn

[S34] C++：遍历 vector
来源：http://tu.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://mw.yuexingan06.cn

[S35] C++：map
来源：http://ap.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pb.shtwfgs.cn

[S36] C++：unordered_map
来源：http://od.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://po.szxytkj.cn

[S37] C++：set
来源：http://uk.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dd.lnxyls.cn

[S38] C++：排序
来源：http://oc.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://vn.521024.cn

[S39] C++：自定义比较器排序
来源：http://sz.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://he.newstarts.cn

[S40] C++：查找元素
来源：http://fu.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gn.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ie.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gm.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://pz.521024.cn

class B : public Base { public: void f() override {} };
来源：http://zs.haigaiapp.cn

[S43] C++：智能指针
来源：http://sy.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://gc.shxzukj.cn

[S44] C++：引用传参
来源：http://iw.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://wy.521024.cn

[S45] C++：lambda
来源：http://fu.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cz.shtwfgs.cn

[S46] C++：函数模板
来源：http://dp.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zc.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://kp.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ui.szsharing.cn

[S48] C++：逐行读文件
来源：http://hl.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gm.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ix.shxzskj.cn

[S49] C++：写文件
来源：http://zj.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lp.huixiangedu.cn

[S50] C++：格式化数字
来源：http://gc.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xc.colortex.cn

[S51] C++：显式类型转换
来源：http://cr.shxzukj.cn

static_cast<double>(a) / b
来源：http://ep.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://ri.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://zg.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://gr.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://bb.haigaiapp.cn

[S54] C++：异常处理
来源：http://yf.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hl.9csxet.cn

[S55] C++：结构化绑定
来源：http://hu.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kl.chemitech.net.cn

[S56] C++：optional
来源：http://tg.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pq.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ym.haigaiapp.cn

constexpr int N = 10;
来源：http://dy.szxytkj.cn

[S58] C++：命名空间
来源：http://qb.521024.cn

namespace ns { int f() { return 1; } }
来源：http://va.lnxyls.cn

[S59] C++：静态断言
来源：http://og.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fb.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://ng.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kx.asd995.cn

================================================================================
来源：http://vi.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pq.nicolike.cn

================================================================================
来源：http://wj.newstarts.cn

[T01] Kotlin：Hello World
来源：http://za.haigaiapp.cn

println("Hello")
来源：http://gv.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://en.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ds.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://tg.lnxyls.cn

"值: $b"
来源：http://hl.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://lx.panjiajie.cn

val n: String? = null;  n?.length
来源：http://vm.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://ex.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wd.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://mm.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hw.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://ri.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vi.szxytkj.cn

[T08] Kotlin：数据类
来源：http://mx.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://ur.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://dg.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://xm.newstarts.cn

[T10] Kotlin：默认参数
来源：http://wg.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yq.nszjky.cn

[T11] Kotlin：协程
来源：http://ot.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pu.huanxung.cn

[T12] Kotlin：解构声明
来源：http://do.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://dn.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://cq.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://uk.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://sw.huanxung.cn

for (i in 1..10) println(i)
来源：http://vp.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://cv.521024.cn

interface Shape { fun area(): Double }
来源：http://zq.wgjwhj.cn

[T16] Swift：Hello World
来源：http://us.shxzukj.cn

print("Hello")
来源：http://zf.hahajie.cn

[T17] Swift：变量与常量
来源：http://ur.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ki.hahajie.cn

[T18] Swift：字符串插值
来源：http://sj.szxytkj.cn

"值: \(b)"
来源：http://ij.hahajie.cn

[T19] Swift：可选绑定
来源：http://kq.bjjhwx.cn

if let n = opt { print(n) }
来源：http://uy.lnxyls.cn

[T20] Swift：数组操作
来源：http://mr.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lh.szsharing.cn

[T21] Swift：遍历
来源：http://tp.nszjky.cn

for x in a { print(x) }
来源：http://ez.shtwfgs.cn

[T22] Swift：字典
来源：http://ne.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kv.521024.cn

[T23] Swift：函数
来源：http://ix.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iv.shxzukj.cn

[T24] Swift：闭包
来源：http://ek.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ss.asd995.cn

[T25] Swift：结构体
来源：http://pd.huixiangedu.cn

struct P { var x: Int }
来源：http://ft.gzmigu.cn

[T26] Swift：类与重写
来源：http://tr.hnjuh.cn

class A: Base { override func f() {} }
来源：http://iy.szxytkj.cn

[T27] Swift：错误处理
来源：http://as.colortex.cn

do { try f() } catch { print(error) }
来源：http://rz.521024.cn

[T28] Swift：枚举
来源：http://bm.haigaiapp.cn

enum Color { case red, green }
来源：http://wr.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://sz.nszjky.cn

guard let x = opt else { return }
来源：http://hf.jianghongdianzi.cn

[T30] Swift：协议
来源：http://zb.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://bf.9csxet.cn

[T31] Lua：Hello World
来源：http://gy.shxzskj.cn

print("Hello")
来源：http://lx.haigaiapp.cn

[T32] Lua：局部变量
来源：http://ga.shxzskj.cn

local a = 1
来源：http://cu.shxzukj.cn

[T33] Lua：表（数组）
来源：http://su.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ps.panjiajie.cn

[T34] Lua：遍历表
来源：http://fl.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hv.gzmigu.cn

[T35] Lua：字典表
来源：http://wr.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://pu.asd995.cn

[T36] Lua：函数
来源：http://gy.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://pp.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://ne.huanxung.cn

"a" .. "b"
来源：http://as.shtwfgs.cn

[T38] Lua：条件
来源：http://sp.nszjky.cn

if x > 0 then print("正") end
来源：http://ly.shxzukj.cn

[T39] Lua：模式匹配
来源：http://gd.colortex.cn

string.find(s, "%d+")
来源：http://jj.huixinmuqiang.cn

[T40] Lua：元表
来源：http://fi.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://ij.haigaiapp.cn

[T41] Perl：Hello World
来源：http://gj.haigaiapp.cn

print "Hello\n";
来源：http://xk.huanxung.cn

[T42] Perl：变量类型
来源：http://jw.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sz.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://mp.haigaiapp.cn

"值: $a"
来源：http://tx.lnxyls.cn

[T44] Perl：条件
来源：http://en.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://dj.huanxung.cn

[T45] Perl：数组遍历
来源：http://kb.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://qr.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://ui.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vi.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://mz.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bb.hnjuh.cn

[T48] Perl：正则替换
来源：http://oq.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://me.521024.cn

[T49] Perl：函数
来源：http://tm.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pg.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://um.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fh.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ru.hahajie.cn

[T51] Scala：Hello World
来源：http://gy.shxzukj.cn

println("Hello")
来源：http://ms.muxihuayi.cn

[T52] Scala：变量
来源：http://tn.nicolike.cn

val a = 1;  var b = 2
来源：http://nr.szxytkj.cn

[T53] Scala：字符串插值
来源：http://sc.9csxet.cn

s"值: $b"
来源：http://fy.panjiajie.cn

[T54] Scala：集合映射
来源：http://er.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://bi.521024.cn

[T55] Scala：集合过滤
来源：http://at.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xi.panjiajie.cn

[T56] Scala：样例类
来源：http://am.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://hc.panjiajie.cn

[T57] Scala：模式匹配
来源：http://as.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iw.panjiajie.cn

[T58] Scala：函数定义
来源：http://yx.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bi.newstarts.cn

[T59] Scala：循环
来源：http://xa.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://oy.lnxyls.cn

[T60] Scala：折叠
来源：http://br.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jy.huixiangedu.cn

================================================================================
来源：http://vk.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jq.shxzukj.cn

================================================================================
来源：http://rn.521024.cn

[U01] Py：创建虚拟环境
来源：http://zb.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ol.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://sj.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uh.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://bs.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://si.shxzukj.cn

[U04] Py：变量调试打印
来源：http://ii.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vd.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://wu.bookmarksfly.cn

list(dict.fromkeys(arr))
来源：http://dy.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://be.jianghongdianzi.cn

{**a, **b}
来源：http://da.lnxyls.cn

[U07] Py：反转字典键值
来源：http://pn.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://zs.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://ab.shtwfgs.cn

[y for x in nested for y in x]
来源：http://xc.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://gd.szxytkj.cn

max(d, key=d.get)
来源：http://em.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://nt.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sn.huanxung.cn

[U11] Py：生成器表达式
来源：http://nk.muxihuayi.cn

(x * 2 for x in arr)
来源：http://jo.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://st.lnxyls.cn

Counter(arr).most_common(3)
来源：http://cu.huanxung.cn


<!-- 参考信息 -->