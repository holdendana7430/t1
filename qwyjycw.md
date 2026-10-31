代发 wailian999

df -h;  du -sh *
来源：http://xw.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://at.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://hs.bookmarksfly.cn

[R63] 内存与进程
来源：http://xx.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://yx.jctech888.com.cn

[R64] 结束进程
来源：http://jn.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://tc.nicolike.cn

[R65] 查看端口占用
来源：http://sj.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fp.shxzskj.cn

[R66] 定时任务
来源：http://wy.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://et.colortex.cn

[R67] 生成随机十六进制串
来源：http://yn.shtwfgs.cn

openssl rand -hex 16
来源：http://oy.shxzukj.cn

[R68] 计算文件校验值
来源：http://mg.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nr.chemitech.net.cn

[R69] 生成随机密码
来源：http://eb.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://hv.newstarts.cn

[R70] 时间戳与互转
来源：http://wr.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://fb.haigaiapp.cn

[R71] 日期格式化
来源：http://qx.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hw.huanxung.cn

[R72] 等待端口就绪
来源：http://sg.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xo.wgjwhj.cn

[R73] 分割大日志
来源：http://dy.haigaiapp.cn

split -l 1000 big.log part_
来源：http://bk.hahajie.cn

[R74] 批量重命名
来源：http://dj.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rv.hahajie.cn

[R75] 导出环境变量
来源：http://qg.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://ls.szxytkj.cn

[R76] 使用临时文件
来源：http://mw.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zw.asd995.cn

[R77] 读取用户输入
来源：http://vq.shxzskj.cn

read -rp "请输入: " ans
来源：http://uw.lnxyls.cn

[R78] 交互式菜单
来源：http://bd.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kj.chemitech.net.cn

[R79] 解析命令行选项
来源：http://ak.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ia.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://rg.wgjwhj.cn

time ./run.sh
来源：http://zm.chemitech.net.cn

================================================================================
来源：http://gg.wgjwhj.cn

S. C / C++ 专题
来源：http://go.huanxung.cn

================================================================================
来源：http://qe.yuexingan06.cn

[S01] C：Hello World
来源：http://dw.newstarts.cn

#include <stdio.h>
来源：http://ru.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://js.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://fh.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://kr.bookmarksfly.cn

[S03] C：读入整数
来源：http://fc.lnxyls.cn

int x; scanf("%d", &x);
来源：http://kx.shtwfgs.cn

[S04] C：字符串复制
来源：http://xf.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yy.newstarts.cn

[S05] C：字符串长度
来源：http://nd.haigaiapp.cn

strlen(s)
来源：http://mu.wgjwhj.cn

[S06] C：字符串比较
来源：http://kc.szsharing.cn

strcmp(a, b) == 0
来源：http://sw.newstarts.cn

[S07] C：数组遍历求和
来源：http://jy.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qe.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://ci.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ax.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://hc.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fd.szsharing.cn

[S10] C：指针与解引用
来源：http://mw.asd995.cn

int *p = &a;  *p = 5;
来源：http://pj.hnjuh.cn

[S11] C：逐行读文件
来源：http://ws.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://lq.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bb.haigaiapp.cn

fclose(f);
来源：http://bi.shtwfgs.cn

[S12] C：写文件
来源：http://au.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fn.hnjuh.cn

[S13] C：宏定义
来源：http://us.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fv.panjiajie.cn

[S14] C：枚举
来源：http://um.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://lb.9csxet.cn

[S15] C：类型转换
来源：http://ko.bjjhwx.cn

(double) a / b
来源：http://mv.asd995.cn

[S16] C：位操作置位
来源：http://fo.nicolike.cn

x |= (1 << 3);
来源：http://ji.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://nq.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kj.chemitech.net.cn

[S18] C：命令行参数
来源：http://tc.muxihuayi.cn

int main(int argc, char **argv)
来源：http://zc.yuexingan06.cn

[S19] C：快速排序
来源：http://iz.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rx.szxytkj.cn

[S20] C：二分查找
来源：http://mh.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tp.panjiajie.cn

[S21] C：字符类别判断
来源：http://tz.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://of.wgjwhj.cn

[S22] C：字符串转数字
来源：http://wn.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gr.jianghongdianzi.cn

[S23] C：随机数
来源：http://wn.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wz.colortex.cn

[S24] C：获取本地时间
来源：http://kr.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mt.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://xz.hnjuh.cn

memcpy(dst, src, n);
来源：http://qd.9csxet.cn

[S26] C：内存清零
来源：http://bn.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://dt.nicolike.cn

[S27] C：定义常量
来源：http://lv.szxytkj.cn

const double PI = 3.14159;
来源：http://mh.lnxyls.cn

[S28] C：静态变量
来源：http://bs.huixiangedu.cn

static int counter = 0;
来源：http://jb.wgjwhj.cn

[S29] C：变参函数
来源：http://yo.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lt.panjiajie.cn

[S30] C：头文件保护
来源：http://dz.muxihuayi.cn

#ifndef X_H
来源：http://hn.jctech888.com.cn

#define X_H
来源：http://qd.nszjky.cn

#endif
来源：http://vx.nicolike.cn

[S31] C++：Hello World
来源：http://az.szxytkj.cn

#include <iostream>
来源：http://vv.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://qz.bjjhwx.cn

[S32] C++：字符串
来源：http://kf.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://gp.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://qf.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://co.huanxung.cn

[S34] C++：遍历 vector
来源：http://ag.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://th.chemitech.net.cn

[S35] C++：map
来源：http://rd.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pn.shxzskj.cn

[S36] C++：unordered_map
来源：http://nh.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tu.huanxung.cn

[S37] C++：set
来源：http://ma.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cu.szxytkj.cn

[S38] C++：排序
来源：http://ll.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://rf.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://nv.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://id.shxzukj.cn

[S40] C++：查找元素
来源：http://zm.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ol.colortex.cn

[S41] C++：类与构造函数
来源：http://rt.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://df.nicolike.cn

[S42] C++：继承与虚函数
来源：http://pc.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://jh.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://vu.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://vh.jctech888.com.cn

[S44] C++：引用传参
来源：http://ia.szsharing.cn

void inc(int &x) { ++x; }
来源：http://js.nszjky.cn

[S45] C++：lambda
来源：http://sc.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rg.chemitech.net.cn

[S46] C++：函数模板
来源：http://ge.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ia.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://cz.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gv.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ga.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://em.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://gf.huixiangedu.cn

[S49] C++：写文件
来源：http://mu.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zp.szxytkj.cn

[S50] C++：格式化数字
来源：http://bb.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qs.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://qg.colortex.cn

static_cast<double>(a) / b
来源：http://jt.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yi.huanxung.cn

int size() const noexcept { return n_; }
来源：http://qa.muxihuayi.cn

[S53] C++：移动语义
来源：http://ki.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://je.nszjky.cn

[S54] C++：异常处理
来源：http://ak.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uz.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://jy.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xl.hnjuh.cn

[S56] C++：optional
来源：http://cs.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sa.bjjhwx.cn

[S57] C++：编译期常量
来源：http://dg.asd995.cn

constexpr int N = 10;
来源：http://fc.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://pt.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://gs.jctech888.com.cn

[S59] C++：静态断言
来源：http://fx.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ua.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://nu.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ag.521024.cn

================================================================================
来源：http://ih.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ma.9csxet.cn

================================================================================
来源：http://xp.asd995.cn

[T01] Kotlin：Hello World
来源：http://js.chemitech.net.cn

println("Hello")
来源：http://xp.nszjky.cn

[T02] Kotlin：变量
来源：http://jh.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fh.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://qd.gzmigu.cn

"值: $b"
来源：http://yx.szsharing.cn

[T04] Kotlin：空安全
来源：http://bk.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://zv.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://uu.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wf.nicolike.cn

[T06] Kotlin：集合映射
来源：http://nt.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wf.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://vo.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wb.panjiajie.cn

[T08] Kotlin：数据类
来源：http://gg.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://dn.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://bo.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://so.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://bs.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iq.521024.cn

[T11] Kotlin：协程
来源：http://fi.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xr.asd995.cn

[T12] Kotlin：解构声明
来源：http://zf.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://kz.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://xe.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://cw.hnjuh.cn

[T14] Kotlin：循环
来源：http://jt.huanxung.cn

for (i in 1..10) println(i)
来源：http://lf.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://mt.newstarts.cn

interface Shape { fun area(): Double }
来源：http://lk.colortex.cn

[T16] Swift：Hello World
来源：http://jz.lnxyls.cn

print("Hello")
来源：http://bn.nszjky.cn

[T17] Swift：变量与常量
来源：http://bo.lnxyls.cn

var a = 1;  let b = 2
来源：http://ay.nszjky.cn

[T18] Swift：字符串插值
来源：http://fb.nszjky.cn

"值: \(b)"
来源：http://cd.szsharing.cn

[T19] Swift：可选绑定
来源：http://ko.shxzukj.cn

if let n = opt { print(n) }
来源：http://oc.9csxet.cn

[T20] Swift：数组操作
来源：http://af.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kh.szxytkj.cn

[T21] Swift：遍历
来源：http://em.jianghongdianzi.cn

for x in a { print(x) }
来源：http://bl.huanxung.cn

[T22] Swift：字典
来源：http://yt.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ek.yuexingan06.cn

[T23] Swift：函数
来源：http://oo.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ec.bjjhwx.cn

[T24] Swift：闭包
来源：http://kd.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ik.hahajie.cn

[T25] Swift：结构体
来源：http://cj.newstarts.cn

struct P { var x: Int }
来源：http://qi.haigaiapp.cn

[T26] Swift：类与重写
来源：http://xq.nicolike.cn

class A: Base { override func f() {} }
来源：http://br.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://st.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://et.panjiajie.cn

[T28] Swift：枚举
来源：http://vw.nszjky.cn

enum Color { case red, green }
来源：http://ew.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://ki.szxytkj.cn

guard let x = opt else { return }
来源：http://bs.gzmigu.cn

[T30] Swift：协议
来源：http://nb.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://xu.hnjuh.cn

[T31] Lua：Hello World
来源：http://kh.huixiangedu.cn

print("Hello")
来源：http://zh.nicolike.cn

[T32] Lua：局部变量
来源：http://yh.huanxung.cn

local a = 1
来源：http://nd.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://uw.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nk.asd995.cn

[T34] Lua：遍历表
来源：http://vc.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ur.gzmigu.cn

[T35] Lua：字典表
来源：http://xp.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://ur.jianghongdianzi.cn

[T36] Lua：函数
来源：http://cc.lnxyls.cn

function add(a, b) return a + b end
来源：http://mf.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://qp.bjjhwx.cn

"a" .. "b"
来源：http://xw.szxytkj.cn

[T38] Lua：条件
来源：http://vb.asd995.cn

if x > 0 then print("正") end
来源：http://gu.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://rq.huixiangedu.cn

string.find(s, "%d+")
来源：http://mf.colortex.cn

[T40] Lua：元表
来源：http://pg.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://xr.colortex.cn

[T41] Perl：Hello World
来源：http://nl.bookmarksfly.cn

print "Hello\n";
来源：http://hw.nicolike.cn

[T42] Perl：变量类型
来源：http://yz.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ls.asd995.cn

[T43] Perl：字符串插值
来源：http://pz.huanxung.cn

"值: $a"
来源：http://hu.lnxyls.cn

[T44] Perl：条件
来源：http://dt.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://xv.nicolike.cn

[T45] Perl：数组遍历
来源：http://ky.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://hv.newstarts.cn

[T46] Perl：哈希操作
来源：http://qg.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cg.hnjuh.cn

[T47] Perl：正则捕获
来源：http://tr.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dv.hnjuh.cn

[T48] Perl：正则替换
来源：http://os.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://fw.panjiajie.cn

[T49] Perl：函数
来源：http://yq.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fh.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://qf.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uj.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://on.lnxyls.cn

[T51] Scala：Hello World
来源：http://tr.szxytkj.cn

println("Hello")
来源：http://dw.jctech888.com.cn

[T52] Scala：变量
来源：http://ew.panjiajie.cn

val a = 1;  var b = 2
来源：http://av.nicolike.cn

[T53] Scala：字符串插值
来源：http://om.521024.cn

s"值: $b"
来源：http://ii.huixiangedu.cn

[T54] Scala：集合映射
来源：http://zu.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://uw.521024.cn

[T55] Scala：集合过滤
来源：http://ej.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzmigu.cn

[T56] Scala：样例类
来源：http://rh.521024.cn

case class User(name: String, age: Int)
来源：http://lr.panjiajie.cn

[T57] Scala：模式匹配
来源：http://ui.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hc.colortex.cn

[T58] Scala：函数定义
来源：http://lp.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yn.9csxet.cn

[T59] Scala：循环
来源：http://rc.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://cx.szxytkj.cn

[T60] Scala：折叠
来源：http://yn.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wj.jianghongdianzi.cn

================================================================================
来源：http://wj.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vh.haigaiapp.cn

================================================================================
来源：http://xa.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://og.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://np.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://zj.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ax.muxihuayi.cn


<!-- 参考信息 -->