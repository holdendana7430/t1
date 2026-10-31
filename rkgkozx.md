代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uj.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://fn.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vu.huixiangedu.cn

[R61] 磁盘占用
来源：http://db.shxzskj.cn

df -h;  du -sh *
来源：http://lx.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://yu.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://bm.huixinmuqiang.cn

[R63] 内存与进程
来源：http://ye.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://wu.huanxung.cn

[R64] 结束进程
来源：http://vb.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://hx.muxihuayi.cn

[R65] 查看端口占用
来源：http://to.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iq.521024.cn

[R66] 定时任务
来源：http://hb.yuexingan06.cn

crontab -e;  crontab -l
来源：http://lo.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://rj.huixiangedu.cn

openssl rand -hex 16
来源：http://ye.panjiajie.cn

[R68] 计算文件校验值
来源：http://wk.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yy.hahajie.cn

[R69] 生成随机密码
来源：http://db.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://fn.jctech888.com.cn

[R70] 时间戳与互转
来源：http://rn.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ty.huixiangedu.cn

[R71] 日期格式化
来源：http://sv.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mf.9csxet.cn

[R72] 等待端口就绪
来源：http://wl.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cx.huixiangedu.cn

[R73] 分割大日志
来源：http://vk.szsharing.cn

split -l 1000 big.log part_
来源：http://ta.wgjwhj.cn

[R74] 批量重命名
来源：http://cb.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://km.haigaiapp.cn

[R75] 导出环境变量
来源：http://tp.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://oa.bookmarksfly.cn

[R76] 使用临时文件
来源：http://rr.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qs.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://rq.szsharing.cn

read -rp "请输入: " ans
来源：http://wr.hnjuh.cn

[R78] 交互式菜单
来源：http://ok.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vy.jctech888.com.cn

[R79] 解析命令行选项
来源：http://ro.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ml.asd995.cn

[R80] 查看脚本执行耗时
来源：http://mw.muxihuayi.cn

time ./run.sh
来源：http://eq.nicolike.cn

================================================================================
来源：http://of.asd995.cn

S. C / C++ 专题
来源：http://ps.newstarts.cn

================================================================================
来源：http://gn.asd995.cn

[S01] C：Hello World
来源：http://se.newstarts.cn

#include <stdio.h>
来源：http://cj.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://go.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://hw.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://ot.521024.cn

[S03] C：读入整数
来源：http://ng.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://gv.colortex.cn

[S04] C：字符串复制
来源：http://nx.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cw.panjiajie.cn

[S05] C：字符串长度
来源：http://kx.huixinmuqiang.cn

strlen(s)
来源：http://jh.shtwfgs.cn

[S06] C：字符串比较
来源：http://yw.asd995.cn

strcmp(a, b) == 0
来源：http://rx.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://ze.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bt.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://oa.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zw.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://mu.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jt.hnjuh.cn

[S10] C：指针与解引用
来源：http://ye.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://co.asd995.cn

[S11] C：逐行读文件
来源：http://hc.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://jv.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dd.huixiangedu.cn

fclose(f);
来源：http://nm.nicolike.cn

[S12] C：写文件
来源：http://qb.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gc.wgjwhj.cn

[S13] C：宏定义
来源：http://sg.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tj.nszjky.cn

[S14] C：枚举
来源：http://dh.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://kp.muxihuayi.cn

[S15] C：类型转换
来源：http://my.521024.cn

(double) a / b
来源：http://du.jctech888.com.cn

[S16] C：位操作置位
来源：http://nf.gzmigu.cn

x |= (1 << 3);
来源：http://rz.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://it.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vp.wgjwhj.cn

[S18] C：命令行参数
来源：http://bi.hnjuh.cn

int main(int argc, char **argv)
来源：http://rl.9csxet.cn

[S19] C：快速排序
来源：http://hm.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cv.huixiangedu.cn

[S20] C：二分查找
来源：http://aa.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://im.haigaiapp.cn

[S21] C：字符类别判断
来源：http://iz.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cu.521024.cn

[S22] C：字符串转数字
来源：http://pt.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vu.shxzukj.cn

[S23] C：随机数
来源：http://gt.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zi.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://fi.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sk.chemitech.net.cn

[S25] C：内存拷贝
来源：http://qs.muxihuayi.cn

memcpy(dst, src, n);
来源：http://hc.szsharing.cn

[S26] C：内存清零
来源：http://ze.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://hu.lnxyls.cn

[S27] C：定义常量
来源：http://fe.bjjhwx.cn

const double PI = 3.14159;
来源：http://xg.huanxung.cn

[S28] C：静态变量
来源：http://jq.shxzukj.cn

static int counter = 0;
来源：http://ah.szxytkj.cn

[S29] C：变参函数
来源：http://vm.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gh.hnjuh.cn

[S30] C：头文件保护
来源：http://po.huanxung.cn

#ifndef X_H
来源：http://xn.hnjuh.cn

#define X_H
来源：http://yn.9csxet.cn

#endif
来源：http://mu.shxzukj.cn

[S31] C++：Hello World
来源：http://ty.gzmigu.cn

#include <iostream>
来源：http://cu.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://oo.haigaiapp.cn

[S32] C++：字符串
来源：http://qw.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://ty.hahajie.cn

[S33] C++：vector 增删
来源：http://ye.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mp.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://xl.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://kp.bjjhwx.cn

[S35] C++：map
来源：http://sh.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pn.newstarts.cn

[S36] C++：unordered_map
来源：http://qq.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tx.nszjky.cn

[S37] C++：set
来源：http://oz.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cc.yuntaijiaju.cn

[S38] C++：排序
来源：http://hi.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://ca.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://yw.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qf.szsharing.cn

[S40] C++：查找元素
来源：http://yy.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ag.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://bq.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mo.hahajie.cn

[S42] C++：继承与虚函数
来源：http://mq.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://my.haigaiapp.cn

[S43] C++：智能指针
来源：http://ia.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://bn.gzmigu.cn

[S44] C++：引用传参
来源：http://bg.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://cn.wgjwhj.cn

[S45] C++：lambda
来源：http://wo.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xc.shxzskj.cn

[S46] C++：函数模板
来源：http://rj.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cc.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://zj.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yh.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://og.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gn.nicolike.cn

while (std::getline(in, line)) { }
来源：http://gp.szsharing.cn

[S49] C++：写文件
来源：http://lq.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qc.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ao.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ao.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://hj.chemitech.net.cn

static_cast<double>(a) / b
来源：http://ql.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://gs.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://fq.yuexingan06.cn

[S53] C++：移动语义
来源：http://se.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://un.jctech888.com.cn

[S54] C++：异常处理
来源：http://ft.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://me.huanxung.cn

[S55] C++：结构化绑定
来源：http://it.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vi.bjjhwx.cn

[S56] C++：optional
来源：http://qz.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wp.bjjhwx.cn

[S57] C++：编译期常量
来源：http://hb.wgjwhj.cn

constexpr int N = 10;
来源：http://io.newstarts.cn

[S58] C++：命名空间
来源：http://po.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://iu.shxzskj.cn

[S59] C++：静态断言
来源：http://fc.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oi.colortex.cn

[S60] C++：遍历并删除元素
来源：http://kk.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kk.shxzskj.cn

================================================================================
来源：http://dk.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hb.huanxung.cn

================================================================================
来源：http://fj.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://td.huanxung.cn

println("Hello")
来源：http://ah.hahajie.cn

[T02] Kotlin：变量
来源：http://ep.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ot.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://kt.colortex.cn

"值: $b"
来源：http://bb.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://pd.asd995.cn

val n: String? = null;  n?.length
来源：http://jf.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://zo.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zu.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://ed.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ys.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://dg.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eb.nicolike.cn

[T08] Kotlin：数据类
来源：http://cd.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ix.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://rq.521024.cn

fun String.exclaim() = this + "!"
来源：http://ga.nicolike.cn

[T10] Kotlin：默认参数
来源：http://cq.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mt.shtwfgs.cn

[T11] Kotlin：协程
来源：http://fh.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sl.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://nw.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://fc.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://jj.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://hs.huanxung.cn

[T14] Kotlin：循环
来源：http://pd.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://wd.521024.cn

[T15] Kotlin：接口
来源：http://zr.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://yo.szxytkj.cn

[T16] Swift：Hello World
来源：http://ea.shtwfgs.cn

print("Hello")
来源：http://se.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://gt.chemitech.net.cn

var a = 1;  let b = 2
来源：http://mj.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://jy.521024.cn

"值: \(b)"
来源：http://ta.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://ma.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://yq.nicolike.cn

[T20] Swift：数组操作
来源：http://sj.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ey.colortex.cn

[T21] Swift：遍历
来源：http://zd.shxzukj.cn

for x in a { print(x) }
来源：http://sm.nicolike.cn

[T22] Swift：字典
来源：http://vy.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sy.shtwfgs.cn

[T23] Swift：函数
来源：http://qn.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dy.szsharing.cn

[T24] Swift：闭包
来源：http://oo.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://io.hahajie.cn

[T25] Swift：结构体
来源：http://ut.jianghongdianzi.cn

struct P { var x: Int }
来源：http://xm.9csxet.cn

[T26] Swift：类与重写
来源：http://bh.shxzskj.cn

class A: Base { override func f() {} }
来源：http://sm.shxzukj.cn

[T27] Swift：错误处理
来源：http://te.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://qu.muxihuayi.cn

[T28] Swift：枚举
来源：http://pb.jctech888.com.cn

enum Color { case red, green }
来源：http://qj.colortex.cn

[T29] Swift：guard 提前返回
来源：http://mr.lnxyls.cn

guard let x = opt else { return }
来源：http://qt.yuntaijiaju.cn

[T30] Swift：协议
来源：http://fw.colortex.cn

protocol Shape { func area() -> Double }
来源：http://ys.shxzukj.cn

[T31] Lua：Hello World
来源：http://xf.jianghongdianzi.cn

print("Hello")
来源：http://dx.nszjky.cn

[T32] Lua：局部变量
来源：http://lv.hahajie.cn

local a = 1
来源：http://sl.huanxung.cn

[T33] Lua：表（数组）
来源：http://pa.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wk.lnxyls.cn

[T34] Lua：遍历表
来源：http://qi.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bc.bjjhwx.cn

[T35] Lua：字典表
来源：http://ym.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://ct.yuexingan06.cn

[T36] Lua：函数
来源：http://wh.newstarts.cn

function add(a, b) return a + b end
来源：http://zo.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://uy.hnjuh.cn

"a" .. "b"
来源：http://ko.gzmigu.cn

[T38] Lua：条件
来源：http://tt.hahajie.cn

if x > 0 then print("正") end
来源：http://mb.9csxet.cn

[T39] Lua：模式匹配
来源：http://lw.huanxung.cn

string.find(s, "%d+")
来源：http://rt.yuexingan06.cn

[T40] Lua：元表
来源：http://wq.huanxung.cn

setmetatable({}, { __index = base })
来源：http://ud.nszjky.cn

[T41] Perl：Hello World
来源：http://fe.shxzskj.cn

print "Hello\n";
来源：http://xm.nszjky.cn

[T42] Perl：变量类型
来源：http://kh.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uy.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://oc.yuexingan06.cn

"值: $a"
来源：http://zm.jctech888.com.cn

[T44] Perl：条件
来源：http://wm.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://xi.521024.cn

[T45] Perl：数组遍历
来源：http://lu.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://hf.colortex.cn

[T46] Perl：哈希操作
来源：http://da.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jk.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://yr.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qd.bjjhwx.cn

[T48] Perl：正则替换
来源：http://oy.shxzskj.cn

$s =~ s/old/new/g;
来源：http://xa.huanxung.cn

[T49] Perl：函数
来源：http://pi.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://go.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://jv.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wc.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://bd.gzmigu.cn

[T51] Scala：Hello World
来源：http://iq.colortex.cn

println("Hello")
来源：http://rz.szsharing.cn

[T52] Scala：变量
来源：http://sy.haigaiapp.cn

val a = 1;  var b = 2
来源：http://rh.shxzukj.cn

[T53] Scala：字符串插值
来源：http://ar.newstarts.cn

s"值: $b"
来源：http://ty.jctech888.com.cn

[T54] Scala：集合映射
来源：http://yq.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ax.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://zp.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nh.lnxyls.cn

[T56] Scala：样例类
来源：http://di.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://bv.nszjky.cn

[T57] Scala：模式匹配
来源：http://xr.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qt.nicolike.cn

[T58] Scala：函数定义
来源：http://ul.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://om.521024.cn

[T59] Scala：循环
来源：http://ro.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://cw.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://pb.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://du.shtwfgs.cn

================================================================================
来源：http://vh.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oa.szxytkj.cn

================================================================================
来源：http://pw.huixinmuqiang.cn


<!-- 参考信息 -->