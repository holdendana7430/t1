代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nn.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ip.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xt.haigaiapp.cn

[R61] 磁盘占用
来源：http://pm.jctech888.com.cn

df -h;  du -sh *
来源：http://ql.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://xf.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://gq.jctech888.com.cn

[R63] 内存与进程
来源：http://fn.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://ng.panjiajie.cn

[R64] 结束进程
来源：http://be.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://tv.colortex.cn

[R65] 查看端口占用
来源：http://ze.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yb.hahajie.cn

[R66] 定时任务
来源：http://wt.bjjhwx.cn

crontab -e;  crontab -l
来源：http://ko.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://wf.muxihuayi.cn

openssl rand -hex 16
来源：http://jy.shtwfgs.cn

[R68] 计算文件校验值
来源：http://ny.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://so.hnjuh.cn

[R69] 生成随机密码
来源：http://qy.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://ad.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://qt.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ni.hahajie.cn

[R71] 日期格式化
来源：http://ou.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gb.muxihuayi.cn

[R72] 等待端口就绪
来源：http://dy.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rj.colortex.cn

[R73] 分割大日志
来源：http://mq.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://bs.lnxyls.cn

[R74] 批量重命名
来源：http://bl.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rx.gzmigu.cn

[R75] 导出环境变量
来源：http://wl.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://ud.colortex.cn

[R76] 使用临时文件
来源：http://zk.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sm.jctech888.com.cn

[R77] 读取用户输入
来源：http://ez.shtwfgs.cn

read -rp "请输入: " ans
来源：http://eu.521024.cn

[R78] 交互式菜单
来源：http://lc.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ko.szsharing.cn

[R79] 解析命令行选项
来源：http://iq.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hm.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://io.nicolike.cn

time ./run.sh
来源：http://zf.hnjuh.cn

================================================================================
来源：http://mw.521024.cn

S. C / C++ 专题
来源：http://ib.huixinmuqiang.cn

================================================================================
来源：http://lo.huanxung.cn

[S01] C：Hello World
来源：http://ft.chemitech.net.cn

#include <stdio.h>
来源：http://xq.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nw.huanxung.cn

[S02] C：变量与格式化输出
来源：http://ao.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://uz.shxzukj.cn

[S03] C：读入整数
来源：http://ko.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://ht.szsharing.cn

[S04] C：字符串复制
来源：http://sv.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ui.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://fh.huanxung.cn

strlen(s)
来源：http://fs.haigaiapp.cn

[S06] C：字符串比较
来源：http://ud.nicolike.cn

strcmp(a, b) == 0
来源：http://fx.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://zh.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bn.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://yv.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pb.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://hh.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xt.huanxung.cn

[S10] C：指针与解引用
来源：http://rf.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://mg.hnjuh.cn

[S11] C：逐行读文件
来源：http://kq.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://nj.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uz.newstarts.cn

fclose(f);
来源：http://bj.bookmarksfly.cn

[S12] C：写文件
来源：http://tn.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fv.hnjuh.cn

[S13] C：宏定义
来源：http://jk.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nf.huixiangedu.cn

[S14] C：枚举
来源：http://ul.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://ek.yuntaijiaju.cn

[S15] C：类型转换
来源：http://mj.huanxung.cn

(double) a / b
来源：http://ms.9csxet.cn

[S16] C：位操作置位
来源：http://jy.szsharing.cn

x |= (1 << 3);
来源：http://wa.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://ff.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://la.bookmarksfly.cn

[S18] C：命令行参数
来源：http://pc.huanxung.cn

int main(int argc, char **argv)
来源：http://vh.hahajie.cn

[S19] C：快速排序
来源：http://ph.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yv.huixiangedu.cn

[S20] C：二分查找
来源：http://ea.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bo.shtwfgs.cn

[S21] C：字符类别判断
来源：http://gk.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://er.shxzukj.cn

[S22] C：字符串转数字
来源：http://bx.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ri.szsharing.cn

[S23] C：随机数
来源：http://cn.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://po.colortex.cn

[S24] C：获取本地时间
来源：http://xl.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://un.muxihuayi.cn

[S25] C：内存拷贝
来源：http://dx.szxytkj.cn

memcpy(dst, src, n);
来源：http://ct.muxihuayi.cn

[S26] C：内存清零
来源：http://hf.asd995.cn

memset(a, 0, sizeof a);
来源：http://nd.jianghongdianzi.cn

[S27] C：定义常量
来源：http://ye.gzmigu.cn

const double PI = 3.14159;
来源：http://kp.chemitech.net.cn

[S28] C：静态变量
来源：http://ug.gzmigu.cn

static int counter = 0;
来源：http://vu.shxzukj.cn

[S29] C：变参函数
来源：http://cr.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://om.shxzskj.cn

[S30] C：头文件保护
来源：http://bq.huixiangedu.cn

#ifndef X_H
来源：http://lo.jianghongdianzi.cn

#define X_H
来源：http://qy.szxytkj.cn

#endif
来源：http://wx.asd995.cn

[S31] C++：Hello World
来源：http://ch.panjiajie.cn

#include <iostream>
来源：http://nt.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://yl.panjiajie.cn

[S32] C++：字符串
来源：http://gk.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://qy.asd995.cn

[S33] C++：vector 增删
来源：http://rn.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pi.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://ag.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://ss.hahajie.cn

[S35] C++：map
来源：http://lu.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ov.huixiangedu.cn

[S36] C++：unordered_map
来源：http://yu.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ze.hahajie.cn

[S37] C++：set
来源：http://gd.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wu.jianghongdianzi.cn

[S38] C++：排序
来源：http://oi.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://wx.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://gk.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gm.chemitech.net.cn

[S40] C++：查找元素
来源：http://wv.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fd.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://ft.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://px.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://ek.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://ev.9csxet.cn

[S43] C++：智能指针
来源：http://al.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://tr.lnxyls.cn

[S44] C++：引用传参
来源：http://xd.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://yh.shtwfgs.cn

[S45] C++：lambda
来源：http://zk.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ew.asd995.cn

[S46] C++：函数模板
来源：http://uv.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jt.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://zl.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qt.szsharing.cn

[S48] C++：逐行读文件
来源：http://ij.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zt.521024.cn

while (std::getline(in, line)) { }
来源：http://uq.chemitech.net.cn

[S49] C++：写文件
来源：http://wx.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pn.gzmigu.cn

[S50] C++：格式化数字
来源：http://wq.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kj.newstarts.cn

[S51] C++：显式类型转换
来源：http://qi.bjjhwx.cn

static_cast<double>(a) / b
来源：http://uu.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://dm.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://ws.szsharing.cn

[S53] C++：移动语义
来源：http://jc.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://pw.nszjky.cn

[S54] C++：异常处理
来源：http://rr.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sx.gzmigu.cn

[S55] C++：结构化绑定
来源：http://do.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mp.nszjky.cn

[S56] C++：optional
来源：http://ds.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fb.haigaiapp.cn

[S57] C++：编译期常量
来源：http://mf.asd995.cn

constexpr int N = 10;
来源：http://xd.panjiajie.cn

[S58] C++：命名空间
来源：http://ee.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://rv.gzmigu.cn

[S59] C++：静态断言
来源：http://mj.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jq.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://uo.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wx.yuexingan06.cn

================================================================================
来源：http://uk.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oa.muxihuayi.cn

================================================================================
来源：http://wt.9csxet.cn

[T01] Kotlin：Hello World
来源：http://zd.nszjky.cn

println("Hello")
来源：http://vu.yuexingan06.cn

[T02] Kotlin：变量
来源：http://op.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kn.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://yh.jianghongdianzi.cn

"值: $b"
来源：http://zi.asd995.cn

[T04] Kotlin：空安全
来源：http://sa.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://cp.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://jp.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ih.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://rv.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vd.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://ii.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eb.panjiajie.cn

[T08] Kotlin：数据类
来源：http://gm.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://au.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://pc.521024.cn

fun String.exclaim() = this + "!"
来源：http://hx.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://fr.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jq.hahajie.cn

[T11] Kotlin：协程
来源：http://ei.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hr.nicolike.cn

[T12] Kotlin：解构声明
来源：http://uj.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://gx.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://zc.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://sq.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://ae.hnjuh.cn

for (i in 1..10) println(i)
来源：http://bc.9csxet.cn

[T15] Kotlin：接口
来源：http://fd.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://uq.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://uc.panjiajie.cn

print("Hello")
来源：http://wt.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://hl.muxihuayi.cn

var a = 1;  let b = 2
来源：http://mw.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://mo.jianghongdianzi.cn

"值: \(b)"
来源：http://bd.colortex.cn

[T19] Swift：可选绑定
来源：http://fm.jctech888.com.cn

if let n = opt { print(n) }
来源：http://wd.newstarts.cn

[T20] Swift：数组操作
来源：http://ta.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yk.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://rm.shtwfgs.cn

for x in a { print(x) }
来源：http://ke.haigaiapp.cn

[T22] Swift：字典
来源：http://xg.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lr.huanxung.cn

[T23] Swift：函数
来源：http://fi.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cw.wgjwhj.cn

[T24] Swift：闭包
来源：http://py.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vq.gzmigu.cn

[T25] Swift：结构体
来源：http://qe.huanxung.cn

struct P { var x: Int }
来源：http://pg.hnjuh.cn

[T26] Swift：类与重写
来源：http://fv.szxytkj.cn

class A: Base { override func f() {} }
来源：http://tj.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://vf.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ab.shtwfgs.cn

[T28] Swift：枚举
来源：http://gj.yuntaijiaju.cn

enum Color { case red, green }
来源：http://xo.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://zv.nszjky.cn

guard let x = opt else { return }
来源：http://dd.panjiajie.cn

[T30] Swift：协议
来源：http://oi.asd995.cn

protocol Shape { func area() -> Double }
来源：http://mx.521024.cn

[T31] Lua：Hello World
来源：http://az.huixinmuqiang.cn

print("Hello")
来源：http://pl.nszjky.cn

[T32] Lua：局部变量
来源：http://gz.shxzskj.cn

local a = 1
来源：http://ez.colortex.cn

[T33] Lua：表（数组）
来源：http://ye.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rq.szxytkj.cn

[T34] Lua：遍历表
来源：http://lg.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ao.wgjwhj.cn

[T35] Lua：字典表
来源：http://ly.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://qk.newstarts.cn

[T36] Lua：函数
来源：http://ot.shxzskj.cn

function add(a, b) return a + b end
来源：http://nj.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://hn.szsharing.cn

"a" .. "b"
来源：http://eg.shxzskj.cn

[T38] Lua：条件
来源：http://pm.lnxyls.cn

if x > 0 then print("正") end
来源：http://fj.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://ls.haigaiapp.cn

string.find(s, "%d+")
来源：http://si.huixiangedu.cn

[T40] Lua：元表
来源：http://kh.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://lq.hahajie.cn

[T41] Perl：Hello World
来源：http://hq.yuntaijiaju.cn

print "Hello\n";
来源：http://qu.wgjwhj.cn

[T42] Perl：变量类型
来源：http://zv.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mz.newstarts.cn

[T43] Perl：字符串插值
来源：http://pg.shtwfgs.cn

"值: $a"
来源：http://fn.szsharing.cn

[T44] Perl：条件
来源：http://me.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://ra.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://ci.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://vg.lnxyls.cn

[T46] Perl：哈希操作
来源：http://wf.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yi.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://fc.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sv.shtwfgs.cn

[T48] Perl：正则替换
来源：http://st.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://kh.lnxyls.cn

[T49] Perl：函数
来源：http://ox.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yi.hahajie.cn

[T50] Perl：逐行读文件
来源：http://iu.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qx.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://ax.wgjwhj.cn

[T51] Scala：Hello World
来源：http://qt.szsharing.cn

println("Hello")
来源：http://ba.wgjwhj.cn

[T52] Scala：变量
来源：http://mr.asd995.cn

val a = 1;  var b = 2
来源：http://um.hahajie.cn

[T53] Scala：字符串插值
来源：http://td.wgjwhj.cn

s"值: $b"
来源：http://ry.gzmigu.cn

[T54] Scala：集合映射
来源：http://fh.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://nn.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://lw.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kc.lnxyls.cn

[T56] Scala：样例类
来源：http://zv.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ty.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://ow.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ga.panjiajie.cn

[T58] Scala：函数定义
来源：http://ib.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tj.huixinmuqiang.cn

[T59] Scala：循环
来源：http://me.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://qa.hahajie.cn

[T60] Scala：折叠
来源：http://er.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wt.colortex.cn

================================================================================
来源：http://az.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cb.shtwfgs.cn

================================================================================
来源：http://bf.lnxyls.cn


<!-- 参考信息 -->