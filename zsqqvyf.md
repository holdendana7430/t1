代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vf.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://eb.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dp.shtwfgs.cn

[R61] 磁盘占用
来源：http://ic.lnxyls.cn

df -h;  du -sh *
来源：http://gx.hnjuh.cn

[R62] 找最占空间的文件
来源：http://lj.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://ui.bookmarksfly.cn

[R63] 内存与进程
来源：http://pu.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://yz.jianghongdianzi.cn

[R64] 结束进程
来源：http://xg.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://yo.colortex.cn

[R65] 查看端口占用
来源：http://ka.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fw.yuexingan06.cn

[R66] 定时任务
来源：http://dc.wgjwhj.cn

crontab -e;  crontab -l
来源：http://kn.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://fd.yuexingan06.cn

openssl rand -hex 16
来源：http://gr.newstarts.cn

[R68] 计算文件校验值
来源：http://ex.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gx.lnxyls.cn

[R69] 生成随机密码
来源：http://rf.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://lw.lnxyls.cn

[R70] 时间戳与互转
来源：http://tv.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://hq.huixiangedu.cn

[R71] 日期格式化
来源：http://ae.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wf.asd995.cn

[R72] 等待端口就绪
来源：http://vy.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ja.panjiajie.cn

[R73] 分割大日志
来源：http://xu.newstarts.cn

split -l 1000 big.log part_
来源：http://gk.shxzskj.cn

[R74] 批量重命名
来源：http://yn.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ww.9csxet.cn

[R75] 导出环境变量
来源：http://pb.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://pn.haigaiapp.cn

[R76] 使用临时文件
来源：http://ap.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hu.haigaiapp.cn

[R77] 读取用户输入
来源：http://lb.yuexingan06.cn

read -rp "请输入: " ans
来源：http://dt.chemitech.net.cn

[R78] 交互式菜单
来源：http://iq.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://we.shxzukj.cn

[R79] 解析命令行选项
来源：http://gu.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ty.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://bw.hahajie.cn

time ./run.sh
来源：http://sq.yuntaijiaju.cn

================================================================================
来源：http://fr.panjiajie.cn

S. C / C++ 专题
来源：http://if.nszjky.cn

================================================================================
来源：http://pm.lnxyls.cn

[S01] C：Hello World
来源：http://gz.huixiangedu.cn

#include <stdio.h>
来源：http://db.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ci.hahajie.cn

[S02] C：变量与格式化输出
来源：http://sj.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://iy.szxytkj.cn

[S03] C：读入整数
来源：http://rf.asd995.cn

int x; scanf("%d", &x);
来源：http://oc.gzmigu.cn

[S04] C：字符串复制
来源：http://ua.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lc.chemitech.net.cn

[S05] C：字符串长度
来源：http://qk.shxzukj.cn

strlen(s)
来源：http://fy.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://tf.shxzskj.cn

strcmp(a, b) == 0
来源：http://jq.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://tr.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jq.521024.cn

[S08] C：动态内存分配与释放
来源：http://xi.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://en.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://zf.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ob.hahajie.cn

[S10] C：指针与解引用
来源：http://yg.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ck.haigaiapp.cn

[S11] C：逐行读文件
来源：http://xv.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://kv.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bq.shxzukj.cn

fclose(f);
来源：http://hg.asd995.cn

[S12] C：写文件
来源：http://rn.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qc.bjjhwx.cn

[S13] C：宏定义
来源：http://lv.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cr.muxihuayi.cn

[S14] C：枚举
来源：http://rh.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://pj.shtwfgs.cn

[S15] C：类型转换
来源：http://fh.nszjky.cn

(double) a / b
来源：http://vj.521024.cn

[S16] C：位操作置位
来源：http://vs.shxzskj.cn

x |= (1 << 3);
来源：http://gw.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ay.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oz.szsharing.cn

[S18] C：命令行参数
来源：http://em.szsharing.cn

int main(int argc, char **argv)
来源：http://rw.lnxyls.cn

[S19] C：快速排序
来源：http://lo.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jb.yuexingan06.cn

[S20] C：二分查找
来源：http://ag.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oh.asd995.cn

[S21] C：字符类别判断
来源：http://gn.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mp.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://tm.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jq.hnjuh.cn

[S23] C：随机数
来源：http://vd.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xo.asd995.cn

[S24] C：获取本地时间
来源：http://dd.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ih.9csxet.cn

[S25] C：内存拷贝
来源：http://ip.hahajie.cn

memcpy(dst, src, n);
来源：http://qg.haigaiapp.cn

[S26] C：内存清零
来源：http://iq.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://ra.jctech888.com.cn

[S27] C：定义常量
来源：http://nw.chemitech.net.cn

const double PI = 3.14159;
来源：http://vv.nszjky.cn

[S28] C：静态变量
来源：http://jp.hnjuh.cn

static int counter = 0;
来源：http://rh.521024.cn

[S29] C：变参函数
来源：http://am.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://an.asd995.cn

[S30] C：头文件保护
来源：http://iv.bjjhwx.cn

#ifndef X_H
来源：http://iy.gzmigu.cn

#define X_H
来源：http://hj.bjjhwx.cn

#endif
来源：http://za.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://gw.chemitech.net.cn

#include <iostream>
来源：http://gl.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://ix.hahajie.cn

[S32] C++：字符串
来源：http://kl.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://ue.bjjhwx.cn

[S33] C++：vector 增删
来源：http://vy.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nz.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://va.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://ig.huixinmuqiang.cn

[S35] C++：map
来源：http://lb.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gh.haigaiapp.cn

[S36] C++：unordered_map
来源：http://sx.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mo.yuntaijiaju.cn

[S37] C++：set
来源：http://ib.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cc.panjiajie.cn

[S38] C++：排序
来源：http://dd.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://tw.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://xj.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ol.szxytkj.cn

[S40] C++：查找元素
来源：http://iw.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://io.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://bw.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cg.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://vj.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://qu.lnxyls.cn

[S43] C++：智能指针
来源：http://qk.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://fy.huanxung.cn

[S44] C++：引用传参
来源：http://ik.nicolike.cn

void inc(int &x) { ++x; }
来源：http://er.szsharing.cn

[S45] C++：lambda
来源：http://cr.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gg.chemitech.net.cn

[S46] C++：函数模板
来源：http://mg.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gi.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://wo.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ih.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://zu.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yn.colortex.cn

while (std::getline(in, line)) { }
来源：http://vn.nszjky.cn

[S49] C++：写文件
来源：http://qn.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ow.shxzukj.cn

[S50] C++：格式化数字
来源：http://es.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tt.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://xb.hnjuh.cn

static_cast<double>(a) / b
来源：http://hr.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://no.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://ud.muxihuayi.cn

[S53] C++：移动语义
来源：http://pz.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://jy.hahajie.cn

[S54] C++：异常处理
来源：http://kg.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sj.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://xz.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://og.521024.cn

[S56] C++：optional
来源：http://nn.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tg.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://tt.jianghongdianzi.cn

constexpr int N = 10;
来源：http://pz.bjjhwx.cn

[S58] C++：命名空间
来源：http://vw.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://po.huixiangedu.cn

[S59] C++：静态断言
来源：http://sc.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gk.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://ug.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sc.huanxung.cn

================================================================================
来源：http://fc.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://er.jctech888.com.cn

================================================================================
来源：http://fq.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://si.panjiajie.cn

println("Hello")
来源：http://zq.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://sa.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jc.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://ar.hnjuh.cn

"值: $b"
来源：http://vm.521024.cn

[T04] Kotlin：空安全
来源：http://lf.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://iu.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://nv.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sm.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://te.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rt.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://fy.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iz.shxzskj.cn

[T08] Kotlin：数据类
来源：http://nf.521024.cn

data class User(val name: String, val age: Int)
来源：http://sr.colortex.cn

[T09] Kotlin：扩展函数
来源：http://tv.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://dt.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://ex.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wm.nicolike.cn

[T11] Kotlin：协程
来源：http://kh.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wz.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://be.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://kv.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://zb.hahajie.cn

val m = mapOf("a" to 1)
来源：http://mc.bjjhwx.cn

[T14] Kotlin：循环
来源：http://mu.lnxyls.cn

for (i in 1..10) println(i)
来源：http://qe.gzmigu.cn

[T15] Kotlin：接口
来源：http://al.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://wq.9csxet.cn

[T16] Swift：Hello World
来源：http://qv.panjiajie.cn

print("Hello")
来源：http://rl.panjiajie.cn

[T17] Swift：变量与常量
来源：http://cl.9csxet.cn

var a = 1;  let b = 2
来源：http://uc.shxzukj.cn

[T18] Swift：字符串插值
来源：http://pi.szsharing.cn

"值: \(b)"
来源：http://jm.asd995.cn

[T19] Swift：可选绑定
来源：http://yb.nicolike.cn

if let n = opt { print(n) }
来源：http://br.newstarts.cn

[T20] Swift：数组操作
来源：http://ys.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rh.shtwfgs.cn

[T21] Swift：遍历
来源：http://qf.nszjky.cn

for x in a { print(x) }
来源：http://oi.yuntaijiaju.cn

[T22] Swift：字典
来源：http://eu.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ws.521024.cn

[T23] Swift：函数
来源：http://hg.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hk.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://ll.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aa.muxihuayi.cn

[T25] Swift：结构体
来源：http://hz.bookmarksfly.cn

struct P { var x: Int }
来源：http://jo.huanxung.cn

[T26] Swift：类与重写
来源：http://fi.9csxet.cn

class A: Base { override func f() {} }
来源：http://yk.lnxyls.cn

[T27] Swift：错误处理
来源：http://oa.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://qx.asd995.cn

[T28] Swift：枚举
来源：http://ec.bjjhwx.cn

enum Color { case red, green }
来源：http://bd.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://cw.panjiajie.cn

guard let x = opt else { return }
来源：http://so.huixiangedu.cn

[T30] Swift：协议
来源：http://pj.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://xc.yuexingan06.cn

[T31] Lua：Hello World
来源：http://hq.bjjhwx.cn

print("Hello")
来源：http://fx.shxzukj.cn

[T32] Lua：局部变量
来源：http://mu.huixiangedu.cn

local a = 1
来源：http://zi.asd995.cn

[T33] Lua：表（数组）
来源：http://rt.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://st.haigaiapp.cn

[T34] Lua：遍历表
来源：http://ba.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fk.nicolike.cn

[T35] Lua：字典表
来源：http://qb.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://va.hahajie.cn

[T36] Lua：函数
来源：http://zj.asd995.cn

function add(a, b) return a + b end
来源：http://mb.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://ij.huixiangedu.cn

"a" .. "b"
来源：http://ct.hahajie.cn

[T38] Lua：条件
来源：http://aa.colortex.cn

if x > 0 then print("正") end
来源：http://zg.shxzskj.cn

[T39] Lua：模式匹配
来源：http://zk.nszjky.cn

string.find(s, "%d+")
来源：http://zx.gzmigu.cn

[T40] Lua：元表
来源：http://br.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://uw.szsharing.cn

[T41] Perl：Hello World
来源：http://zk.yuntaijiaju.cn

print "Hello\n";
来源：http://ly.haigaiapp.cn

[T42] Perl：变量类型
来源：http://fu.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hn.asd995.cn

[T43] Perl：字符串插值
来源：http://de.hahajie.cn

"值: $a"
来源：http://gl.lnxyls.cn

[T44] Perl：条件
来源：http://sv.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://hk.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://iu.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://hw.gzmigu.cn

[T46] Perl：哈希操作
来源：http://bz.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zy.nszjky.cn

[T47] Perl：正则捕获
来源：http://mz.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lw.yuexingan06.cn

[T48] Perl：正则替换
来源：http://rz.nicolike.cn

$s =~ s/old/new/g;
来源：http://rz.shtwfgs.cn

[T49] Perl：函数
来源：http://bn.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vz.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://ks.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://id.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://wa.huanxung.cn

[T51] Scala：Hello World
来源：http://sz.newstarts.cn

println("Hello")
来源：http://cz.hnjuh.cn

[T52] Scala：变量
来源：http://hj.9csxet.cn

val a = 1;  var b = 2
来源：http://wo.hnjuh.cn

[T53] Scala：字符串插值
来源：http://kg.shtwfgs.cn

s"值: $b"
来源：http://as.nszjky.cn

[T54] Scala：集合映射
来源：http://dt.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://js.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://uw.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zh.shxzskj.cn

[T56] Scala：样例类
来源：http://wd.shxzukj.cn

case class User(name: String, age: Int)
来源：http://fd.hnjuh.cn

[T57] Scala：模式匹配
来源：http://oe.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nq.hahajie.cn

[T58] Scala：函数定义
来源：http://iq.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wr.szsharing.cn

[T59] Scala：循环
来源：http://ro.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://rj.huixiangedu.cn

[T60] Scala：折叠
来源：http://gl.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jh.nszjky.cn

================================================================================
来源：http://yk.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rk.9csxet.cn

================================================================================
来源：http://pl.521024.cn


<!-- 参考信息 -->