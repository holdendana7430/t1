代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kh.haigaiapp.cn

[R56] 远程拷贝
来源：http://lx.jctech888.com.cn

scp file user@host:/path/
来源：http://da.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://rm.panjiajie.cn

ssh user@host 'uptime'
来源：http://yo.bookmarksfly.cn

[R58] 下载文件
来源：http://ed.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oe.lnxyls.cn

[R59] 发 POST JSON
来源：http://ra.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kz.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://xh.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://au.shxzskj.cn

[R61] 磁盘占用
来源：http://ky.huixiangedu.cn

df -h;  du -sh *
来源：http://vw.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://kr.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://yq.haigaiapp.cn

[R63] 内存与进程
来源：http://sg.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://ok.nszjky.cn

[R64] 结束进程
来源：http://bc.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://qs.9csxet.cn

[R65] 查看端口占用
来源：http://fk.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://du.bookmarksfly.cn

[R66] 定时任务
来源：http://ld.nicolike.cn

crontab -e;  crontab -l
来源：http://qw.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://xz.newstarts.cn

openssl rand -hex 16
来源：http://ri.shtwfgs.cn

[R68] 计算文件校验值
来源：http://tr.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mi.shtwfgs.cn

[R69] 生成随机密码
来源：http://ss.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://nr.521024.cn

[R70] 时间戳与互转
来源：http://qj.nicolike.cn

date +%s;  date -d @1700000000
来源：http://tn.haigaiapp.cn

[R71] 日期格式化
来源：http://hd.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jf.jctech888.com.cn

[R72] 等待端口就绪
来源：http://cg.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ir.wgjwhj.cn

[R73] 分割大日志
来源：http://qa.asd995.cn

split -l 1000 big.log part_
来源：http://aa.nszjky.cn

[R74] 批量重命名
来源：http://op.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bc.huanxung.cn

[R75] 导出环境变量
来源：http://jc.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://il.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://bi.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ue.chemitech.net.cn

[R77] 读取用户输入
来源：http://gq.szxytkj.cn

read -rp "请输入: " ans
来源：http://ds.newstarts.cn

[R78] 交互式菜单
来源：http://wb.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kv.huanxung.cn

[R79] 解析命令行选项
来源：http://wc.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qs.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://km.newstarts.cn

time ./run.sh
来源：http://ho.huanxung.cn

================================================================================
来源：http://sg.chemitech.net.cn

S. C / C++ 专题
来源：http://wv.shxzskj.cn

================================================================================
来源：http://du.shxzskj.cn

[S01] C：Hello World
来源：http://gw.szxytkj.cn

#include <stdio.h>
来源：http://em.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pz.asd995.cn

[S02] C：变量与格式化输出
来源：http://df.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://wk.shtwfgs.cn

[S03] C：读入整数
来源：http://uy.hnjuh.cn

int x; scanf("%d", &x);
来源：http://at.hnjuh.cn

[S04] C：字符串复制
来源：http://ev.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jp.szxytkj.cn

[S05] C：字符串长度
来源：http://fc.lnxyls.cn

strlen(s)
来源：http://mb.nszjky.cn

[S06] C：字符串比较
来源：http://qv.wgjwhj.cn

strcmp(a, b) == 0
来源：http://zo.hahajie.cn

[S07] C：数组遍历求和
来源：http://su.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hm.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://ip.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tx.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://pg.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ex.nicolike.cn

[S10] C：指针与解引用
来源：http://sy.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://rk.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://sj.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://hf.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bb.nszjky.cn

fclose(f);
来源：http://uz.hnjuh.cn

[S12] C：写文件
来源：http://lt.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://an.521024.cn

[S13] C：宏定义
来源：http://vk.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cl.szxytkj.cn

[S14] C：枚举
来源：http://jb.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://dc.yuexingan06.cn

[S15] C：类型转换
来源：http://pc.shxzskj.cn

(double) a / b
来源：http://vx.yuexingan06.cn

[S16] C：位操作置位
来源：http://tz.shtwfgs.cn

x |= (1 << 3);
来源：http://yr.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://zy.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oa.muxihuayi.cn

[S18] C：命令行参数
来源：http://qr.newstarts.cn

int main(int argc, char **argv)
来源：http://au.szxytkj.cn

[S19] C：快速排序
来源：http://ng.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dk.panjiajie.cn

[S20] C：二分查找
来源：http://pj.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://su.haigaiapp.cn

[S21] C：字符类别判断
来源：http://xt.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bz.muxihuayi.cn

[S22] C：字符串转数字
来源：http://ag.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wu.jctech888.com.cn

[S23] C：随机数
来源：http://fe.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ff.521024.cn

[S24] C：获取本地时间
来源：http://jb.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hv.wgjwhj.cn

[S25] C：内存拷贝
来源：http://yn.hnjuh.cn

memcpy(dst, src, n);
来源：http://gu.hahajie.cn

[S26] C：内存清零
来源：http://yd.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://xe.jctech888.com.cn

[S27] C：定义常量
来源：http://rm.huixiangedu.cn

const double PI = 3.14159;
来源：http://fb.huixiangedu.cn

[S28] C：静态变量
来源：http://qq.chemitech.net.cn

static int counter = 0;
来源：http://po.panjiajie.cn

[S29] C：变参函数
来源：http://dk.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nr.shxzukj.cn

[S30] C：头文件保护
来源：http://lr.jctech888.com.cn

#ifndef X_H
来源：http://uy.bookmarksfly.cn

#define X_H
来源：http://qr.bjjhwx.cn

#endif
来源：http://zf.lnxyls.cn

[S31] C++：Hello World
来源：http://dd.jctech888.com.cn

#include <iostream>
来源：http://dp.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://tx.shtwfgs.cn

[S32] C++：字符串
来源：http://we.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://yz.huixiangedu.cn

[S33] C++：vector 增删
来源：http://nz.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ns.huanxung.cn

[S34] C++：遍历 vector
来源：http://zv.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://qs.9csxet.cn

[S35] C++：map
来源：http://bk.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gh.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://in.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ki.huixiangedu.cn

[S37] C++：set
来源：http://vb.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tf.9csxet.cn

[S38] C++：排序
来源：http://cc.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://bi.colortex.cn

[S39] C++：自定义比较器排序
来源：http://ed.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pl.asd995.cn

[S40] C++：查找元素
来源：http://hm.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ht.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://ez.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oj.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://cz.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://fc.lnxyls.cn

[S43] C++：智能指针
来源：http://wy.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://en.nszjky.cn

[S44] C++：引用传参
来源：http://kx.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://gm.colortex.cn

[S45] C++：lambda
来源：http://wh.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gv.colortex.cn

[S46] C++：函数模板
来源：http://vy.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wo.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://yh.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ed.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://st.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kn.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://en.nicolike.cn

[S49] C++：写文件
来源：http://mt.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qq.asd995.cn

[S50] C++：格式化数字
来源：http://he.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xy.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://kc.nszjky.cn

static_cast<double>(a) / b
来源：http://nb.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://wi.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://da.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://wm.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://nh.bookmarksfly.cn

[S54] C++：异常处理
来源：http://fg.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tx.huanxung.cn

[S55] C++：结构化绑定
来源：http://qc.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qr.gzmigu.cn

[S56] C++：optional
来源：http://zz.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aq.hnjuh.cn

[S57] C++：编译期常量
来源：http://ck.szsharing.cn

constexpr int N = 10;
来源：http://un.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://id.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://gc.newstarts.cn

[S59] C++：静态断言
来源：http://mn.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eu.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://er.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ev.521024.cn

================================================================================
来源：http://ux.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cn.hahajie.cn

================================================================================
来源：http://ad.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://bl.newstarts.cn

println("Hello")
来源：http://ai.521024.cn

[T02] Kotlin：变量
来源：http://kp.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ij.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://ai.nszjky.cn

"值: $b"
来源：http://pk.colortex.cn

[T04] Kotlin：空安全
来源：http://hj.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://cm.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://pw.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kg.huanxung.cn

[T06] Kotlin：集合映射
来源：http://ni.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mf.521024.cn

[T07] Kotlin：集合过滤
来源：http://ih.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ld.huanxung.cn

[T08] Kotlin：数据类
来源：http://cm.asd995.cn

data class User(val name: String, val age: Int)
来源：http://go.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://tr.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://eb.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://pe.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xf.szsharing.cn

[T11] Kotlin：协程
来源：http://vu.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://le.9csxet.cn

[T12] Kotlin：解构声明
来源：http://tg.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://uh.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://nb.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://ec.wgjwhj.cn

[T14] Kotlin：循环
来源：http://sg.9csxet.cn

for (i in 1..10) println(i)
来源：http://gb.lnxyls.cn

[T15] Kotlin：接口
来源：http://ks.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://ne.hahajie.cn

[T16] Swift：Hello World
来源：http://aa.haigaiapp.cn

print("Hello")
来源：http://jb.9csxet.cn

[T17] Swift：变量与常量
来源：http://tz.szxytkj.cn

var a = 1;  let b = 2
来源：http://sc.gzmigu.cn

[T18] Swift：字符串插值
来源：http://cz.colortex.cn

"值: \(b)"
来源：http://os.521024.cn

[T19] Swift：可选绑定
来源：http://sd.muxihuayi.cn

if let n = opt { print(n) }
来源：http://nv.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://gv.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ze.shxzskj.cn

[T21] Swift：遍历
来源：http://at.nszjky.cn

for x in a { print(x) }
来源：http://qg.huixinmuqiang.cn

[T22] Swift：字典
来源：http://bu.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nr.hnjuh.cn

[T23] Swift：函数
来源：http://ao.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tq.shxzukj.cn

[T24] Swift：闭包
来源：http://fr.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uz.nszjky.cn

[T25] Swift：结构体
来源：http://lg.colortex.cn

struct P { var x: Int }
来源：http://iz.shxzskj.cn

[T26] Swift：类与重写
来源：http://bz.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://jd.wgjwhj.cn

[T27] Swift：错误处理
来源：http://jw.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ej.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://nw.shtwfgs.cn

enum Color { case red, green }
来源：http://dq.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://zd.asd995.cn

guard let x = opt else { return }
来源：http://dk.haigaiapp.cn

[T30] Swift：协议
来源：http://ww.asd995.cn

protocol Shape { func area() -> Double }
来源：http://gw.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ec.nszjky.cn

print("Hello")
来源：http://ar.nszjky.cn

[T32] Lua：局部变量
来源：http://zh.nicolike.cn

local a = 1
来源：http://mp.521024.cn

[T33] Lua：表（数组）
来源：http://em.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hg.newstarts.cn

[T34] Lua：遍历表
来源：http://sz.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vk.huanxung.cn

[T35] Lua：字典表
来源：http://vu.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://kp.gzmigu.cn

[T36] Lua：函数
来源：http://jh.shxzskj.cn

function add(a, b) return a + b end
来源：http://lc.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://ow.asd995.cn

"a" .. "b"
来源：http://xj.hahajie.cn

[T38] Lua：条件
来源：http://of.521024.cn

if x > 0 then print("正") end
来源：http://ws.panjiajie.cn

[T39] Lua：模式匹配
来源：http://ul.bjjhwx.cn

string.find(s, "%d+")
来源：http://xt.shxzskj.cn

[T40] Lua：元表
来源：http://gy.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ti.newstarts.cn

[T41] Perl：Hello World
来源：http://sl.shxzukj.cn

print "Hello\n";
来源：http://zv.newstarts.cn

[T42] Perl：变量类型
来源：http://mx.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bb.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://lq.newstarts.cn

"值: $a"
来源：http://xe.newstarts.cn

[T44] Perl：条件
来源：http://cl.asd995.cn

if ($a > 0) { print "正"; }
来源：http://fp.hnjuh.cn

[T45] Perl：数组遍历
来源：http://yb.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://gi.newstarts.cn

[T46] Perl：哈希操作
来源：http://kw.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jp.hnjuh.cn

[T47] Perl：正则捕获
来源：http://zd.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ss.shxzukj.cn

[T48] Perl：正则替换
来源：http://zs.shxzskj.cn

$s =~ s/old/new/g;
来源：http://nj.jianghongdianzi.cn

[T49] Perl：函数
来源：http://rg.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gq.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://zi.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lx.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://xj.colortex.cn

[T51] Scala：Hello World
来源：http://ko.hnjuh.cn

println("Hello")
来源：http://bo.gzmigu.cn

[T52] Scala：变量
来源：http://gf.shxzskj.cn

val a = 1;  var b = 2
来源：http://tf.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://dt.szxytkj.cn

s"值: $b"
来源：http://lt.asd995.cn

[T54] Scala：集合映射
来源：http://td.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://ht.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://ir.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jq.hnjuh.cn

[T56] Scala：样例类
来源：http://tt.asd995.cn

case class User(name: String, age: Int)
来源：http://dg.nicolike.cn

[T57] Scala：模式匹配
来源：http://yt.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gk.hahajie.cn

[T58] Scala：函数定义
来源：http://dv.asd995.cn


<!-- 参考信息 -->