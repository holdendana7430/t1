代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qb.lnxyls.cn

[R66] 定时任务
来源：http://fz.szxytkj.cn

crontab -e;  crontab -l
来源：http://mt.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://nc.shxzskj.cn

openssl rand -hex 16
来源：http://nm.521024.cn

[R68] 计算文件校验值
来源：http://pj.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lt.huanxung.cn

[R69] 生成随机密码
来源：http://fl.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://nd.panjiajie.cn

[R70] 时间戳与互转
来源：http://jl.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://pa.panjiajie.cn

[R71] 日期格式化
来源：http://tx.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vp.szxytkj.cn

[R72] 等待端口就绪
来源：http://dp.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gl.hahajie.cn

[R73] 分割大日志
来源：http://wt.shxzukj.cn

split -l 1000 big.log part_
来源：http://re.yuexingan06.cn

[R74] 批量重命名
来源：http://oc.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iz.asd995.cn

[R75] 导出环境变量
来源：http://mg.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://vk.muxihuayi.cn

[R76] 使用临时文件
来源：http://it.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://et.shtwfgs.cn

[R77] 读取用户输入
来源：http://bp.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://rg.huixiangedu.cn

[R78] 交互式菜单
来源：http://tf.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pp.szxytkj.cn

[R79] 解析命令行选项
来源：http://nh.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tx.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://hu.muxihuayi.cn

time ./run.sh
来源：http://xh.szxytkj.cn

================================================================================
来源：http://ez.huanxung.cn

S. C / C++ 专题
来源：http://da.bjjhwx.cn

================================================================================
来源：http://jf.wgjwhj.cn

[S01] C：Hello World
来源：http://aj.jctech888.com.cn

#include <stdio.h>
来源：http://bz.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nl.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://pe.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://lq.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ls.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://fm.bjjhwx.cn

[S04] C：字符串复制
来源：http://jt.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ik.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ko.jianghongdianzi.cn

strlen(s)
来源：http://nf.huixiangedu.cn

[S06] C：字符串比较
来源：http://hf.szsharing.cn

strcmp(a, b) == 0
来源：http://cq.nszjky.cn

[S07] C：数组遍历求和
来源：http://it.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mn.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://sr.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bm.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://np.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zv.9csxet.cn

[S10] C：指针与解引用
来源：http://ub.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://fc.bjjhwx.cn

[S11] C：逐行读文件
来源：http://bt.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://nl.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zi.haigaiapp.cn

fclose(f);
来源：http://vt.asd995.cn

[S12] C：写文件
来源：http://oy.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zq.yuexingan06.cn

[S13] C：宏定义
来源：http://wp.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wq.9csxet.cn

[S14] C：枚举
来源：http://pe.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://hy.huanxung.cn

[S15] C：类型转换
来源：http://ec.chemitech.net.cn

(double) a / b
来源：http://oz.haigaiapp.cn

[S16] C：位操作置位
来源：http://eg.haigaiapp.cn

x |= (1 << 3);
来源：http://ob.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://gq.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hu.panjiajie.cn

[S18] C：命令行参数
来源：http://io.haigaiapp.cn

int main(int argc, char **argv)
来源：http://hl.521024.cn

[S19] C：快速排序
来源：http://qw.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://my.chemitech.net.cn

[S20] C：二分查找
来源：http://xe.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zo.asd995.cn

[S21] C：字符类别判断
来源：http://mm.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ey.muxihuayi.cn

[S22] C：字符串转数字
来源：http://vh.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jg.huixinmuqiang.cn

[S23] C：随机数
来源：http://kc.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ai.colortex.cn

[S24] C：获取本地时间
来源：http://ax.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zs.bjjhwx.cn

[S25] C：内存拷贝
来源：http://qb.panjiajie.cn

memcpy(dst, src, n);
来源：http://by.bjjhwx.cn

[S26] C：内存清零
来源：http://in.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://wj.shtwfgs.cn

[S27] C：定义常量
来源：http://xv.hnjuh.cn

const double PI = 3.14159;
来源：http://jd.wgjwhj.cn

[S28] C：静态变量
来源：http://pt.9csxet.cn

static int counter = 0;
来源：http://fl.gzmigu.cn

[S29] C：变参函数
来源：http://la.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hg.nszjky.cn

[S30] C：头文件保护
来源：http://pv.muxihuayi.cn

#ifndef X_H
来源：http://rj.huanxung.cn

#define X_H
来源：http://wu.bookmarksfly.cn

#endif
来源：http://it.panjiajie.cn

[S31] C++：Hello World
来源：http://su.chemitech.net.cn

#include <iostream>
来源：http://dd.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://bn.hnjuh.cn

[S32] C++：字符串
来源：http://xm.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://es.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ls.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://do.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://lm.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://bo.hnjuh.cn

[S35] C++：map
来源：http://qh.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rq.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://fv.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://re.szxytkj.cn

[S37] C++：set
来源：http://ez.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gg.chemitech.net.cn

[S38] C++：排序
来源：http://ax.asd995.cn

std::sort(v.begin(), v.end());
来源：http://uq.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://up.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qs.colortex.cn

[S40] C++：查找元素
来源：http://hl.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kp.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://iw.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ki.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://xj.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://nt.hnjuh.cn

[S43] C++：智能指针
来源：http://pk.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://di.shtwfgs.cn

[S44] C++：引用传参
来源：http://uh.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://qw.huixiangedu.cn

[S45] C++：lambda
来源：http://tx.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wd.yuexingan06.cn

[S46] C++：函数模板
来源：http://rm.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gu.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://md.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://di.gzmigu.cn

[S48] C++：逐行读文件
来源：http://ln.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ax.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://sg.huanxung.cn

[S49] C++：写文件
来源：http://la.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cb.hnjuh.cn

[S50] C++：格式化数字
来源：http://cx.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kf.nicolike.cn

[S51] C++：显式类型转换
来源：http://yi.colortex.cn

static_cast<double>(a) / b
来源：http://rm.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://uo.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://hq.newstarts.cn

[S53] C++：移动语义
来源：http://se.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://zu.colortex.cn

[S54] C++：异常处理
来源：http://fi.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://he.szsharing.cn

[S55] C++：结构化绑定
来源：http://id.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cu.szxytkj.cn

[S56] C++：optional
来源：http://sk.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ih.yuexingan06.cn

[S57] C++：编译期常量
来源：http://cg.chemitech.net.cn

constexpr int N = 10;
来源：http://ri.newstarts.cn

[S58] C++：命名空间
来源：http://sm.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://gu.521024.cn

[S59] C++：静态断言
来源：http://ip.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rt.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://oo.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mz.jctech888.com.cn

================================================================================
来源：http://rx.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kr.colortex.cn

================================================================================
来源：http://fk.colortex.cn

[T01] Kotlin：Hello World
来源：http://el.huanxung.cn

println("Hello")
来源：http://oy.muxihuayi.cn

[T02] Kotlin：变量
来源：http://zx.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mz.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://mn.shxzskj.cn

"值: $b"
来源：http://dn.nicolike.cn

[T04] Kotlin：空安全
来源：http://qo.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://yo.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://gk.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://by.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://sb.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tl.asd995.cn

[T07] Kotlin：集合过滤
来源：http://ev.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tx.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://st.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://jx.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://ri.asd995.cn

fun String.exclaim() = this + "!"
来源：http://wf.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://kj.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://he.panjiajie.cn

[T11] Kotlin：协程
来源：http://uy.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xp.9csxet.cn

[T12] Kotlin：解构声明
来源：http://un.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://en.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://bk.colortex.cn

val m = mapOf("a" to 1)
来源：http://jm.asd995.cn

[T14] Kotlin：循环
来源：http://rz.szxytkj.cn

for (i in 1..10) println(i)
来源：http://df.jctech888.com.cn

[T15] Kotlin：接口
来源：http://eg.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://mk.lnxyls.cn

[T16] Swift：Hello World
来源：http://xm.asd995.cn

print("Hello")
来源：http://pf.nszjky.cn

[T17] Swift：变量与常量
来源：http://sn.shxzskj.cn

var a = 1;  let b = 2
来源：http://we.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://mw.shtwfgs.cn

"值: \(b)"
来源：http://ld.hnjuh.cn

[T19] Swift：可选绑定
来源：http://xr.huixiangedu.cn

if let n = opt { print(n) }
来源：http://sz.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://ev.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yz.colortex.cn

[T21] Swift：遍历
来源：http://fl.muxihuayi.cn

for x in a { print(x) }
来源：http://qx.huixiangedu.cn

[T22] Swift：字典
来源：http://zl.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vr.yuntaijiaju.cn

[T23] Swift：函数
来源：http://dg.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jl.haigaiapp.cn

[T24] Swift：闭包
来源：http://oj.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lk.szxytkj.cn

[T25] Swift：结构体
来源：http://us.jianghongdianzi.cn

struct P { var x: Int }
来源：http://jk.huanxung.cn

[T26] Swift：类与重写
来源：http://xl.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://jp.9csxet.cn

[T27] Swift：错误处理
来源：http://pw.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://ft.jctech888.com.cn

[T28] Swift：枚举
来源：http://qc.yuntaijiaju.cn

enum Color { case red, green }
来源：http://cf.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://pp.panjiajie.cn

guard let x = opt else { return }
来源：http://us.521024.cn

[T30] Swift：协议
来源：http://vl.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://af.huanxung.cn

[T31] Lua：Hello World
来源：http://lx.huanxung.cn

print("Hello")
来源：http://rh.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://cy.wgjwhj.cn

local a = 1
来源：http://ux.nszjky.cn

[T33] Lua：表（数组）
来源：http://hz.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jp.huixiangedu.cn

[T34] Lua：遍历表
来源：http://pb.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nu.huanxung.cn

[T35] Lua：字典表
来源：http://nd.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://ev.9csxet.cn

[T36] Lua：函数
来源：http://da.newstarts.cn

function add(a, b) return a + b end
来源：http://bh.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://db.wgjwhj.cn

"a" .. "b"
来源：http://ki.wgjwhj.cn

[T38] Lua：条件
来源：http://hf.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://ew.hahajie.cn

[T39] Lua：模式匹配
来源：http://tk.lnxyls.cn

string.find(s, "%d+")
来源：http://tb.muxihuayi.cn

[T40] Lua：元表
来源：http://vm.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://yc.lnxyls.cn

[T41] Perl：Hello World
来源：http://sy.nszjky.cn

print "Hello\n";
来源：http://yt.shxzskj.cn

[T42] Perl：变量类型
来源：http://sb.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gt.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://sc.huixiangedu.cn

"值: $a"
来源：http://zf.colortex.cn

[T44] Perl：条件
来源：http://al.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://fk.hnjuh.cn

[T45] Perl：数组遍历
来源：http://oq.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://hq.colortex.cn

[T46] Perl：哈希操作
来源：http://ly.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cu.9csxet.cn

[T47] Perl：正则捕获
来源：http://ki.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rk.9csxet.cn

[T48] Perl：正则替换
来源：http://pp.gzmigu.cn

$s =~ s/old/new/g;
来源：http://mx.yuntaijiaju.cn

[T49] Perl：函数
来源：http://zp.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://di.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://nc.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://db.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://hu.haigaiapp.cn

[T51] Scala：Hello World
来源：http://lm.jctech888.com.cn

println("Hello")
来源：http://iv.szxytkj.cn

[T52] Scala：变量
来源：http://de.shxzskj.cn

val a = 1;  var b = 2
来源：http://xp.panjiajie.cn

[T53] Scala：字符串插值
来源：http://lx.9csxet.cn

s"值: $b"
来源：http://qo.panjiajie.cn

[T54] Scala：集合映射
来源：http://qc.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://zr.shxzukj.cn

[T55] Scala：集合过滤
来源：http://jd.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uv.colortex.cn

[T56] Scala：样例类
来源：http://uz.huanxung.cn

case class User(name: String, age: Int)
来源：http://vj.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ii.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sa.nicolike.cn

[T58] Scala：函数定义
来源：http://gq.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://op.asd995.cn

[T59] Scala：循环
来源：http://zf.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://dt.haigaiapp.cn

[T60] Scala：折叠
来源：http://ye.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ek.chemitech.net.cn

================================================================================
来源：http://js.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uj.yuntaijiaju.cn

================================================================================
来源：http://jz.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://oj.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jw.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://vk.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jq.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://ih.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://to.nicolike.cn

[U04] Py：变量调试打印
来源：http://lj.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fm.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://so.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ug.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://hv.asd995.cn

{**a, **b}
来源：http://cq.hnjuh.cn


<!-- 参考信息 -->