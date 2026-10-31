代发 wailian999

split -l 1000 big.log part_
来源：http://iy.lnxyls.cn

[R74] 批量重命名
来源：http://pw.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ah.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://vz.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://qw.jctech888.com.cn

[R76] 使用临时文件
来源：http://ka.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mt.panjiajie.cn

[R77] 读取用户输入
来源：http://by.chemitech.net.cn

read -rp "请输入: " ans
来源：http://nn.yuexingan06.cn

[R78] 交互式菜单
来源：http://ep.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rw.yuexingan06.cn

[R79] 解析命令行选项
来源：http://aw.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nj.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://bt.colortex.cn

time ./run.sh
来源：http://oa.muxihuayi.cn

================================================================================
来源：http://rs.newstarts.cn

S. C / C++ 专题
来源：http://xb.szsharing.cn

================================================================================
来源：http://em.gzmigu.cn

[S01] C：Hello World
来源：http://qj.haigaiapp.cn

#include <stdio.h>
来源：http://rw.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zy.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://xb.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://pq.szsharing.cn

[S03] C：读入整数
来源：http://be.hahajie.cn

int x; scanf("%d", &x);
来源：http://ck.shxzukj.cn

[S04] C：字符串复制
来源：http://bh.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vm.szxytkj.cn

[S05] C：字符串长度
来源：http://hc.hahajie.cn

strlen(s)
来源：http://mj.lnxyls.cn

[S06] C：字符串比较
来源：http://nz.szxytkj.cn

strcmp(a, b) == 0
来源：http://yc.hnjuh.cn

[S07] C：数组遍历求和
来源：http://id.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vr.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://hm.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://px.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://sm.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fe.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://lf.newstarts.cn

int *p = &a;  *p = 5;
来源：http://jq.shxzukj.cn

[S11] C：逐行读文件
来源：http://nv.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://nk.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ow.panjiajie.cn

fclose(f);
来源：http://mu.huixinmuqiang.cn

[S12] C：写文件
来源：http://re.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nq.huixinmuqiang.cn

[S13] C：宏定义
来源：http://mx.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kg.szxytkj.cn

[S14] C：枚举
来源：http://hv.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://wa.bookmarksfly.cn

[S15] C：类型转换
来源：http://uc.nicolike.cn

(double) a / b
来源：http://go.9csxet.cn

[S16] C：位操作置位
来源：http://ph.huanxung.cn

x |= (1 << 3);
来源：http://tp.nicolike.cn

[S17] C：安全拼接字符串
来源：http://mb.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ip.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://ml.huanxung.cn

int main(int argc, char **argv)
来源：http://qo.gzmigu.cn

[S19] C：快速排序
来源：http://tp.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hc.colortex.cn

[S20] C：二分查找
来源：http://gi.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://si.hahajie.cn

[S21] C：字符类别判断
来源：http://ap.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ku.hnjuh.cn

[S22] C：字符串转数字
来源：http://xf.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yl.nszjky.cn

[S23] C：随机数
来源：http://ha.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yj.wgjwhj.cn

[S24] C：获取本地时间
来源：http://gd.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fp.wgjwhj.cn

[S25] C：内存拷贝
来源：http://wf.gzmigu.cn

memcpy(dst, src, n);
来源：http://rz.shtwfgs.cn

[S26] C：内存清零
来源：http://qt.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://xd.gzmigu.cn

[S27] C：定义常量
来源：http://ih.haigaiapp.cn

const double PI = 3.14159;
来源：http://rt.huanxung.cn

[S28] C：静态变量
来源：http://in.lnxyls.cn

static int counter = 0;
来源：http://jk.panjiajie.cn

[S29] C：变参函数
来源：http://dv.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pv.gzmigu.cn

[S30] C：头文件保护
来源：http://lm.jianghongdianzi.cn

#ifndef X_H
来源：http://vj.szxytkj.cn

#define X_H
来源：http://vs.shtwfgs.cn

#endif
来源：http://op.yuexingan06.cn

[S31] C++：Hello World
来源：http://rq.muxihuayi.cn

#include <iostream>
来源：http://pq.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://vy.haigaiapp.cn

[S32] C++：字符串
来源：http://hd.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://cf.bjjhwx.cn

[S33] C++：vector 增删
来源：http://se.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rc.szxytkj.cn

[S34] C++：遍历 vector
来源：http://ck.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ib.asd995.cn

[S35] C++：map
来源：http://om.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pc.shxzukj.cn

[S36] C++：unordered_map
来源：http://ed.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ns.hnjuh.cn

[S37] C++：set
来源：http://sr.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ae.wgjwhj.cn

[S38] C++：排序
来源：http://iy.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://el.521024.cn

[S39] C++：自定义比较器排序
来源：http://pm.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ji.newstarts.cn

[S40] C++：查找元素
来源：http://qq.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sc.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://gg.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vi.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://db.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://ev.haigaiapp.cn

[S43] C++：智能指针
来源：http://vq.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://kp.shxzskj.cn

[S44] C++：引用传参
来源：http://kr.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://sy.shtwfgs.cn

[S45] C++：lambda
来源：http://ur.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ln.wgjwhj.cn

[S46] C++：函数模板
来源：http://ib.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://da.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://qd.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mp.colortex.cn

[S48] C++：逐行读文件
来源：http://zt.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dr.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://uy.jctech888.com.cn

[S49] C++：写文件
来源：http://ll.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pj.colortex.cn

[S50] C++：格式化数字
来源：http://sb.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kh.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://md.lnxyls.cn

static_cast<double>(a) / b
来源：http://zi.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://dz.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://vv.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://dl.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://lf.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://tm.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kg.gzmigu.cn

[S55] C++：结构化绑定
来源：http://vw.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nn.hahajie.cn

[S56] C++：optional
来源：http://vs.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://us.haigaiapp.cn

[S57] C++：编译期常量
来源：http://kw.shtwfgs.cn

constexpr int N = 10;
来源：http://jl.hahajie.cn

[S58] C++：命名空间
来源：http://rj.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://bp.yuexingan06.cn

[S59] C++：静态断言
来源：http://vn.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sz.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://ky.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lb.wgjwhj.cn

================================================================================
来源：http://xv.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zv.wgjwhj.cn

================================================================================
来源：http://fl.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://fv.bookmarksfly.cn

println("Hello")
来源：http://vs.nszjky.cn

[T02] Kotlin：变量
来源：http://dw.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kv.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://zh.colortex.cn

"值: $b"
来源：http://cf.nszjky.cn

[T04] Kotlin：空安全
来源：http://gk.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://bj.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://je.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nt.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://bf.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mw.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://ra.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oh.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://ls.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://bv.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://pg.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://ji.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://sa.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fa.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://eq.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nv.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://hy.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://ve.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://ti.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://hb.huanxung.cn

[T14] Kotlin：循环
来源：http://nu.nszjky.cn

for (i in 1..10) println(i)
来源：http://ph.huanxung.cn

[T15] Kotlin：接口
来源：http://sp.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://pr.huanxung.cn

[T16] Swift：Hello World
来源：http://ty.huixinmuqiang.cn

print("Hello")
来源：http://zb.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ly.huanxung.cn

var a = 1;  let b = 2
来源：http://gd.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://iq.asd995.cn

"值: \(b)"
来源：http://pw.szsharing.cn

[T19] Swift：可选绑定
来源：http://wb.huixiangedu.cn

if let n = opt { print(n) }
来源：http://aq.colortex.cn

[T20] Swift：数组操作
来源：http://ue.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dl.szsharing.cn

[T21] Swift：遍历
来源：http://dm.wgjwhj.cn

for x in a { print(x) }
来源：http://vv.huixinmuqiang.cn

[T22] Swift：字典
来源：http://vb.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qr.wgjwhj.cn

[T23] Swift：函数
来源：http://if.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ut.shxzukj.cn

[T24] Swift：闭包
来源：http://di.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zs.colortex.cn

[T25] Swift：结构体
来源：http://ba.szsharing.cn

struct P { var x: Int }
来源：http://zv.bjjhwx.cn

[T26] Swift：类与重写
来源：http://ri.szxytkj.cn

class A: Base { override func f() {} }
来源：http://sk.hahajie.cn

[T27] Swift：错误处理
来源：http://jp.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://pq.panjiajie.cn

[T28] Swift：枚举
来源：http://nb.newstarts.cn

enum Color { case red, green }
来源：http://wu.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ge.shxzskj.cn

guard let x = opt else { return }
来源：http://za.nicolike.cn

[T30] Swift：协议
来源：http://pw.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://fb.lnxyls.cn

[T31] Lua：Hello World
来源：http://os.shxzukj.cn

print("Hello")
来源：http://jg.wgjwhj.cn

[T32] Lua：局部变量
来源：http://dt.jianghongdianzi.cn

local a = 1
来源：http://sd.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://px.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zj.shxzukj.cn

[T34] Lua：遍历表
来源：http://hl.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fk.szsharing.cn

[T35] Lua：字典表
来源：http://dw.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://sq.shtwfgs.cn

[T36] Lua：函数
来源：http://qr.huanxung.cn

function add(a, b) return a + b end
来源：http://zr.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://xa.huixinmuqiang.cn

"a" .. "b"
来源：http://lz.colortex.cn

[T38] Lua：条件
来源：http://ec.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://sc.szsharing.cn

[T39] Lua：模式匹配
来源：http://ew.jctech888.com.cn

string.find(s, "%d+")
来源：http://zq.bjjhwx.cn

[T40] Lua：元表
来源：http://vt.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://lr.hnjuh.cn

[T41] Perl：Hello World
来源：http://rv.shtwfgs.cn

print "Hello\n";
来源：http://wi.szsharing.cn

[T42] Perl：变量类型
来源：http://of.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kg.panjiajie.cn

[T43] Perl：字符串插值
来源：http://gl.lnxyls.cn

"值: $a"
来源：http://gm.bjjhwx.cn

[T44] Perl：条件
来源：http://lr.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://fo.huanxung.cn

[T45] Perl：数组遍历
来源：http://ga.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://dn.hahajie.cn

[T46] Perl：哈希操作
来源：http://yj.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kn.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://rj.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wo.colortex.cn

[T48] Perl：正则替换
来源：http://br.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://ae.lnxyls.cn

[T49] Perl：函数
来源：http://qs.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ym.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://ge.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://db.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://mw.nicolike.cn

[T51] Scala：Hello World
来源：http://eh.huanxung.cn

println("Hello")
来源：http://lh.huanxung.cn

[T52] Scala：变量
来源：http://xm.colortex.cn

val a = 1;  var b = 2
来源：http://hh.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ee.jctech888.com.cn

s"值: $b"
来源：http://fv.521024.cn

[T54] Scala：集合映射
来源：http://we.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://wc.asd995.cn

[T55] Scala：集合过滤
来源：http://dw.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lo.shxzukj.cn

[T56] Scala：样例类
来源：http://zo.hahajie.cn

case class User(name: String, age: Int)
来源：http://cl.lnxyls.cn

[T57] Scala：模式匹配
来源：http://tc.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tf.hnjuh.cn

[T58] Scala：函数定义
来源：http://ns.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lu.yuntaijiaju.cn

[T59] Scala：循环
来源：http://ph.newstarts.cn

for (i <- 1 to 10) println(i)
来源：http://do.szxytkj.cn

[T60] Scala：折叠
来源：http://hq.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rx.lnxyls.cn

================================================================================
来源：http://zw.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://am.panjiajie.cn

================================================================================
来源：http://tc.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://py.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ud.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://ub.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wd.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://ph.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sk.colortex.cn

[U04] Py：变量调试打印
来源：http://aj.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bd.colortex.cn

[U05] Py：列表去重且保序
来源：http://ku.colortex.cn

list(dict.fromkeys(arr))
来源：http://tu.colortex.cn

[U06] Py：合并两个字典
来源：http://if.muxihuayi.cn

{**a, **b}
来源：http://uu.colortex.cn

[U07] Py：反转字典键值
来源：http://aa.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://py.asd995.cn

[U08] Py：展平二维列表
来源：http://aa.gzmigu.cn

[y for x in nested for y in x]
来源：http://co.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://ib.bjjhwx.cn

max(d, key=d.get)
来源：http://ek.huanxung.cn

[U10] Py：按值排序字典
来源：http://gj.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xw.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://mv.hnjuh.cn

(x * 2 for x in arr)
来源：http://mi.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cf.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://xj.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://jq.nszjky.cn

deque(maxlen=10)
来源：http://rt.asd995.cn

[U14] Py：分组收集到列表
来源：http://sj.bjjhwx.cn

defaultdict(list)
来源：http://bs.hahajie.cn


<!-- 参考信息 -->