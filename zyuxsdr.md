代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://en.muxihuayi.cn

[R56] 远程拷贝
来源：http://ee.colortex.cn

scp file user@host:/path/
来源：http://mz.bjjhwx.cn

[R57] 远程执行命令
来源：http://xd.bjjhwx.cn

ssh user@host 'uptime'
来源：http://yb.szsharing.cn

[R58] 下载文件
来源：http://cr.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pk.szxytkj.cn

[R59] 发 POST JSON
来源：http://ym.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yr.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://ic.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sg.shxzukj.cn

[R61] 磁盘占用
来源：http://er.nicolike.cn

df -h;  du -sh *
来源：http://zl.nicolike.cn

[R62] 找最占空间的文件
来源：http://ac.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://pg.lnxyls.cn

[R63] 内存与进程
来源：http://kl.521024.cn

free -h;  ps aux | grep nginx
来源：http://mv.szxytkj.cn

[R64] 结束进程
来源：http://dw.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://tz.bookmarksfly.cn

[R65] 查看端口占用
来源：http://ey.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xh.hnjuh.cn

[R66] 定时任务
来源：http://wo.panjiajie.cn

crontab -e;  crontab -l
来源：http://nd.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://xq.shtwfgs.cn

openssl rand -hex 16
来源：http://rk.szsharing.cn

[R68] 计算文件校验值
来源：http://vo.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ve.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://wo.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://ju.nszjky.cn

[R70] 时间戳与互转
来源：http://vq.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://sz.huanxung.cn

[R71] 日期格式化
来源：http://mr.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sv.huanxung.cn

[R72] 等待端口就绪
来源：http://tf.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zp.haigaiapp.cn

[R73] 分割大日志
来源：http://cb.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://fg.huixiangedu.cn

[R74] 批量重命名
来源：http://yh.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xe.huanxung.cn

[R75] 导出环境变量
来源：http://nz.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://oi.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://sg.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zu.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://np.muxihuayi.cn

read -rp "请输入: " ans
来源：http://iy.bjjhwx.cn

[R78] 交互式菜单
来源：http://ye.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://on.szxytkj.cn

[R79] 解析命令行选项
来源：http://jm.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gz.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://dq.szsharing.cn

time ./run.sh
来源：http://wm.jianghongdianzi.cn

================================================================================
来源：http://vi.jianghongdianzi.cn

S. C / C++ 专题
来源：http://ls.szsharing.cn

================================================================================
来源：http://rd.bjjhwx.cn

[S01] C：Hello World
来源：http://ij.shtwfgs.cn

#include <stdio.h>
来源：http://nd.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ca.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://lb.521024.cn

int a = 10; printf("%d\n", a);
来源：http://lr.bjjhwx.cn

[S03] C：读入整数
来源：http://kp.szxytkj.cn

int x; scanf("%d", &x);
来源：http://qz.chemitech.net.cn

[S04] C：字符串复制
来源：http://yp.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://at.newstarts.cn

[S05] C：字符串长度
来源：http://oq.9csxet.cn

strlen(s)
来源：http://ju.colortex.cn

[S06] C：字符串比较
来源：http://ij.nszjky.cn

strcmp(a, b) == 0
来源：http://zs.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://vi.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bh.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://lm.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bm.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://ql.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://in.wgjwhj.cn

[S10] C：指针与解引用
来源：http://tx.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://ty.yuexingan06.cn

[S11] C：逐行读文件
来源：http://ir.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://qw.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uf.panjiajie.cn

fclose(f);
来源：http://kq.nicolike.cn

[S12] C：写文件
来源：http://fz.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yu.yuntaijiaju.cn

[S13] C：宏定义
来源：http://pc.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bi.yuexingan06.cn

[S14] C：枚举
来源：http://qj.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://op.huixiangedu.cn

[S15] C：类型转换
来源：http://or.nicolike.cn

(double) a / b
来源：http://fd.hahajie.cn

[S16] C：位操作置位
来源：http://hc.nszjky.cn

x |= (1 << 3);
来源：http://ut.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://xb.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ew.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://fk.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://rb.szxytkj.cn

[S19] C：快速排序
来源：http://cd.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ew.521024.cn

[S20] C：二分查找
来源：http://we.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://se.asd995.cn

[S21] C：字符类别判断
来源：http://ut.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fk.nicolike.cn

[S22] C：字符串转数字
来源：http://hu.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xz.newstarts.cn

[S23] C：随机数
来源：http://kg.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rl.huixiangedu.cn

[S24] C：获取本地时间
来源：http://op.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://am.colortex.cn

[S25] C：内存拷贝
来源：http://xk.nszjky.cn

memcpy(dst, src, n);
来源：http://xp.yuexingan06.cn

[S26] C：内存清零
来源：http://wd.hahajie.cn

memset(a, 0, sizeof a);
来源：http://lb.asd995.cn

[S27] C：定义常量
来源：http://ly.nicolike.cn

const double PI = 3.14159;
来源：http://br.chemitech.net.cn

[S28] C：静态变量
来源：http://ny.colortex.cn

static int counter = 0;
来源：http://zy.szsharing.cn

[S29] C：变参函数
来源：http://on.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cs.chemitech.net.cn

[S30] C：头文件保护
来源：http://vj.huixinmuqiang.cn

#ifndef X_H
来源：http://gm.huixinmuqiang.cn

#define X_H
来源：http://ch.huixinmuqiang.cn

#endif
来源：http://ux.yuexingan06.cn

[S31] C++：Hello World
来源：http://kb.szsharing.cn

#include <iostream>
来源：http://cm.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://gm.jianghongdianzi.cn

[S32] C++：字符串
来源：http://cq.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://rz.9csxet.cn

[S33] C++：vector 增删
来源：http://lt.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jd.colortex.cn

[S34] C++：遍历 vector
来源：http://sq.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://nk.yuntaijiaju.cn

[S35] C++：map
来源：http://hr.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ev.szsharing.cn

[S36] C++：unordered_map
来源：http://ta.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jl.521024.cn

[S37] C++：set
来源：http://tl.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ng.huixinmuqiang.cn

[S38] C++：排序
来源：http://mu.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://zn.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://ox.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oo.gzmigu.cn

[S40] C++：查找元素
来源：http://oe.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bd.shxzskj.cn

[S41] C++：类与构造函数
来源：http://fr.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://za.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://gc.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://rj.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://zd.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://td.hnjuh.cn

[S44] C++：引用传参
来源：http://wi.huanxung.cn

void inc(int &x) { ++x; }
来源：http://zm.szxytkj.cn

[S45] C++：lambda
来源：http://ql.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yh.521024.cn

[S46] C++：函数模板
来源：http://za.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wp.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://ui.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kb.szsharing.cn

[S48] C++：逐行读文件
来源：http://ez.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hn.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://kx.jctech888.com.cn

[S49] C++：写文件
来源：http://yh.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oe.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://mc.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sk.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://fp.wgjwhj.cn

static_cast<double>(a) / b
来源：http://wb.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://cl.hahajie.cn

int size() const noexcept { return n_; }
来源：http://yg.shxzukj.cn

[S53] C++：移动语义
来源：http://mf.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://xg.szsharing.cn

[S54] C++：异常处理
来源：http://ks.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ud.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://rc.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pj.yuexingan06.cn

[S56] C++：optional
来源：http://ef.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ea.shxzskj.cn

[S57] C++：编译期常量
来源：http://kn.9csxet.cn

constexpr int N = 10;
来源：http://ra.nicolike.cn

[S58] C++：命名空间
来源：http://ct.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://wd.asd995.cn

[S59] C++：静态断言
来源：http://tx.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xc.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ns.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vu.wgjwhj.cn

================================================================================
来源：http://na.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lc.hnjuh.cn

================================================================================
来源：http://wr.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://lz.lnxyls.cn

println("Hello")
来源：http://hs.shxzskj.cn

[T02] Kotlin：变量
来源：http://ui.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ou.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://al.gzmigu.cn

"值: $b"
来源：http://pd.gzmigu.cn

[T04] Kotlin：空安全
来源：http://jw.9csxet.cn

val n: String? = null;  n?.length
来源：http://ma.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://hq.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hu.nszjky.cn

[T06] Kotlin：集合映射
来源：http://gp.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yv.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://xx.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sk.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://di.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://wp.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://mh.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://zw.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://jb.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yt.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://dk.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://po.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://go.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://yo.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://lh.asd995.cn

val m = mapOf("a" to 1)
来源：http://bi.9csxet.cn

[T14] Kotlin：循环
来源：http://ad.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://lw.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://ew.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://si.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://qr.asd995.cn

print("Hello")
来源：http://ey.hahajie.cn

[T17] Swift：变量与常量
来源：http://wq.huixiangedu.cn

var a = 1;  let b = 2
来源：http://ir.shxzukj.cn

[T18] Swift：字符串插值
来源：http://mt.huixinmuqiang.cn

"值: \(b)"
来源：http://mq.hahajie.cn

[T19] Swift：可选绑定
来源：http://ni.hnjuh.cn

if let n = opt { print(n) }
来源：http://sw.shxzukj.cn

[T20] Swift：数组操作
来源：http://np.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ru.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://ma.shxzskj.cn

for x in a { print(x) }
来源：http://kk.colortex.cn

[T22] Swift：字典
来源：http://ta.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jw.asd995.cn

[T23] Swift：函数
来源：http://iw.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ld.chemitech.net.cn

[T24] Swift：闭包
来源：http://um.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eq.yuexingan06.cn

[T25] Swift：结构体
来源：http://gd.szxytkj.cn

struct P { var x: Int }
来源：http://ih.shtwfgs.cn

[T26] Swift：类与重写
来源：http://ia.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://km.haigaiapp.cn

[T27] Swift：错误处理
来源：http://zo.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://vi.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://zg.shxzskj.cn

enum Color { case red, green }
来源：http://wi.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://xt.shxzukj.cn

guard let x = opt else { return }
来源：http://fm.huixiangedu.cn

[T30] Swift：协议
来源：http://ar.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://jb.521024.cn

[T31] Lua：Hello World
来源：http://lw.yuntaijiaju.cn

print("Hello")
来源：http://sh.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://ia.chemitech.net.cn

local a = 1
来源：http://am.521024.cn

[T33] Lua：表（数组）
来源：http://jd.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uj.wgjwhj.cn

[T34] Lua：遍历表
来源：http://dy.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ci.panjiajie.cn

[T35] Lua：字典表
来源：http://xh.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://mt.panjiajie.cn

[T36] Lua：函数
来源：http://ow.panjiajie.cn

function add(a, b) return a + b end
来源：http://xo.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://qx.shxzskj.cn

"a" .. "b"
来源：http://zx.asd995.cn

[T38] Lua：条件
来源：http://ei.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://vt.gzmigu.cn

[T39] Lua：模式匹配
来源：http://ig.haigaiapp.cn

string.find(s, "%d+")
来源：http://or.colortex.cn

[T40] Lua：元表
来源：http://tl.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://it.asd995.cn

[T41] Perl：Hello World
来源：http://rd.huixinmuqiang.cn

print "Hello\n";
来源：http://ki.lnxyls.cn

[T42] Perl：变量类型
来源：http://ri.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ay.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://jt.lnxyls.cn

"值: $a"
来源：http://fv.muxihuayi.cn

[T44] Perl：条件
来源：http://vq.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://yq.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://gb.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://lc.asd995.cn

[T46] Perl：哈希操作
来源：http://kk.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hg.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://bu.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jq.gzmigu.cn

[T48] Perl：正则替换
来源：http://of.huanxung.cn

$s =~ s/old/new/g;
来源：http://rq.shxzukj.cn

[T49] Perl：函数
来源：http://bo.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lh.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://zo.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nl.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ui.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://eu.asd995.cn

println("Hello")
来源：http://ww.szxytkj.cn

[T52] Scala：变量
来源：http://xd.szsharing.cn

val a = 1;  var b = 2
来源：http://te.newstarts.cn

[T53] Scala：字符串插值
来源：http://lx.muxihuayi.cn

s"值: $b"
来源：http://py.shxzskj.cn

[T54] Scala：集合映射
来源：http://bt.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://eo.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://sb.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://to.gzmigu.cn

[T56] Scala：样例类
来源：http://up.lnxyls.cn

case class User(name: String, age: Int)
来源：http://uy.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://zb.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ru.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://bn.szsharing.cn


<!-- 参考信息 -->