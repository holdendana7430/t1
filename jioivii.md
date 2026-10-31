代发 wailian999

ssh user@host 'uptime'
来源：http://yw.jianghongdianzi.cn

[R58] 下载文件
来源：http://gs.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ln.chemitech.net.cn

[R59] 发 POST JSON
来源：http://cv.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ae.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://aw.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pt.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://qw.huanxung.cn

df -h;  du -sh *
来源：http://hu.huanxung.cn

[R62] 找最占空间的文件
来源：http://wl.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://hy.shtwfgs.cn

[R63] 内存与进程
来源：http://nc.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://wk.huixinmuqiang.cn

[R64] 结束进程
来源：http://fe.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://oy.bjjhwx.cn

[R65] 查看端口占用
来源：http://vv.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qh.yuntaijiaju.cn

[R66] 定时任务
来源：http://tn.shxzskj.cn

crontab -e;  crontab -l
来源：http://de.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://oq.nszjky.cn

openssl rand -hex 16
来源：http://lk.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://we.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tb.huanxung.cn

[R69] 生成随机密码
来源：http://lf.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://ck.gzmigu.cn

[R70] 时间戳与互转
来源：http://cm.jctech888.com.cn

date +%s;  date -d @1700000000
来源：http://ia.9csxet.cn

[R71] 日期格式化
来源：http://ej.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ax.shxzukj.cn

[R72] 等待端口就绪
来源：http://qa.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ox.521024.cn

[R73] 分割大日志
来源：http://rj.newstarts.cn

split -l 1000 big.log part_
来源：http://ra.shxzskj.cn

[R74] 批量重命名
来源：http://gi.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uh.panjiajie.cn

[R75] 导出环境变量
来源：http://af.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ul.bjjhwx.cn

[R76] 使用临时文件
来源：http://ec.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cv.nicolike.cn

[R77] 读取用户输入
来源：http://fd.wgjwhj.cn

read -rp "请输入: " ans
来源：http://mu.yuexingan06.cn

[R78] 交互式菜单
来源：http://du.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eb.nszjky.cn

[R79] 解析命令行选项
来源：http://oq.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gx.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://ja.9csxet.cn

time ./run.sh
来源：http://ob.hahajie.cn

================================================================================
来源：http://ih.muxihuayi.cn

S. C / C++ 专题
来源：http://xs.shxzukj.cn

================================================================================
来源：http://xi.panjiajie.cn

[S01] C：Hello World
来源：http://ao.asd995.cn

#include <stdio.h>
来源：http://mi.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ni.asd995.cn

[S02] C：变量与格式化输出
来源：http://ny.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://ml.yuexingan06.cn

[S03] C：读入整数
来源：http://tj.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://kx.yuexingan06.cn

[S04] C：字符串复制
来源：http://mt.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vx.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://fx.lnxyls.cn

strlen(s)
来源：http://rw.bookmarksfly.cn

[S06] C：字符串比较
来源：http://pu.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ju.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://tg.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ks.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://wk.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vk.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://dy.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://em.nszjky.cn

[S10] C：指针与解引用
来源：http://wk.nicolike.cn

int *p = &a;  *p = 5;
来源：http://og.lnxyls.cn

[S11] C：逐行读文件
来源：http://qm.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://wv.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pn.yuexingan06.cn

fclose(f);
来源：http://sy.huixinmuqiang.cn

[S12] C：写文件
来源：http://in.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vg.panjiajie.cn

[S13] C：宏定义
来源：http://zt.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://du.9csxet.cn

[S14] C：枚举
来源：http://yf.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://og.jianghongdianzi.cn

[S15] C：类型转换
来源：http://dj.szxytkj.cn

(double) a / b
来源：http://gq.nicolike.cn

[S16] C：位操作置位
来源：http://nh.lnxyls.cn

x |= (1 << 3);
来源：http://kx.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://tl.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ce.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://mg.jctech888.com.cn

int main(int argc, char **argv)
来源：http://cu.huixiangedu.cn

[S19] C：快速排序
来源：http://ik.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ye.lnxyls.cn

[S20] C：二分查找
来源：http://jt.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lr.wgjwhj.cn

[S21] C：字符类别判断
来源：http://yg.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://le.huixiangedu.cn

[S22] C：字符串转数字
来源：http://il.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ce.jctech888.com.cn

[S23] C：随机数
来源：http://nm.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cc.lnxyls.cn

[S24] C：获取本地时间
来源：http://im.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sf.szsharing.cn

[S25] C：内存拷贝
来源：http://ao.shtwfgs.cn

memcpy(dst, src, n);
来源：http://hk.gzmigu.cn

[S26] C：内存清零
来源：http://uc.huanxung.cn

memset(a, 0, sizeof a);
来源：http://hb.panjiajie.cn

[S27] C：定义常量
来源：http://xf.gzmigu.cn

const double PI = 3.14159;
来源：http://xr.hnjuh.cn

[S28] C：静态变量
来源：http://tp.jctech888.com.cn

static int counter = 0;
来源：http://oj.newstarts.cn

[S29] C：变参函数
来源：http://tj.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wa.nicolike.cn

[S30] C：头文件保护
来源：http://uu.yuexingan06.cn

#ifndef X_H
来源：http://vd.gzmigu.cn

#define X_H
来源：http://ds.lnxyls.cn

#endif
来源：http://jg.shxzukj.cn

[S31] C++：Hello World
来源：http://xn.shtwfgs.cn

#include <iostream>
来源：http://zo.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://zk.lnxyls.cn

[S32] C++：字符串
来源：http://rl.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://gz.hahajie.cn

[S33] C++：vector 增删
来源：http://kg.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qt.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://dz.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://jo.colortex.cn

[S35] C++：map
来源：http://ux.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://er.huixiangedu.cn

[S36] C++：unordered_map
来源：http://md.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jy.bookmarksfly.cn

[S37] C++：set
来源：http://md.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://od.newstarts.cn

[S38] C++：排序
来源：http://yf.colortex.cn

std::sort(v.begin(), v.end());
来源：http://cs.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://bt.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sn.shxzukj.cn

[S40] C++：查找元素
来源：http://xg.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gt.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://lt.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://em.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://fc.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://wv.szxytkj.cn

[S43] C++：智能指针
来源：http://vn.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ou.shtwfgs.cn

[S44] C++：引用传参
来源：http://qu.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://pi.jctech888.com.cn

[S45] C++：lambda
来源：http://va.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ko.gzmigu.cn

[S46] C++：函数模板
来源：http://cl.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ji.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://gs.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ut.521024.cn

[S48] C++：逐行读文件
来源：http://az.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xm.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://pz.colortex.cn

[S49] C++：写文件
来源：http://nw.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fz.jctech888.com.cn

[S50] C++：格式化数字
来源：http://cq.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wr.shxzskj.cn

[S51] C++：显式类型转换
来源：http://ki.yuexingan06.cn

static_cast<double>(a) / b
来源：http://xa.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://fn.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://uh.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://pf.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://zz.jctech888.com.cn

[S54] C++：异常处理
来源：http://vq.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wa.hahajie.cn

[S55] C++：结构化绑定
来源：http://gs.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fr.jianghongdianzi.cn

[S56] C++：optional
来源：http://ul.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zl.bjjhwx.cn

[S57] C++：编译期常量
来源：http://ve.shxzskj.cn

constexpr int N = 10;
来源：http://vn.huixiangedu.cn

[S58] C++：命名空间
来源：http://zw.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://nw.colortex.cn

[S59] C++：静态断言
来源：http://qx.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fr.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://sx.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vk.szsharing.cn

================================================================================
来源：http://xj.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://le.hahajie.cn

================================================================================
来源：http://ic.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://bs.huixinmuqiang.cn

println("Hello")
来源：http://tb.chemitech.net.cn

[T02] Kotlin：变量
来源：http://lz.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ts.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://xf.jianghongdianzi.cn

"值: $b"
来源：http://il.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://qz.huanxung.cn

val n: String? = null;  n?.length
来源：http://od.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://mw.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mm.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://fz.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xb.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://fo.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iq.hnjuh.cn

[T08] Kotlin：数据类
来源：http://dt.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://xw.asd995.cn

[T09] Kotlin：扩展函数
来源：http://je.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://vd.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://lf.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ec.shxzskj.cn

[T11] Kotlin：协程
来源：http://qa.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fg.nszjky.cn

[T12] Kotlin：解构声明
来源：http://wt.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://zr.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://jr.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://ux.gzmigu.cn

[T14] Kotlin：循环
来源：http://tr.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://pa.hnjuh.cn

[T15] Kotlin：接口
来源：http://es.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://hm.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://ed.yuexingan06.cn

print("Hello")
来源：http://qk.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://um.yuexingan06.cn

var a = 1;  let b = 2
来源：http://cn.asd995.cn

[T18] Swift：字符串插值
来源：http://bc.wgjwhj.cn

"值: \(b)"
来源：http://fw.shxzskj.cn

[T19] Swift：可选绑定
来源：http://zu.shxzukj.cn

if let n = opt { print(n) }
来源：http://um.wgjwhj.cn

[T20] Swift：数组操作
来源：http://ke.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ff.hahajie.cn

[T21] Swift：遍历
来源：http://vo.chemitech.net.cn

for x in a { print(x) }
来源：http://ai.lnxyls.cn

[T22] Swift：字典
来源：http://am.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mk.bjjhwx.cn

[T23] Swift：函数
来源：http://zr.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://of.nszjky.cn

[T24] Swift：闭包
来源：http://kp.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wf.jctech888.com.cn

[T25] Swift：结构体
来源：http://nz.colortex.cn

struct P { var x: Int }
来源：http://ok.huanxung.cn

[T26] Swift：类与重写
来源：http://yd.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://vf.szsharing.cn

[T27] Swift：错误处理
来源：http://xy.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://gg.haigaiapp.cn

[T28] Swift：枚举
来源：http://xh.nicolike.cn

enum Color { case red, green }
来源：http://dy.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://dd.asd995.cn

guard let x = opt else { return }
来源：http://uk.chemitech.net.cn

[T30] Swift：协议
来源：http://eq.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://ra.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://fx.521024.cn

print("Hello")
来源：http://ve.asd995.cn

[T32] Lua：局部变量
来源：http://rp.colortex.cn

local a = 1
来源：http://oz.nszjky.cn

[T33] Lua：表（数组）
来源：http://cm.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jg.shxzukj.cn

[T34] Lua：遍历表
来源：http://rp.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lx.lnxyls.cn

[T35] Lua：字典表
来源：http://or.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://hr.bookmarksfly.cn

[T36] Lua：函数
来源：http://ka.szsharing.cn

function add(a, b) return a + b end
来源：http://ny.9csxet.cn

[T37] Lua：字符串拼接
来源：http://hu.hnjuh.cn

"a" .. "b"
来源：http://ym.hnjuh.cn

[T38] Lua：条件
来源：http://qp.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://zj.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://sx.hahajie.cn

string.find(s, "%d+")
来源：http://hw.shxzskj.cn

[T40] Lua：元表
来源：http://fg.colortex.cn

setmetatable({}, { __index = base })
来源：http://ti.colortex.cn

[T41] Perl：Hello World
来源：http://zf.huixiangedu.cn

print "Hello\n";
来源：http://ip.shxzskj.cn

[T42] Perl：变量类型
来源：http://ag.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cu.panjiajie.cn

[T43] Perl：字符串插值
来源：http://rf.shxzukj.cn

"值: $a"
来源：http://rh.colortex.cn

[T44] Perl：条件
来源：http://qh.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://lf.hahajie.cn

[T45] Perl：数组遍历
来源：http://sq.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://my.lnxyls.cn

[T46] Perl：哈希操作
来源：http://fy.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qo.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://xz.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cp.haigaiapp.cn

[T48] Perl：正则替换
来源：http://ey.szsharing.cn

$s =~ s/old/new/g;
来源：http://xi.jianghongdianzi.cn

[T49] Perl：函数
来源：http://me.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://el.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://lx.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hc.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://ag.yuexingan06.cn

[T51] Scala：Hello World
来源：http://ky.hahajie.cn

println("Hello")
来源：http://vh.gzmigu.cn

[T52] Scala：变量
来源：http://dj.shtwfgs.cn

val a = 1;  var b = 2
来源：http://ds.colortex.cn

[T53] Scala：字符串插值
来源：http://wt.panjiajie.cn

s"值: $b"
来源：http://gf.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://td.panjiajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://jp.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://nk.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://px.gzmigu.cn

[T56] Scala：样例类
来源：http://xh.hahajie.cn

case class User(name: String, age: Int)
来源：http://be.colortex.cn

[T57] Scala：模式匹配
来源：http://jk.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kn.lnxyls.cn

[T58] Scala：函数定义
来源：http://xj.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ul.nicolike.cn

[T59] Scala：循环
来源：http://xy.nicolike.cn

for (i <- 1 to 10) println(i)
来源：http://ox.jctech888.com.cn

[T60] Scala：折叠
来源：http://cr.huixinmuqiang.cn


<!-- 参考信息 -->