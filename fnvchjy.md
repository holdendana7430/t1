代发 wailian999

split -l 1000 big.log part_
来源：http://zk.shxzukj.cn

[R74] 批量重命名
来源：http://zm.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ux.nicolike.cn

[R75] 导出环境变量
来源：http://mg.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://gt.gzmigu.cn

[R76] 使用临时文件
来源：http://aw.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uz.hahajie.cn

[R77] 读取用户输入
来源：http://mq.shtwfgs.cn

read -rp "请输入: " ans
来源：http://sq.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://zh.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nm.szsharing.cn

[R79] 解析命令行选项
来源：http://vk.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sl.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://ss.huixinmuqiang.cn

time ./run.sh
来源：http://ys.szsharing.cn

================================================================================
来源：http://sr.shtwfgs.cn

S. C / C++ 专题
来源：http://rj.huixiangedu.cn

================================================================================
来源：http://uv.yuexingan06.cn

[S01] C：Hello World
来源：http://os.lnxyls.cn

#include <stdio.h>
来源：http://kc.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ik.huanxung.cn

[S02] C：变量与格式化输出
来源：http://gj.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://ly.muxihuayi.cn

[S03] C：读入整数
来源：http://ls.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ja.yuexingan06.cn

[S04] C：字符串复制
来源：http://bs.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nszjky.cn

[S05] C：字符串长度
来源：http://qx.muxihuayi.cn

strlen(s)
来源：http://ku.colortex.cn

[S06] C：字符串比较
来源：http://hf.szxytkj.cn

strcmp(a, b) == 0
来源：http://kj.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://hp.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lp.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://wh.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jj.asd995.cn

[S09] C：结构体定义与初始化
来源：http://et.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qe.wgjwhj.cn

[S10] C：指针与解引用
来源：http://vf.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ie.huanxung.cn

[S11] C：逐行读文件
来源：http://bc.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ed.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fc.shxzukj.cn

fclose(f);
来源：http://dn.nszjky.cn

[S12] C：写文件
来源：http://zy.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://do.colortex.cn

[S13] C：宏定义
来源：http://kr.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rp.shxzskj.cn

[S14] C：枚举
来源：http://xz.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://tq.lnxyls.cn

[S15] C：类型转换
来源：http://vp.muxihuayi.cn

(double) a / b
来源：http://lo.panjiajie.cn

[S16] C：位操作置位
来源：http://ko.huixiangedu.cn

x |= (1 << 3);
来源：http://bw.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://pp.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xi.hnjuh.cn

[S18] C：命令行参数
来源：http://gj.bjjhwx.cn

int main(int argc, char **argv)
来源：http://lq.jianghongdianzi.cn

[S19] C：快速排序
来源：http://ui.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ut.yuntaijiaju.cn

[S20] C：二分查找
来源：http://kl.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://us.chemitech.net.cn

[S21] C：字符类别判断
来源：http://tk.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://op.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://bn.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bv.chemitech.net.cn

[S23] C：随机数
来源：http://ab.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mf.shxzukj.cn

[S24] C：获取本地时间
来源：http://ae.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iv.jctech888.com.cn

[S25] C：内存拷贝
来源：http://fd.huixiangedu.cn

memcpy(dst, src, n);
来源：http://pc.shxzskj.cn

[S26] C：内存清零
来源：http://ww.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://yw.hahajie.cn

[S27] C：定义常量
来源：http://na.chemitech.net.cn

const double PI = 3.14159;
来源：http://cr.huixiangedu.cn

[S28] C：静态变量
来源：http://hb.szsharing.cn

static int counter = 0;
来源：http://ho.nszjky.cn

[S29] C：变参函数
来源：http://kp.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://us.hnjuh.cn

[S30] C：头文件保护
来源：http://nq.huixinmuqiang.cn

#ifndef X_H
来源：http://td.shxzskj.cn

#define X_H
来源：http://mr.9csxet.cn

#endif
来源：http://hq.9csxet.cn

[S31] C++：Hello World
来源：http://gj.haigaiapp.cn

#include <iostream>
来源：http://di.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ll.shxzukj.cn

[S32] C++：字符串
来源：http://yp.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://xz.huixiangedu.cn

[S33] C++：vector 增删
来源：http://hn.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ji.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://xd.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://ht.jctech888.com.cn

[S35] C++：map
来源：http://md.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mv.huixiangedu.cn

[S36] C++：unordered_map
来源：http://jk.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uf.521024.cn

[S37] C++：set
来源：http://zp.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ly.hnjuh.cn

[S38] C++：排序
来源：http://uy.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://nq.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://ds.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iw.hnjuh.cn

[S40] C++：查找元素
来源：http://lh.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zn.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://so.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ux.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://fx.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://lx.9csxet.cn

[S43] C++：智能指针
来源：http://zv.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://ie.jctech888.com.cn

[S44] C++：引用传参
来源：http://rs.colortex.cn

void inc(int &x) { ++x; }
来源：http://ia.shtwfgs.cn

[S45] C++：lambda
来源：http://kf.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uk.nszjky.cn

[S46] C++：函数模板
来源：http://rr.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tc.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://fs.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bl.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://km.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zf.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ze.nicolike.cn

[S49] C++：写文件
来源：http://lq.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lh.chemitech.net.cn

[S50] C++：格式化数字
来源：http://lg.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tc.521024.cn

[S51] C++：显式类型转换
来源：http://dz.nszjky.cn

static_cast<double>(a) / b
来源：http://xi.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://tu.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://un.gzmigu.cn

[S53] C++：移动语义
来源：http://zc.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://bs.bookmarksfly.cn

[S54] C++：异常处理
来源：http://cu.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iz.nszjky.cn

[S55] C++：结构化绑定
来源：http://gd.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bx.521024.cn

[S56] C++：optional
来源：http://ou.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pu.szxytkj.cn

[S57] C++：编译期常量
来源：http://ob.521024.cn

constexpr int N = 10;
来源：http://zb.panjiajie.cn

[S58] C++：命名空间
来源：http://fd.521024.cn

namespace ns { int f() { return 1; } }
来源：http://dj.521024.cn

[S59] C++：静态断言
来源：http://mh.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ar.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://kv.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qj.521024.cn

================================================================================
来源：http://uq.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ki.nicolike.cn

================================================================================
来源：http://rs.huanxung.cn

[T01] Kotlin：Hello World
来源：http://vh.bookmarksfly.cn

println("Hello")
来源：http://kt.asd995.cn

[T02] Kotlin：变量
来源：http://ok.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nq.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://ms.nszjky.cn

"值: $b"
来源：http://oz.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://qf.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://jm.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://bf.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nr.huanxung.cn

[T06] Kotlin：集合映射
来源：http://cz.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ai.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://lu.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jn.newstarts.cn

[T08] Kotlin：数据类
来源：http://dn.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://bz.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://vp.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://wt.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://zw.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vb.panjiajie.cn

[T11] Kotlin：协程
来源：http://qy.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kz.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://sy.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://ho.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://yf.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://tp.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://np.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://jv.muxihuayi.cn

[T15] Kotlin：接口
来源：http://ss.huanxung.cn

interface Shape { fun area(): Double }
来源：http://db.9csxet.cn

[T16] Swift：Hello World
来源：http://xb.szsharing.cn

print("Hello")
来源：http://nu.huanxung.cn

[T17] Swift：变量与常量
来源：http://fb.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://nh.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://fa.hnjuh.cn

"值: \(b)"
来源：http://ul.shxzukj.cn

[T19] Swift：可选绑定
来源：http://dh.shxzukj.cn

if let n = opt { print(n) }
来源：http://gg.chemitech.net.cn

[T20] Swift：数组操作
来源：http://xw.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ku.9csxet.cn

[T21] Swift：遍历
来源：http://pd.haigaiapp.cn

for x in a { print(x) }
来源：http://me.jianghongdianzi.cn

[T22] Swift：字典
来源：http://zo.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ml.huixinmuqiang.cn

[T23] Swift：函数
来源：http://jg.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cl.yuexingan06.cn

[T24] Swift：闭包
来源：http://am.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dk.shxzukj.cn

[T25] Swift：结构体
来源：http://io.muxihuayi.cn

struct P { var x: Int }
来源：http://om.huanxung.cn

[T26] Swift：类与重写
来源：http://mh.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://cl.9csxet.cn

[T27] Swift：错误处理
来源：http://aa.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://tb.jctech888.com.cn

[T28] Swift：枚举
来源：http://uw.jctech888.com.cn

enum Color { case red, green }
来源：http://cr.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://kt.muxihuayi.cn

guard let x = opt else { return }
来源：http://sl.yuexingan06.cn

[T30] Swift：协议
来源：http://ej.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://ic.wgjwhj.cn

[T31] Lua：Hello World
来源：http://ml.huixinmuqiang.cn

print("Hello")
来源：http://kd.shxzskj.cn

[T32] Lua：局部变量
来源：http://hc.jctech888.com.cn

local a = 1
来源：http://bc.521024.cn

[T33] Lua：表（数组）
来源：http://vz.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ye.nszjky.cn

[T34] Lua：遍历表
来源：http://bo.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tp.hahajie.cn

[T35] Lua：字典表
来源：http://vc.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://mr.newstarts.cn

[T36] Lua：函数
来源：http://md.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://dw.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://zz.huanxung.cn

"a" .. "b"
来源：http://rv.panjiajie.cn

[T38] Lua：条件
来源：http://ec.shxzskj.cn

if x > 0 then print("正") end
来源：http://vc.huanxung.cn

[T39] Lua：模式匹配
来源：http://rh.bookmarksfly.cn

string.find(s, "%d+")
来源：http://bs.bookmarksfly.cn

[T40] Lua：元表
来源：http://bz.newstarts.cn

setmetatable({}, { __index = base })
来源：http://pw.lnxyls.cn

[T41] Perl：Hello World
来源：http://zw.huixinmuqiang.cn

print "Hello\n";
来源：http://hn.yuexingan06.cn

[T42] Perl：变量类型
来源：http://zr.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jl.newstarts.cn

[T43] Perl：字符串插值
来源：http://wf.shtwfgs.cn

"值: $a"
来源：http://ad.521024.cn

[T44] Perl：条件
来源：http://cy.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://wf.huanxung.cn

[T45] Perl：数组遍历
来源：http://ri.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://fp.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://qd.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ks.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://ek.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lq.shtwfgs.cn

[T48] Perl：正则替换
来源：http://nh.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://kw.huanxung.cn

[T49] Perl：函数
来源：http://bn.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qb.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://by.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ng.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://xs.huixiangedu.cn

[T51] Scala：Hello World
来源：http://ns.huanxung.cn

println("Hello")
来源：http://iq.yuntaijiaju.cn

[T52] Scala：变量
来源：http://wy.huanxung.cn

val a = 1;  var b = 2
来源：http://nr.hahajie.cn

[T53] Scala：字符串插值
来源：http://qu.colortex.cn

s"值: $b"
来源：http://ah.gzmigu.cn

[T54] Scala：集合映射
来源：http://rd.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://js.colortex.cn

[T55] Scala：集合过滤
来源：http://kw.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sd.hahajie.cn

[T56] Scala：样例类
来源：http://on.panjiajie.cn

case class User(name: String, age: Int)
来源：http://yu.lnxyls.cn

[T57] Scala：模式匹配
来源：http://xo.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ve.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://tk.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xb.muxihuayi.cn

[T59] Scala：循环
来源：http://yj.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://xe.panjiajie.cn

[T60] Scala：折叠
来源：http://sf.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qp.shtwfgs.cn

================================================================================
来源：http://up.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cm.wgjwhj.cn

================================================================================
来源：http://ry.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://pk.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wm.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://ap.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gm.colortex.cn

[U03] Py：加载 .env 配置
来源：http://nx.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ck.colortex.cn

[U04] Py：变量调试打印
来源：http://mo.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rr.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://ju.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://bg.asd995.cn

[U06] Py：合并两个字典
来源：http://uy.asd995.cn

{**a, **b}
来源：http://oj.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://gr.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://ij.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://av.hahajie.cn

[y for x in nested for y in x]
来源：http://qe.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://un.bookmarksfly.cn

max(d, key=d.get)
来源：http://rl.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://mc.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gc.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://gf.hnjuh.cn

(x * 2 for x in arr)
来源：http://su.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wy.szxytkj.cn

Counter(arr).most_common(3)
来源：http://zu.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://ix.asd995.cn

deque(maxlen=10)
来源：http://qw.szsharing.cn

[U14] Py：分组收集到列表
来源：http://tn.newstarts.cn

defaultdict(list)
来源：http://pf.muxihuayi.cn


<!-- 参考信息 -->