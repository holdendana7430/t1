代发 wailian999

ssh user@host 'uptime'
来源：http://ct.huanxung.cn

[R58] 下载文件
来源：http://tp.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ko.shxzukj.cn

[R59] 发 POST JSON
来源：http://xb.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yg.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://af.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vs.shxzukj.cn

[R61] 磁盘占用
来源：http://bq.shxzskj.cn

df -h;  du -sh *
来源：http://jl.huanxung.cn

[R62] 找最占空间的文件
来源：http://ts.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://ag.jianghongdianzi.cn

[R63] 内存与进程
来源：http://jn.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://vy.wgjwhj.cn

[R64] 结束进程
来源：http://td.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://yt.asd995.cn

[R65] 查看端口占用
来源：http://yi.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zl.huixinmuqiang.cn

[R66] 定时任务
来源：http://hf.nszjky.cn

crontab -e;  crontab -l
来源：http://xc.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://it.bjjhwx.cn

openssl rand -hex 16
来源：http://hv.jctech888.com.cn

[R68] 计算文件校验值
来源：http://uk.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vg.lnxyls.cn

[R69] 生成随机密码
来源：http://hv.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://dz.shxzskj.cn

[R70] 时间戳与互转
来源：http://le.nicolike.cn

date +%s;  date -d @1700000000
来源：http://sv.yuexingan06.cn

[R71] 日期格式化
来源：http://ss.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bn.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://jp.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mi.szxytkj.cn

[R73] 分割大日志
来源：http://sr.newstarts.cn

split -l 1000 big.log part_
来源：http://fl.gzmigu.cn

[R74] 批量重命名
来源：http://ba.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bi.shtwfgs.cn

[R75] 导出环境变量
来源：http://yx.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://sv.nszjky.cn

[R76] 使用临时文件
来源：http://px.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://up.hnjuh.cn

[R77] 读取用户输入
来源：http://fk.colortex.cn

read -rp "请输入: " ans
来源：http://zu.muxihuayi.cn

[R78] 交互式菜单
来源：http://tn.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hx.huixiangedu.cn

[R79] 解析命令行选项
来源：http://fg.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qq.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://ao.521024.cn

time ./run.sh
来源：http://pk.9csxet.cn

================================================================================
来源：http://ht.bjjhwx.cn

S. C / C++ 专题
来源：http://sc.colortex.cn

================================================================================
来源：http://le.jctech888.com.cn

[S01] C：Hello World
来源：http://mk.colortex.cn

#include <stdio.h>
来源：http://wi.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://it.asd995.cn

[S02] C：变量与格式化输出
来源：http://ml.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://ll.colortex.cn

[S03] C：读入整数
来源：http://eh.colortex.cn

int x; scanf("%d", &x);
来源：http://oj.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://gw.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cg.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://ut.szxytkj.cn

strlen(s)
来源：http://qe.521024.cn

[S06] C：字符串比较
来源：http://zn.asd995.cn

strcmp(a, b) == 0
来源：http://ln.newstarts.cn

[S07] C：数组遍历求和
来源：http://af.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yf.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://vt.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ma.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://yu.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nj.shtwfgs.cn

[S10] C：指针与解引用
来源：http://me.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://ff.9csxet.cn

[S11] C：逐行读文件
来源：http://uc.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://wn.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jd.bookmarksfly.cn

fclose(f);
来源：http://gs.shxzskj.cn

[S12] C：写文件
来源：http://vr.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bc.nszjky.cn

[S13] C：宏定义
来源：http://da.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jo.newstarts.cn

[S14] C：枚举
来源：http://zg.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://yv.wgjwhj.cn

[S15] C：类型转换
来源：http://ae.nicolike.cn

(double) a / b
来源：http://nz.newstarts.cn

[S16] C：位操作置位
来源：http://it.huanxung.cn

x |= (1 << 3);
来源：http://iq.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://xn.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fi.bjjhwx.cn

[S18] C：命令行参数
来源：http://ys.shtwfgs.cn

int main(int argc, char **argv)
来源：http://fe.yuntaijiaju.cn

[S19] C：快速排序
来源：http://vq.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://np.bookmarksfly.cn

[S20] C：二分查找
来源：http://wr.9csxet.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://og.szsharing.cn

[S21] C：字符类别判断
来源：http://oh.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ac.huixiangedu.cn

[S22] C：字符串转数字
来源：http://pf.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://di.nszjky.cn

[S23] C：随机数
来源：http://ab.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xl.nszjky.cn

[S24] C：获取本地时间
来源：http://io.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qq.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ki.szsharing.cn

memcpy(dst, src, n);
来源：http://rr.lnxyls.cn

[S26] C：内存清零
来源：http://ae.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ot.bookmarksfly.cn

[S27] C：定义常量
来源：http://uo.gzmigu.cn

const double PI = 3.14159;
来源：http://zn.shtwfgs.cn

[S28] C：静态变量
来源：http://mu.shxzskj.cn

static int counter = 0;
来源：http://bn.shxzskj.cn

[S29] C：变参函数
来源：http://bp.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qe.szsharing.cn

[S30] C：头文件保护
来源：http://tj.shxzskj.cn

#ifndef X_H
来源：http://ke.chemitech.net.cn

#define X_H
来源：http://le.yuexingan06.cn

#endif
来源：http://tu.muxihuayi.cn

[S31] C++：Hello World
来源：http://qo.gzmigu.cn

#include <iostream>
来源：http://hl.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://ty.9csxet.cn

[S32] C++：字符串
来源：http://sr.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://bx.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://vu.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wp.huanxung.cn

[S34] C++：遍历 vector
来源：http://zq.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://bh.huixiangedu.cn

[S35] C++：map
来源：http://qk.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mr.nicolike.cn

[S36] C++：unordered_map
来源：http://md.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lz.huixinmuqiang.cn

[S37] C++：set
来源：http://fi.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xn.nicolike.cn

[S38] C++：排序
来源：http://dr.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://ke.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://ur.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hahajie.cn

[S40] C++：查找元素
来源：http://wq.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ul.asd995.cn

[S41] C++：类与构造函数
来源：http://tf.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oq.9csxet.cn

[S42] C++：继承与虚函数
来源：http://he.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://xq.nszjky.cn

[S43] C++：智能指针
来源：http://ib.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://ky.shtwfgs.cn

[S44] C++：引用传参
来源：http://je.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://sq.jianghongdianzi.cn

[S45] C++：lambda
来源：http://bt.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uq.nszjky.cn

[S46] C++：函数模板
来源：http://po.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xy.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://iq.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mk.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://jf.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fk.9csxet.cn

while (std::getline(in, line)) { }
来源：http://to.yuntaijiaju.cn

[S49] C++：写文件
来源：http://jc.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zz.nicolike.cn

[S50] C++：格式化数字
来源：http://xl.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ui.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://sh.newstarts.cn

static_cast<double>(a) / b
来源：http://ii.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://vn.asd995.cn

int size() const noexcept { return n_; }
来源：http://dc.newstarts.cn

[S53] C++：移动语义
来源：http://ov.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://pt.panjiajie.cn

[S54] C++：异常处理
来源：http://cc.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fd.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://bc.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pu.huixinmuqiang.cn

[S56] C++：optional
来源：http://ed.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lh.szsharing.cn

[S57] C++：编译期常量
来源：http://di.chemitech.net.cn

constexpr int N = 10;
来源：http://eq.hahajie.cn

[S58] C++：命名空间
来源：http://jv.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://jm.yuexingan06.cn

[S59] C++：静态断言
来源：http://xr.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cq.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://wc.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vk.nicolike.cn

================================================================================
来源：http://zg.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://th.hnjuh.cn

================================================================================
来源：http://vi.9csxet.cn

[T01] Kotlin：Hello World
来源：http://wh.muxihuayi.cn

println("Hello")
来源：http://up.shxzskj.cn

[T02] Kotlin：变量
来源：http://nm.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ba.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://sx.huixiangedu.cn

"值: $b"
来源：http://wx.nicolike.cn

[T04] Kotlin：空安全
来源：http://lp.nicolike.cn

val n: String? = null;  n?.length
来源：http://ih.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ew.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bl.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://xf.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fm.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://qr.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ud.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://yq.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://st.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://uu.521024.cn

fun String.exclaim() = this + "!"
来源：http://bi.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://dm.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ga.panjiajie.cn

[T11] Kotlin：协程
来源：http://zt.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bc.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://le.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://rs.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://de.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://ht.lnxyls.cn

[T14] Kotlin：循环
来源：http://zz.colortex.cn

for (i in 1..10) println(i)
来源：http://at.nszjky.cn

[T15] Kotlin：接口
来源：http://bc.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://ou.haigaiapp.cn

[T16] Swift：Hello World
来源：http://qn.nszjky.cn

print("Hello")
来源：http://qv.shxzukj.cn

[T17] Swift：变量与常量
来源：http://ks.asd995.cn

var a = 1;  let b = 2
来源：http://vn.hnjuh.cn

[T18] Swift：字符串插值
来源：http://en.jctech888.com.cn

"值: \(b)"
来源：http://ez.szxytkj.cn

[T19] Swift：可选绑定
来源：http://qm.szsharing.cn

if let n = opt { print(n) }
来源：http://hy.newstarts.cn

[T20] Swift：数组操作
来源：http://se.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lb.haigaiapp.cn

[T21] Swift：遍历
来源：http://jk.chemitech.net.cn

for x in a { print(x) }
来源：http://nw.huixinmuqiang.cn

[T22] Swift：字典
来源：http://ey.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kf.bjjhwx.cn

[T23] Swift：函数
来源：http://ax.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ti.gzmigu.cn

[T24] Swift：闭包
来源：http://dr.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zd.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://pb.colortex.cn

struct P { var x: Int }
来源：http://tp.panjiajie.cn

[T26] Swift：类与重写
来源：http://dz.huanxung.cn

class A: Base { override func f() {} }
来源：http://bg.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://vh.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://yd.shtwfgs.cn

[T28] Swift：枚举
来源：http://dv.jctech888.com.cn

enum Color { case red, green }
来源：http://uw.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://em.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://hu.huixinmuqiang.cn

[T30] Swift：协议
来源：http://ye.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://mm.hnjuh.cn

[T31] Lua：Hello World
来源：http://tm.panjiajie.cn

print("Hello")
来源：http://vi.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://zm.muxihuayi.cn

local a = 1
来源：http://kz.szxytkj.cn

[T33] Lua：表（数组）
来源：http://oh.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aw.hahajie.cn

[T34] Lua：遍历表
来源：http://kt.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gj.muxihuayi.cn

[T35] Lua：字典表
来源：http://ek.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://ev.huanxung.cn

[T36] Lua：函数
来源：http://ik.huixiangedu.cn

function add(a, b) return a + b end
来源：http://vy.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://dv.bookmarksfly.cn

"a" .. "b"
来源：http://my.521024.cn

[T38] Lua：条件
来源：http://yq.chemitech.net.cn

if x > 0 then print("正") end
来源：http://iq.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://li.521024.cn

string.find(s, "%d+")
来源：http://bj.chemitech.net.cn

[T40] Lua：元表
来源：http://bg.huanxung.cn

setmetatable({}, { __index = base })
来源：http://kj.hnjuh.cn

[T41] Perl：Hello World
来源：http://qq.nszjky.cn

print "Hello\n";
来源：http://rx.haigaiapp.cn

[T42] Perl：变量类型
来源：http://jh.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ba.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://kc.jctech888.com.cn

"值: $a"
来源：http://oq.muxihuayi.cn

[T44] Perl：条件
来源：http://rr.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://ri.nicolike.cn

[T45] Perl：数组遍历
来源：http://pt.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://jf.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://bq.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ef.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://pa.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bv.szsharing.cn

[T48] Perl：正则替换
来源：http://pt.newstarts.cn

$s =~ s/old/new/g;
来源：http://zu.bookmarksfly.cn

[T49] Perl：函数
来源：http://as.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vj.asd995.cn

[T50] Perl：逐行读文件
来源：http://sg.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vu.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://sb.panjiajie.cn

[T51] Scala：Hello World
来源：http://iq.shtwfgs.cn

println("Hello")
来源：http://sh.szsharing.cn

[T52] Scala：变量
来源：http://py.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://un.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://ib.jianghongdianzi.cn

s"值: $b"
来源：http://nd.hnjuh.cn

[T54] Scala：集合映射
来源：http://tu.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://wx.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://uk.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wb.lnxyls.cn

[T56] Scala：样例类
来源：http://tw.nicolike.cn

case class User(name: String, age: Int)
来源：http://kr.shxzukj.cn

[T57] Scala：模式匹配
来源：http://up.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qz.chemitech.net.cn

[T58] Scala：函数定义
来源：http://ur.chemitech.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ri.szsharing.cn

[T59] Scala：循环
来源：http://jt.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://ut.521024.cn

[T60] Scala：折叠
来源：http://pf.9csxet.cn


<!-- 参考信息 -->