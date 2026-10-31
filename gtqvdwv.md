代发 wailian999

free -h;  ps aux | grep nginx
来源：http://zb.yuexingan06.cn

[R64] 结束进程
来源：http://ry.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://en.wgjwhj.cn

[R65] 查看端口占用
来源：http://xn.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ls.yuexingan06.cn

[R66] 定时任务
来源：http://wo.haigaiapp.cn

crontab -e;  crontab -l
来源：http://la.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://kb.hahajie.cn

openssl rand -hex 16
来源：http://vg.nicolike.cn

[R68] 计算文件校验值
来源：http://fb.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rs.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://qp.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://bi.jctech888.com.cn

[R70] 时间戳与互转
来源：http://br.521024.cn

date +%s;  date -d @1700000000
来源：http://lf.shtwfgs.cn

[R71] 日期格式化
来源：http://wp.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ra.colortex.cn

[R72] 等待端口就绪
来源：http://ad.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vv.nszjky.cn

[R73] 分割大日志
来源：http://zu.shxzukj.cn

split -l 1000 big.log part_
来源：http://ms.bookmarksfly.cn

[R74] 批量重命名
来源：http://vz.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ze.bookmarksfly.cn

[R75] 导出环境变量
来源：http://wm.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://oa.shxzukj.cn

[R76] 使用临时文件
来源：http://vi.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lo.hnjuh.cn

[R77] 读取用户输入
来源：http://ay.521024.cn

read -rp "请输入: " ans
来源：http://tn.asd995.cn

[R78] 交互式菜单
来源：http://kr.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qm.gzmigu.cn

[R79] 解析命令行选项
来源：http://qk.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hv.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://pu.jianghongdianzi.cn

time ./run.sh
来源：http://ma.shxzskj.cn

================================================================================
来源：http://ke.shtwfgs.cn

S. C / C++ 专题
来源：http://cf.bookmarksfly.cn

================================================================================
来源：http://cm.gzmigu.cn

[S01] C：Hello World
来源：http://hh.bookmarksfly.cn

#include <stdio.h>
来源：http://wh.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://di.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://za.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://sq.colortex.cn

[S03] C：读入整数
来源：http://ba.9csxet.cn

int x; scanf("%d", &x);
来源：http://tq.haigaiapp.cn

[S04] C：字符串复制
来源：http://jv.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://am.shxzukj.cn

[S05] C：字符串长度
来源：http://qn.lnxyls.cn

strlen(s)
来源：http://vh.gzmigu.cn

[S06] C：字符串比较
来源：http://ay.wgjwhj.cn

strcmp(a, b) == 0
来源：http://rs.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://xg.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fl.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://jx.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zk.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://kz.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wk.panjiajie.cn

[S10] C：指针与解引用
来源：http://zm.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://iv.shtwfgs.cn

[S11] C：逐行读文件
来源：http://ff.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://xk.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ol.bookmarksfly.cn

fclose(f);
来源：http://ke.lnxyls.cn

[S12] C：写文件
来源：http://am.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vs.panjiajie.cn

[S13] C：宏定义
来源：http://vg.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gx.521024.cn

[S14] C：枚举
来源：http://px.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://zw.huixiangedu.cn

[S15] C：类型转换
来源：http://uh.asd995.cn

(double) a / b
来源：http://ao.chemitech.net.cn

[S16] C：位操作置位
来源：http://qv.nszjky.cn

x |= (1 << 3);
来源：http://lj.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://fg.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bi.wgjwhj.cn

[S18] C：命令行参数
来源：http://xm.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://eo.chemitech.net.cn

[S19] C：快速排序
来源：http://zj.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eq.yuexingan06.cn

[S20] C：二分查找
来源：http://vl.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kh.szsharing.cn

[S21] C：字符类别判断
来源：http://xl.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zm.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://gy.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bu.haigaiapp.cn

[S23] C：随机数
来源：http://cd.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ct.shxzukj.cn

[S24] C：获取本地时间
来源：http://la.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bi.chemitech.net.cn

[S25] C：内存拷贝
来源：http://hw.asd995.cn

memcpy(dst, src, n);
来源：http://np.521024.cn

[S26] C：内存清零
来源：http://zp.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://kz.nicolike.cn

[S27] C：定义常量
来源：http://nz.muxihuayi.cn

const double PI = 3.14159;
来源：http://hj.gzmigu.cn

[S28] C：静态变量
来源：http://mp.shxzskj.cn

static int counter = 0;
来源：http://pb.jianghongdianzi.cn

[S29] C：变参函数
来源：http://ab.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jt.szxytkj.cn

[S30] C：头文件保护
来源：http://eo.jianghongdianzi.cn

#ifndef X_H
来源：http://en.haigaiapp.cn

#define X_H
来源：http://my.haigaiapp.cn

#endif
来源：http://hi.haigaiapp.cn

[S31] C++：Hello World
来源：http://ul.jctech888.com.cn

#include <iostream>
来源：http://oq.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://mg.wgjwhj.cn

[S32] C++：字符串
来源：http://am.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://nc.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://rd.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lw.lnxyls.cn

[S34] C++：遍历 vector
来源：http://vc.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://ff.szxytkj.cn

[S35] C++：map
来源：http://tx.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ed.szsharing.cn

[S36] C++：unordered_map
来源：http://cq.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pp.huanxung.cn

[S37] C++：set
来源：http://bo.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ji.bjjhwx.cn

[S38] C++：排序
来源：http://ai.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://md.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://vl.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tv.521024.cn

[S40] C++：查找元素
来源：http://yg.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pp.newstarts.cn

[S41] C++：类与构造函数
来源：http://xu.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vk.9csxet.cn

[S42] C++：继承与虚函数
来源：http://ob.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://ed.bjjhwx.cn

[S43] C++：智能指针
来源：http://sl.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://ju.chemitech.net.cn

[S44] C++：引用传参
来源：http://co.nicolike.cn

void inc(int &x) { ++x; }
来源：http://xg.521024.cn

[S45] C++：lambda
来源：http://tc.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fj.jctech888.com.cn

[S46] C++：函数模板
来源：http://mr.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ut.521024.cn

[S47] C++：结构化绑定遍历
来源：http://ag.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zf.huanxung.cn

[S48] C++：逐行读文件
来源：http://yc.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jc.521024.cn

while (std::getline(in, line)) { }
来源：http://nb.szxytkj.cn

[S49] C++：写文件
来源：http://gp.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://at.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://qo.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://do.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://wz.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://vg.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://gf.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://vl.haigaiapp.cn

[S53] C++：移动语义
来源：http://yy.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://nb.yuexingan06.cn

[S54] C++：异常处理
来源：http://rs.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kf.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://nl.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jk.colortex.cn

[S56] C++：optional
来源：http://vn.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fu.shtwfgs.cn

[S57] C++：编译期常量
来源：http://vn.huanxung.cn

constexpr int N = 10;
来源：http://wb.nicolike.cn

[S58] C++：命名空间
来源：http://ni.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://uf.shxzskj.cn

[S59] C++：静态断言
来源：http://te.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qr.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://mq.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hx.521024.cn

================================================================================
来源：http://cz.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fn.szxytkj.cn

================================================================================
来源：http://nf.asd995.cn

[T01] Kotlin：Hello World
来源：http://he.hahajie.cn

println("Hello")
来源：http://bf.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://tg.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xq.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://vv.shtwfgs.cn

"值: $b"
来源：http://mt.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://be.asd995.cn

val n: String? = null;  n?.length
来源：http://tj.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://yr.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bc.newstarts.cn

[T06] Kotlin：集合映射
来源：http://sn.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://da.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://ey.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qg.newstarts.cn

[T08] Kotlin：数据类
来源：http://kc.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://kj.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://xi.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://dd.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://sg.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jv.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://uq.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zk.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://jb.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://az.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://fa.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://xw.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://qv.shxzskj.cn

for (i in 1..10) println(i)
来源：http://kw.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://dz.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://er.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ux.521024.cn

print("Hello")
来源：http://em.hahajie.cn

[T17] Swift：变量与常量
来源：http://gg.shxzskj.cn

var a = 1;  let b = 2
来源：http://sp.panjiajie.cn

[T18] Swift：字符串插值
来源：http://yx.lnxyls.cn

"值: \(b)"
来源：http://wb.szxytkj.cn

[T19] Swift：可选绑定
来源：http://jx.chemitech.net.cn

if let n = opt { print(n) }
来源：http://oq.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://lr.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hk.colortex.cn

[T21] Swift：遍历
来源：http://fu.shxzukj.cn

for x in a { print(x) }
来源：http://hx.shxzukj.cn

[T22] Swift：字典
来源：http://ar.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://np.muxihuayi.cn

[T23] Swift：函数
来源：http://xr.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zh.szxytkj.cn

[T24] Swift：闭包
来源：http://go.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pb.nicolike.cn

[T25] Swift：结构体
来源：http://xp.yuntaijiaju.cn

struct P { var x: Int }
来源：http://et.yuexingan06.cn

[T26] Swift：类与重写
来源：http://fe.gzmigu.cn

class A: Base { override func f() {} }
来源：http://ue.chemitech.net.cn

[T27] Swift：错误处理
来源：http://yv.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://vr.wgjwhj.cn

[T28] Swift：枚举
来源：http://lx.nszjky.cn

enum Color { case red, green }
来源：http://ge.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://qq.szxytkj.cn

guard let x = opt else { return }
来源：http://hd.bjjhwx.cn

[T30] Swift：协议
来源：http://av.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://hp.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://dh.lnxyls.cn

print("Hello")
来源：http://ei.wgjwhj.cn

[T32] Lua：局部变量
来源：http://xa.haigaiapp.cn

local a = 1
来源：http://hr.shxzukj.cn

[T33] Lua：表（数组）
来源：http://xu.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ng.haigaiapp.cn

[T34] Lua：遍历表
来源：http://qt.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ww.shtwfgs.cn

[T35] Lua：字典表
来源：http://kn.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://dk.shxzukj.cn

[T36] Lua：函数
来源：http://ys.9csxet.cn

function add(a, b) return a + b end
来源：http://ht.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://uc.asd995.cn

"a" .. "b"
来源：http://vw.yuexingan06.cn

[T38] Lua：条件
来源：http://br.muxihuayi.cn

if x > 0 then print("正") end
来源：http://da.lnxyls.cn

[T39] Lua：模式匹配
来源：http://yn.nicolike.cn

string.find(s, "%d+")
来源：http://ne.hnjuh.cn

[T40] Lua：元表
来源：http://ro.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://ee.hnjuh.cn

[T41] Perl：Hello World
来源：http://ki.521024.cn

print "Hello\n";
来源：http://ry.asd995.cn

[T42] Perl：变量类型
来源：http://if.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fi.asd995.cn

[T43] Perl：字符串插值
来源：http://wb.wgjwhj.cn

"值: $a"
来源：http://gw.521024.cn

[T44] Perl：条件
来源：http://vv.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://di.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://gs.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://ft.panjiajie.cn

[T46] Perl：哈希操作
来源：http://zl.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ri.huanxung.cn

[T47] Perl：正则捕获
来源：http://mk.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rk.szxytkj.cn

[T48] Perl：正则替换
来源：http://so.gzmigu.cn

$s =~ s/old/new/g;
来源：http://yi.bjjhwx.cn

[T49] Perl：函数
来源：http://li.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uv.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://xm.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nl.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://wv.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://ho.yuexingan06.cn

println("Hello")
来源：http://ht.hnjuh.cn

[T52] Scala：变量
来源：http://cb.gzmigu.cn

val a = 1;  var b = 2
来源：http://tx.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://ac.bjjhwx.cn

s"值: $b"
来源：http://vs.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://dd.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://sb.colortex.cn

[T55] Scala：集合过滤
来源：http://wl.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ev.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://kz.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://ef.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://qp.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wx.panjiajie.cn

[T58] Scala：函数定义
来源：http://ef.gzmigu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cm.521024.cn

[T59] Scala：循环
来源：http://dm.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://cw.huixiangedu.cn

[T60] Scala：折叠
来源：http://dj.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://md.huixiangedu.cn

================================================================================
来源：http://bd.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gt.panjiajie.cn

================================================================================
来源：http://hu.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://yc.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kh.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://kc.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qe.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://mz.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ys.gzmigu.cn

[U04] Py：变量调试打印
来源：http://ds.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nb.bjjhwx.cn


<!-- 参考信息 -->