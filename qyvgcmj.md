代发 wailian999

df -h;  du -sh *
来源：http://ff.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://on.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://jz.muxihuayi.cn

[R63] 内存与进程
来源：http://oa.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://kj.haigaiapp.cn

[R64] 结束进程
来源：http://yc.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://sp.shxzskj.cn

[R65] 查看端口占用
来源：http://rx.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cr.panjiajie.cn

[R66] 定时任务
来源：http://jv.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://bd.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://wz.newstarts.cn

openssl rand -hex 16
来源：http://za.shtwfgs.cn

[R68] 计算文件校验值
来源：http://kz.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ns.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://wp.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://yd.huixiangedu.cn

[R70] 时间戳与互转
来源：http://sm.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://mu.asd995.cn

[R71] 日期格式化
来源：http://vm.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vr.panjiajie.cn

[R72] 等待端口就绪
来源：http://ga.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://po.yuntaijiaju.cn

[R73] 分割大日志
来源：http://vk.newstarts.cn

split -l 1000 big.log part_
来源：http://mk.yuexingan06.cn

[R74] 批量重命名
来源：http://la.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://um.jctech888.com.cn

[R75] 导出环境变量
来源：http://ow.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://ek.shxzukj.cn

[R76] 使用临时文件
来源：http://la.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lc.shtwfgs.cn

[R77] 读取用户输入
来源：http://yl.huixiangedu.cn

read -rp "请输入: " ans
来源：http://sk.shtwfgs.cn

[R78] 交互式菜单
来源：http://hq.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://my.huanxung.cn

[R79] 解析命令行选项
来源：http://yk.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://py.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://on.jianghongdianzi.cn

time ./run.sh
来源：http://fo.jianghongdianzi.cn

================================================================================
来源：http://rt.hahajie.cn

S. C / C++ 专题
来源：http://at.shxzukj.cn

================================================================================
来源：http://qa.hnjuh.cn

[S01] C：Hello World
来源：http://fu.gzmigu.cn

#include <stdio.h>
来源：http://iz.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vk.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://di.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://qe.huanxung.cn

[S03] C：读入整数
来源：http://fn.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://ii.yuexingan06.cn

[S04] C：字符串复制
来源：http://bo.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gk.shxzukj.cn

[S05] C：字符串长度
来源：http://we.521024.cn

strlen(s)
来源：http://jl.521024.cn

[S06] C：字符串比较
来源：http://ex.shxzukj.cn

strcmp(a, b) == 0
来源：http://rb.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://pa.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xi.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://cc.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zl.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://au.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ic.9csxet.cn

[S10] C：指针与解引用
来源：http://cm.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://kz.gzmigu.cn

[S11] C：逐行读文件
来源：http://eh.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://vz.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yt.yuexingan06.cn

fclose(f);
来源：http://wk.nicolike.cn

[S12] C：写文件
来源：http://zl.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://md.asd995.cn

[S13] C：宏定义
来源：http://ro.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zq.huixinmuqiang.cn

[S14] C：枚举
来源：http://td.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://ed.haigaiapp.cn

[S15] C：类型转换
来源：http://nl.bjjhwx.cn

(double) a / b
来源：http://ex.szxytkj.cn

[S16] C：位操作置位
来源：http://jx.asd995.cn

x |= (1 << 3);
来源：http://be.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://la.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yo.hnjuh.cn

[S18] C：命令行参数
来源：http://hz.szxytkj.cn

int main(int argc, char **argv)
来源：http://xs.haigaiapp.cn

[S19] C：快速排序
来源：http://lf.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qg.jianghongdianzi.cn

[S20] C：二分查找
来源：http://kk.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://le.shtwfgs.cn

[S21] C：字符类别判断
来源：http://mx.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nv.bjjhwx.cn

[S22] C：字符串转数字
来源：http://dx.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://td.gzmigu.cn

[S23] C：随机数
来源：http://er.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gn.hnjuh.cn

[S24] C：获取本地时间
来源：http://fc.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rg.hnjuh.cn

[S25] C：内存拷贝
来源：http://xo.haigaiapp.cn

memcpy(dst, src, n);
来源：http://nj.chemitech.net.cn

[S26] C：内存清零
来源：http://ke.9csxet.cn

memset(a, 0, sizeof a);
来源：http://mn.huixiangedu.cn

[S27] C：定义常量
来源：http://nc.hahajie.cn

const double PI = 3.14159;
来源：http://le.yuntaijiaju.cn

[S28] C：静态变量
来源：http://qq.newstarts.cn

static int counter = 0;
来源：http://jp.muxihuayi.cn

[S29] C：变参函数
来源：http://wc.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://de.haigaiapp.cn

[S30] C：头文件保护
来源：http://jd.asd995.cn

#ifndef X_H
来源：http://cg.szxytkj.cn

#define X_H
来源：http://uv.lnxyls.cn

#endif
来源：http://iu.szsharing.cn

[S31] C++：Hello World
来源：http://ey.huixiangedu.cn

#include <iostream>
来源：http://yr.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://aw.gzmigu.cn

[S32] C++：字符串
来源：http://ne.colortex.cn

std::string s = "hi";  s += "!";
来源：http://sk.jctech888.com.cn

[S33] C++：vector 增删
来源：http://mo.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lw.nszjky.cn

[S34] C++：遍历 vector
来源：http://sx.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://si.shtwfgs.cn

[S35] C++：map
来源：http://nb.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fn.shtwfgs.cn

[S36] C++：unordered_map
来源：http://hb.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sw.lnxyls.cn

[S37] C++：set
来源：http://gz.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qr.haigaiapp.cn

[S38] C++：排序
来源：http://et.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://hn.521024.cn

[S39] C++：自定义比较器排序
来源：http://li.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uq.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ty.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mw.asd995.cn

[S41] C++：类与构造函数
来源：http://dp.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hj.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://yk.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://op.newstarts.cn

[S43] C++：智能指针
来源：http://tn.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://yd.asd995.cn

[S44] C++：引用传参
来源：http://yn.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://uw.hahajie.cn

[S45] C++：lambda
来源：http://cg.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://th.szsharing.cn

[S46] C++：函数模板
来源：http://au.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cu.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://qe.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://km.szsharing.cn

[S48] C++：逐行读文件
来源：http://py.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mp.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://pm.shxzukj.cn

[S49] C++：写文件
来源：http://ry.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ui.hahajie.cn

[S50] C++：格式化数字
来源：http://bq.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bf.shxzskj.cn

[S51] C++：显式类型转换
来源：http://vr.521024.cn

static_cast<double>(a) / b
来源：http://me.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://nt.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://kk.shxzukj.cn

[S53] C++：移动语义
来源：http://tp.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://cn.shxzskj.cn

[S54] C++：异常处理
来源：http://we.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nw.9csxet.cn

[S55] C++：结构化绑定
来源：http://hv.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ja.wgjwhj.cn

[S56] C++：optional
来源：http://zs.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vo.huanxung.cn

[S57] C++：编译期常量
来源：http://tb.jctech888.com.cn

constexpr int N = 10;
来源：http://rv.shtwfgs.cn

[S58] C++：命名空间
来源：http://qm.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://jc.jctech888.com.cn

[S59] C++：静态断言
来源：http://yd.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fv.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://to.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wg.chemitech.net.cn

================================================================================
来源：http://tn.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ef.huixinmuqiang.cn

================================================================================
来源：http://zt.9csxet.cn

[T01] Kotlin：Hello World
来源：http://gn.wgjwhj.cn

println("Hello")
来源：http://ia.chemitech.net.cn

[T02] Kotlin：变量
来源：http://on.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vw.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://wk.bjjhwx.cn

"值: $b"
来源：http://lc.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://pk.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://mn.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://cs.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fz.9csxet.cn

[T06] Kotlin：集合映射
来源：http://xh.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kx.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://zm.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yn.shxzukj.cn

[T08] Kotlin：数据类
来源：http://ec.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ab.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://ny.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://ye.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://ii.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vu.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://ps.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://to.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://cc.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://ui.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://fd.newstarts.cn

val m = mapOf("a" to 1)
来源：http://gr.huixiangedu.cn

[T14] Kotlin：循环
来源：http://hx.nszjky.cn

for (i in 1..10) println(i)
来源：http://pd.asd995.cn

[T15] Kotlin：接口
来源：http://uk.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://rv.yuexingan06.cn

[T16] Swift：Hello World
来源：http://pz.chemitech.net.cn

print("Hello")
来源：http://px.hnjuh.cn

[T17] Swift：变量与常量
来源：http://gj.nicolike.cn

var a = 1;  let b = 2
来源：http://nn.shxzskj.cn

[T18] Swift：字符串插值
来源：http://rm.panjiajie.cn

"值: \(b)"
来源：http://sm.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://so.nszjky.cn

if let n = opt { print(n) }
来源：http://cz.521024.cn

[T20] Swift：数组操作
来源：http://ie.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://us.shxzskj.cn

[T21] Swift：遍历
来源：http://nc.bjjhwx.cn

for x in a { print(x) }
来源：http://vd.haigaiapp.cn

[T22] Swift：字典
来源：http://br.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tn.huanxung.cn

[T23] Swift：函数
来源：http://wc.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yg.szsharing.cn

[T24] Swift：闭包
来源：http://tq.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vv.szsharing.cn

[T25] Swift：结构体
来源：http://ax.szxytkj.cn

struct P { var x: Int }
来源：http://ja.yuexingan06.cn

[T26] Swift：类与重写
来源：http://sk.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://cr.gzmigu.cn

[T27] Swift：错误处理
来源：http://il.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://ba.shxzskj.cn

[T28] Swift：枚举
来源：http://xd.colortex.cn

enum Color { case red, green }
来源：http://vr.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://co.nszjky.cn

guard let x = opt else { return }
来源：http://fp.shxzukj.cn

[T30] Swift：协议
来源：http://mu.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://am.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://tl.shxzskj.cn

print("Hello")
来源：http://uv.muxihuayi.cn

[T32] Lua：局部变量
来源：http://wj.huanxung.cn

local a = 1
来源：http://su.hnjuh.cn

[T33] Lua：表（数组）
来源：http://si.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vu.shxzskj.cn

[T34] Lua：遍历表
来源：http://nb.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ce.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ar.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://tc.colortex.cn

[T36] Lua：函数
来源：http://il.wgjwhj.cn

function add(a, b) return a + b end
来源：http://nd.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://tb.huixiangedu.cn

"a" .. "b"
来源：http://ns.muxihuayi.cn

[T38] Lua：条件
来源：http://rs.haigaiapp.cn

if x > 0 then print("正") end
来源：http://fk.newstarts.cn

[T39] Lua：模式匹配
来源：http://hy.panjiajie.cn

string.find(s, "%d+")
来源：http://pe.shxzskj.cn

[T40] Lua：元表
来源：http://yy.asd995.cn

setmetatable({}, { __index = base })
来源：http://wi.nszjky.cn

[T41] Perl：Hello World
来源：http://ot.9csxet.cn

print "Hello\n";
来源：http://fg.lnxyls.cn

[T42] Perl：变量类型
来源：http://cr.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qu.panjiajie.cn

[T43] Perl：字符串插值
来源：http://vi.bjjhwx.cn

"值: $a"
来源：http://gf.hahajie.cn

[T44] Perl：条件
来源：http://qm.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://zb.9csxet.cn

[T45] Perl：数组遍历
来源：http://jv.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://zs.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://hr.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://po.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://aj.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nx.nszjky.cn

[T48] Perl：正则替换
来源：http://jv.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://zw.jctech888.com.cn

[T49] Perl：函数
来源：http://kt.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vr.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://wx.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lp.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://xj.szxytkj.cn

[T51] Scala：Hello World
来源：http://ev.panjiajie.cn

println("Hello")
来源：http://ln.jianghongdianzi.cn

[T52] Scala：变量
来源：http://ju.nszjky.cn

val a = 1;  var b = 2
来源：http://cj.szxytkj.cn

[T53] Scala：字符串插值
来源：http://gk.hnjuh.cn

s"值: $b"
来源：http://ko.jctech888.com.cn

[T54] Scala：集合映射
来源：http://mz.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://mf.hnjuh.cn

[T55] Scala：集合过滤
来源：http://ki.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ed.chemitech.net.cn

[T56] Scala：样例类
来源：http://dx.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://vm.hahajie.cn

[T57] Scala：模式匹配
来源：http://iv.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tt.9csxet.cn

[T58] Scala：函数定义
来源：http://zw.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oi.colortex.cn

[T59] Scala：循环
来源：http://oi.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://vd.panjiajie.cn

[T60] Scala：折叠
来源：http://yn.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fo.9csxet.cn

================================================================================
来源：http://wt.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jk.szsharing.cn

================================================================================
来源：http://nn.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://cq.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kg.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://ob.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://co.bookmarksfly.cn


<!-- 参考信息 -->