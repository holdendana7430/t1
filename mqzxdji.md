代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://np.szxytkj.cn

[R56] 远程拷贝
来源：http://fr.shtwfgs.cn

scp file user@host:/path/
来源：http://ss.9csxet.cn

[R57] 远程执行命令
来源：http://ko.szxytkj.cn

ssh user@host 'uptime'
来源：http://le.shxzukj.cn

[R58] 下载文件
来源：http://gl.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tq.newstarts.cn

[R59] 发 POST JSON
来源：http://sf.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mp.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://zw.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ec.chemitech.net.cn

[R61] 磁盘占用
来源：http://dr.521024.cn

df -h;  du -sh *
来源：http://bw.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://lc.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://ol.wgjwhj.cn

[R63] 内存与进程
来源：http://yn.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://ck.bookmarksfly.cn

[R64] 结束进程
来源：http://bn.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://qg.nicolike.cn

[R65] 查看端口占用
来源：http://jd.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cv.nicolike.cn

[R66] 定时任务
来源：http://va.yuexingan06.cn

crontab -e;  crontab -l
来源：http://jc.colortex.cn

[R67] 生成随机十六进制串
来源：http://ej.nicolike.cn

openssl rand -hex 16
来源：http://dt.newstarts.cn

[R68] 计算文件校验值
来源：http://zf.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cc.lnxyls.cn

[R69] 生成随机密码
来源：http://ku.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://sq.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://xr.hahajie.cn

date +%s;  date -d @1700000000
来源：http://tq.hahajie.cn

[R71] 日期格式化
来源：http://aq.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gr.521024.cn

[R72] 等待端口就绪
来源：http://vf.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bs.chemitech.net.cn

[R73] 分割大日志
来源：http://ym.muxihuayi.cn

split -l 1000 big.log part_
来源：http://dz.gzmigu.cn

[R74] 批量重命名
来源：http://zi.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ml.hnjuh.cn

[R75] 导出环境变量
来源：http://bs.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://hk.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://py.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://it.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://qi.yuexingan06.cn

read -rp "请输入: " ans
来源：http://at.panjiajie.cn

[R78] 交互式菜单
来源：http://qu.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vj.shxzskj.cn

[R79] 解析命令行选项
来源：http://vy.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ip.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://sg.colortex.cn

time ./run.sh
来源：http://df.shtwfgs.cn

================================================================================
来源：http://ni.colortex.cn

S. C / C++ 专题
来源：http://lt.bookmarksfly.cn

================================================================================
来源：http://vn.haigaiapp.cn

[S01] C：Hello World
来源：http://bk.huixiangedu.cn

#include <stdio.h>
来源：http://zy.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xr.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://ro.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://bw.521024.cn

[S03] C：读入整数
来源：http://ob.nszjky.cn

int x; scanf("%d", &x);
来源：http://hz.newstarts.cn

[S04] C：字符串复制
来源：http://zk.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dx.haigaiapp.cn

[S05] C：字符串长度
来源：http://wx.haigaiapp.cn

strlen(s)
来源：http://nn.gzmigu.cn

[S06] C：字符串比较
来源：http://er.newstarts.cn

strcmp(a, b) == 0
来源：http://ky.9csxet.cn

[S07] C：数组遍历求和
来源：http://ac.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fb.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://da.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yn.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://kc.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bc.bjjhwx.cn

[S10] C：指针与解引用
来源：http://oh.asd995.cn

int *p = &a;  *p = 5;
来源：http://jl.szsharing.cn

[S11] C：逐行读文件
来源：http://lv.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://iv.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ra.szsharing.cn

fclose(f);
来源：http://mb.hahajie.cn

[S12] C：写文件
来源：http://ru.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uw.shtwfgs.cn

[S13] C：宏定义
来源：http://ve.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qg.yuexingan06.cn

[S14] C：枚举
来源：http://qa.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ap.newstarts.cn

[S15] C：类型转换
来源：http://pb.9csxet.cn

(double) a / b
来源：http://jp.nszjky.cn

[S16] C：位操作置位
来源：http://qa.shxzskj.cn

x |= (1 << 3);
来源：http://qs.szsharing.cn

[S17] C：安全拼接字符串
来源：http://qo.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ab.colortex.cn

[S18] C：命令行参数
来源：http://qp.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://fl.bookmarksfly.cn

[S19] C：快速排序
来源：http://bb.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bv.jctech888.com.cn

[S20] C：二分查找
来源：http://rn.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oc.lnxyls.cn

[S21] C：字符类别判断
来源：http://nh.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ej.szxytkj.cn

[S22] C：字符串转数字
来源：http://av.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zt.521024.cn

[S23] C：随机数
来源：http://fg.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ju.haigaiapp.cn

[S24] C：获取本地时间
来源：http://cc.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wo.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://nw.wgjwhj.cn

memcpy(dst, src, n);
来源：http://jt.lnxyls.cn

[S26] C：内存清零
来源：http://zx.521024.cn

memset(a, 0, sizeof a);
来源：http://dw.huixinmuqiang.cn

[S27] C：定义常量
来源：http://yo.huanxung.cn

const double PI = 3.14159;
来源：http://bl.szxytkj.cn

[S28] C：静态变量
来源：http://sh.gzmigu.cn

static int counter = 0;
来源：http://zl.nicolike.cn

[S29] C：变参函数
来源：http://ni.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://du.muxihuayi.cn

[S30] C：头文件保护
来源：http://mp.gzmigu.cn

#ifndef X_H
来源：http://bx.yuntaijiaju.cn

#define X_H
来源：http://es.shxzukj.cn

#endif
来源：http://re.szsharing.cn

[S31] C++：Hello World
来源：http://zh.yuexingan06.cn

#include <iostream>
来源：http://gy.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://tu.chemitech.net.cn

[S32] C++：字符串
来源：http://ea.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://jh.panjiajie.cn

[S33] C++：vector 增删
来源：http://qw.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mo.huanxung.cn

[S34] C++：遍历 vector
来源：http://ab.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://ch.huanxung.cn

[S35] C++：map
来源：http://ll.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xo.haigaiapp.cn

[S36] C++：unordered_map
来源：http://mz.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zc.huixiangedu.cn

[S37] C++：set
来源：http://mp.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rh.haigaiapp.cn

[S38] C++：排序
来源：http://nw.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://jt.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://ux.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fo.bjjhwx.cn

[S40] C++：查找元素
来源：http://gl.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uu.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://jq.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wl.colortex.cn

[S42] C++：继承与虚函数
来源：http://ru.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://gm.hnjuh.cn

[S43] C++：智能指针
来源：http://mp.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://qt.newstarts.cn

[S44] C++：引用传参
来源：http://ro.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://zr.bookmarksfly.cn

[S45] C++：lambda
来源：http://av.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hd.jctech888.com.cn

[S46] C++：函数模板
来源：http://sg.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mx.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://at.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jh.newstarts.cn

[S48] C++：逐行读文件
来源：http://bc.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://in.hahajie.cn

while (std::getline(in, line)) { }
来源：http://bu.lnxyls.cn

[S49] C++：写文件
来源：http://kk.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fp.nszjky.cn

[S50] C++：格式化数字
来源：http://op.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cc.huanxung.cn

[S51] C++：显式类型转换
来源：http://uy.jctech888.com.cn

static_cast<double>(a) / b
来源：http://wg.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://sm.nszjky.cn

int size() const noexcept { return n_; }
来源：http://kd.szsharing.cn

[S53] C++：移动语义
来源：http://wx.asd995.cn

std::vector<int> w = std::move(v);
来源：http://aq.colortex.cn

[S54] C++：异常处理
来源：http://an.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cv.asd995.cn

[S55] C++：结构化绑定
来源：http://oa.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yi.shtwfgs.cn

[S56] C++：optional
来源：http://zh.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kl.haigaiapp.cn

[S57] C++：编译期常量
来源：http://sk.szxytkj.cn

constexpr int N = 10;
来源：http://ta.huixiangedu.cn

[S58] C++：命名空间
来源：http://nq.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://qx.haigaiapp.cn

[S59] C++：静态断言
来源：http://wp.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bw.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://sx.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tc.bjjhwx.cn

================================================================================
来源：http://rn.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zl.huixinmuqiang.cn

================================================================================
来源：http://it.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://xs.huanxung.cn

println("Hello")
来源：http://ku.9csxet.cn

[T02] Kotlin：变量
来源：http://au.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jk.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://um.hahajie.cn

"值: $b"
来源：http://mh.lnxyls.cn

[T04] Kotlin：空安全
来源：http://vs.gzmigu.cn

val n: String? = null;  n?.length
来源：http://qw.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://dy.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gj.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://qt.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nz.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://up.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zp.asd995.cn

[T08] Kotlin：数据类
来源：http://qi.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://cs.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://kj.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://qa.newstarts.cn

[T10] Kotlin：默认参数
来源：http://gi.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nx.szxytkj.cn

[T11] Kotlin：协程
来源：http://vt.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hd.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://xs.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://dp.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://bv.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://ih.521024.cn

[T14] Kotlin：循环
来源：http://pe.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://nt.haigaiapp.cn

[T15] Kotlin：接口
来源：http://kr.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://kp.colortex.cn

[T16] Swift：Hello World
来源：http://ya.huixiangedu.cn

print("Hello")
来源：http://hp.shxzskj.cn

[T17] Swift：变量与常量
来源：http://qy.9csxet.cn

var a = 1;  let b = 2
来源：http://ck.gzmigu.cn

[T18] Swift：字符串插值
来源：http://su.huanxung.cn

"值: \(b)"
来源：http://uy.shxzukj.cn

[T19] Swift：可选绑定
来源：http://sk.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://fp.nicolike.cn

[T20] Swift：数组操作
来源：http://ls.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ic.shxzskj.cn

[T21] Swift：遍历
来源：http://pf.colortex.cn

for x in a { print(x) }
来源：http://mj.panjiajie.cn

[T22] Swift：字典
来源：http://sp.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kv.bjjhwx.cn

[T23] Swift：函数
来源：http://nx.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vs.9csxet.cn

[T24] Swift：闭包
来源：http://lp.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iq.asd995.cn

[T25] Swift：结构体
来源：http://uu.huixiangedu.cn

struct P { var x: Int }
来源：http://yq.chemitech.net.cn

[T26] Swift：类与重写
来源：http://qx.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://mn.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://rr.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://gs.asd995.cn

[T28] Swift：枚举
来源：http://gf.bookmarksfly.cn

enum Color { case red, green }
来源：http://xy.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://vv.lnxyls.cn

guard let x = opt else { return }
来源：http://il.haigaiapp.cn

[T30] Swift：协议
来源：http://aj.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://ww.521024.cn

[T31] Lua：Hello World
来源：http://gs.gzmigu.cn

print("Hello")
来源：http://ko.nicolike.cn

[T32] Lua：局部变量
来源：http://so.panjiajie.cn

local a = 1
来源：http://ux.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://xl.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xw.huixiangedu.cn

[T34] Lua：遍历表
来源：http://se.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zr.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://yu.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://qc.bjjhwx.cn

[T36] Lua：函数
来源：http://qf.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://lx.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://xm.shtwfgs.cn

"a" .. "b"
来源：http://gi.jctech888.com.cn

[T38] Lua：条件
来源：http://yb.jctech888.com.cn

if x > 0 then print("正") end
来源：http://ih.hahajie.cn

[T39] Lua：模式匹配
来源：http://wj.nicolike.cn

string.find(s, "%d+")
来源：http://wx.bookmarksfly.cn

[T40] Lua：元表
来源：http://si.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://xf.521024.cn

[T41] Perl：Hello World
来源：http://fe.wgjwhj.cn

print "Hello\n";
来源：http://bt.chemitech.net.cn

[T42] Perl：变量类型
来源：http://zw.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ts.521024.cn

[T43] Perl：字符串插值
来源：http://ra.hahajie.cn

"值: $a"
来源：http://oh.gzmigu.cn

[T44] Perl：条件
来源：http://tl.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://ob.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://eu.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ap.shxzukj.cn

[T46] Perl：哈希操作
来源：http://dk.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gl.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://wc.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zx.hnjuh.cn

[T48] Perl：正则替换
来源：http://mn.lnxyls.cn

$s =~ s/old/new/g;
来源：http://iv.huanxung.cn

[T49] Perl：函数
来源：http://cn.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nv.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://nl.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xh.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://vt.lnxyls.cn

[T51] Scala：Hello World
来源：http://dl.huanxung.cn

println("Hello")
来源：http://jj.521024.cn

[T52] Scala：变量
来源：http://vj.szsharing.cn

val a = 1;  var b = 2
来源：http://vy.nicolike.cn

[T53] Scala：字符串插值
来源：http://pl.colortex.cn

s"值: $b"
来源：http://xt.haigaiapp.cn

[T54] Scala：集合映射
来源：http://fb.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://hp.nszjky.cn

[T55] Scala：集合过滤
来源：http://oa.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xw.szxytkj.cn

[T56] Scala：样例类
来源：http://dy.newstarts.cn

case class User(name: String, age: Int)
来源：http://lp.lnxyls.cn

[T57] Scala：模式匹配
来源：http://kv.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ax.huanxung.cn

[T58] Scala：函数定义
来源：http://im.yuntaijiaju.cn


<!-- 参考信息 -->