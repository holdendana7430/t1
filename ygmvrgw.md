代发 wailian999

free -h;  ps aux | grep nginx
来源：http://dz.wgjwhj.cn

[R64] 结束进程
来源：http://dv.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://rh.wgjwhj.cn

[R65] 查看端口占用
来源：http://mh.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pm.shxzskj.cn

[R66] 定时任务
来源：http://qk.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://bq.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://yl.lnxyls.cn

openssl rand -hex 16
来源：http://qn.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://kv.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cb.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://ad.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://mt.shxzskj.cn

[R70] 时间戳与互转
来源：http://yx.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://af.muxihuayi.cn

[R71] 日期格式化
来源：http://xs.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uy.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://mb.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nk.shxzskj.cn

[R73] 分割大日志
来源：http://ek.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://kf.panjiajie.cn

[R74] 批量重命名
来源：http://td.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ec.yuexingan06.cn

[R75] 导出环境变量
来源：http://ja.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://qc.wgjwhj.cn

[R76] 使用临时文件
来源：http://en.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jg.newstarts.cn

[R77] 读取用户输入
来源：http://uv.521024.cn

read -rp "请输入: " ans
来源：http://vc.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://ca.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hh.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ms.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ov.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://nt.newstarts.cn

time ./run.sh
来源：http://vf.jctech888.com.cn

================================================================================
来源：http://ss.haigaiapp.cn

S. C / C++ 专题
来源：http://as.haigaiapp.cn

================================================================================
来源：http://xv.shxzukj.cn

[S01] C：Hello World
来源：http://fw.huixinmuqiang.cn

#include <stdio.h>
来源：http://ql.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oi.newstarts.cn

[S02] C：变量与格式化输出
来源：http://na.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://fu.jianghongdianzi.cn

[S03] C：读入整数
来源：http://yj.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://gf.asd995.cn

[S04] C：字符串复制
来源：http://fo.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ye.panjiajie.cn

[S05] C：字符串长度
来源：http://cq.huanxung.cn

strlen(s)
来源：http://xb.521024.cn

[S06] C：字符串比较
来源：http://qh.newstarts.cn

strcmp(a, b) == 0
来源：http://iu.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://ky.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uo.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://vm.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cw.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://vm.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://io.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://rc.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://ta.newstarts.cn

[S11] C：逐行读文件
来源：http://fx.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://cx.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xp.521024.cn

fclose(f);
来源：http://eb.nszjky.cn

[S12] C：写文件
来源：http://va.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wl.colortex.cn

[S13] C：宏定义
来源：http://ts.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vf.521024.cn

[S14] C：枚举
来源：http://ax.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://md.jianghongdianzi.cn

[S15] C：类型转换
来源：http://rq.shtwfgs.cn

(double) a / b
来源：http://dm.muxihuayi.cn

[S16] C：位操作置位
来源：http://lz.521024.cn

x |= (1 << 3);
来源：http://xz.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://ln.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kc.hahajie.cn

[S18] C：命令行参数
来源：http://ok.nicolike.cn

int main(int argc, char **argv)
来源：http://xt.szxytkj.cn

[S19] C：快速排序
来源：http://py.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eo.521024.cn

[S20] C：二分查找
来源：http://wx.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yh.haigaiapp.cn

[S21] C：字符类别判断
来源：http://yc.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vn.szsharing.cn

[S22] C：字符串转数字
来源：http://rw.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kc.hahajie.cn

[S23] C：随机数
来源：http://wf.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://id.haigaiapp.cn

[S24] C：获取本地时间
来源：http://rp.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mh.szxytkj.cn

[S25] C：内存拷贝
来源：http://bh.asd995.cn

memcpy(dst, src, n);
来源：http://ui.huixinmuqiang.cn

[S26] C：内存清零
来源：http://hq.hahajie.cn

memset(a, 0, sizeof a);
来源：http://zc.huixinmuqiang.cn

[S27] C：定义常量
来源：http://yh.gzmigu.cn

const double PI = 3.14159;
来源：http://ae.szsharing.cn

[S28] C：静态变量
来源：http://pe.shxzukj.cn

static int counter = 0;
来源：http://iz.nicolike.cn

[S29] C：变参函数
来源：http://gm.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ok.hahajie.cn

[S30] C：头文件保护
来源：http://ld.hnjuh.cn

#ifndef X_H
来源：http://ud.shxzskj.cn

#define X_H
来源：http://rh.panjiajie.cn

#endif
来源：http://wd.bjjhwx.cn

[S31] C++：Hello World
来源：http://nf.jianghongdianzi.cn

#include <iostream>
来源：http://pq.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://oy.yuntaijiaju.cn

[S32] C++：字符串
来源：http://ri.colortex.cn

std::string s = "hi";  s += "!";
来源：http://xg.gzmigu.cn

[S33] C++：vector 增删
来源：http://cw.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ta.asd995.cn

[S34] C++：遍历 vector
来源：http://mc.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://oz.szsharing.cn

[S35] C++：map
来源：http://jt.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ie.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://ub.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://om.yuexingan06.cn

[S37] C++：set
来源：http://lx.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oh.muxihuayi.cn

[S38] C++：排序
来源：http://vo.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://ah.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://dp.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sf.szsharing.cn

[S40] C++：查找元素
来源：http://vx.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qg.shxzukj.cn

[S41] C++：类与构造函数
来源：http://lk.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://no.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://it.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://wl.panjiajie.cn

[S43] C++：智能指针
来源：http://nz.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://rt.521024.cn

[S44] C++：引用传参
来源：http://ls.nszjky.cn

void inc(int &x) { ++x; }
来源：http://xc.hahajie.cn

[S45] C++：lambda
来源：http://av.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jm.huanxung.cn

[S46] C++：函数模板
来源：http://ic.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hy.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://nx.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gw.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://gw.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pa.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://pp.wgjwhj.cn

[S49] C++：写文件
来源：http://ds.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ie.chemitech.net.cn

[S50] C++：格式化数字
来源：http://zt.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vg.newstarts.cn

[S51] C++：显式类型转换
来源：http://xd.bjjhwx.cn

static_cast<double>(a) / b
来源：http://ra.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://tt.colortex.cn

int size() const noexcept { return n_; }
来源：http://qi.hahajie.cn

[S53] C++：移动语义
来源：http://ug.521024.cn

std::vector<int> w = std::move(v);
来源：http://ms.shtwfgs.cn

[S54] C++：异常处理
来源：http://uz.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ja.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://el.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qh.gzmigu.cn

[S56] C++：optional
来源：http://et.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uf.shxzukj.cn

[S57] C++：编译期常量
来源：http://zj.521024.cn

constexpr int N = 10;
来源：http://od.nszjky.cn

[S58] C++：命名空间
来源：http://ek.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://th.wgjwhj.cn

[S59] C++：静态断言
来源：http://ku.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ds.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://yw.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oc.nszjky.cn

================================================================================
来源：http://yk.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ke.szsharing.cn

================================================================================
来源：http://bm.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://xx.shtwfgs.cn

println("Hello")
来源：http://wg.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://vv.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cu.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://xh.huixinmuqiang.cn

"值: $b"
来源：http://xm.nszjky.cn

[T04] Kotlin：空安全
来源：http://ch.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://vm.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://kz.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ww.nicolike.cn

[T06] Kotlin：集合映射
来源：http://yo.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ey.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://ju.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://el.shxzskj.cn

[T08] Kotlin：数据类
来源：http://vg.colortex.cn

data class User(val name: String, val age: Int)
来源：http://bz.521024.cn

[T09] Kotlin：扩展函数
来源：http://ps.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://rg.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://zy.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://in.yuexingan06.cn

[T11] Kotlin：协程
来源：http://xa.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wr.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ph.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://ju.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://uq.newstarts.cn

val m = mapOf("a" to 1)
来源：http://xf.huixiangedu.cn

[T14] Kotlin：循环
来源：http://cd.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://ex.chemitech.net.cn

[T15] Kotlin：接口
来源：http://uz.521024.cn

interface Shape { fun area(): Double }
来源：http://gu.bjjhwx.cn

[T16] Swift：Hello World
来源：http://bg.muxihuayi.cn

print("Hello")
来源：http://tl.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://zc.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://me.szxytkj.cn

[T18] Swift：字符串插值
来源：http://ka.panjiajie.cn

"值: \(b)"
来源：http://yh.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://uy.muxihuayi.cn

if let n = opt { print(n) }
来源：http://gj.nicolike.cn

[T20] Swift：数组操作
来源：http://gt.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fw.newstarts.cn

[T21] Swift：遍历
来源：http://if.newstarts.cn

for x in a { print(x) }
来源：http://vj.shxzskj.cn

[T22] Swift：字典
来源：http://hc.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yj.nszjky.cn

[T23] Swift：函数
来源：http://zu.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qi.wgjwhj.cn

[T24] Swift：闭包
来源：http://om.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zs.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://qa.wgjwhj.cn

struct P { var x: Int }
来源：http://yw.nicolike.cn

[T26] Swift：类与重写
来源：http://pn.nicolike.cn

class A: Base { override func f() {} }
来源：http://yc.shtwfgs.cn

[T27] Swift：错误处理
来源：http://am.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://ro.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://md.hnjuh.cn

enum Color { case red, green }
来源：http://rj.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://as.newstarts.cn

guard let x = opt else { return }
来源：http://ky.gzmigu.cn

[T30] Swift：协议
来源：http://ji.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://bk.wgjwhj.cn

[T31] Lua：Hello World
来源：http://fx.bjjhwx.cn

print("Hello")
来源：http://lg.521024.cn

[T32] Lua：局部变量
来源：http://tc.muxihuayi.cn

local a = 1
来源：http://ii.huanxung.cn

[T33] Lua：表（数组）
来源：http://ju.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zf.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ac.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zr.szxytkj.cn

[T35] Lua：字典表
来源：http://kh.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://ff.521024.cn

[T36] Lua：函数
来源：http://pe.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://vl.szsharing.cn

[T37] Lua：字符串拼接
来源：http://cr.haigaiapp.cn

"a" .. "b"
来源：http://wm.shtwfgs.cn

[T38] Lua：条件
来源：http://vo.521024.cn

if x > 0 then print("正") end
来源：http://ek.nicolike.cn

[T39] Lua：模式匹配
来源：http://yp.colortex.cn

string.find(s, "%d+")
来源：http://yy.szsharing.cn

[T40] Lua：元表
来源：http://nh.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://uz.szsharing.cn

[T41] Perl：Hello World
来源：http://nm.chemitech.net.cn

print "Hello\n";
来源：http://ze.wgjwhj.cn

[T42] Perl：变量类型
来源：http://ww.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kx.hnjuh.cn

[T43] Perl：字符串插值
来源：http://ib.wgjwhj.cn

"值: $a"
来源：http://if.shxzskj.cn

[T44] Perl：条件
来源：http://db.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://gh.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://jc.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://vl.panjiajie.cn

[T46] Perl：哈希操作
来源：http://ha.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fi.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://dz.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qc.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://st.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://da.huixinmuqiang.cn

[T49] Perl：函数
来源：http://ds.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://du.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://qq.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qh.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://uy.muxihuayi.cn

[T51] Scala：Hello World
来源：http://xe.asd995.cn

println("Hello")
来源：http://af.yuntaijiaju.cn

[T52] Scala：变量
来源：http://wy.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://ke.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://ie.hnjuh.cn

s"值: $b"
来源：http://nx.haigaiapp.cn

[T54] Scala：集合映射
来源：http://gq.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://ar.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://qm.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lr.colortex.cn

[T56] Scala：样例类
来源：http://ft.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://hz.hnjuh.cn

[T57] Scala：模式匹配
来源：http://ae.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://we.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://cu.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ej.nszjky.cn

[T59] Scala：循环
来源：http://eb.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://nw.panjiajie.cn

[T60] Scala：折叠
来源：http://bc.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ve.jianghongdianzi.cn

================================================================================
来源：http://ey.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wh.panjiajie.cn

================================================================================
来源：http://jo.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://bv.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rl.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://pg.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xg.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://lu.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://et.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://sz.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pt.521024.cn


<!-- 参考信息 -->