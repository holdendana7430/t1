代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ga.newstarts.cn

[R66] 定时任务
来源：http://ww.szxytkj.cn

crontab -e;  crontab -l
来源：http://kq.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://dq.haigaiapp.cn

openssl rand -hex 16
来源：http://gu.huixiangedu.cn

[R68] 计算文件校验值
来源：http://jk.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ke.panjiajie.cn

[R69] 生成随机密码
来源：http://ie.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://wf.nszjky.cn

[R70] 时间戳与互转
来源：http://dd.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://ef.yuexingan06.cn

[R71] 日期格式化
来源：http://yx.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://er.521024.cn

[R72] 等待端口就绪
来源：http://ik.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rk.nszjky.cn

[R73] 分割大日志
来源：http://xz.szxytkj.cn

split -l 1000 big.log part_
来源：http://se.asd995.cn

[R74] 批量重命名
来源：http://po.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xb.gzmigu.cn

[R75] 导出环境变量
来源：http://zh.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://nc.jctech888.com.cn

[R76] 使用临时文件
来源：http://lh.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xs.szxytkj.cn

[R77] 读取用户输入
来源：http://ge.wgjwhj.cn

read -rp "请输入: " ans
来源：http://cz.huixiangedu.cn

[R78] 交互式菜单
来源：http://by.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fn.jctech888.com.cn

[R79] 解析命令行选项
来源：http://hi.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jg.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://rz.newstarts.cn

time ./run.sh
来源：http://zs.9csxet.cn

================================================================================
来源：http://wb.hnjuh.cn

S. C / C++ 专题
来源：http://ge.chemitech.net.cn

================================================================================
来源：http://lh.wgjwhj.cn

[S01] C：Hello World
来源：http://ix.szsharing.cn

#include <stdio.h>
来源：http://uv.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sp.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://ki.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://zm.yuntaijiaju.cn

[S03] C：读入整数
来源：http://yu.9csxet.cn

int x; scanf("%d", &x);
来源：http://ep.wgjwhj.cn

[S04] C：字符串复制
来源：http://he.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://se.panjiajie.cn

[S05] C：字符串长度
来源：http://cl.9csxet.cn

strlen(s)
来源：http://qa.colortex.cn

[S06] C：字符串比较
来源：http://ij.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://po.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://gn.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iq.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://xp.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eb.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://df.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://in.haigaiapp.cn

[S10] C：指针与解引用
来源：http://rm.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://co.nszjky.cn

[S11] C：逐行读文件
来源：http://un.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://fy.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://my.panjiajie.cn

fclose(f);
来源：http://yf.jctech888.com.cn

[S12] C：写文件
来源：http://xo.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qy.asd995.cn

[S13] C：宏定义
来源：http://oc.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nh.newstarts.cn

[S14] C：枚举
来源：http://im.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://qf.bookmarksfly.cn

[S15] C：类型转换
来源：http://bf.huixiangedu.cn

(double) a / b
来源：http://ti.shxzskj.cn

[S16] C：位操作置位
来源：http://rt.shtwfgs.cn

x |= (1 << 3);
来源：http://yd.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://su.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lw.521024.cn

[S18] C：命令行参数
来源：http://ic.shtwfgs.cn

int main(int argc, char **argv)
来源：http://ir.jianghongdianzi.cn

[S19] C：快速排序
来源：http://nd.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jo.jctech888.com.cn

[S20] C：二分查找
来源：http://hx.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pu.bjjhwx.cn

[S21] C：字符类别判断
来源：http://uz.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wj.bjjhwx.cn

[S22] C：字符串转数字
来源：http://ej.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mo.lnxyls.cn

[S23] C：随机数
来源：http://ci.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dn.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://mz.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mv.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ln.nszjky.cn

memcpy(dst, src, n);
来源：http://qo.wgjwhj.cn

[S26] C：内存清零
来源：http://pg.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://wd.haigaiapp.cn

[S27] C：定义常量
来源：http://xp.521024.cn

const double PI = 3.14159;
来源：http://qk.huixiangedu.cn

[S28] C：静态变量
来源：http://yb.asd995.cn

static int counter = 0;
来源：http://et.szsharing.cn

[S29] C：变参函数
来源：http://je.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jn.gzmigu.cn

[S30] C：头文件保护
来源：http://yz.gzmigu.cn

#ifndef X_H
来源：http://ti.muxihuayi.cn

#define X_H
来源：http://za.jianghongdianzi.cn

#endif
来源：http://ct.nszjky.cn

[S31] C++：Hello World
来源：http://mo.lnxyls.cn

#include <iostream>
来源：http://bk.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://xv.shxzukj.cn

[S32] C++：字符串
来源：http://ma.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://pf.colortex.cn

[S33] C++：vector 增删
来源：http://vd.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://br.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://sp.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://fx.lnxyls.cn

[S35] C++：map
来源：http://zq.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nicolike.cn

[S36] C++：unordered_map
来源：http://th.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mn.yuexingan06.cn

[S37] C++：set
来源：http://vo.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fx.521024.cn

[S38] C++：排序
来源：http://hh.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://go.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://ir.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uu.521024.cn

[S40] C++：查找元素
来源：http://op.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ty.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://xj.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cx.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://st.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://aj.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://pa.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ih.nszjky.cn

[S44] C++：引用传参
来源：http://ma.9csxet.cn

void inc(int &x) { ++x; }
来源：http://ig.muxihuayi.cn

[S45] C++：lambda
来源：http://eo.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qo.jctech888.com.cn

[S46] C++：函数模板
来源：http://jb.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vh.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://yr.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gf.521024.cn

[S48] C++：逐行读文件
来源：http://iq.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jo.szsharing.cn

while (std::getline(in, line)) { }
来源：http://tx.jctech888.com.cn

[S49] C++：写文件
来源：http://qa.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://km.szxytkj.cn

[S50] C++：格式化数字
来源：http://pm.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ba.9csxet.cn

[S51] C++：显式类型转换
来源：http://mo.muxihuayi.cn

static_cast<double>(a) / b
来源：http://dj.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://nf.newstarts.cn

int size() const noexcept { return n_; }
来源：http://jx.chemitech.net.cn

[S53] C++：移动语义
来源：http://gu.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ww.huanxung.cn

[S54] C++：异常处理
来源：http://zl.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://su.nszjky.cn

[S55] C++：结构化绑定
来源：http://ei.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://op.bjjhwx.cn

[S56] C++：optional
来源：http://hi.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pf.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://ge.szsharing.cn

constexpr int N = 10;
来源：http://oe.asd995.cn

[S58] C++：命名空间
来源：http://hk.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://pf.hahajie.cn

[S59] C++：静态断言
来源：http://ky.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gj.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://lp.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nn.shxzskj.cn

================================================================================
来源：http://aa.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ub.colortex.cn

================================================================================
来源：http://gr.szsharing.cn

[T01] Kotlin：Hello World
来源：http://rj.bookmarksfly.cn

println("Hello")
来源：http://sq.chemitech.net.cn

[T02] Kotlin：变量
来源：http://au.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eo.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://ni.wgjwhj.cn

"值: $b"
来源：http://sy.szxytkj.cn

[T04] Kotlin：空安全
来源：http://qp.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://vm.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://mm.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cg.nicolike.cn

[T06] Kotlin：集合映射
来源：http://mz.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oa.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://vp.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ko.shxzukj.cn

[T08] Kotlin：数据类
来源：http://aq.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://bj.asd995.cn

[T09] Kotlin：扩展函数
来源：http://hs.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://lt.hahajie.cn

[T10] Kotlin：默认参数
来源：http://zi.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tx.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ar.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qg.hahajie.cn

[T12] Kotlin：解构声明
来源：http://wl.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://ct.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://jz.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://ki.lnxyls.cn

[T14] Kotlin：循环
来源：http://vv.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://ej.shxzskj.cn

[T15] Kotlin：接口
来源：http://qy.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://hc.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://gj.haigaiapp.cn

print("Hello")
来源：http://um.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://eq.haigaiapp.cn

var a = 1;  let b = 2
来源：http://fw.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://la.shxzskj.cn

"值: \(b)"
来源：http://rd.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://sa.szsharing.cn

if let n = opt { print(n) }
来源：http://hs.muxihuayi.cn

[T20] Swift：数组操作
来源：http://ht.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sy.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://ln.huanxung.cn

for x in a { print(x) }
来源：http://tu.huixinmuqiang.cn

[T22] Swift：字典
来源：http://gy.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://js.muxihuayi.cn

[T23] Swift：函数
来源：http://rp.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yd.chemitech.net.cn

[T24] Swift：闭包
来源：http://bn.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://az.521024.cn

[T25] Swift：结构体
来源：http://ll.nicolike.cn

struct P { var x: Int }
来源：http://jb.9csxet.cn

[T26] Swift：类与重写
来源：http://wz.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://hx.shxzukj.cn

[T27] Swift：错误处理
来源：http://sn.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://jc.shtwfgs.cn

[T28] Swift：枚举
来源：http://lx.shxzukj.cn

enum Color { case red, green }
来源：http://dy.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://mk.521024.cn

guard let x = opt else { return }
来源：http://he.hahajie.cn

[T30] Swift：协议
来源：http://bt.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://pw.colortex.cn

[T31] Lua：Hello World
来源：http://es.bookmarksfly.cn

print("Hello")
来源：http://uh.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://pt.hnjuh.cn

local a = 1
来源：http://rb.hnjuh.cn

[T33] Lua：表（数组）
来源：http://nz.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tx.hahajie.cn

[T34] Lua：遍历表
来源：http://oc.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fc.hahajie.cn

[T35] Lua：字典表
来源：http://ug.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://qm.asd995.cn

[T36] Lua：函数
来源：http://ff.yuexingan06.cn

function add(a, b) return a + b end
来源：http://oc.newstarts.cn

[T37] Lua：字符串拼接
来源：http://zt.colortex.cn

"a" .. "b"
来源：http://nd.lnxyls.cn

[T38] Lua：条件
来源：http://ri.asd995.cn

if x > 0 then print("正") end
来源：http://yy.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://mb.nszjky.cn

string.find(s, "%d+")
来源：http://er.muxihuayi.cn

[T40] Lua：元表
来源：http://xo.521024.cn

setmetatable({}, { __index = base })
来源：http://we.wgjwhj.cn

[T41] Perl：Hello World
来源：http://dj.gzmigu.cn

print "Hello\n";
来源：http://qe.szsharing.cn

[T42] Perl：变量类型
来源：http://cb.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pw.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://uj.wgjwhj.cn

"值: $a"
来源：http://bv.nicolike.cn

[T44] Perl：条件
来源：http://hi.colortex.cn

if ($a > 0) { print "正"; }
来源：http://tf.lnxyls.cn

[T45] Perl：数组遍历
来源：http://cb.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://hi.lnxyls.cn

[T46] Perl：哈希操作
来源：http://dq.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ef.colortex.cn

[T47] Perl：正则捕获
来源：http://dq.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nm.nicolike.cn

[T48] Perl：正则替换
来源：http://qa.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://jk.huanxung.cn

[T49] Perl：函数
来源：http://mj.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://um.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://ol.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bi.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://zf.hnjuh.cn

[T51] Scala：Hello World
来源：http://ci.panjiajie.cn

println("Hello")
来源：http://fe.chemitech.net.cn

[T52] Scala：变量
来源：http://zm.521024.cn

val a = 1;  var b = 2
来源：http://uc.nszjky.cn

[T53] Scala：字符串插值
来源：http://xu.jianghongdianzi.cn

s"值: $b"
来源：http://dj.shxzukj.cn

[T54] Scala：集合映射
来源：http://wh.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://bz.shxzskj.cn

[T55] Scala：集合过滤
来源：http://lm.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ly.shxzukj.cn

[T56] Scala：样例类
来源：http://vf.nicolike.cn

case class User(name: String, age: Int)
来源：http://kh.szsharing.cn

[T57] Scala：模式匹配
来源：http://hy.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mp.asd995.cn

[T58] Scala：函数定义
来源：http://yh.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fi.bookmarksfly.cn

[T59] Scala：循环
来源：http://cq.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://ds.chemitech.net.cn

[T60] Scala：折叠
来源：http://vd.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://px.colortex.cn

================================================================================
来源：http://rl.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://um.hahajie.cn

================================================================================
来源：http://ol.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://id.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vb.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://hr.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zq.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://mv.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vq.nicolike.cn

[U04] Py：变量调试打印
来源：http://rk.huanxung.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ns.nicolike.cn

[U05] Py：列表去重且保序
来源：http://ev.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://bh.newstarts.cn

[U06] Py：合并两个字典
来源：http://wy.bookmarksfly.cn

{**a, **b}
来源：http://ff.chemitech.net.cn


<!-- 参考信息 -->