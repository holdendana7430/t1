代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://to.nicolike.cn

[R72] 等待端口就绪
来源：http://gx.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iy.szxytkj.cn

[R73] 分割大日志
来源：http://vf.hnjuh.cn

split -l 1000 big.log part_
来源：http://iu.nicolike.cn

[R74] 批量重命名
来源：http://tl.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fq.szsharing.cn

[R75] 导出环境变量
来源：http://ah.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://no.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://mb.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ko.bjjhwx.cn

[R77] 读取用户输入
来源：http://ut.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://ef.gzmigu.cn

[R78] 交互式菜单
来源：http://rl.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ty.panjiajie.cn

[R79] 解析命令行选项
来源：http://ot.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jy.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://el.huanxung.cn

time ./run.sh
来源：http://go.shxzukj.cn

================================================================================
来源：http://ct.9csxet.cn

S. C / C++ 专题
来源：http://hz.bjjhwx.cn

================================================================================
来源：http://gd.panjiajie.cn

[S01] C：Hello World
来源：http://fx.szsharing.cn

#include <stdio.h>
来源：http://vc.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://io.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://hi.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://xr.shxzukj.cn

[S03] C：读入整数
来源：http://lp.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://je.shtwfgs.cn

[S04] C：字符串复制
来源：http://wj.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ia.nicolike.cn

[S05] C：字符串长度
来源：http://kt.shtwfgs.cn

strlen(s)
来源：http://uo.shxzukj.cn

[S06] C：字符串比较
来源：http://ar.newstarts.cn

strcmp(a, b) == 0
来源：http://tt.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://nj.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eq.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://kp.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bn.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://ub.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yn.szsharing.cn

[S10] C：指针与解引用
来源：http://wl.huanxung.cn

int *p = &a;  *p = 5;
来源：http://lq.gzmigu.cn

[S11] C：逐行读文件
来源：http://gf.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://wd.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lo.muxihuayi.cn

fclose(f);
来源：http://rz.huixiangedu.cn

[S12] C：写文件
来源：http://oy.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sp.hnjuh.cn

[S13] C：宏定义
来源：http://ze.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zz.bjjhwx.cn

[S14] C：枚举
来源：http://dt.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://rj.9csxet.cn

[S15] C：类型转换
来源：http://il.haigaiapp.cn

(double) a / b
来源：http://bq.asd995.cn

[S16] C：位操作置位
来源：http://eu.huixiangedu.cn

x |= (1 << 3);
来源：http://ud.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://gc.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cc.haigaiapp.cn

[S18] C：命令行参数
来源：http://zn.nszjky.cn

int main(int argc, char **argv)
来源：http://ec.lnxyls.cn

[S19] C：快速排序
来源：http://hn.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yk.nicolike.cn

[S20] C：二分查找
来源：http://ey.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wk.9csxet.cn

[S21] C：字符类别判断
来源：http://tg.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ry.wgjwhj.cn

[S22] C：字符串转数字
来源：http://ob.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ew.9csxet.cn

[S23] C：随机数
来源：http://jn.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sm.nszjky.cn

[S24] C：获取本地时间
来源：http://kg.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://es.panjiajie.cn

[S25] C：内存拷贝
来源：http://my.nicolike.cn

memcpy(dst, src, n);
来源：http://zk.jianghongdianzi.cn

[S26] C：内存清零
来源：http://wa.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://yz.yuntaijiaju.cn

[S27] C：定义常量
来源：http://dn.bookmarksfly.cn

const double PI = 3.14159;
来源：http://du.muxihuayi.cn

[S28] C：静态变量
来源：http://js.hahajie.cn

static int counter = 0;
来源：http://ji.asd995.cn

[S29] C：变参函数
来源：http://yb.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ow.panjiajie.cn

[S30] C：头文件保护
来源：http://ay.szxytkj.cn

#ifndef X_H
来源：http://cx.shxzukj.cn

#define X_H
来源：http://fg.yuntaijiaju.cn

#endif
来源：http://bi.newstarts.cn

[S31] C++：Hello World
来源：http://ta.newstarts.cn

#include <iostream>
来源：http://an.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://po.yuexingan06.cn

[S32] C++：字符串
来源：http://my.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://kr.szsharing.cn

[S33] C++：vector 增删
来源：http://up.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kv.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://uw.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ed.jctech888.com.cn

[S35] C++：map
来源：http://ts.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pd.chemitech.net.cn

[S36] C++：unordered_map
来源：http://fw.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hm.panjiajie.cn

[S37] C++：set
来源：http://gf.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wq.521024.cn

[S38] C++：排序
来源：http://ho.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://uk.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://fm.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cg.chemitech.net.cn

[S40] C++：查找元素
来源：http://dp.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eh.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://sr.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tb.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://ks.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://xr.jctech888.com.cn

[S43] C++：智能指针
来源：http://yo.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://of.nicolike.cn

[S44] C++：引用传参
来源：http://nb.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ux.nicolike.cn

[S45] C++：lambda
来源：http://nb.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ve.haigaiapp.cn

[S46] C++：函数模板
来源：http://hc.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://li.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://gz.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hv.hnjuh.cn

[S48] C++：逐行读文件
来源：http://uj.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gj.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://zt.colortex.cn

[S49] C++：写文件
来源：http://vp.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yk.muxihuayi.cn

[S50] C++：格式化数字
来源：http://xj.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sc.gzmigu.cn

[S51] C++：显式类型转换
来源：http://ak.shtwfgs.cn

static_cast<double>(a) / b
来源：http://tq.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ke.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://lw.huanxung.cn

[S53] C++：移动语义
来源：http://sr.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://pd.gzmigu.cn

[S54] C++：异常处理
来源：http://wj.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bi.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://sm.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gt.colortex.cn

[S56] C++：optional
来源：http://si.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yz.haigaiapp.cn

[S57] C++：编译期常量
来源：http://be.hahajie.cn

constexpr int N = 10;
来源：http://jz.colortex.cn

[S58] C++：命名空间
来源：http://ji.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://fq.colortex.cn

[S59] C++：静态断言
来源：http://ne.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://er.asd995.cn

[S60] C++：遍历并删除元素
来源：http://wt.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ti.nszjky.cn

================================================================================
来源：http://fk.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iu.haigaiapp.cn

================================================================================
来源：http://xu.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://jd.huanxung.cn

println("Hello")
来源：http://ct.9csxet.cn

[T02] Kotlin：变量
来源：http://xw.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sk.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://am.lnxyls.cn

"值: $b"
来源：http://ke.nszjky.cn

[T04] Kotlin：空安全
来源：http://sm.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://lc.colortex.cn

[T05] Kotlin：when 表达式
来源：http://sx.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gk.newstarts.cn

[T06] Kotlin：集合映射
来源：http://xg.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nz.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://vs.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xq.newstarts.cn

[T08] Kotlin：数据类
来源：http://yv.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://ep.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://mx.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://vp.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://yd.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://am.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://ce.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ko.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://np.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://oo.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://gl.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://dh.newstarts.cn

[T14] Kotlin：循环
来源：http://ap.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://dc.nszjky.cn

[T15] Kotlin：接口
来源：http://df.asd995.cn

interface Shape { fun area(): Double }
来源：http://yi.chemitech.net.cn

[T16] Swift：Hello World
来源：http://av.gzmigu.cn

print("Hello")
来源：http://mb.asd995.cn

[T17] Swift：变量与常量
来源：http://td.nszjky.cn

var a = 1;  let b = 2
来源：http://bb.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://pk.muxihuayi.cn

"值: \(b)"
来源：http://xj.huanxung.cn

[T19] Swift：可选绑定
来源：http://zv.hahajie.cn

if let n = opt { print(n) }
来源：http://dr.huanxung.cn

[T20] Swift：数组操作
来源：http://kk.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oy.colortex.cn

[T21] Swift：遍历
来源：http://qi.hnjuh.cn

for x in a { print(x) }
来源：http://nq.szsharing.cn

[T22] Swift：字典
来源：http://eo.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dp.chemitech.net.cn

[T23] Swift：函数
来源：http://qg.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pn.szxytkj.cn

[T24] Swift：闭包
来源：http://td.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nh.hahajie.cn

[T25] Swift：结构体
来源：http://yu.hahajie.cn

struct P { var x: Int }
来源：http://hf.hahajie.cn

[T26] Swift：类与重写
来源：http://jv.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ud.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://gw.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://sk.wgjwhj.cn

[T28] Swift：枚举
来源：http://mf.huixiangedu.cn

enum Color { case red, green }
来源：http://bv.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://wm.hnjuh.cn

guard let x = opt else { return }
来源：http://jc.hnjuh.cn

[T30] Swift：协议
来源：http://as.asd995.cn

protocol Shape { func area() -> Double }
来源：http://ue.muxihuayi.cn

[T31] Lua：Hello World
来源：http://yr.jianghongdianzi.cn

print("Hello")
来源：http://sq.panjiajie.cn

[T32] Lua：局部变量
来源：http://ko.panjiajie.cn

local a = 1
来源：http://rs.colortex.cn

[T33] Lua：表（数组）
来源：http://dy.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xz.gzmigu.cn

[T34] Lua：遍历表
来源：http://nc.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zv.nszjky.cn

[T35] Lua：字典表
来源：http://sd.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://ov.huixiangedu.cn

[T36] Lua：函数
来源：http://zg.hahajie.cn

function add(a, b) return a + b end
来源：http://mx.szsharing.cn

[T37] Lua：字符串拼接
来源：http://cp.chemitech.net.cn

"a" .. "b"
来源：http://md.gzmigu.cn

[T38] Lua：条件
来源：http://eu.hahajie.cn

if x > 0 then print("正") end
来源：http://fh.shxzukj.cn

[T39] Lua：模式匹配
来源：http://zh.521024.cn

string.find(s, "%d+")
来源：http://lx.9csxet.cn

[T40] Lua：元表
来源：http://at.colortex.cn

setmetatable({}, { __index = base })
来源：http://ww.szxytkj.cn

[T41] Perl：Hello World
来源：http://jo.yuntaijiaju.cn

print "Hello\n";
来源：http://tu.yuexingan06.cn

[T42] Perl：变量类型
来源：http://fu.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uk.9csxet.cn

[T43] Perl：字符串插值
来源：http://vd.wgjwhj.cn

"值: $a"
来源：http://uw.asd995.cn

[T44] Perl：条件
来源：http://ki.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://wo.panjiajie.cn

[T45] Perl：数组遍历
来源：http://bx.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://pg.9csxet.cn

[T46] Perl：哈希操作
来源：http://vc.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ur.521024.cn

[T47] Perl：正则捕获
来源：http://ln.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lf.jctech888.com.cn

[T48] Perl：正则替换
来源：http://aw.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://yl.panjiajie.cn

[T49] Perl：函数
来源：http://bg.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lt.nicolike.cn

[T50] Perl：逐行读文件
来源：http://ty.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fz.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://cq.szsharing.cn

[T51] Scala：Hello World
来源：http://ws.bjjhwx.cn

println("Hello")
来源：http://ra.chemitech.net.cn

[T52] Scala：变量
来源：http://au.hahajie.cn

val a = 1;  var b = 2
来源：http://ak.szxytkj.cn

[T53] Scala：字符串插值
来源：http://sx.huanxung.cn

s"值: $b"
来源：http://dg.muxihuayi.cn

[T54] Scala：集合映射
来源：http://th.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://lo.nicolike.cn

[T55] Scala：集合过滤
来源：http://ur.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bd.521024.cn

[T56] Scala：样例类
来源：http://dz.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://gt.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://nb.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dj.haigaiapp.cn

[T58] Scala：函数定义
来源：http://gm.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gv.521024.cn

[T59] Scala：循环
来源：http://ry.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ly.lnxyls.cn

[T60] Scala：折叠
来源：http://je.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://em.bookmarksfly.cn

================================================================================
来源：http://qz.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qc.hahajie.cn

================================================================================
来源：http://af.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://yo.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mk.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://wl.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oo.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://xh.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zi.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://ry.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wu.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://an.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://xr.hnjuh.cn

[U06] Py：合并两个字典
来源：http://yz.hahajie.cn

{**a, **b}
来源：http://og.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://pt.huanxung.cn

{v: k for k, v in d.items()}
来源：http://kd.colortex.cn

[U08] Py：展平二维列表
来源：http://jn.asd995.cn

[y for x in nested for y in x]
来源：http://hu.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://rc.shtwfgs.cn

max(d, key=d.get)
来源：http://oo.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://zz.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://di.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://bo.newstarts.cn

(x * 2 for x in arr)
来源：http://jj.panjiajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sm.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://uq.9csxet.cn


<!-- 参考信息 -->