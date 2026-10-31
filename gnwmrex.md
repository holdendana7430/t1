代发 wailian999

df -h;  du -sh *
来源：http://sa.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://vn.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://yp.gzmigu.cn

[R63] 内存与进程
来源：http://dc.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://ip.hahajie.cn

[R64] 结束进程
来源：http://pe.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://tn.haigaiapp.cn

[R65] 查看端口占用
来源：http://uf.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gn.szsharing.cn

[R66] 定时任务
来源：http://fa.panjiajie.cn

crontab -e;  crontab -l
来源：http://th.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://zz.9csxet.cn

openssl rand -hex 16
来源：http://uk.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://xq.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jb.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://ac.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://pa.wgjwhj.cn

[R70] 时间戳与互转
来源：http://cd.nszjky.cn

date +%s;  date -d @1700000000
来源：http://cq.wgjwhj.cn

[R71] 日期格式化
来源：http://bw.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sd.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://ni.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ed.yuexingan06.cn

[R73] 分割大日志
来源：http://kq.panjiajie.cn

split -l 1000 big.log part_
来源：http://ug.lnxyls.cn

[R74] 批量重命名
来源：http://gq.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fq.nicolike.cn

[R75] 导出环境变量
来源：http://af.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://cz.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://az.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ou.521024.cn

[R77] 读取用户输入
来源：http://cv.bjjhwx.cn

read -rp "请输入: " ans
来源：http://yh.chemitech.net.cn

[R78] 交互式菜单
来源：http://hc.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zf.asd995.cn

[R79] 解析命令行选项
来源：http://cd.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ut.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://mi.haigaiapp.cn

time ./run.sh
来源：http://gt.huanxung.cn

================================================================================
来源：http://rp.hahajie.cn

S. C / C++ 专题
来源：http://jb.yuntaijiaju.cn

================================================================================
来源：http://hx.szsharing.cn

[S01] C：Hello World
来源：http://pb.muxihuayi.cn

#include <stdio.h>
来源：http://dn.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wx.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://si.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://cg.huanxung.cn

[S03] C：读入整数
来源：http://dz.shxzskj.cn

int x; scanf("%d", &x);
来源：http://gd.gzmigu.cn

[S04] C：字符串复制
来源：http://ii.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tv.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://ho.bookmarksfly.cn

strlen(s)
来源：http://gu.nicolike.cn

[S06] C：字符串比较
来源：http://uh.huixiangedu.cn

strcmp(a, b) == 0
来源：http://ui.hahajie.cn

[S07] C：数组遍历求和
来源：http://kk.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://er.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://mo.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qx.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://uh.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://in.hahajie.cn

[S10] C：指针与解引用
来源：http://de.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://gx.shxzskj.cn

[S11] C：逐行读文件
来源：http://pf.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://uq.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ur.huixiangedu.cn

fclose(f);
来源：http://eq.hnjuh.cn

[S12] C：写文件
来源：http://vl.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bl.szsharing.cn

[S13] C：宏定义
来源：http://dl.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://do.haigaiapp.cn

[S14] C：枚举
来源：http://fl.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://dm.521024.cn

[S15] C：类型转换
来源：http://mo.hnjuh.cn

(double) a / b
来源：http://dg.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://ah.huanxung.cn

x |= (1 << 3);
来源：http://oh.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://sm.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://af.szxytkj.cn

[S18] C：命令行参数
来源：http://oa.newstarts.cn

int main(int argc, char **argv)
来源：http://rv.shtwfgs.cn

[S19] C：快速排序
来源：http://ch.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sx.nszjky.cn

[S20] C：二分查找
来源：http://wj.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://my.huixiangedu.cn

[S21] C：字符类别判断
来源：http://nj.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ez.jctech888.com.cn

[S22] C：字符串转数字
来源：http://ir.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fy.szsharing.cn

[S23] C：随机数
来源：http://li.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wd.hnjuh.cn

[S24] C：获取本地时间
来源：http://to.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nc.colortex.cn

[S25] C：内存拷贝
来源：http://go.nszjky.cn

memcpy(dst, src, n);
来源：http://wz.muxihuayi.cn

[S26] C：内存清零
来源：http://wc.nszjky.cn

memset(a, 0, sizeof a);
来源：http://vc.haigaiapp.cn

[S27] C：定义常量
来源：http://lb.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://xn.lnxyls.cn

[S28] C：静态变量
来源：http://hz.haigaiapp.cn

static int counter = 0;
来源：http://ab.shtwfgs.cn

[S29] C：变参函数
来源：http://oz.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://px.shxzskj.cn

[S30] C：头文件保护
来源：http://yx.muxihuayi.cn

#ifndef X_H
来源：http://zw.asd995.cn

#define X_H
来源：http://md.bjjhwx.cn

#endif
来源：http://nu.bjjhwx.cn

[S31] C++：Hello World
来源：http://ce.hahajie.cn

#include <iostream>
来源：http://xl.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://zn.jctech888.com.cn

[S32] C++：字符串
来源：http://ud.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://ws.chemitech.net.cn

[S33] C++：vector 增删
来源：http://kj.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vj.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://ud.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://ji.szsharing.cn

[S35] C++：map
来源：http://hb.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tf.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://kr.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xy.szsharing.cn

[S37] C++：set
来源：http://ze.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qu.9csxet.cn

[S38] C++：排序
来源：http://fa.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://zf.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://fe.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cg.lnxyls.cn

[S40] C++：查找元素
来源：http://xe.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sz.nicolike.cn

[S41] C++：类与构造函数
来源：http://wn.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bl.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://qm.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ez.wgjwhj.cn

[S43] C++：智能指针
来源：http://gw.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://ha.colortex.cn

[S44] C++：引用传参
来源：http://uf.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://dj.nicolike.cn

[S45] C++：lambda
来源：http://fz.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://us.hahajie.cn

[S46] C++：函数模板
来源：http://ue.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://at.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://wm.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gn.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://fd.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kq.9csxet.cn

while (std::getline(in, line)) { }
来源：http://fj.chemitech.net.cn

[S49] C++：写文件
来源：http://wq.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nw.bjjhwx.cn

[S50] C++：格式化数字
来源：http://xd.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yw.hnjuh.cn

[S51] C++：显式类型转换
来源：http://fp.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://qv.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://zg.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://jg.lnxyls.cn

[S53] C++：移动语义
来源：http://ay.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://ck.nszjky.cn

[S54] C++：异常处理
来源：http://sg.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mv.hnjuh.cn

[S55] C++：结构化绑定
来源：http://rj.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gc.panjiajie.cn

[S56] C++：optional
来源：http://rf.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zc.hahajie.cn

[S57] C++：编译期常量
来源：http://pw.nszjky.cn

constexpr int N = 10;
来源：http://re.newstarts.cn

[S58] C++：命名空间
来源：http://yy.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://ry.wgjwhj.cn

[S59] C++：静态断言
来源：http://zq.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cp.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://xl.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jl.shxzukj.cn

================================================================================
来源：http://vu.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hl.muxihuayi.cn

================================================================================
来源：http://pp.nszjky.cn

[T01] Kotlin：Hello World
来源：http://ix.asd995.cn

println("Hello")
来源：http://bs.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ur.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uc.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://qw.huanxung.cn

"值: $b"
来源：http://av.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://xz.nicolike.cn

val n: String? = null;  n?.length
来源：http://me.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://ry.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wa.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://rs.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qt.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://fp.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jq.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://oj.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://qy.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://ec.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://qx.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://gv.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zc.huixiangedu.cn

[T11] Kotlin：协程
来源：http://yp.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://he.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://ua.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://ki.521024.cn

[T13] Kotlin：只读 Map
来源：http://fh.asd995.cn

val m = mapOf("a" to 1)
来源：http://kl.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://hn.panjiajie.cn

for (i in 1..10) println(i)
来源：http://hv.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://ay.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ku.shxzukj.cn

[T16] Swift：Hello World
来源：http://ck.hahajie.cn

print("Hello")
来源：http://tc.szxytkj.cn

[T17] Swift：变量与常量
来源：http://qo.chemitech.net.cn

var a = 1;  let b = 2
来源：http://tj.lnxyls.cn

[T18] Swift：字符串插值
来源：http://lc.gzmigu.cn

"值: \(b)"
来源：http://bq.gzmigu.cn

[T19] Swift：可选绑定
来源：http://hp.nszjky.cn

if let n = opt { print(n) }
来源：http://ny.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://rv.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vx.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://zz.huixiangedu.cn

for x in a { print(x) }
来源：http://kl.9csxet.cn

[T22] Swift：字典
来源：http://bu.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uq.szsharing.cn

[T23] Swift：函数
来源：http://hj.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cq.szsharing.cn

[T24] Swift：闭包
来源：http://kw.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zb.szsharing.cn

[T25] Swift：结构体
来源：http://fa.shxzukj.cn

struct P { var x: Int }
来源：http://wb.szxytkj.cn

[T26] Swift：类与重写
来源：http://od.szsharing.cn

class A: Base { override func f() {} }
来源：http://js.gzmigu.cn

[T27] Swift：错误处理
来源：http://ne.hahajie.cn

do { try f() } catch { print(error) }
来源：http://hz.shtwfgs.cn

[T28] Swift：枚举
来源：http://hv.haigaiapp.cn

enum Color { case red, green }
来源：http://ae.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://vz.huanxung.cn

guard let x = opt else { return }
来源：http://lt.521024.cn

[T30] Swift：协议
来源：http://yg.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://py.521024.cn

[T31] Lua：Hello World
来源：http://gm.panjiajie.cn

print("Hello")
来源：http://eh.lnxyls.cn

[T32] Lua：局部变量
来源：http://gh.szxytkj.cn

local a = 1
来源：http://fi.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://eq.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://if.hnjuh.cn

[T34] Lua：遍历表
来源：http://hh.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dc.panjiajie.cn

[T35] Lua：字典表
来源：http://ip.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://pr.huixiangedu.cn

[T36] Lua：函数
来源：http://bm.asd995.cn

function add(a, b) return a + b end
来源：http://gg.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://hc.shxzukj.cn

"a" .. "b"
来源：http://el.shxzskj.cn

[T38] Lua：条件
来源：http://cj.chemitech.net.cn

if x > 0 then print("正") end
来源：http://dj.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://tm.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://hx.newstarts.cn

[T40] Lua：元表
来源：http://yc.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://dx.nicolike.cn

[T41] Perl：Hello World
来源：http://tw.nicolike.cn

print "Hello\n";
来源：http://dx.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://se.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://os.colortex.cn

[T43] Perl：字符串插值
来源：http://xz.huixiangedu.cn

"值: $a"
来源：http://zy.shtwfgs.cn

[T44] Perl：条件
来源：http://oo.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://hv.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://tn.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://bb.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://yl.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mr.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://md.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fv.shxzskj.cn

[T48] Perl：正则替换
来源：http://nw.hnjuh.cn

$s =~ s/old/new/g;
来源：http://ej.yuexingan06.cn

[T49] Perl：函数
来源：http://oa.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vt.huanxung.cn

[T50] Perl：逐行读文件
来源：http://dv.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sl.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://ua.gzmigu.cn

[T51] Scala：Hello World
来源：http://ot.gzmigu.cn

println("Hello")
来源：http://fv.hnjuh.cn

[T52] Scala：变量
来源：http://pd.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://jh.asd995.cn

[T53] Scala：字符串插值
来源：http://rc.huanxung.cn

s"值: $b"
来源：http://wd.nicolike.cn

[T54] Scala：集合映射
来源：http://sp.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://kw.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://ca.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gu.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://gg.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://pp.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://hr.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rp.hnjuh.cn

[T58] Scala：函数定义
来源：http://uk.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wd.yuexingan06.cn

[T59] Scala：循环
来源：http://gd.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://bu.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://nd.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xm.nicolike.cn

================================================================================
来源：http://ec.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gg.bookmarksfly.cn

================================================================================
来源：http://uk.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://he.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://db.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://zx.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tx.hahajie.cn


<!-- 参考信息 -->