代发 wailian999

df -h;  du -sh *
来源：http://xb.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://wg.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://xg.panjiajie.cn

[R63] 内存与进程
来源：http://oe.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://lu.colortex.cn

[R64] 结束进程
来源：http://lm.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://oe.gzmigu.cn

[R65] 查看端口占用
来源：http://wr.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dp.huixinmuqiang.cn

[R66] 定时任务
来源：http://xm.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://jg.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://ya.521024.cn

openssl rand -hex 16
来源：http://ly.szxytkj.cn

[R68] 计算文件校验值
来源：http://vy.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sn.shxzskj.cn

[R69] 生成随机密码
来源：http://ij.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://kc.newstarts.cn

[R70] 时间戳与互转
来源：http://hg.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://kg.huixinmuqiang.cn

[R71] 日期格式化
来源：http://kj.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ym.bjjhwx.cn

[R72] 等待端口就绪
来源：http://gx.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hl.bookmarksfly.cn

[R73] 分割大日志
来源：http://fg.shxzukj.cn

split -l 1000 big.log part_
来源：http://vb.newstarts.cn

[R74] 批量重命名
来源：http://ep.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qz.lnxyls.cn

[R75] 导出环境变量
来源：http://fe.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://xz.bjjhwx.cn

[R76] 使用临时文件
来源：http://za.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://od.colortex.cn

[R77] 读取用户输入
来源：http://op.huixiangedu.cn

read -rp "请输入: " ans
来源：http://se.muxihuayi.cn

[R78] 交互式菜单
来源：http://nb.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jf.nicolike.cn

[R79] 解析命令行选项
来源：http://sh.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://on.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://xy.shtwfgs.cn

time ./run.sh
来源：http://ii.shxzskj.cn

================================================================================
来源：http://qk.521024.cn

S. C / C++ 专题
来源：http://bj.nszjky.cn

================================================================================
来源：http://rr.gzmigu.cn

[S01] C：Hello World
来源：http://ap.shxzskj.cn

#include <stdio.h>
来源：http://hr.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fw.hahajie.cn

[S02] C：变量与格式化输出
来源：http://yr.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://mu.chemitech.net.cn

[S03] C：读入整数
来源：http://ym.colortex.cn

int x; scanf("%d", &x);
来源：http://zw.shxzskj.cn

[S04] C：字符串复制
来源：http://jo.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ro.colortex.cn

[S05] C：字符串长度
来源：http://gn.shxzskj.cn

strlen(s)
来源：http://vx.nszjky.cn

[S06] C：字符串比较
来源：http://nx.bjjhwx.cn

strcmp(a, b) == 0
来源：http://qk.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://qa.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fr.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://pt.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yl.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://mz.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rl.hnjuh.cn

[S10] C：指针与解引用
来源：http://bb.nszjky.cn

int *p = &a;  *p = 5;
来源：http://ze.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://qa.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://sl.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://de.wgjwhj.cn

fclose(f);
来源：http://vm.hnjuh.cn

[S12] C：写文件
来源：http://sw.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wf.wgjwhj.cn

[S13] C：宏定义
来源：http://so.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zq.shxzskj.cn

[S14] C：枚举
来源：http://dc.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://rc.lnxyls.cn

[S15] C：类型转换
来源：http://ys.haigaiapp.cn

(double) a / b
来源：http://bh.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://nd.nicolike.cn

x |= (1 << 3);
来源：http://gb.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://vb.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nx.shxzskj.cn

[S18] C：命令行参数
来源：http://xa.muxihuayi.cn

int main(int argc, char **argv)
来源：http://ur.huixiangedu.cn

[S19] C：快速排序
来源：http://ue.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sy.521024.cn

[S20] C：二分查找
来源：http://fc.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nk.nicolike.cn

[S21] C：字符类别判断
来源：http://su.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qq.nicolike.cn

[S22] C：字符串转数字
来源：http://ep.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://st.szxytkj.cn

[S23] C：随机数
来源：http://nc.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wb.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://ft.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ns.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://fd.szxytkj.cn

memcpy(dst, src, n);
来源：http://ir.shtwfgs.cn

[S26] C：内存清零
来源：http://hz.nicolike.cn

memset(a, 0, sizeof a);
来源：http://ie.yuexingan06.cn

[S27] C：定义常量
来源：http://tk.shxzukj.cn

const double PI = 3.14159;
来源：http://fg.nicolike.cn

[S28] C：静态变量
来源：http://br.shxzskj.cn

static int counter = 0;
来源：http://fg.szxytkj.cn

[S29] C：变参函数
来源：http://tw.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tb.newstarts.cn

[S30] C：头文件保护
来源：http://kn.panjiajie.cn

#ifndef X_H
来源：http://nk.hahajie.cn

#define X_H
来源：http://cj.muxihuayi.cn

#endif
来源：http://ae.hnjuh.cn

[S31] C++：Hello World
来源：http://sz.gzmigu.cn

#include <iostream>
来源：http://wz.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ao.panjiajie.cn

[S32] C++：字符串
来源：http://tg.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://ti.hnjuh.cn

[S33] C++：vector 增删
来源：http://wd.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ah.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://wu.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://em.shxzskj.cn

[S35] C++：map
来源：http://up.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wv.panjiajie.cn

[S36] C++：unordered_map
来源：http://it.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qn.bjjhwx.cn

[S37] C++：set
来源：http://vn.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sd.9csxet.cn

[S38] C++：排序
来源：http://nz.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://hh.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://by.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cl.newstarts.cn

[S40] C++：查找元素
来源：http://dq.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qw.shxzskj.cn

[S41] C++：类与构造函数
来源：http://ga.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rb.colortex.cn

[S42] C++：继承与虚函数
来源：http://rr.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://zz.szsharing.cn

[S43] C++：智能指针
来源：http://jl.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://zo.bjjhwx.cn

[S44] C++：引用传参
来源：http://wa.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://eg.hahajie.cn

[S45] C++：lambda
来源：http://jx.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nj.huanxung.cn

[S46] C++：函数模板
来源：http://be.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vg.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://xb.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fg.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://ih.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fj.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://se.asd995.cn

[S49] C++：写文件
来源：http://hy.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xy.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://za.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pj.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://rn.huanxung.cn

static_cast<double>(a) / b
来源：http://mk.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yy.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://hh.521024.cn

[S53] C++：移动语义
来源：http://al.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://so.newstarts.cn

[S54] C++：异常处理
来源：http://ip.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ot.szsharing.cn

[S55] C++：结构化绑定
来源：http://oi.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kk.szxytkj.cn

[S56] C++：optional
来源：http://qv.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gc.panjiajie.cn

[S57] C++：编译期常量
来源：http://nw.wgjwhj.cn

constexpr int N = 10;
来源：http://hx.szxytkj.cn

[S58] C++：命名空间
来源：http://id.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://gj.521024.cn

[S59] C++：静态断言
来源：http://no.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://he.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://qy.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fm.hahajie.cn

================================================================================
来源：http://uo.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iw.yuexingan06.cn

================================================================================
来源：http://mc.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://kq.bookmarksfly.cn

println("Hello")
来源：http://uz.9csxet.cn

[T02] Kotlin：变量
来源：http://fy.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vo.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://sq.nicolike.cn

"值: $b"
来源：http://jg.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://wc.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://xx.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://ca.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zt.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://aq.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wk.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://bv.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://js.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://qx.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://il.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://jr.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://pz.huanxung.cn

[T10] Kotlin：默认参数
来源：http://et.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lc.521024.cn

[T11] Kotlin：协程
来源：http://ef.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yj.szsharing.cn

[T12] Kotlin：解构声明
来源：http://fk.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://bl.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://tp.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ml.shtwfgs.cn

[T14] Kotlin：循环
来源：http://tj.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://pu.shxzukj.cn

[T15] Kotlin：接口
来源：http://kj.colortex.cn

interface Shape { fun area(): Double }
来源：http://st.huixiangedu.cn

[T16] Swift：Hello World
来源：http://he.nicolike.cn

print("Hello")
来源：http://yg.nszjky.cn

[T17] Swift：变量与常量
来源：http://ad.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://py.9csxet.cn

[T18] Swift：字符串插值
来源：http://ty.wgjwhj.cn

"值: \(b)"
来源：http://vc.huanxung.cn

[T19] Swift：可选绑定
来源：http://me.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://wi.szxytkj.cn

[T20] Swift：数组操作
来源：http://jb.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://px.szsharing.cn

[T21] Swift：遍历
来源：http://is.gzmigu.cn

for x in a { print(x) }
来源：http://hk.wgjwhj.cn

[T22] Swift：字典
来源：http://qc.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jr.hahajie.cn

[T23] Swift：函数
来源：http://tk.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jr.colortex.cn

[T24] Swift：闭包
来源：http://ri.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cv.hnjuh.cn

[T25] Swift：结构体
来源：http://mb.shxzukj.cn

struct P { var x: Int }
来源：http://pa.jctech888.com.cn

[T26] Swift：类与重写
来源：http://ix.shxzskj.cn

class A: Base { override func f() {} }
来源：http://dk.lnxyls.cn

[T27] Swift：错误处理
来源：http://hx.nicolike.cn

do { try f() } catch { print(error) }
来源：http://wl.yuexingan06.cn

[T28] Swift：枚举
来源：http://hs.yuntaijiaju.cn

enum Color { case red, green }
来源：http://ph.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://jz.nicolike.cn

guard let x = opt else { return }
来源：http://ya.haigaiapp.cn

[T30] Swift：协议
来源：http://zo.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://ld.colortex.cn

[T31] Lua：Hello World
来源：http://pp.szsharing.cn

print("Hello")
来源：http://hr.bjjhwx.cn

[T32] Lua：局部变量
来源：http://wn.szxytkj.cn

local a = 1
来源：http://wh.lnxyls.cn

[T33] Lua：表（数组）
来源：http://qr.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fg.shtwfgs.cn

[T34] Lua：遍历表
来源：http://og.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://px.szsharing.cn

[T35] Lua：字典表
来源：http://ed.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://sn.chemitech.net.cn

[T36] Lua：函数
来源：http://af.shxzukj.cn

function add(a, b) return a + b end
来源：http://an.huanxung.cn

[T37] Lua：字符串拼接
来源：http://ht.chemitech.net.cn

"a" .. "b"
来源：http://kc.9csxet.cn

[T38] Lua：条件
来源：http://bd.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://hd.szsharing.cn

[T39] Lua：模式匹配
来源：http://lv.muxihuayi.cn

string.find(s, "%d+")
来源：http://zg.shtwfgs.cn

[T40] Lua：元表
来源：http://xx.szsharing.cn

setmetatable({}, { __index = base })
来源：http://vg.521024.cn

[T41] Perl：Hello World
来源：http://he.wgjwhj.cn

print "Hello\n";
来源：http://dn.wgjwhj.cn

[T42] Perl：变量类型
来源：http://kf.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nc.colortex.cn

[T43] Perl：字符串插值
来源：http://vt.muxihuayi.cn

"值: $a"
来源：http://qy.shxzskj.cn

[T44] Perl：条件
来源：http://an.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://oe.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://aw.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ad.panjiajie.cn

[T46] Perl：哈希操作
来源：http://dp.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vr.521024.cn

[T47] Perl：正则捕获
来源：http://pg.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://au.wgjwhj.cn

[T48] Perl：正则替换
来源：http://ar.panjiajie.cn

$s =~ s/old/new/g;
来源：http://za.nszjky.cn

[T49] Perl：函数
来源：http://iz.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kf.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://um.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rs.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://zi.nicolike.cn

[T51] Scala：Hello World
来源：http://ip.wgjwhj.cn

println("Hello")
来源：http://pd.huixiangedu.cn

[T52] Scala：变量
来源：http://nl.shtwfgs.cn

val a = 1;  var b = 2
来源：http://jf.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://uk.haigaiapp.cn

s"值: $b"
来源：http://rc.nszjky.cn

[T54] Scala：集合映射
来源：http://vj.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://qn.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://fp.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rg.asd995.cn

[T56] Scala：样例类
来源：http://lm.gzmigu.cn

case class User(name: String, age: Int)
来源：http://yh.nszjky.cn

[T57] Scala：模式匹配
来源：http://zj.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oq.nszjky.cn

[T58] Scala：函数定义
来源：http://wq.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lc.colortex.cn

[T59] Scala：循环
来源：http://wa.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://ao.nicolike.cn

[T60] Scala：折叠
来源：http://rn.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cq.huixiangedu.cn

================================================================================
来源：http://gy.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cl.hahajie.cn

================================================================================
来源：http://rq.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://df.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xu.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://vr.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xs.jianghongdianzi.cn


<!-- 参考信息 -->