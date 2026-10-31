代发 wailian999

free -h;  ps aux | grep nginx
来源：http://pi.shxzskj.cn

[R64] 结束进程
来源：http://yr.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://bp.wgjwhj.cn

[R65] 查看端口占用
来源：http://fi.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cw.wgjwhj.cn

[R66] 定时任务
来源：http://ij.gzmigu.cn

crontab -e;  crontab -l
来源：http://cm.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://ty.huixiangedu.cn

openssl rand -hex 16
来源：http://op.bjjhwx.cn

[R68] 计算文件校验值
来源：http://ij.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uw.muxihuayi.cn

[R69] 生成随机密码
来源：http://zw.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://uk.szsharing.cn

[R70] 时间戳与互转
来源：http://np.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://zq.huanxung.cn

[R71] 日期格式化
来源：http://qg.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hk.nicolike.cn

[R72] 等待端口就绪
来源：http://be.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wq.yuexingan06.cn

[R73] 分割大日志
来源：http://ni.hahajie.cn

split -l 1000 big.log part_
来源：http://xp.bookmarksfly.cn

[R74] 批量重命名
来源：http://vc.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bw.chemitech.net.cn

[R75] 导出环境变量
来源：http://ov.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://qr.yuexingan06.cn

[R76] 使用临时文件
来源：http://gp.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wb.9csxet.cn

[R77] 读取用户输入
来源：http://wl.haigaiapp.cn

read -rp "请输入: " ans
来源：http://wl.chemitech.net.cn

[R78] 交互式菜单
来源：http://cv.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pk.shxzukj.cn

[R79] 解析命令行选项
来源：http://un.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mq.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://lr.nicolike.cn

time ./run.sh
来源：http://ph.huanxung.cn

================================================================================
来源：http://mx.9csxet.cn

S. C / C++ 专题
来源：http://aw.szxytkj.cn

================================================================================
来源：http://hb.shxzukj.cn

[S01] C：Hello World
来源：http://tb.yuntaijiaju.cn

#include <stdio.h>
来源：http://mg.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pw.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://pg.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://ub.shtwfgs.cn

[S03] C：读入整数
来源：http://uk.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://pr.hahajie.cn

[S04] C：字符串复制
来源：http://iq.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cp.shtwfgs.cn

[S05] C：字符串长度
来源：http://nr.521024.cn

strlen(s)
来源：http://xd.haigaiapp.cn

[S06] C：字符串比较
来源：http://so.huixiangedu.cn

strcmp(a, b) == 0
来源：http://yy.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://ma.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yd.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://uz.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vg.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://wx.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://er.szxytkj.cn

[S10] C：指针与解引用
来源：http://em.colortex.cn

int *p = &a;  *p = 5;
来源：http://qm.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://yw.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://tz.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bx.521024.cn

fclose(f);
来源：http://kf.lnxyls.cn

[S12] C：写文件
来源：http://ma.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://be.huixiangedu.cn

[S13] C：宏定义
来源：http://ed.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wm.bjjhwx.cn

[S14] C：枚举
来源：http://rb.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://ze.9csxet.cn

[S15] C：类型转换
来源：http://qb.chemitech.net.cn

(double) a / b
来源：http://oe.wgjwhj.cn

[S16] C：位操作置位
来源：http://yd.szsharing.cn

x |= (1 << 3);
来源：http://na.asd995.cn

[S17] C：安全拼接字符串
来源：http://ms.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lv.bjjhwx.cn

[S18] C：命令行参数
来源：http://bx.panjiajie.cn

int main(int argc, char **argv)
来源：http://di.haigaiapp.cn

[S19] C：快速排序
来源：http://tn.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jo.szsharing.cn

[S20] C：二分查找
来源：http://wa.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mu.huixiangedu.cn

[S21] C：字符类别判断
来源：http://jc.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uu.jctech888.com.cn

[S22] C：字符串转数字
来源：http://vl.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tg.wgjwhj.cn

[S23] C：随机数
来源：http://gd.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vm.haigaiapp.cn

[S24] C：获取本地时间
来源：http://md.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mw.yuexingan06.cn

[S25] C：内存拷贝
来源：http://eh.szsharing.cn

memcpy(dst, src, n);
来源：http://ld.szsharing.cn

[S26] C：内存清零
来源：http://uf.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://yu.panjiajie.cn

[S27] C：定义常量
来源：http://ji.gzmigu.cn

const double PI = 3.14159;
来源：http://de.bookmarksfly.cn

[S28] C：静态变量
来源：http://kt.huanxung.cn

static int counter = 0;
来源：http://ln.shxzukj.cn

[S29] C：变参函数
来源：http://zb.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://si.hahajie.cn

[S30] C：头文件保护
来源：http://rt.szsharing.cn

#ifndef X_H
来源：http://ew.jianghongdianzi.cn

#define X_H
来源：http://oj.nicolike.cn

#endif
来源：http://bz.gzmigu.cn

[S31] C++：Hello World
来源：http://em.yuexingan06.cn

#include <iostream>
来源：http://cs.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://ge.yuexingan06.cn

[S32] C++：字符串
来源：http://ex.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://xl.wgjwhj.cn

[S33] C++：vector 增删
来源：http://fa.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wg.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://ax.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://fz.shtwfgs.cn

[S35] C++：map
来源：http://up.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dz.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://tq.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cl.nszjky.cn

[S37] C++：set
来源：http://gk.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zq.haigaiapp.cn

[S38] C++：排序
来源：http://fm.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://vv.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://cb.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hf.huanxung.cn

[S40] C++：查找元素
来源：http://sz.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wr.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ky.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yr.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://xk.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ye.huanxung.cn

[S43] C++：智能指针
来源：http://dn.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://tl.nszjky.cn

[S44] C++：引用传参
来源：http://wq.huanxung.cn

void inc(int &x) { ++x; }
来源：http://xz.hahajie.cn

[S45] C++：lambda
来源：http://zq.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fs.newstarts.cn

[S46] C++：函数模板
来源：http://zj.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pt.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://zr.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ll.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://dp.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://om.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://sa.yuntaijiaju.cn

[S49] C++：写文件
来源：http://yi.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bj.szsharing.cn

[S50] C++：格式化数字
来源：http://hy.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zz.hahajie.cn

[S51] C++：显式类型转换
来源：http://ft.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://ze.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://wi.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://xe.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://st.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://tk.chemitech.net.cn

[S54] C++：异常处理
来源：http://fz.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://la.panjiajie.cn

[S55] C++：结构化绑定
来源：http://bf.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cy.colortex.cn

[S56] C++：optional
来源：http://us.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nk.huanxung.cn

[S57] C++：编译期常量
来源：http://sv.lnxyls.cn

constexpr int N = 10;
来源：http://yp.shxzskj.cn

[S58] C++：命名空间
来源：http://vt.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://sq.jctech888.com.cn

[S59] C++：静态断言
来源：http://gi.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hx.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://ge.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qh.jctech888.com.cn

================================================================================
来源：http://fk.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oh.muxihuayi.cn

================================================================================
来源：http://ri.asd995.cn

[T01] Kotlin：Hello World
来源：http://lo.nicolike.cn

println("Hello")
来源：http://rj.hnjuh.cn

[T02] Kotlin：变量
来源：http://rw.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ep.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://cq.9csxet.cn

"值: $b"
来源：http://su.nszjky.cn

[T04] Kotlin：空安全
来源：http://ky.colortex.cn

val n: String? = null;  n?.length
来源：http://bx.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://cs.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ql.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://jf.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ax.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ta.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hl.asd995.cn

[T08] Kotlin：数据类
来源：http://pk.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ae.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://tz.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://sa.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ho.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yu.wgjwhj.cn

[T11] Kotlin：协程
来源：http://te.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://im.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://tr.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://cm.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://sc.szsharing.cn

val m = mapOf("a" to 1)
来源：http://yr.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ib.gzmigu.cn

for (i in 1..10) println(i)
来源：http://wh.shtwfgs.cn

[T15] Kotlin：接口
来源：http://mc.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://kf.hnjuh.cn

[T16] Swift：Hello World
来源：http://ze.521024.cn

print("Hello")
来源：http://az.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://df.newstarts.cn

var a = 1;  let b = 2
来源：http://tr.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://di.yuexingan06.cn

"值: \(b)"
来源：http://eb.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://fp.panjiajie.cn

if let n = opt { print(n) }
来源：http://px.szsharing.cn

[T20] Swift：数组操作
来源：http://lo.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lq.521024.cn

[T21] Swift：遍历
来源：http://wd.gzmigu.cn

for x in a { print(x) }
来源：http://mz.nszjky.cn

[T22] Swift：字典
来源：http://eb.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pp.muxihuayi.cn

[T23] Swift：函数
来源：http://ge.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kw.hnjuh.cn

[T24] Swift：闭包
来源：http://sa.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ho.shtwfgs.cn

[T25] Swift：结构体
来源：http://gq.yuntaijiaju.cn

struct P { var x: Int }
来源：http://cc.nicolike.cn

[T26] Swift：类与重写
来源：http://ci.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://sh.huanxung.cn

[T27] Swift：错误处理
来源：http://ws.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://rr.521024.cn

[T28] Swift：枚举
来源：http://ek.szsharing.cn

enum Color { case red, green }
来源：http://qe.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://bz.huanxung.cn

guard let x = opt else { return }
来源：http://lg.lnxyls.cn

[T30] Swift：协议
来源：http://vz.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://ia.hahajie.cn

[T31] Lua：Hello World
来源：http://fr.szsharing.cn

print("Hello")
来源：http://ic.9csxet.cn

[T32] Lua：局部变量
来源：http://pc.9csxet.cn

local a = 1
来源：http://iz.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://lm.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cd.gzmigu.cn

[T34] Lua：遍历表
来源：http://nc.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://so.yuexingan06.cn

[T35] Lua：字典表
来源：http://nm.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://vi.yuntaijiaju.cn

[T36] Lua：函数
来源：http://bl.shxzukj.cn

function add(a, b) return a + b end
来源：http://dt.huanxung.cn

[T37] Lua：字符串拼接
来源：http://sj.521024.cn

"a" .. "b"
来源：http://uc.haigaiapp.cn

[T38] Lua：条件
来源：http://yk.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://dl.nicolike.cn

[T39] Lua：模式匹配
来源：http://oi.shtwfgs.cn

string.find(s, "%d+")
来源：http://wl.shxzukj.cn

[T40] Lua：元表
来源：http://gg.9csxet.cn

setmetatable({}, { __index = base })
来源：http://el.huanxung.cn

[T41] Perl：Hello World
来源：http://mc.szsharing.cn

print "Hello\n";
来源：http://ft.newstarts.cn

[T42] Perl：变量类型
来源：http://ku.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://re.nicolike.cn

[T43] Perl：字符串插值
来源：http://ys.colortex.cn

"值: $a"
来源：http://hz.yuexingan06.cn

[T44] Perl：条件
来源：http://oa.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://nv.hahajie.cn

[T45] Perl：数组遍历
来源：http://vp.asd995.cn

for my $x (@arr) { print $x; }
来源：http://ci.lnxyls.cn

[T46] Perl：哈希操作
来源：http://lj.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fm.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://zq.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yu.szxytkj.cn

[T48] Perl：正则替换
来源：http://au.hahajie.cn

$s =~ s/old/new/g;
来源：http://kf.huixiangedu.cn

[T49] Perl：函数
来源：http://ca.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oo.nicolike.cn

[T50] Perl：逐行读文件
来源：http://ne.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wo.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://mh.gzmigu.cn

[T51] Scala：Hello World
来源：http://um.shtwfgs.cn

println("Hello")
来源：http://cm.huanxung.cn

[T52] Scala：变量
来源：http://bn.newstarts.cn

val a = 1;  var b = 2
来源：http://lw.hahajie.cn

[T53] Scala：字符串插值
来源：http://zq.shxzskj.cn

s"值: $b"
来源：http://ek.wgjwhj.cn

[T54] Scala：集合映射
来源：http://dy.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://oy.9csxet.cn

[T55] Scala：集合过滤
来源：http://rj.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mc.newstarts.cn

[T56] Scala：样例类
来源：http://lb.asd995.cn

case class User(name: String, age: Int)
来源：http://kn.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://bm.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hf.muxihuayi.cn

[T58] Scala：函数定义
来源：http://wa.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nx.nszjky.cn

[T59] Scala：循环
来源：http://gr.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://vv.shxzukj.cn

[T60] Scala：折叠
来源：http://xf.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jn.huixinmuqiang.cn

================================================================================
来源：http://vw.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ip.521024.cn

================================================================================
来源：http://kv.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://ui.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ji.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://rv.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lj.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://kj.haigaiapp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ji.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://to.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lf.lnxyls.cn


<!-- 参考信息 -->