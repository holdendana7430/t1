代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ey.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://fi.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cd.yuexingan06.cn

[R61] 磁盘占用
来源：http://ok.hahajie.cn

df -h;  du -sh *
来源：http://jp.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ak.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://fv.szsharing.cn

[R63] 内存与进程
来源：http://bb.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://id.nicolike.cn

[R64] 结束进程
来源：http://oq.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://dk.521024.cn

[R65] 查看端口占用
来源：http://ls.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dr.jctech888.com.cn

[R66] 定时任务
来源：http://ja.521024.cn

crontab -e;  crontab -l
来源：http://jx.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://yk.huanxung.cn

openssl rand -hex 16
来源：http://go.szsharing.cn

[R68] 计算文件校验值
来源：http://yb.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ko.huixiangedu.cn

[R69] 生成随机密码
来源：http://ce.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://os.shxzukj.cn

[R70] 时间戳与互转
来源：http://wu.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://pp.gzmigu.cn

[R71] 日期格式化
来源：http://hc.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lj.nszjky.cn

[R72] 等待端口就绪
来源：http://os.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nx.szxytkj.cn

[R73] 分割大日志
来源：http://mf.muxihuayi.cn

split -l 1000 big.log part_
来源：http://ol.nicolike.cn

[R74] 批量重命名
来源：http://cs.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yi.muxihuayi.cn

[R75] 导出环境变量
来源：http://jg.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://bn.9csxet.cn

[R76] 使用临时文件
来源：http://hy.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nj.haigaiapp.cn

[R77] 读取用户输入
来源：http://jz.nicolike.cn

read -rp "请输入: " ans
来源：http://mi.9csxet.cn

[R78] 交互式菜单
来源：http://bj.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rk.panjiajie.cn

[R79] 解析命令行选项
来源：http://he.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fj.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://yg.hnjuh.cn

time ./run.sh
来源：http://mb.hnjuh.cn

================================================================================
来源：http://la.colortex.cn

S. C / C++ 专题
来源：http://yi.muxihuayi.cn

================================================================================
来源：http://hv.hahajie.cn

[S01] C：Hello World
来源：http://ih.hahajie.cn

#include <stdio.h>
来源：http://bq.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tt.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://wg.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://uh.nicolike.cn

[S03] C：读入整数
来源：http://ai.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://zc.huixiangedu.cn

[S04] C：字符串复制
来源：http://cb.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kt.haigaiapp.cn

[S05] C：字符串长度
来源：http://dd.gzmigu.cn

strlen(s)
来源：http://mo.szxytkj.cn

[S06] C：字符串比较
来源：http://ge.hahajie.cn

strcmp(a, b) == 0
来源：http://cy.nicolike.cn

[S07] C：数组遍历求和
来源：http://ls.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bj.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://sx.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nf.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://nq.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wk.shxzukj.cn

[S10] C：指针与解引用
来源：http://bj.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://yx.newstarts.cn

[S11] C：逐行读文件
来源：http://hj.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://rd.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://me.jctech888.com.cn

fclose(f);
来源：http://kk.huixinmuqiang.cn

[S12] C：写文件
来源：http://hw.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wi.jianghongdianzi.cn

[S13] C：宏定义
来源：http://fh.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wl.hahajie.cn

[S14] C：枚举
来源：http://kv.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://af.muxihuayi.cn

[S15] C：类型转换
来源：http://pa.jianghongdianzi.cn

(double) a / b
来源：http://rb.gzmigu.cn

[S16] C：位操作置位
来源：http://eu.nicolike.cn

x |= (1 << 3);
来源：http://du.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://bw.haigaiapp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rq.yuexingan06.cn

[S18] C：命令行参数
来源：http://bn.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://yi.colortex.cn

[S19] C：快速排序
来源：http://nz.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mi.hahajie.cn

[S20] C：二分查找
来源：http://te.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xi.szsharing.cn

[S21] C：字符类别判断
来源：http://ud.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nb.chemitech.net.cn

[S22] C：字符串转数字
来源：http://uu.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://da.yuexingan06.cn

[S23] C：随机数
来源：http://xz.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ng.colortex.cn

[S24] C：获取本地时间
来源：http://iv.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pl.9csxet.cn

[S25] C：内存拷贝
来源：http://gh.shxzukj.cn

memcpy(dst, src, n);
来源：http://yg.wgjwhj.cn

[S26] C：内存清零
来源：http://ao.newstarts.cn

memset(a, 0, sizeof a);
来源：http://se.nicolike.cn

[S27] C：定义常量
来源：http://pm.shxzskj.cn

const double PI = 3.14159;
来源：http://ze.szsharing.cn

[S28] C：静态变量
来源：http://rw.bjjhwx.cn

static int counter = 0;
来源：http://mg.9csxet.cn

[S29] C：变参函数
来源：http://xz.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://no.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://jy.521024.cn

#ifndef X_H
来源：http://mx.shtwfgs.cn

#define X_H
来源：http://gn.shtwfgs.cn

#endif
来源：http://nv.huanxung.cn

[S31] C++：Hello World
来源：http://aw.huixinmuqiang.cn

#include <iostream>
来源：http://rr.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://br.chemitech.net.cn

[S32] C++：字符串
来源：http://dy.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://uw.nszjky.cn

[S33] C++：vector 增删
来源：http://yf.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fd.panjiajie.cn

[S34] C++：遍历 vector
来源：http://ui.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://rv.nicolike.cn

[S35] C++：map
来源：http://ki.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tz.shxzskj.cn

[S36] C++：unordered_map
来源：http://au.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ef.hnjuh.cn

[S37] C++：set
来源：http://xs.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ar.szxytkj.cn

[S38] C++：排序
来源：http://lg.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://xh.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://pm.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eb.nicolike.cn

[S40] C++：查找元素
来源：http://kd.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ak.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://ii.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qp.newstarts.cn

[S42] C++：继承与虚函数
来源：http://fb.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://ca.wgjwhj.cn

[S43] C++：智能指针
来源：http://pp.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://te.wgjwhj.cn

[S44] C++：引用传参
来源：http://qd.huanxung.cn

void inc(int &x) { ++x; }
来源：http://yo.nicolike.cn

[S45] C++：lambda
来源：http://yl.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sj.yuexingan06.cn

[S46] C++：函数模板
来源：http://xg.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mc.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://ka.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pa.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://st.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cs.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://un.huanxung.cn

[S49] C++：写文件
来源：http://ho.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tg.muxihuayi.cn

[S50] C++：格式化数字
来源：http://zm.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ax.lnxyls.cn

[S51] C++：显式类型转换
来源：http://uu.huixiangedu.cn

static_cast<double>(a) / b
来源：http://vz.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://gw.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://fd.newstarts.cn

[S53] C++：移动语义
来源：http://gn.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://xl.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://rr.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zr.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://ds.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bi.lnxyls.cn

[S56] C++：optional
来源：http://zl.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mf.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://rx.lnxyls.cn

constexpr int N = 10;
来源：http://yx.haigaiapp.cn

[S58] C++：命名空间
来源：http://dz.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://yg.shtwfgs.cn

[S59] C++：静态断言
来源：http://iz.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vz.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://wv.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sr.huanxung.cn

================================================================================
来源：http://vm.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xr.szsharing.cn

================================================================================
来源：http://rl.9csxet.cn

[T01] Kotlin：Hello World
来源：http://as.9csxet.cn

println("Hello")
来源：http://yq.haigaiapp.cn

[T02] Kotlin：变量
来源：http://oi.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yv.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://ry.gzmigu.cn

"值: $b"
来源：http://bq.shxzukj.cn

[T04] Kotlin：空安全
来源：http://be.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://ei.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://mi.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ne.asd995.cn

[T06] Kotlin：集合映射
来源：http://cs.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mo.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://ty.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vf.szxytkj.cn

[T08] Kotlin：数据类
来源：http://ih.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://qj.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://os.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ps.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://bk.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nw.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://wh.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ee.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://qy.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://uo.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://hn.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://wu.newstarts.cn

[T14] Kotlin：循环
来源：http://se.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://jt.shtwfgs.cn

[T15] Kotlin：接口
来源：http://te.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://ba.lnxyls.cn

[T16] Swift：Hello World
来源：http://kr.nicolike.cn

print("Hello")
来源：http://ju.hnjuh.cn

[T17] Swift：变量与常量
来源：http://ul.bjjhwx.cn

var a = 1;  let b = 2
来源：http://ln.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://nv.asd995.cn

"值: \(b)"
来源：http://bc.panjiajie.cn

[T19] Swift：可选绑定
来源：http://bz.shxzukj.cn

if let n = opt { print(n) }
来源：http://pc.nicolike.cn

[T20] Swift：数组操作
来源：http://tx.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zz.lnxyls.cn

[T21] Swift：遍历
来源：http://iz.chemitech.net.cn

for x in a { print(x) }
来源：http://pr.muxihuayi.cn

[T22] Swift：字典
来源：http://aj.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rf.haigaiapp.cn

[T23] Swift：函数
来源：http://pw.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ke.szxytkj.cn

[T24] Swift：闭包
来源：http://sc.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mw.huixiangedu.cn

[T25] Swift：结构体
来源：http://in.newstarts.cn

struct P { var x: Int }
来源：http://lt.muxihuayi.cn

[T26] Swift：类与重写
来源：http://cs.szxytkj.cn

class A: Base { override func f() {} }
来源：http://ko.colortex.cn

[T27] Swift：错误处理
来源：http://tb.9csxet.cn

do { try f() } catch { print(error) }
来源：http://qx.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://cl.yuexingan06.cn

enum Color { case red, green }
来源：http://sw.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://ma.9csxet.cn

guard let x = opt else { return }
来源：http://bq.colortex.cn

[T30] Swift：协议
来源：http://of.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://vc.nszjky.cn

[T31] Lua：Hello World
来源：http://xv.muxihuayi.cn

print("Hello")
来源：http://jp.huanxung.cn

[T32] Lua：局部变量
来源：http://oz.shxzskj.cn

local a = 1
来源：http://xl.huanxung.cn

[T33] Lua：表（数组）
来源：http://lf.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ny.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://jj.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yp.bookmarksfly.cn

[T35] Lua：字典表
来源：http://mu.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://fl.wgjwhj.cn

[T36] Lua：函数
来源：http://ee.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://jj.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://za.chemitech.net.cn

"a" .. "b"
来源：http://ql.huixinmuqiang.cn

[T38] Lua：条件
来源：http://ut.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://bl.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://xr.chemitech.net.cn

string.find(s, "%d+")
来源：http://tl.bjjhwx.cn

[T40] Lua：元表
来源：http://dd.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://rg.colortex.cn

[T41] Perl：Hello World
来源：http://zw.asd995.cn

print "Hello\n";
来源：http://da.asd995.cn

[T42] Perl：变量类型
来源：http://tu.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wc.colortex.cn

[T43] Perl：字符串插值
来源：http://oj.huanxung.cn

"值: $a"
来源：http://le.asd995.cn

[T44] Perl：条件
来源：http://ua.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://nk.nszjky.cn

[T45] Perl：数组遍历
来源：http://uw.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://cv.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://ho.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tr.gzmigu.cn

[T47] Perl：正则捕获
来源：http://iu.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bo.szxytkj.cn

[T48] Perl：正则替换
来源：http://ul.szsharing.cn

$s =~ s/old/new/g;
来源：http://hn.huixiangedu.cn

[T49] Perl：函数
来源：http://op.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://um.huanxung.cn

[T50] Perl：逐行读文件
来源：http://ot.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ie.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://pu.szsharing.cn

[T51] Scala：Hello World
来源：http://vn.lnxyls.cn

println("Hello")
来源：http://zx.nszjky.cn

[T52] Scala：变量
来源：http://fo.huixiangedu.cn

val a = 1;  var b = 2
来源：http://rk.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://dx.wgjwhj.cn

s"值: $b"
来源：http://do.hahajie.cn

[T54] Scala：集合映射
来源：http://ri.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://td.9csxet.cn

[T55] Scala：集合过滤
来源：http://wx.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bt.huixiangedu.cn

[T56] Scala：样例类
来源：http://ii.huanxung.cn

case class User(name: String, age: Int)
来源：http://uw.9csxet.cn

[T57] Scala：模式匹配
来源：http://bh.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://do.lnxyls.cn

[T58] Scala：函数定义
来源：http://ov.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ez.shxzukj.cn

[T59] Scala：循环
来源：http://vf.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://vs.haigaiapp.cn

[T60] Scala：折叠
来源：http://kn.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ug.jctech888.com.cn

================================================================================
来源：http://oi.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cb.haigaiapp.cn

================================================================================
来源：http://hz.chemitech.net.cn


<!-- 参考信息 -->