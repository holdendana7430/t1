代发 wailian999

df -h;  du -sh *
来源：http://hg.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://gf.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ew.huixiangedu.cn

[R63] 内存与进程
来源：http://ym.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://hc.newstarts.cn

[R64] 结束进程
来源：http://gc.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://sf.lnxyls.cn

[R65] 查看端口占用
来源：http://sm.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gb.huanxung.cn

[R66] 定时任务
来源：http://dw.521024.cn

crontab -e;  crontab -l
来源：http://ls.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://mz.szxytkj.cn

openssl rand -hex 16
来源：http://tf.asd995.cn

[R68] 计算文件校验值
来源：http://sl.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://la.lnxyls.cn

[R69] 生成随机密码
来源：http://fb.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://hl.haigaiapp.cn

[R70] 时间戳与互转
来源：http://ha.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://ge.jianghongdianzi.cn

[R71] 日期格式化
来源：http://gd.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ry.shtwfgs.cn

[R72] 等待端口就绪
来源：http://bo.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ak.shtwfgs.cn

[R73] 分割大日志
来源：http://ks.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ii.huixiangedu.cn

[R74] 批量重命名
来源：http://aw.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://by.bookmarksfly.cn

[R75] 导出环境变量
来源：http://qh.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://af.asd995.cn

[R76] 使用临时文件
来源：http://fc.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gh.haigaiapp.cn

[R77] 读取用户输入
来源：http://lr.521024.cn

read -rp "请输入: " ans
来源：http://mu.wgjwhj.cn

[R78] 交互式菜单
来源：http://aq.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xa.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://ap.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ut.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://re.hnjuh.cn

time ./run.sh
来源：http://yw.colortex.cn

================================================================================
来源：http://nl.bookmarksfly.cn

S. C / C++ 专题
来源：http://bu.yuexingan06.cn

================================================================================
来源：http://iv.bjjhwx.cn

[S01] C：Hello World
来源：http://xr.lnxyls.cn

#include <stdio.h>
来源：http://bn.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nl.asd995.cn

[S02] C：变量与格式化输出
来源：http://gv.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://fj.nicolike.cn

[S03] C：读入整数
来源：http://fh.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://sl.bjjhwx.cn

[S04] C：字符串复制
来源：http://cx.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gz.hahajie.cn

[S05] C：字符串长度
来源：http://fm.wgjwhj.cn

strlen(s)
来源：http://df.9csxet.cn

[S06] C：字符串比较
来源：http://en.muxihuayi.cn

strcmp(a, b) == 0
来源：http://ja.szxytkj.cn

[S07] C：数组遍历求和
来源：http://oj.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yq.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://rq.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pg.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://wl.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ax.jctech888.com.cn

[S10] C：指针与解引用
来源：http://tj.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://gy.huixiangedu.cn

[S11] C：逐行读文件
来源：http://xz.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xh.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dw.panjiajie.cn

fclose(f);
来源：http://xo.szsharing.cn

[S12] C：写文件
来源：http://um.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oi.nicolike.cn

[S13] C：宏定义
来源：http://gv.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wl.szsharing.cn

[S14] C：枚举
来源：http://qs.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://qt.szxytkj.cn

[S15] C：类型转换
来源：http://jw.szsharing.cn

(double) a / b
来源：http://bj.lnxyls.cn

[S16] C：位操作置位
来源：http://lh.9csxet.cn

x |= (1 << 3);
来源：http://dz.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://zb.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wm.bookmarksfly.cn

[S18] C：命令行参数
来源：http://bm.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://wx.wgjwhj.cn

[S19] C：快速排序
来源：http://zd.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pz.9csxet.cn

[S20] C：二分查找
来源：http://zf.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yz.shtwfgs.cn

[S21] C：字符类别判断
来源：http://mr.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wn.9csxet.cn

[S22] C：字符串转数字
来源：http://pt.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uo.szxytkj.cn

[S23] C：随机数
来源：http://ib.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iu.shtwfgs.cn

[S24] C：获取本地时间
来源：http://ky.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hi.szxytkj.cn

[S25] C：内存拷贝
来源：http://vc.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ob.colortex.cn

[S26] C：内存清零
来源：http://ze.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://tn.haigaiapp.cn

[S27] C：定义常量
来源：http://bx.nicolike.cn

const double PI = 3.14159;
来源：http://pi.521024.cn

[S28] C：静态变量
来源：http://zj.szxytkj.cn

static int counter = 0;
来源：http://eg.huixiangedu.cn

[S29] C：变参函数
来源：http://xr.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xe.hnjuh.cn

[S30] C：头文件保护
来源：http://hp.hnjuh.cn

#ifndef X_H
来源：http://xl.gzmigu.cn

#define X_H
来源：http://cx.hnjuh.cn

#endif
来源：http://ws.nicolike.cn

[S31] C++：Hello World
来源：http://zk.muxihuayi.cn

#include <iostream>
来源：http://lx.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://xp.nicolike.cn

[S32] C++：字符串
来源：http://ew.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://bk.hahajie.cn

[S33] C++：vector 增删
来源：http://gx.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bn.nicolike.cn

[S34] C++：遍历 vector
来源：http://ux.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://lr.colortex.cn

[S35] C++：map
来源：http://ex.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ci.lnxyls.cn

[S36] C++：unordered_map
来源：http://ea.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lm.nicolike.cn

[S37] C++：set
来源：http://rw.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lp.yuexingan06.cn

[S38] C++：排序
来源：http://zr.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://uf.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://ad.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rf.jctech888.com.cn

[S40] C++：查找元素
来源：http://dx.bookmarksfly.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sc.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://id.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wg.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://gh.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://wm.haigaiapp.cn

[S43] C++：智能指针
来源：http://eb.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://qv.nicolike.cn

[S44] C++：引用传参
来源：http://px.asd995.cn

void inc(int &x) { ++x; }
来源：http://il.asd995.cn

[S45] C++：lambda
来源：http://zx.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://po.szxytkj.cn

[S46] C++：函数模板
来源：http://og.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ph.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://pq.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wr.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://pv.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qx.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://vp.bookmarksfly.cn

[S49] C++：写文件
来源：http://un.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qv.shtwfgs.cn

[S50] C++：格式化数字
来源：http://fn.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fk.asd995.cn

[S51] C++：显式类型转换
来源：http://et.nicolike.cn

static_cast<double>(a) / b
来源：http://hn.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://gn.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://kj.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://nz.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://fd.jctech888.com.cn

[S54] C++：异常处理
来源：http://ih.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nx.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://rb.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nh.newstarts.cn

[S56] C++：optional
来源：http://bv.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zu.wgjwhj.cn

[S57] C++：编译期常量
来源：http://fy.shxzukj.cn

constexpr int N = 10;
来源：http://hd.gzmigu.cn

[S58] C++：命名空间
来源：http://gf.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://jc.huixiangedu.cn

[S59] C++：静态断言
来源：http://xz.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mu.colortex.cn

[S60] C++：遍历并删除元素
来源：http://lh.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iy.9csxet.cn

================================================================================
来源：http://dc.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aw.9csxet.cn

================================================================================
来源：http://ep.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://nc.huixinmuqiang.cn

println("Hello")
来源：http://au.szxytkj.cn

[T02] Kotlin：变量
来源：http://pj.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gw.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://zg.bjjhwx.cn

"值: $b"
来源：http://ip.gzmigu.cn

[T04] Kotlin：空安全
来源：http://gz.nicolike.cn

val n: String? = null;  n?.length
来源：http://uq.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://lw.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qq.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://xs.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://io.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://nm.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fh.szxytkj.cn

[T08] Kotlin：数据类
来源：http://tq.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://sl.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://is.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://fm.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://sm.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uk.huixiangedu.cn

[T11] Kotlin：协程
来源：http://lq.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ck.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://sh.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://hg.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://gu.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://un.huanxung.cn

[T14] Kotlin：循环
来源：http://sn.shxzskj.cn

for (i in 1..10) println(i)
来源：http://at.newstarts.cn

[T15] Kotlin：接口
来源：http://lj.newstarts.cn

interface Shape { fun area(): Double }
来源：http://wv.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://sk.nszjky.cn

print("Hello")
来源：http://fb.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://le.szsharing.cn

var a = 1;  let b = 2
来源：http://bs.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://bd.bookmarksfly.cn

"值: \(b)"
来源：http://pt.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://qk.wgjwhj.cn

if let n = opt { print(n) }
来源：http://rq.yuexingan06.cn

[T20] Swift：数组操作
来源：http://jg.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cr.nicolike.cn

[T21] Swift：遍历
来源：http://bd.szsharing.cn

for x in a { print(x) }
来源：http://uk.wgjwhj.cn

[T22] Swift：字典
来源：http://lm.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xh.jctech888.com.cn

[T23] Swift：函数
来源：http://mk.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ru.jctech888.com.cn

[T24] Swift：闭包
来源：http://to.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ts.jctech888.com.cn

[T25] Swift：结构体
来源：http://ad.shxzukj.cn

struct P { var x: Int }
来源：http://hd.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://lz.nszjky.cn

class A: Base { override func f() {} }
来源：http://ve.huixiangedu.cn

[T27] Swift：错误处理
来源：http://sq.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://uj.nicolike.cn

[T28] Swift：枚举
来源：http://us.panjiajie.cn

enum Color { case red, green }
来源：http://gy.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://dy.asd995.cn

guard let x = opt else { return }
来源：http://wz.nszjky.cn

[T30] Swift：协议
来源：http://pf.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://qk.hahajie.cn

[T31] Lua：Hello World
来源：http://rr.hnjuh.cn

print("Hello")
来源：http://bl.gzmigu.cn

[T32] Lua：局部变量
来源：http://mm.panjiajie.cn

local a = 1
来源：http://ep.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://fo.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wo.muxihuayi.cn

[T34] Lua：遍历表
来源：http://ah.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://js.colortex.cn

[T35] Lua：字典表
来源：http://cp.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://rs.yuexingan06.cn

[T36] Lua：函数
来源：http://gi.nicolike.cn

function add(a, b) return a + b end
来源：http://oc.nszjky.cn

[T37] Lua：字符串拼接
来源：http://ps.hahajie.cn

"a" .. "b"
来源：http://kn.shxzskj.cn

[T38] Lua：条件
来源：http://nn.colortex.cn

if x > 0 then print("正") end
来源：http://bm.lnxyls.cn

[T39] Lua：模式匹配
来源：http://cv.panjiajie.cn

string.find(s, "%d+")
来源：http://vo.asd995.cn

[T40] Lua：元表
来源：http://zj.9csxet.cn

setmetatable({}, { __index = base })
来源：http://sz.szxytkj.cn

[T41] Perl：Hello World
来源：http://qa.newstarts.cn

print "Hello\n";
来源：http://jp.lnxyls.cn

[T42] Perl：变量类型
来源：http://rm.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uj.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ff.nszjky.cn

"值: $a"
来源：http://rc.colortex.cn

[T44] Perl：条件
来源：http://qp.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://cz.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://gr.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://uf.lnxyls.cn

[T46] Perl：哈希操作
来源：http://lu.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ax.hnjuh.cn

[T47] Perl：正则捕获
来源：http://rk.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gy.panjiajie.cn

[T48] Perl：正则替换
来源：http://di.newstarts.cn

$s =~ s/old/new/g;
来源：http://gb.szsharing.cn

[T49] Perl：函数
来源：http://uo.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yq.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://tb.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pq.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://qt.colortex.cn

[T51] Scala：Hello World
来源：http://jw.huixinmuqiang.cn

println("Hello")
来源：http://zt.panjiajie.cn

[T52] Scala：变量
来源：http://ty.jctech888.com.cn

val a = 1;  var b = 2
来源：http://nd.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://eg.lnxyls.cn

s"值: $b"
来源：http://ix.szxytkj.cn

[T54] Scala：集合映射
来源：http://ub.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://fy.lnxyls.cn

[T55] Scala：集合过滤
来源：http://qn.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://si.newstarts.cn

[T56] Scala：样例类
来源：http://az.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://jk.shxzskj.cn

[T57] Scala：模式匹配
来源：http://st.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wz.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://cb.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ld.bookmarksfly.cn

[T59] Scala：循环
来源：http://yv.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://lf.lnxyls.cn

[T60] Scala：折叠
来源：http://fo.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dl.szsharing.cn

================================================================================
来源：http://ua.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ur.huixinmuqiang.cn

================================================================================
来源：http://vi.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://lz.haigaiapp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xh.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://py.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ay.panjiajie.cn


<!-- 参考信息 -->