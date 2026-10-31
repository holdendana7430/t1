代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zl.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://oc.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oz.szsharing.cn

[R61] 磁盘占用
来源：http://wz.9csxet.cn

df -h;  du -sh *
来源：http://mf.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://lo.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://gm.yuntaijiaju.cn

[R63] 内存与进程
来源：http://nz.bjjhwx.cn

free -h;  ps aux | grep nginx
来源：http://fg.nicolike.cn

[R64] 结束进程
来源：http://mo.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://zm.huixiangedu.cn

[R65] 查看端口占用
来源：http://qn.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zt.chemitech.net.cn

[R66] 定时任务
来源：http://ki.shxzukj.cn

crontab -e;  crontab -l
来源：http://oa.newstarts.cn

[R67] 生成随机十六进制串
来源：http://gg.jctech888.com.cn

openssl rand -hex 16
来源：http://ig.wgjwhj.cn

[R68] 计算文件校验值
来源：http://ys.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ko.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://ct.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://no.nicolike.cn

[R70] 时间戳与互转
来源：http://so.521024.cn

date +%s;  date -d @1700000000
来源：http://sb.nicolike.cn

[R71] 日期格式化
来源：http://fs.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://si.chemitech.net.cn

[R72] 等待端口就绪
来源：http://zu.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ui.521024.cn

[R73] 分割大日志
来源：http://bu.chemitech.net.cn

split -l 1000 big.log part_
来源：http://fs.hahajie.cn

[R74] 批量重命名
来源：http://uo.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lh.colortex.cn

[R75] 导出环境变量
来源：http://jj.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://iz.colortex.cn

[R76] 使用临时文件
来源：http://wk.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hu.lnxyls.cn

[R77] 读取用户输入
来源：http://qu.panjiajie.cn

read -rp "请输入: " ans
来源：http://ol.9csxet.cn

[R78] 交互式菜单
来源：http://yb.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ar.haigaiapp.cn

[R79] 解析命令行选项
来源：http://lu.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://re.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://uh.szsharing.cn

time ./run.sh
来源：http://rr.lnxyls.cn

================================================================================
来源：http://as.nszjky.cn

S. C / C++ 专题
来源：http://eg.jctech888.com.cn

================================================================================
来源：http://gz.jianghongdianzi.cn

[S01] C：Hello World
来源：http://th.muxihuayi.cn

#include <stdio.h>
来源：http://dc.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gl.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://nu.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://ew.szsharing.cn

[S03] C：读入整数
来源：http://qk.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://dy.huixiangedu.cn

[S04] C：字符串复制
来源：http://cg.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rn.lnxyls.cn

[S05] C：字符串长度
来源：http://jg.yuexingan06.cn

strlen(s)
来源：http://tb.shtwfgs.cn

[S06] C：字符串比较
来源：http://pn.hahajie.cn

strcmp(a, b) == 0
来源：http://mw.nicolike.cn

[S07] C：数组遍历求和
来源：http://fc.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jw.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://ij.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rr.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://ov.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pf.yuexingan06.cn

[S10] C：指针与解引用
来源：http://wv.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://xl.shtwfgs.cn

[S11] C：逐行读文件
来源：http://mr.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://jn.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tr.huanxung.cn

fclose(f);
来源：http://jh.521024.cn

[S12] C：写文件
来源：http://xe.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wk.haigaiapp.cn

[S13] C：宏定义
来源：http://ma.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wc.hahajie.cn

[S14] C：枚举
来源：http://dr.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://yy.asd995.cn

[S15] C：类型转换
来源：http://nc.jctech888.com.cn

(double) a / b
来源：http://mq.nicolike.cn

[S16] C：位操作置位
来源：http://ko.521024.cn

x |= (1 << 3);
来源：http://ft.nszjky.cn

[S17] C：安全拼接字符串
来源：http://sv.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://up.nszjky.cn

[S18] C：命令行参数
来源：http://pl.asd995.cn

int main(int argc, char **argv)
来源：http://mx.bjjhwx.cn

[S19] C：快速排序
来源：http://hg.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oa.nicolike.cn

[S20] C：二分查找
来源：http://vg.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pt.hahajie.cn

[S21] C：字符类别判断
来源：http://ih.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ws.panjiajie.cn

[S22] C：字符串转数字
来源：http://xw.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://no.asd995.cn

[S23] C：随机数
来源：http://jw.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hj.huanxung.cn

[S24] C：获取本地时间
来源：http://ni.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ol.gzmigu.cn

[S25] C：内存拷贝
来源：http://cn.bjjhwx.cn

memcpy(dst, src, n);
来源：http://eq.9csxet.cn

[S26] C：内存清零
来源：http://dc.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://bw.hahajie.cn

[S27] C：定义常量
来源：http://li.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://wa.gzmigu.cn

[S28] C：静态变量
来源：http://ah.lnxyls.cn

static int counter = 0;
来源：http://qu.bookmarksfly.cn

[S29] C：变参函数
来源：http://ql.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kj.shxzskj.cn

[S30] C：头文件保护
来源：http://cs.nicolike.cn

#ifndef X_H
来源：http://fb.hnjuh.cn

#define X_H
来源：http://qx.shxzskj.cn

#endif
来源：http://mq.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://nq.haigaiapp.cn

#include <iostream>
来源：http://np.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ht.lnxyls.cn

[S32] C++：字符串
来源：http://ez.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://im.haigaiapp.cn

[S33] C++：vector 增删
来源：http://zy.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kw.nszjky.cn

[S34] C++：遍历 vector
来源：http://xo.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ti.lnxyls.cn

[S35] C++：map
来源：http://gx.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yp.chemitech.net.cn

[S36] C++：unordered_map
来源：http://am.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qo.lnxyls.cn

[S37] C++：set
来源：http://mn.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hi.yuntaijiaju.cn

[S38] C++：排序
来源：http://nk.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://kl.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://az.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fs.panjiajie.cn

[S40] C++：查找元素
来源：http://wg.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kb.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://py.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xr.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://oc.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://na.hnjuh.cn

[S43] C++：智能指针
来源：http://rz.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://du.bookmarksfly.cn

[S44] C++：引用传参
来源：http://dl.szsharing.cn

void inc(int &x) { ++x; }
来源：http://bl.newstarts.cn

[S45] C++：lambda
来源：http://wn.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nn.9csxet.cn

[S46] C++：函数模板
来源：http://hd.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oy.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://ev.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dw.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://ht.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kw.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://mi.gzmigu.cn

[S49] C++：写文件
来源：http://uh.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ci.shxzskj.cn

[S50] C++：格式化数字
来源：http://bg.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lz.shxzukj.cn

[S51] C++：显式类型转换
来源：http://dc.jctech888.com.cn

static_cast<double>(a) / b
来源：http://bj.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://xp.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://ao.szxytkj.cn

[S53] C++：移动语义
来源：http://qz.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://of.nicolike.cn

[S54] C++：异常处理
来源：http://ea.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ka.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://rk.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yf.wgjwhj.cn

[S56] C++：optional
来源：http://we.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://td.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://xn.521024.cn

constexpr int N = 10;
来源：http://aj.bookmarksfly.cn

[S58] C++：命名空间
来源：http://jo.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://vy.chemitech.net.cn

[S59] C++：静态断言
来源：http://by.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://em.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://un.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qb.shxzukj.cn

================================================================================
来源：http://rs.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pt.asd995.cn

================================================================================
来源：http://bb.nszjky.cn

[T01] Kotlin：Hello World
来源：http://qj.yuexingan06.cn

println("Hello")
来源：http://br.muxihuayi.cn

[T02] Kotlin：变量
来源：http://qo.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bh.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://ws.wgjwhj.cn

"值: $b"
来源：http://wu.colortex.cn

[T04] Kotlin：空安全
来源：http://dg.9csxet.cn

val n: String? = null;  n?.length
来源：http://qw.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://az.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tb.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://zl.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://he.521024.cn

[T07] Kotlin：集合过滤
来源：http://vi.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ug.szxytkj.cn

[T08] Kotlin：数据类
来源：http://ac.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ln.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://na.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://ji.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://lv.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ew.wgjwhj.cn

[T11] Kotlin：协程
来源：http://jk.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sl.newstarts.cn

[T12] Kotlin：解构声明
来源：http://xz.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://bw.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://kb.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://ot.chemitech.net.cn

[T14] Kotlin：循环
来源：http://jo.521024.cn

for (i in 1..10) println(i)
来源：http://he.hahajie.cn

[T15] Kotlin：接口
来源：http://yj.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://om.haigaiapp.cn

[T16] Swift：Hello World
来源：http://be.szsharing.cn

print("Hello")
来源：http://wt.nicolike.cn

[T17] Swift：变量与常量
来源：http://at.shxzukj.cn

var a = 1;  let b = 2
来源：http://ts.shxzukj.cn

[T18] Swift：字符串插值
来源：http://be.nszjky.cn

"值: \(b)"
来源：http://ev.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://ki.chemitech.net.cn

if let n = opt { print(n) }
来源：http://rm.newstarts.cn

[T20] Swift：数组操作
来源：http://pg.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fq.huixiangedu.cn

[T21] Swift：遍历
来源：http://ve.haigaiapp.cn

for x in a { print(x) }
来源：http://ic.9csxet.cn

[T22] Swift：字典
来源：http://va.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://io.yuexingan06.cn

[T23] Swift：函数
来源：http://qa.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fg.yuexingan06.cn

[T24] Swift：闭包
来源：http://cd.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gg.yuexingan06.cn

[T25] Swift：结构体
来源：http://bz.9csxet.cn

struct P { var x: Int }
来源：http://ws.shxzskj.cn

[T26] Swift：类与重写
来源：http://ej.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://bh.panjiajie.cn

[T27] Swift：错误处理
来源：http://bu.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://kn.hahajie.cn

[T28] Swift：枚举
来源：http://lo.szsharing.cn

enum Color { case red, green }
来源：http://cv.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://pn.newstarts.cn

guard let x = opt else { return }
来源：http://zc.wgjwhj.cn

[T30] Swift：协议
来源：http://kk.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://zv.huixiangedu.cn

[T31] Lua：Hello World
来源：http://xd.hnjuh.cn

print("Hello")
来源：http://et.hnjuh.cn

[T32] Lua：局部变量
来源：http://xh.chemitech.net.cn

local a = 1
来源：http://dt.gzmigu.cn

[T33] Lua：表（数组）
来源：http://ly.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nm.huixiangedu.cn

[T34] Lua：遍历表
来源：http://mc.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sa.panjiajie.cn

[T35] Lua：字典表
来源：http://uq.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://ou.wgjwhj.cn

[T36] Lua：函数
来源：http://yv.asd995.cn

function add(a, b) return a + b end
来源：http://ri.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://dj.lnxyls.cn

"a" .. "b"
来源：http://cm.shxzskj.cn

[T38] Lua：条件
来源：http://rs.yuexingan06.cn

if x > 0 then print("正") end
来源：http://oa.shxzukj.cn

[T39] Lua：模式匹配
来源：http://pv.szsharing.cn

string.find(s, "%d+")
来源：http://it.asd995.cn

[T40] Lua：元表
来源：http://qh.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://jp.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://fj.yuexingan06.cn

print "Hello\n";
来源：http://ja.asd995.cn

[T42] Perl：变量类型
来源：http://ve.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mr.9csxet.cn

[T43] Perl：字符串插值
来源：http://yx.haigaiapp.cn

"值: $a"
来源：http://pl.shtwfgs.cn

[T44] Perl：条件
来源：http://lw.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://zt.hahajie.cn

[T45] Perl：数组遍历
来源：http://nz.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ph.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://js.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iv.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://wi.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bx.9csxet.cn

[T48] Perl：正则替换
来源：http://sn.lnxyls.cn

$s =~ s/old/new/g;
来源：http://uv.bjjhwx.cn

[T49] Perl：函数
来源：http://by.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yl.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://dh.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ho.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://bz.newstarts.cn

[T51] Scala：Hello World
来源：http://np.lnxyls.cn

println("Hello")
来源：http://pv.newstarts.cn

[T52] Scala：变量
来源：http://va.hnjuh.cn

val a = 1;  var b = 2
来源：http://wa.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://kp.haigaiapp.cn

s"值: $b"
来源：http://yr.jctech888.com.cn

[T54] Scala：集合映射
来源：http://xu.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://dn.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://wv.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ia.521024.cn

[T56] Scala：样例类
来源：http://zf.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://pt.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://xa.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hf.hnjuh.cn

[T58] Scala：函数定义
来源：http://nm.wgjwhj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nd.shxzskj.cn

[T59] Scala：循环
来源：http://se.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://fb.521024.cn

[T60] Scala：折叠
来源：http://hh.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wv.hahajie.cn

================================================================================
来源：http://jt.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sb.bjjhwx.cn

================================================================================
来源：http://wl.9csxet.cn


<!-- 参考信息 -->