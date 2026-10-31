代发 wailian999

ssh user@host 'uptime'
来源：http://lt.hnjuh.cn

[R58] 下载文件
来源：http://uy.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ol.szxytkj.cn

[R59] 发 POST JSON
来源：http://qt.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nw.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://kh.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ke.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://lj.huixiangedu.cn

df -h;  du -sh *
来源：http://uw.9csxet.cn

[R62] 找最占空间的文件
来源：http://ki.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://xa.shxzskj.cn

[R63] 内存与进程
来源：http://oy.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://lc.hnjuh.cn

[R64] 结束进程
来源：http://yf.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://lj.nszjky.cn

[R65] 查看端口占用
来源：http://ph.huixiangedu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wa.9csxet.cn

[R66] 定时任务
来源：http://ju.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://bd.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://zw.bookmarksfly.cn

openssl rand -hex 16
来源：http://sk.bjjhwx.cn

[R68] 计算文件校验值
来源：http://pg.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jq.lnxyls.cn

[R69] 生成随机密码
来源：http://ku.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://xk.huixiangedu.cn

[R70] 时间戳与互转
来源：http://vn.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://oe.nicolike.cn

[R71] 日期格式化
来源：http://wq.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://od.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://wy.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pe.yuntaijiaju.cn

[R73] 分割大日志
来源：http://oo.hnjuh.cn

split -l 1000 big.log part_
来源：http://al.szxytkj.cn

[R74] 批量重命名
来源：http://fx.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ju.jctech888.com.cn

[R75] 导出环境变量
来源：http://nj.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://om.nicolike.cn

[R76] 使用临时文件
来源：http://du.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mx.szxytkj.cn

[R77] 读取用户输入
来源：http://ix.muxihuayi.cn

read -rp "请输入: " ans
来源：http://vh.yuexingan06.cn

[R78] 交互式菜单
来源：http://to.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pf.asd995.cn

[R79] 解析命令行选项
来源：http://uw.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qw.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://gl.szsharing.cn

time ./run.sh
来源：http://qp.yuexingan06.cn

================================================================================
来源：http://gi.bookmarksfly.cn

S. C / C++ 专题
来源：http://se.gzmigu.cn

================================================================================
来源：http://tt.yuntaijiaju.cn

[S01] C：Hello World
来源：http://nb.jianghongdianzi.cn

#include <stdio.h>
来源：http://lh.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ga.szsharing.cn

[S02] C：变量与格式化输出
来源：http://vp.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://io.newstarts.cn

[S03] C：读入整数
来源：http://gy.asd995.cn

int x; scanf("%d", &x);
来源：http://wr.yuexingan06.cn

[S04] C：字符串复制
来源：http://hs.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tr.panjiajie.cn

[S05] C：字符串长度
来源：http://wg.szsharing.cn

strlen(s)
来源：http://pd.shxzskj.cn

[S06] C：字符串比较
来源：http://jx.9csxet.cn

strcmp(a, b) == 0
来源：http://hu.nszjky.cn

[S07] C：数组遍历求和
来源：http://kx.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xz.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://ly.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ug.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://iu.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ze.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://fr.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://ge.huixiangedu.cn

[S11] C：逐行读文件
来源：http://ko.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://bz.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://re.nicolike.cn

fclose(f);
来源：http://ay.asd995.cn

[S12] C：写文件
来源：http://wu.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vq.shtwfgs.cn

[S13] C：宏定义
来源：http://ym.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mj.newstarts.cn

[S14] C：枚举
来源：http://dh.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://tl.bookmarksfly.cn

[S15] C：类型转换
来源：http://tn.muxihuayi.cn

(double) a / b
来源：http://fa.shxzukj.cn

[S16] C：位操作置位
来源：http://pz.newstarts.cn

x |= (1 << 3);
来源：http://df.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://ki.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zy.huixiangedu.cn

[S18] C：命令行参数
来源：http://wn.shxzukj.cn

int main(int argc, char **argv)
来源：http://kw.shtwfgs.cn

[S19] C：快速排序
来源：http://sm.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ds.nszjky.cn

[S20] C：二分查找
来源：http://il.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sw.yuexingan06.cn

[S21] C：字符类别判断
来源：http://zi.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://to.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://ot.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fz.bjjhwx.cn

[S23] C：随机数
来源：http://kh.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xd.9csxet.cn

[S24] C：获取本地时间
来源：http://tt.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uw.yuexingan06.cn

[S25] C：内存拷贝
来源：http://yd.asd995.cn

memcpy(dst, src, n);
来源：http://df.jctech888.com.cn

[S26] C：内存清零
来源：http://ry.newstarts.cn

memset(a, 0, sizeof a);
来源：http://nd.asd995.cn

[S27] C：定义常量
来源：http://ma.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://ag.huixinmuqiang.cn

[S28] C：静态变量
来源：http://zd.521024.cn

static int counter = 0;
来源：http://vw.9csxet.cn

[S29] C：变参函数
来源：http://pe.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hx.panjiajie.cn

[S30] C：头文件保护
来源：http://kz.jianghongdianzi.cn

#ifndef X_H
来源：http://fc.huixiangedu.cn

#define X_H
来源：http://iy.bjjhwx.cn

#endif
来源：http://zq.newstarts.cn

[S31] C++：Hello World
来源：http://qs.panjiajie.cn

#include <iostream>
来源：http://eb.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://hd.nszjky.cn

[S32] C++：字符串
来源：http://oc.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://gw.shxzskj.cn

[S33] C++：vector 增删
来源：http://qq.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fb.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://rm.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://yj.panjiajie.cn

[S35] C++：map
来源：http://uf.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rc.huanxung.cn

[S36] C++：unordered_map
来源：http://og.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ya.panjiajie.cn

[S37] C++：set
来源：http://ey.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uh.szsharing.cn

[S38] C++：排序
来源：http://ut.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://oc.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://th.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://px.huanxung.cn

[S40] C++：查找元素
来源：http://qe.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bw.nicolike.cn

[S41] C++：类与构造函数
来源：http://eh.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wl.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://qg.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://jv.szsharing.cn

[S43] C++：智能指针
来源：http://ca.521024.cn

auto p = std::make_unique<int>(5);
来源：http://xt.lnxyls.cn

[S44] C++：引用传参
来源：http://yr.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://ok.jianghongdianzi.cn

[S45] C++：lambda
来源：http://qw.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ic.jctech888.com.cn

[S46] C++：函数模板
来源：http://re.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://en.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://kd.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hw.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://en.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xc.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://gw.jctech888.com.cn

[S49] C++：写文件
来源：http://hv.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xy.nszjky.cn

[S50] C++：格式化数字
来源：http://tn.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hi.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://co.521024.cn

static_cast<double>(a) / b
来源：http://js.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ib.9csxet.cn

int size() const noexcept { return n_; }
来源：http://sm.shtwfgs.cn

[S53] C++：移动语义
来源：http://jv.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://ni.muxihuayi.cn

[S54] C++：异常处理
来源：http://ip.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vd.hnjuh.cn

[S55] C++：结构化绑定
来源：http://xe.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xw.colortex.cn

[S56] C++：optional
来源：http://ep.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ce.hnjuh.cn

[S57] C++：编译期常量
来源：http://hj.nicolike.cn

constexpr int N = 10;
来源：http://fn.shxzukj.cn

[S58] C++：命名空间
来源：http://ps.521024.cn

namespace ns { int f() { return 1; } }
来源：http://gu.shxzskj.cn

[S59] C++：静态断言
来源：http://xf.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ss.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://gd.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cp.wgjwhj.cn

================================================================================
来源：http://wr.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ct.jctech888.com.cn

================================================================================
来源：http://uo.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://uw.asd995.cn

println("Hello")
来源：http://qi.gzmigu.cn

[T02] Kotlin：变量
来源：http://bq.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nm.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://tr.yuexingan06.cn

"值: $b"
来源：http://if.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://hv.nicolike.cn

val n: String? = null;  n?.length
来源：http://jl.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://ej.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hm.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://ut.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ib.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://xm.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xh.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://oz.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://dr.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://zw.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://vf.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://uq.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xa.9csxet.cn

[T11] Kotlin：协程
来源：http://mj.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tr.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://om.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://aa.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://zf.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://zq.gzmigu.cn

[T14] Kotlin：循环
来源：http://ko.colortex.cn

for (i in 1..10) println(i)
来源：http://qr.huixiangedu.cn

[T15] Kotlin：接口
来源：http://ya.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://qc.asd995.cn

[T16] Swift：Hello World
来源：http://vv.huanxung.cn

print("Hello")
来源：http://el.nicolike.cn

[T17] Swift：变量与常量
来源：http://ia.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://fs.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://ir.wgjwhj.cn

"值: \(b)"
来源：http://zi.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://yx.hnjuh.cn

if let n = opt { print(n) }
来源：http://ad.gzmigu.cn

[T20] Swift：数组操作
来源：http://ze.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qx.shxzskj.cn

[T21] Swift：遍历
来源：http://bi.shtwfgs.cn

for x in a { print(x) }
来源：http://ls.hnjuh.cn

[T22] Swift：字典
来源：http://ki.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dt.shxzskj.cn

[T23] Swift：函数
来源：http://sq.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iz.newstarts.cn

[T24] Swift：闭包
来源：http://fu.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kt.hahajie.cn

[T25] Swift：结构体
来源：http://ya.bjjhwx.cn

struct P { var x: Int }
来源：http://in.panjiajie.cn

[T26] Swift：类与重写
来源：http://pu.shxzukj.cn

class A: Base { override func f() {} }
来源：http://hq.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://zs.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://mq.lnxyls.cn

[T28] Swift：枚举
来源：http://wm.chemitech.net.cn

enum Color { case red, green }
来源：http://py.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://ji.bjjhwx.cn

guard let x = opt else { return }
来源：http://ms.shxzskj.cn

[T30] Swift：协议
来源：http://gx.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://zr.newstarts.cn

[T31] Lua：Hello World
来源：http://iq.nszjky.cn

print("Hello")
来源：http://lt.haigaiapp.cn

[T32] Lua：局部变量
来源：http://pa.muxihuayi.cn

local a = 1
来源：http://mg.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://rc.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ji.hnjuh.cn

[T34] Lua：遍历表
来源：http://hf.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uk.bjjhwx.cn

[T35] Lua：字典表
来源：http://fq.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://ez.shxzukj.cn

[T36] Lua：函数
来源：http://iu.shxzskj.cn

function add(a, b) return a + b end
来源：http://mq.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://fc.huanxung.cn

"a" .. "b"
来源：http://hh.nszjky.cn

[T38] Lua：条件
来源：http://ui.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://kl.colortex.cn

[T39] Lua：模式匹配
来源：http://qq.bjjhwx.cn

string.find(s, "%d+")
来源：http://ee.huixinmuqiang.cn

[T40] Lua：元表
来源：http://qm.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://xo.wgjwhj.cn

[T41] Perl：Hello World
来源：http://bx.asd995.cn

print "Hello\n";
来源：http://hj.wgjwhj.cn

[T42] Perl：变量类型
来源：http://ju.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rp.lnxyls.cn

[T43] Perl：字符串插值
来源：http://wo.hnjuh.cn

"值: $a"
来源：http://la.haigaiapp.cn

[T44] Perl：条件
来源：http://rz.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://pb.shxzskj.cn

[T45] Perl：数组遍历
来源：http://cn.asd995.cn

for my $x (@arr) { print $x; }
来源：http://bg.huanxung.cn

[T46] Perl：哈希操作
来源：http://ql.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hu.szsharing.cn

[T47] Perl：正则捕获
来源：http://av.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zc.colortex.cn

[T48] Perl：正则替换
来源：http://to.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://kq.wgjwhj.cn

[T49] Perl：函数
来源：http://dx.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lf.colortex.cn

[T50] Perl：逐行读文件
来源：http://ex.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wt.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://qh.huanxung.cn

[T51] Scala：Hello World
来源：http://wz.panjiajie.cn

println("Hello")
来源：http://pl.szxytkj.cn

[T52] Scala：变量
来源：http://ab.lnxyls.cn

val a = 1;  var b = 2
来源：http://wk.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://ag.newstarts.cn

s"值: $b"
来源：http://qf.colortex.cn

[T54] Scala：集合映射
来源：http://ym.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://bb.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://cf.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://du.asd995.cn

[T56] Scala：样例类
来源：http://la.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://ma.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://gx.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://al.521024.cn

[T58] Scala：函数定义
来源：http://bz.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gm.szsharing.cn

[T59] Scala：循环
来源：http://bk.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://sq.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://dm.huixinmuqiang.cn


<!-- 参考信息 -->