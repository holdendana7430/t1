代发 wailian999

df -h;  du -sh *
来源：http://am.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://bj.521024.cn

du -ah . | sort -rh | head -10
来源：http://mn.asd995.cn

[R63] 内存与进程
来源：http://rx.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://rc.yuexingan06.cn

[R64] 结束进程
来源：http://vc.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://wa.shxzukj.cn

[R65] 查看端口占用
来源：http://yd.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ay.bookmarksfly.cn

[R66] 定时任务
来源：http://vh.hahajie.cn

crontab -e;  crontab -l
来源：http://rx.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://ku.bjjhwx.cn

openssl rand -hex 16
来源：http://tc.muxihuayi.cn

[R68] 计算文件校验值
来源：http://fi.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mp.lnxyls.cn

[R69] 生成随机密码
来源：http://hb.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://fw.szsharing.cn

[R70] 时间戳与互转
来源：http://hd.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://aq.colortex.cn

[R71] 日期格式化
来源：http://ko.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://un.nicolike.cn

[R72] 等待端口就绪
来源：http://kb.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nt.shtwfgs.cn

[R73] 分割大日志
来源：http://eh.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ve.haigaiapp.cn

[R74] 批量重命名
来源：http://cc.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kn.521024.cn

[R75] 导出环境变量
来源：http://zq.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://la.shtwfgs.cn

[R76] 使用临时文件
来源：http://ch.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ij.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://zu.shtwfgs.cn

read -rp "请输入: " ans
来源：http://nj.huixiangedu.cn

[R78] 交互式菜单
来源：http://yz.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bb.hnjuh.cn

[R79] 解析命令行选项
来源：http://gr.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xy.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ub.521024.cn

time ./run.sh
来源：http://my.huanxung.cn

================================================================================
来源：http://xp.shxzukj.cn

S. C / C++ 专题
来源：http://nx.shtwfgs.cn

================================================================================
来源：http://vw.jianghongdianzi.cn

[S01] C：Hello World
来源：http://en.9csxet.cn

#include <stdio.h>
来源：http://xu.shxzukj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mg.huanxung.cn

[S02] C：变量与格式化输出
来源：http://ms.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://wc.hahajie.cn

[S03] C：读入整数
来源：http://go.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://jw.szxytkj.cn

[S04] C：字符串复制
来源：http://vk.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ld.shxzskj.cn

[S05] C：字符串长度
来源：http://of.hahajie.cn

strlen(s)
来源：http://we.wgjwhj.cn

[S06] C：字符串比较
来源：http://tt.shtwfgs.cn

strcmp(a, b) == 0
来源：http://uy.asd995.cn

[S07] C：数组遍历求和
来源：http://te.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fo.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ok.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bl.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://gv.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nu.521024.cn

[S10] C：指针与解引用
来源：http://dy.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://vg.huixiangedu.cn

[S11] C：逐行读文件
来源：http://zx.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://ox.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ek.huixinmuqiang.cn

fclose(f);
来源：http://te.huanxung.cn

[S12] C：写文件
来源：http://ah.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xs.nicolike.cn

[S13] C：宏定义
来源：http://kx.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fe.lnxyls.cn

[S14] C：枚举
来源：http://ve.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://qn.shxzukj.cn

[S15] C：类型转换
来源：http://rz.szsharing.cn

(double) a / b
来源：http://rq.huanxung.cn

[S16] C：位操作置位
来源：http://lq.huixiangedu.cn

x |= (1 << 3);
来源：http://jm.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://di.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xx.chemitech.net.cn

[S18] C：命令行参数
来源：http://od.szxytkj.cn

int main(int argc, char **argv)
来源：http://dq.muxihuayi.cn

[S19] C：快速排序
来源：http://nd.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hj.wgjwhj.cn

[S20] C：二分查找
来源：http://iz.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hy.newstarts.cn

[S21] C：字符类别判断
来源：http://ha.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xn.chemitech.net.cn

[S22] C：字符串转数字
来源：http://he.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nh.hahajie.cn

[S23] C：随机数
来源：http://gz.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vm.huixiangedu.cn

[S24] C：获取本地时间
来源：http://pj.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cj.chemitech.net.cn

[S25] C：内存拷贝
来源：http://vs.bjjhwx.cn

memcpy(dst, src, n);
来源：http://bc.huixiangedu.cn

[S26] C：内存清零
来源：http://xb.szsharing.cn

memset(a, 0, sizeof a);
来源：http://wn.yuexingan06.cn

[S27] C：定义常量
来源：http://qm.muxihuayi.cn

const double PI = 3.14159;
来源：http://ny.huixinmuqiang.cn

[S28] C：静态变量
来源：http://tb.bjjhwx.cn

static int counter = 0;
来源：http://ki.hahajie.cn

[S29] C：变参函数
来源：http://lj.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ui.gzmigu.cn

[S30] C：头文件保护
来源：http://jw.nicolike.cn

#ifndef X_H
来源：http://gi.shxzukj.cn

#define X_H
来源：http://zp.bjjhwx.cn

#endif
来源：http://ix.haigaiapp.cn

[S31] C++：Hello World
来源：http://vq.lnxyls.cn

#include <iostream>
来源：http://nx.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://lg.nicolike.cn

[S32] C++：字符串
来源：http://pa.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://kd.gzmigu.cn

[S33] C++：vector 增删
来源：http://uf.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ab.521024.cn

[S34] C++：遍历 vector
来源：http://sn.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://zc.lnxyls.cn

[S35] C++：map
来源：http://re.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bc.asd995.cn

[S36] C++：unordered_map
来源：http://nb.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lx.huixinmuqiang.cn

[S37] C++：set
来源：http://hs.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ir.9csxet.cn

[S38] C++：排序
来源：http://dd.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://qw.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://vy.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oz.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://ud.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pv.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://lm.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xx.huanxung.cn

[S42] C++：继承与虚函数
来源：http://gu.521024.cn

class B : public Base { public: void f() override {} };
来源：http://gr.521024.cn

[S43] C++：智能指针
来源：http://db.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://kt.nicolike.cn

[S44] C++：引用传参
来源：http://yu.9csxet.cn

void inc(int &x) { ++x; }
来源：http://up.gzmigu.cn

[S45] C++：lambda
来源：http://si.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qp.wgjwhj.cn

[S46] C++：函数模板
来源：http://ue.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zt.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://sd.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kt.asd995.cn

[S48] C++：逐行读文件
来源：http://yz.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rk.huanxung.cn

while (std::getline(in, line)) { }
来源：http://zs.bjjhwx.cn

[S49] C++：写文件
来源：http://lh.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wp.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://jk.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tp.newstarts.cn

[S51] C++：显式类型转换
来源：http://gv.muxihuayi.cn

static_cast<double>(a) / b
来源：http://sn.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://os.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://yy.9csxet.cn

[S53] C++：移动语义
来源：http://fu.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://ty.bjjhwx.cn

[S54] C++：异常处理
来源：http://ct.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xl.9csxet.cn

[S55] C++：结构化绑定
来源：http://su.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sg.huixiangedu.cn

[S56] C++：optional
来源：http://pg.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kh.muxihuayi.cn

[S57] C++：编译期常量
来源：http://yh.shxzskj.cn

constexpr int N = 10;
来源：http://sc.gzmigu.cn

[S58] C++：命名空间
来源：http://pp.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://ey.shxzskj.cn

[S59] C++：静态断言
来源：http://ez.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bd.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://xy.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dq.hnjuh.cn

================================================================================
来源：http://mr.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gf.bookmarksfly.cn

================================================================================
来源：http://kf.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://xc.huixiangedu.cn

println("Hello")
来源：http://fz.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://fl.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://km.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://xu.bjjhwx.cn

"值: $b"
来源：http://wg.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://rw.shxzukj.cn

val n: String? = null;  n?.length
来源：http://uz.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://gv.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yf.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://zu.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://os.521024.cn

[T07] Kotlin：集合过滤
来源：http://mg.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tg.hahajie.cn

[T08] Kotlin：数据类
来源：http://th.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ar.521024.cn

[T09] Kotlin：扩展函数
来源：http://ei.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://ye.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://os.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zx.shtwfgs.cn

[T11] Kotlin：协程
来源：http://wl.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yq.nicolike.cn

[T12] Kotlin：解构声明
来源：http://qh.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://ko.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://vu.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://ko.nszjky.cn

[T14] Kotlin：循环
来源：http://qu.nszjky.cn

for (i in 1..10) println(i)
来源：http://hi.wgjwhj.cn

[T15] Kotlin：接口
来源：http://dl.9csxet.cn

interface Shape { fun area(): Double }
来源：http://ev.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://nr.muxihuayi.cn

print("Hello")
来源：http://ov.newstarts.cn

[T17] Swift：变量与常量
来源：http://kz.szsharing.cn

var a = 1;  let b = 2
来源：http://ac.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://lg.bookmarksfly.cn

"值: \(b)"
来源：http://ct.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://mx.lnxyls.cn

if let n = opt { print(n) }
来源：http://gp.jctech888.com.cn

[T20] Swift：数组操作
来源：http://hf.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://op.nszjky.cn

[T21] Swift：遍历
来源：http://sp.muxihuayi.cn

for x in a { print(x) }
来源：http://ep.wgjwhj.cn

[T22] Swift：字典
来源：http://pc.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xl.shtwfgs.cn

[T23] Swift：函数
来源：http://ot.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wn.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://mi.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yv.yuexingan06.cn

[T25] Swift：结构体
来源：http://jg.chemitech.net.cn

struct P { var x: Int }
来源：http://jp.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://na.szsharing.cn

class A: Base { override func f() {} }
来源：http://xz.nszjky.cn

[T27] Swift：错误处理
来源：http://en.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://nk.wgjwhj.cn

[T28] Swift：枚举
来源：http://xp.hnjuh.cn

enum Color { case red, green }
来源：http://hi.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://vd.521024.cn

guard let x = opt else { return }
来源：http://aj.chemitech.net.cn

[T30] Swift：协议
来源：http://kf.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://tv.shxzukj.cn

[T31] Lua：Hello World
来源：http://ij.szxytkj.cn

print("Hello")
来源：http://pj.szxytkj.cn

[T32] Lua：局部变量
来源：http://de.colortex.cn

local a = 1
来源：http://zu.hahajie.cn

[T33] Lua：表（数组）
来源：http://cc.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wz.gzmigu.cn

[T34] Lua：遍历表
来源：http://mx.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pp.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://wd.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://le.wgjwhj.cn

[T36] Lua：函数
来源：http://ez.panjiajie.cn

function add(a, b) return a + b end
来源：http://jr.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://tb.huixiangedu.cn

"a" .. "b"
来源：http://qs.shtwfgs.cn

[T38] Lua：条件
来源：http://jo.szxytkj.cn

if x > 0 then print("正") end
来源：http://hh.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://ye.hahajie.cn

string.find(s, "%d+")
来源：http://ff.521024.cn

[T40] Lua：元表
来源：http://vo.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://vh.nicolike.cn

[T41] Perl：Hello World
来源：http://nn.huixinmuqiang.cn

print "Hello\n";
来源：http://ze.gzmigu.cn

[T42] Perl：变量类型
来源：http://cx.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bk.szsharing.cn

[T43] Perl：字符串插值
来源：http://gi.chemitech.net.cn

"值: $a"
来源：http://mj.yuntaijiaju.cn

[T44] Perl：条件
来源：http://xp.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://wv.colortex.cn

[T45] Perl：数组遍历
来源：http://gf.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://yj.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://ro.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mk.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://sg.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bn.hahajie.cn

[T48] Perl：正则替换
来源：http://wo.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://up.gzmigu.cn

[T49] Perl：函数
来源：http://zu.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kq.asd995.cn

[T50] Perl：逐行读文件
来源：http://db.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://do.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://bu.9csxet.cn

[T51] Scala：Hello World
来源：http://po.shxzskj.cn

println("Hello")
来源：http://bq.huanxung.cn

[T52] Scala：变量
来源：http://yr.chemitech.net.cn

val a = 1;  var b = 2
来源：http://od.colortex.cn

[T53] Scala：字符串插值
来源：http://xr.nszjky.cn

s"值: $b"
来源：http://nl.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://na.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://wz.newstarts.cn

[T55] Scala：集合过滤
来源：http://bd.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mx.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://yi.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://co.9csxet.cn

[T57] Scala：模式匹配
来源：http://ux.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ue.9csxet.cn

[T58] Scala：函数定义
来源：http://ys.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jy.hnjuh.cn

[T59] Scala：循环
来源：http://ya.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://xq.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://rv.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ok.panjiajie.cn

================================================================================
来源：http://dr.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sz.9csxet.cn

================================================================================
来源：http://sw.shtwfgs.cn

[U01] Py：创建虚拟环境
来源：http://ny.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qo.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://bw.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nm.szsharing.cn


<!-- 参考信息 -->