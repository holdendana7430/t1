代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fi.panjiajie.cn

[R66] 定时任务
来源：http://lx.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://sa.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://ty.newstarts.cn

openssl rand -hex 16
来源：http://ki.huanxung.cn

[R68] 计算文件校验值
来源：http://ej.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qs.wgjwhj.cn

[R69] 生成随机密码
来源：http://je.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://jv.wgjwhj.cn

[R70] 时间戳与互转
来源：http://uk.colortex.cn

date +%s;  date -d @1700000000
来源：http://rk.panjiajie.cn

[R71] 日期格式化
来源：http://lm.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ax.hnjuh.cn

[R72] 等待端口就绪
来源：http://hs.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zq.jianghongdianzi.cn

[R73] 分割大日志
来源：http://cp.lnxyls.cn

split -l 1000 big.log part_
来源：http://cv.hnjuh.cn

[R74] 批量重命名
来源：http://ck.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dp.szsharing.cn

[R75] 导出环境变量
来源：http://ht.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://yq.hahajie.cn

[R76] 使用临时文件
来源：http://ht.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mh.huixiangedu.cn

[R77] 读取用户输入
来源：http://la.hahajie.cn

read -rp "请输入: " ans
来源：http://bi.szxytkj.cn

[R78] 交互式菜单
来源：http://tk.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eu.hahajie.cn

[R79] 解析命令行选项
来源：http://zj.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qu.521024.cn

[R80] 查看脚本执行耗时
来源：http://it.panjiajie.cn

time ./run.sh
来源：http://ae.panjiajie.cn

================================================================================
来源：http://np.panjiajie.cn

S. C / C++ 专题
来源：http://gp.shtwfgs.cn

================================================================================
来源：http://hx.jianghongdianzi.cn

[S01] C：Hello World
来源：http://et.huixiangedu.cn

#include <stdio.h>
来源：http://fr.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ua.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://ku.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://tg.chemitech.net.cn

[S03] C：读入整数
来源：http://dp.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://wh.newstarts.cn

[S04] C：字符串复制
来源：http://xk.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ju.wgjwhj.cn

[S05] C：字符串长度
来源：http://zb.chemitech.net.cn

strlen(s)
来源：http://nb.521024.cn

[S06] C：字符串比较
来源：http://qb.nszjky.cn

strcmp(a, b) == 0
来源：http://cn.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://vv.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fq.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://gn.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://is.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://jd.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ms.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://eb.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ee.szxytkj.cn

[S11] C：逐行读文件
来源：http://ps.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://vb.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oo.muxihuayi.cn

fclose(f);
来源：http://ev.9csxet.cn

[S12] C：写文件
来源：http://kl.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kf.asd995.cn

[S13] C：宏定义
来源：http://va.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fj.gzmigu.cn

[S14] C：枚举
来源：http://fu.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://km.nszjky.cn

[S15] C：类型转换
来源：http://em.bjjhwx.cn

(double) a / b
来源：http://mh.szxytkj.cn

[S16] C：位操作置位
来源：http://no.shtwfgs.cn

x |= (1 << 3);
来源：http://vi.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://ii.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dq.huixiangedu.cn

[S18] C：命令行参数
来源：http://dz.bjjhwx.cn

int main(int argc, char **argv)
来源：http://tz.muxihuayi.cn

[S19] C：快速排序
来源：http://cg.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vo.asd995.cn

[S20] C：二分查找
来源：http://fm.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://if.colortex.cn

[S21] C：字符类别判断
来源：http://cc.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hs.521024.cn

[S22] C：字符串转数字
来源：http://my.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cw.chemitech.net.cn

[S23] C：随机数
来源：http://tf.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oc.huixiangedu.cn

[S24] C：获取本地时间
来源：http://ix.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wd.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://bt.shxzukj.cn

memcpy(dst, src, n);
来源：http://aq.shxzskj.cn

[S26] C：内存清零
来源：http://tr.szsharing.cn

memset(a, 0, sizeof a);
来源：http://jk.yuexingan06.cn

[S27] C：定义常量
来源：http://hi.szxytkj.cn

const double PI = 3.14159;
来源：http://zs.shtwfgs.cn

[S28] C：静态变量
来源：http://fo.yuexingan06.cn

static int counter = 0;
来源：http://uy.hnjuh.cn

[S29] C：变参函数
来源：http://po.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fk.shtwfgs.cn

[S30] C：头文件保护
来源：http://th.jctech888.com.cn

#ifndef X_H
来源：http://mb.newstarts.cn

#define X_H
来源：http://yq.hnjuh.cn

#endif
来源：http://ln.chemitech.net.cn

[S31] C++：Hello World
来源：http://tx.jianghongdianzi.cn

#include <iostream>
来源：http://qg.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://ex.gzmigu.cn

[S32] C++：字符串
来源：http://kp.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://ql.lnxyls.cn

[S33] C++：vector 增删
来源：http://zy.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sm.shxzskj.cn

[S34] C++：遍历 vector
来源：http://zc.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://cq.jctech888.com.cn

[S35] C++：map
来源：http://gb.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yi.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://qn.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oe.panjiajie.cn

[S37] C++：set
来源：http://iy.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ny.gzmigu.cn

[S38] C++：排序
来源：http://uq.colortex.cn

std::sort(v.begin(), v.end());
来源：http://se.colortex.cn

[S39] C++：自定义比较器排序
来源：http://qy.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vm.9csxet.cn

[S40] C++：查找元素
来源：http://sd.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ot.asd995.cn

[S41] C++：类与构造函数
来源：http://kn.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fj.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://mg.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://zr.muxihuayi.cn

[S43] C++：智能指针
来源：http://ry.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ls.shxzukj.cn

[S44] C++：引用传参
来源：http://bp.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://fx.haigaiapp.cn

[S45] C++：lambda
来源：http://ej.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qq.hahajie.cn

[S46] C++：函数模板
来源：http://mk.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mz.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://ut.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ak.szsharing.cn

[S48] C++：逐行读文件
来源：http://td.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qe.asd995.cn

while (std::getline(in, line)) { }
来源：http://ie.nszjky.cn

[S49] C++：写文件
来源：http://pg.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vh.chemitech.net.cn

[S50] C++：格式化数字
来源：http://yj.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fo.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://kb.panjiajie.cn

static_cast<double>(a) / b
来源：http://vs.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yw.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://kd.colortex.cn

[S53] C++：移动语义
来源：http://at.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://ty.shtwfgs.cn

[S54] C++：异常处理
来源：http://up.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mh.lnxyls.cn

[S55] C++：结构化绑定
来源：http://my.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mo.gzmigu.cn

[S56] C++：optional
来源：http://ke.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ze.huanxung.cn

[S57] C++：编译期常量
来源：http://on.huixinmuqiang.cn

constexpr int N = 10;
来源：http://di.chemitech.net.cn

[S58] C++：命名空间
来源：http://st.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://gq.jctech888.com.cn

[S59] C++：静态断言
来源：http://gr.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dm.colortex.cn

[S60] C++：遍历并删除元素
来源：http://tv.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lr.shtwfgs.cn

================================================================================
来源：http://uc.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://du.gzmigu.cn

================================================================================
来源：http://sd.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://cz.huanxung.cn

println("Hello")
来源：http://yc.szxytkj.cn

[T02] Kotlin：变量
来源：http://yv.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iq.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://pz.yuntaijiaju.cn

"值: $b"
来源：http://rh.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://hj.colortex.cn

val n: String? = null;  n?.length
来源：http://lz.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://iz.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wx.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://hd.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ac.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://nl.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gg.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://qe.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://gd.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://sw.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://yl.szsharing.cn

[T10] Kotlin：默认参数
来源：http://eq.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lm.wgjwhj.cn

[T11] Kotlin：协程
来源：http://pc.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sd.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://rm.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://yb.521024.cn

[T13] Kotlin：只读 Map
来源：http://dx.hahajie.cn

val m = mapOf("a" to 1)
来源：http://vf.bjjhwx.cn

[T14] Kotlin：循环
来源：http://xi.9csxet.cn

for (i in 1..10) println(i)
来源：http://bh.yuexingan06.cn

[T15] Kotlin：接口
来源：http://am.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://ef.9csxet.cn

[T16] Swift：Hello World
来源：http://za.shtwfgs.cn

print("Hello")
来源：http://dp.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://qt.nszjky.cn

var a = 1;  let b = 2
来源：http://kq.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://yk.521024.cn

"值: \(b)"
来源：http://fz.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://pt.jctech888.com.cn

if let n = opt { print(n) }
来源：http://zp.haigaiapp.cn

[T20] Swift：数组操作
来源：http://yr.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yt.bookmarksfly.cn

[T21] Swift：遍历
来源：http://eg.panjiajie.cn

for x in a { print(x) }
来源：http://ka.lnxyls.cn

[T22] Swift：字典
来源：http://dz.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yc.asd995.cn

[T23] Swift：函数
来源：http://hu.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pl.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://lc.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cu.muxihuayi.cn

[T25] Swift：结构体
来源：http://ne.asd995.cn

struct P { var x: Int }
来源：http://jv.shtwfgs.cn

[T26] Swift：类与重写
来源：http://qn.hnjuh.cn

class A: Base { override func f() {} }
来源：http://co.panjiajie.cn

[T27] Swift：错误处理
来源：http://ek.szsharing.cn

do { try f() } catch { print(error) }
来源：http://kp.wgjwhj.cn

[T28] Swift：枚举
来源：http://co.haigaiapp.cn

enum Color { case red, green }
来源：http://fl.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://oz.chemitech.net.cn

guard let x = opt else { return }
来源：http://kl.nszjky.cn

[T30] Swift：协议
来源：http://qb.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://tl.huanxung.cn

[T31] Lua：Hello World
来源：http://ah.huixinmuqiang.cn

print("Hello")
来源：http://hj.newstarts.cn

[T32] Lua：局部变量
来源：http://du.hnjuh.cn

local a = 1
来源：http://wh.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://dm.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tj.shxzukj.cn

[T34] Lua：遍历表
来源：http://gn.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hc.bookmarksfly.cn

[T35] Lua：字典表
来源：http://yy.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://pd.haigaiapp.cn

[T36] Lua：函数
来源：http://zd.haigaiapp.cn

function add(a, b) return a + b end
来源：http://zm.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://ne.nicolike.cn

"a" .. "b"
来源：http://tk.shxzukj.cn

[T38] Lua：条件
来源：http://ec.hahajie.cn

if x > 0 then print("正") end
来源：http://cy.hnjuh.cn

[T39] Lua：模式匹配
来源：http://ah.shxzskj.cn

string.find(s, "%d+")
来源：http://iz.9csxet.cn

[T40] Lua：元表
来源：http://do.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://wl.chemitech.net.cn

[T41] Perl：Hello World
来源：http://pr.hnjuh.cn

print "Hello\n";
来源：http://zk.nicolike.cn

[T42] Perl：变量类型
来源：http://wd.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dg.gzmigu.cn

[T43] Perl：字符串插值
来源：http://qa.haigaiapp.cn

"值: $a"
来源：http://tf.nszjky.cn

[T44] Perl：条件
来源：http://qf.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://pd.9csxet.cn

[T45] Perl：数组遍历
来源：http://qw.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://na.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://eb.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ok.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://eg.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kp.wgjwhj.cn

[T48] Perl：正则替换
来源：http://eo.hahajie.cn

$s =~ s/old/new/g;
来源：http://lx.521024.cn

[T49] Perl：函数
来源：http://mv.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zw.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://lb.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zq.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://jm.9csxet.cn

[T51] Scala：Hello World
来源：http://um.nicolike.cn

println("Hello")
来源：http://se.nicolike.cn

[T52] Scala：变量
来源：http://go.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://lj.szxytkj.cn

[T53] Scala：字符串插值
来源：http://dw.shtwfgs.cn

s"值: $b"
来源：http://br.lnxyls.cn

[T54] Scala：集合映射
来源：http://wd.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://af.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://mj.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hg.colortex.cn

[T56] Scala：样例类
来源：http://se.nicolike.cn

case class User(name: String, age: Int)
来源：http://jo.hnjuh.cn

[T57] Scala：模式匹配
来源：http://he.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://um.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://st.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pj.9csxet.cn

[T59] Scala：循环
来源：http://ms.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://ef.bookmarksfly.cn

[T60] Scala：折叠
来源：http://go.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kc.huanxung.cn

================================================================================
来源：http://ve.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sf.haigaiapp.cn

================================================================================
来源：http://mh.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://sj.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://df.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://dv.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://py.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://ob.521024.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jw.asd995.cn

[U04] Py：变量调试打印
来源：http://yd.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nn.newstarts.cn

[U05] Py：列表去重且保序
来源：http://id.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://qn.hahajie.cn

[U06] Py：合并两个字典
来源：http://wi.szxytkj.cn

{**a, **b}
来源：http://wh.bookmarksfly.cn


<!-- 参考信息 -->