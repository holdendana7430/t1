代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://at.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://dk.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jy.wgjwhj.cn

[R61] 磁盘占用
来源：http://ts.9csxet.cn

df -h;  du -sh *
来源：http://mg.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://op.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://oe.shxzskj.cn

[R63] 内存与进程
来源：http://zm.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ux.huixiangedu.cn

[R64] 结束进程
来源：http://qu.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://hp.shtwfgs.cn

[R65] 查看端口占用
来源：http://mk.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fu.huanxung.cn

[R66] 定时任务
来源：http://pl.panjiajie.cn

crontab -e;  crontab -l
来源：http://cb.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://ef.521024.cn

openssl rand -hex 16
来源：http://lv.bjjhwx.cn

[R68] 计算文件校验值
来源：http://ey.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uv.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://vh.521024.cn

head -c 16 /dev/urandom | base64
来源：http://gy.asd995.cn

[R70] 时间戳与互转
来源：http://wl.nszjky.cn

date +%s;  date -d @1700000000
来源：http://bp.jctech888.com.cn

[R71] 日期格式化
来源：http://ni.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ea.nicolike.cn

[R72] 等待端口就绪
来源：http://mr.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ii.wgjwhj.cn

[R73] 分割大日志
来源：http://gt.shxzukj.cn

split -l 1000 big.log part_
来源：http://rs.nicolike.cn

[R74] 批量重命名
来源：http://pt.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jm.nszjky.cn

[R75] 导出环境变量
来源：http://ez.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://mr.wgjwhj.cn

[R76] 使用临时文件
来源：http://vq.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kp.haigaiapp.cn

[R77] 读取用户输入
来源：http://jp.panjiajie.cn

read -rp "请输入: " ans
来源：http://eb.nszjky.cn

[R78] 交互式菜单
来源：http://wl.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ro.nszjky.cn

[R79] 解析命令行选项
来源：http://qc.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jb.asd995.cn

[R80] 查看脚本执行耗时
来源：http://ku.lnxyls.cn

time ./run.sh
来源：http://mr.jianghongdianzi.cn

================================================================================
来源：http://nl.bjjhwx.cn

S. C / C++ 专题
来源：http://bc.9csxet.cn

================================================================================
来源：http://gn.panjiajie.cn

[S01] C：Hello World
来源：http://nd.shtwfgs.cn

#include <stdio.h>
来源：http://ma.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fz.nicolike.cn

[S02] C：变量与格式化输出
来源：http://yl.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://jl.shtwfgs.cn

[S03] C：读入整数
来源：http://vu.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://up.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://fk.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tf.hnjuh.cn

[S05] C：字符串长度
来源：http://nb.asd995.cn

strlen(s)
来源：http://vi.muxihuayi.cn

[S06] C：字符串比较
来源：http://ak.szsharing.cn

strcmp(a, b) == 0
来源：http://nn.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://zj.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tn.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://sr.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://te.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://nl.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bq.haigaiapp.cn

[S10] C：指针与解引用
来源：http://sl.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://hd.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://mu.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://cr.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tt.szsharing.cn

fclose(f);
来源：http://hv.asd995.cn

[S12] C：写文件
来源：http://si.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kn.9csxet.cn

[S13] C：宏定义
来源：http://li.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://be.bjjhwx.cn

[S14] C：枚举
来源：http://ee.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://vs.shxzukj.cn

[S15] C：类型转换
来源：http://gg.jctech888.com.cn

(double) a / b
来源：http://td.hnjuh.cn

[S16] C：位操作置位
来源：http://ad.wgjwhj.cn

x |= (1 << 3);
来源：http://tz.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://qx.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gl.newstarts.cn

[S18] C：命令行参数
来源：http://uj.hahajie.cn

int main(int argc, char **argv)
来源：http://xk.nicolike.cn

[S19] C：快速排序
来源：http://jn.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zb.muxihuayi.cn

[S20] C：二分查找
来源：http://ya.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kf.huixiangedu.cn

[S21] C：字符类别判断
来源：http://ni.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gx.lnxyls.cn

[S22] C：字符串转数字
来源：http://pg.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nb.yuntaijiaju.cn

[S23] C：随机数
来源：http://qy.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mx.chemitech.net.cn

[S24] C：获取本地时间
来源：http://qf.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vv.panjiajie.cn

[S25] C：内存拷贝
来源：http://ih.yuexingan06.cn

memcpy(dst, src, n);
来源：http://ox.521024.cn

[S26] C：内存清零
来源：http://rc.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://gj.newstarts.cn

[S27] C：定义常量
来源：http://sw.szsharing.cn

const double PI = 3.14159;
来源：http://ad.hahajie.cn

[S28] C：静态变量
来源：http://yn.shxzukj.cn

static int counter = 0;
来源：http://wf.muxihuayi.cn

[S29] C：变参函数
来源：http://zv.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mb.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://ox.yuexingan06.cn

#ifndef X_H
来源：http://aq.hnjuh.cn

#define X_H
来源：http://wc.huanxung.cn

#endif
来源：http://bk.muxihuayi.cn

[S31] C++：Hello World
来源：http://yo.szsharing.cn

#include <iostream>
来源：http://sk.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://qe.nicolike.cn

[S32] C++：字符串
来源：http://lw.colortex.cn

std::string s = "hi";  s += "!";
来源：http://dl.521024.cn

[S33] C++：vector 增删
来源：http://hb.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rl.panjiajie.cn

[S34] C++：遍历 vector
来源：http://jh.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://zc.newstarts.cn

[S35] C++：map
来源：http://yr.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ly.gzmigu.cn

[S36] C++：unordered_map
来源：http://bn.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wi.wgjwhj.cn

[S37] C++：set
来源：http://rr.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zz.shxzskj.cn

[S38] C++：排序
来源：http://bz.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://ex.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://dz.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nw.muxihuayi.cn

[S40] C++：查找元素
来源：http://kr.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xb.panjiajie.cn

[S41] C++：类与构造函数
来源：http://hx.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hd.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://gr.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://to.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://mt.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://rw.haigaiapp.cn

[S44] C++：引用传参
来源：http://yd.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://qh.bjjhwx.cn

[S45] C++：lambda
来源：http://lw.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rz.jctech888.com.cn

[S46] C++：函数模板
来源：http://ne.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nu.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://dc.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tn.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ku.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cz.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://iy.521024.cn

[S49] C++：写文件
来源：http://fh.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yi.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://xw.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wb.szsharing.cn

[S51] C++：显式类型转换
来源：http://er.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://ih.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://fy.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://hu.hnjuh.cn

[S53] C++：移动语义
来源：http://ao.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://wg.shtwfgs.cn

[S54] C++：异常处理
来源：http://jg.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kn.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://py.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ne.huanxung.cn

[S56] C++：optional
来源：http://tg.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ox.muxihuayi.cn

[S57] C++：编译期常量
来源：http://el.szsharing.cn

constexpr int N = 10;
来源：http://hg.9csxet.cn

[S58] C++：命名空间
来源：http://cn.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://ue.newstarts.cn

[S59] C++：静态断言
来源：http://nl.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wk.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://ur.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://su.huixinmuqiang.cn

================================================================================
来源：http://av.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ff.jianghongdianzi.cn

================================================================================
来源：http://ph.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://uc.yuntaijiaju.cn

println("Hello")
来源：http://kq.nicolike.cn

[T02] Kotlin：变量
来源：http://qq.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vq.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://pw.hahajie.cn

"值: $b"
来源：http://kg.521024.cn

[T04] Kotlin：空安全
来源：http://ft.gzmigu.cn

val n: String? = null;  n?.length
来源：http://eh.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://od.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ja.nicolike.cn

[T06] Kotlin：集合映射
来源：http://sb.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sd.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ln.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pn.nszjky.cn

[T08] Kotlin：数据类
来源：http://bf.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://ck.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://my.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://sk.521024.cn

[T10] Kotlin：默认参数
来源：http://vt.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://as.shxzukj.cn

[T11] Kotlin：协程
来源：http://rm.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ii.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://vi.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://qj.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://zw.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://ur.shxzukj.cn

[T14] Kotlin：循环
来源：http://ig.newstarts.cn

for (i in 1..10) println(i)
来源：http://eb.9csxet.cn

[T15] Kotlin：接口
来源：http://ti.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://nu.lnxyls.cn

[T16] Swift：Hello World
来源：http://qz.wgjwhj.cn

print("Hello")
来源：http://kr.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://jw.shxzukj.cn

var a = 1;  let b = 2
来源：http://pq.szxytkj.cn

[T18] Swift：字符串插值
来源：http://gz.bjjhwx.cn

"值: \(b)"
来源：http://ko.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://am.9csxet.cn

if let n = opt { print(n) }
来源：http://uv.asd995.cn

[T20] Swift：数组操作
来源：http://ks.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bk.huixiangedu.cn

[T21] Swift：遍历
来源：http://fg.jianghongdianzi.cn

for x in a { print(x) }
来源：http://eg.haigaiapp.cn

[T22] Swift：字典
来源：http://sv.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tx.nicolike.cn

[T23] Swift：函数
来源：http://ao.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hj.hnjuh.cn

[T24] Swift：闭包
来源：http://qt.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hd.shxzskj.cn

[T25] Swift：结构体
来源：http://vg.hahajie.cn

struct P { var x: Int }
来源：http://mj.bjjhwx.cn

[T26] Swift：类与重写
来源：http://as.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://hv.wgjwhj.cn

[T27] Swift：错误处理
来源：http://cc.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://ky.shxzskj.cn

[T28] Swift：枚举
来源：http://kf.yuexingan06.cn

enum Color { case red, green }
来源：http://xk.asd995.cn

[T29] Swift：guard 提前返回
来源：http://ld.shxzukj.cn

guard let x = opt else { return }
来源：http://nz.hnjuh.cn

[T30] Swift：协议
来源：http://tg.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://za.shtwfgs.cn

[T31] Lua：Hello World
来源：http://ak.9csxet.cn

print("Hello")
来源：http://xd.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://wi.hnjuh.cn

local a = 1
来源：http://vw.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://pv.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kv.nicolike.cn

[T34] Lua：遍历表
来源：http://zm.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cg.newstarts.cn

[T35] Lua：字典表
来源：http://zv.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://dr.chemitech.net.cn

[T36] Lua：函数
来源：http://tb.szsharing.cn

function add(a, b) return a + b end
来源：http://pz.nszjky.cn

[T37] Lua：字符串拼接
来源：http://ae.szsharing.cn

"a" .. "b"
来源：http://wj.bjjhwx.cn

[T38] Lua：条件
来源：http://zt.gzmigu.cn

if x > 0 then print("正") end
来源：http://gj.nicolike.cn

[T39] Lua：模式匹配
来源：http://ge.lnxyls.cn

string.find(s, "%d+")
来源：http://ln.bookmarksfly.cn

[T40] Lua：元表
来源：http://im.nszjky.cn

setmetatable({}, { __index = base })
来源：http://yb.shxzukj.cn

[T41] Perl：Hello World
来源：http://oc.chemitech.net.cn

print "Hello\n";
来源：http://ie.wgjwhj.cn

[T42] Perl：变量类型
来源：http://pq.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hl.szxytkj.cn

[T43] Perl：字符串插值
来源：http://vt.hnjuh.cn

"值: $a"
来源：http://lb.shxzskj.cn

[T44] Perl：条件
来源：http://ai.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://ls.shxzukj.cn

[T45] Perl：数组遍历
来源：http://rj.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://yc.9csxet.cn

[T46] Perl：哈希操作
来源：http://ir.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wr.hnjuh.cn

[T47] Perl：正则捕获
来源：http://tb.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vb.asd995.cn

[T48] Perl：正则替换
来源：http://dx.panjiajie.cn

$s =~ s/old/new/g;
来源：http://gn.muxihuayi.cn

[T49] Perl：函数
来源：http://jq.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dy.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://ae.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ul.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ob.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://hh.bookmarksfly.cn

println("Hello")
来源：http://ue.jctech888.com.cn

[T52] Scala：变量
来源：http://nf.colortex.cn

val a = 1;  var b = 2
来源：http://pc.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://hv.yuntaijiaju.cn

s"值: $b"
来源：http://hj.nszjky.cn

[T54] Scala：集合映射
来源：http://zy.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://kv.newstarts.cn

[T55] Scala：集合过滤
来源：http://px.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ep.haigaiapp.cn

[T56] Scala：样例类
来源：http://nr.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://nu.9csxet.cn

[T57] Scala：模式匹配
来源：http://qu.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ej.newstarts.cn

[T58] Scala：函数定义
来源：http://ed.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ls.lnxyls.cn

[T59] Scala：循环
来源：http://yt.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://hw.wgjwhj.cn

[T60] Scala：折叠
来源：http://vh.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ih.hahajie.cn

================================================================================
来源：http://nx.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kg.szsharing.cn

================================================================================
来源：http://hx.hnjuh.cn


<!-- 参考信息 -->