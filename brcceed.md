代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://kd.gzmigu.cn

[R52] 统计行数
来源：http://fl.shxzskj.cn

wc -l a.txt
来源：http://fh.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://xj.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://en.huanxung.cn

[R54] 比较两个文件
来源：http://hl.asd995.cn

diff a.txt b.txt
来源：http://ld.panjiajie.cn

[R55] 压缩与解压
来源：http://nx.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mt.szxytkj.cn

[R56] 远程拷贝
来源：http://oo.szsharing.cn

scp file user@host:/path/
来源：http://bj.hnjuh.cn

[R57] 远程执行命令
来源：http://xo.huanxung.cn

ssh user@host 'uptime'
来源：http://pa.shtwfgs.cn

[R58] 下载文件
来源：http://xz.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fn.hahajie.cn

[R59] 发 POST JSON
来源：http://ux.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iu.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://jm.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uy.nicolike.cn

[R61] 磁盘占用
来源：http://zu.nicolike.cn

df -h;  du -sh *
来源：http://wh.panjiajie.cn

[R62] 找最占空间的文件
来源：http://xy.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://kg.szxytkj.cn

[R63] 内存与进程
来源：http://qq.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://wz.nszjky.cn

[R64] 结束进程
来源：http://nq.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://rs.hahajie.cn

[R65] 查看端口占用
来源：http://ib.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://op.newstarts.cn

[R66] 定时任务
来源：http://am.jctech888.com.cn

crontab -e;  crontab -l
来源：http://so.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://uk.hnjuh.cn

openssl rand -hex 16
来源：http://fu.gzmigu.cn

[R68] 计算文件校验值
来源：http://ev.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gn.asd995.cn

[R69] 生成随机密码
来源：http://nx.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://wx.lnxyls.cn

[R70] 时间戳与互转
来源：http://rb.colortex.cn

date +%s;  date -d @1700000000
来源：http://ko.9csxet.cn

[R71] 日期格式化
来源：http://bo.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://at.wgjwhj.cn

[R72] 等待端口就绪
来源：http://fn.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zd.jianghongdianzi.cn

[R73] 分割大日志
来源：http://fv.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://mb.bjjhwx.cn

[R74] 批量重命名
来源：http://yn.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lj.colortex.cn

[R75] 导出环境变量
来源：http://tv.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://zi.nicolike.cn

[R76] 使用临时文件
来源：http://zs.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mz.szsharing.cn

[R77] 读取用户输入
来源：http://rl.gzmigu.cn

read -rp "请输入: " ans
来源：http://ql.hnjuh.cn

[R78] 交互式菜单
来源：http://ty.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bl.shtwfgs.cn

[R79] 解析命令行选项
来源：http://cn.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oz.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://zd.chemitech.net.cn

time ./run.sh
来源：http://ne.lnxyls.cn

================================================================================
来源：http://rf.jianghongdianzi.cn

S. C / C++ 专题
来源：http://sd.newstarts.cn

================================================================================
来源：http://fv.colortex.cn

[S01] C：Hello World
来源：http://nt.colortex.cn

#include <stdio.h>
来源：http://fm.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qr.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://rn.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://fr.colortex.cn

[S03] C：读入整数
来源：http://ov.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://nk.szxytkj.cn

[S04] C：字符串复制
来源：http://yf.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xc.panjiajie.cn

[S05] C：字符串长度
来源：http://wy.hnjuh.cn

strlen(s)
来源：http://kw.panjiajie.cn

[S06] C：字符串比较
来源：http://yw.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ra.huanxung.cn

[S07] C：数组遍历求和
来源：http://jq.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nn.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://va.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wt.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://ji.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fe.shxzskj.cn

[S10] C：指针与解引用
来源：http://ej.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://te.colortex.cn

[S11] C：逐行读文件
来源：http://fc.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://vw.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://as.gzmigu.cn

fclose(f);
来源：http://kj.colortex.cn

[S12] C：写文件
来源：http://jw.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fm.shtwfgs.cn

[S13] C：宏定义
来源：http://rz.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hu.szxytkj.cn

[S14] C：枚举
来源：http://zn.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://bz.9csxet.cn

[S15] C：类型转换
来源：http://ws.hahajie.cn

(double) a / b
来源：http://nw.nicolike.cn

[S16] C：位操作置位
来源：http://hw.colortex.cn

x |= (1 << 3);
来源：http://cc.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://gb.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nn.huanxung.cn

[S18] C：命令行参数
来源：http://df.gzmigu.cn

int main(int argc, char **argv)
来源：http://eh.huixinmuqiang.cn

[S19] C：快速排序
来源：http://ul.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fg.szsharing.cn

[S20] C：二分查找
来源：http://xq.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hd.asd995.cn

[S21] C：字符类别判断
来源：http://ez.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nn.huixiangedu.cn

[S22] C：字符串转数字
来源：http://dy.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cf.huixiangedu.cn

[S23] C：随机数
来源：http://mx.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qp.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://zj.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lr.muxihuayi.cn

[S25] C：内存拷贝
来源：http://vs.521024.cn

memcpy(dst, src, n);
来源：http://ah.nicolike.cn

[S26] C：内存清零
来源：http://oj.asd995.cn

memset(a, 0, sizeof a);
来源：http://ox.jianghongdianzi.cn

[S27] C：定义常量
来源：http://mt.521024.cn

const double PI = 3.14159;
来源：http://ru.newstarts.cn

[S28] C：静态变量
来源：http://lq.nicolike.cn

static int counter = 0;
来源：http://ch.gzmigu.cn

[S29] C：变参函数
来源：http://ok.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tq.521024.cn

[S30] C：头文件保护
来源：http://nh.hnjuh.cn

#ifndef X_H
来源：http://gr.bookmarksfly.cn

#define X_H
来源：http://tl.shxzukj.cn

#endif
来源：http://rb.wgjwhj.cn

[S31] C++：Hello World
来源：http://ih.hahajie.cn

#include <iostream>
来源：http://fc.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://jg.wgjwhj.cn

[S32] C++：字符串
来源：http://fy.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ma.bjjhwx.cn

[S33] C++：vector 增删
来源：http://ah.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fq.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ia.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://wd.wgjwhj.cn

[S35] C++：map
来源：http://kl.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vk.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://lj.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bn.hahajie.cn

[S37] C++：set
来源：http://zo.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pv.nszjky.cn

[S38] C++：排序
来源：http://sk.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://ll.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://zw.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vf.hnjuh.cn

[S40] C++：查找元素
来源：http://dn.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ip.shxzukj.cn

[S41] C++：类与构造函数
来源：http://qx.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ky.szsharing.cn

[S42] C++：继承与虚函数
来源：http://eu.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://pu.521024.cn

[S43] C++：智能指针
来源：http://gv.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://de.newstarts.cn

[S44] C++：引用传参
来源：http://ci.521024.cn

void inc(int &x) { ++x; }
来源：http://hm.muxihuayi.cn

[S45] C++：lambda
来源：http://al.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lw.newstarts.cn

[S46] C++：函数模板
来源：http://zp.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dq.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://tz.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gp.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://bl.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wl.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://hz.gzmigu.cn

[S49] C++：写文件
来源：http://gs.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xg.chemitech.net.cn

[S50] C++：格式化数字
来源：http://os.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ft.521024.cn

[S51] C++：显式类型转换
来源：http://if.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://sr.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://kx.nicolike.cn

int size() const noexcept { return n_; }
来源：http://yo.shtwfgs.cn

[S53] C++：移动语义
来源：http://qx.521024.cn

std::vector<int> w = std::move(v);
来源：http://pk.shxzukj.cn

[S54] C++：异常处理
来源：http://dc.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kv.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://lt.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wx.huixiangedu.cn

[S56] C++：optional
来源：http://pt.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iq.gzmigu.cn

[S57] C++：编译期常量
来源：http://yj.haigaiapp.cn

constexpr int N = 10;
来源：http://yc.gzmigu.cn

[S58] C++：命名空间
来源：http://eu.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://jl.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://df.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rb.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://yv.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nc.huixinmuqiang.cn

================================================================================
来源：http://oq.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rr.panjiajie.cn

================================================================================
来源：http://pg.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://ex.szsharing.cn

println("Hello")
来源：http://ed.haigaiapp.cn

[T02] Kotlin：变量
来源：http://dl.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://na.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://wy.huixiangedu.cn

"值: $b"
来源：http://cr.lnxyls.cn

[T04] Kotlin：空安全
来源：http://nj.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://ot.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://lh.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rg.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://ey.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dw.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://ib.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vr.newstarts.cn

[T08] Kotlin：数据类
来源：http://bs.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://hy.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://ks.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://ru.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://zv.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zq.9csxet.cn

[T11] Kotlin：协程
来源：http://gt.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://as.huanxung.cn

[T12] Kotlin：解构声明
来源：http://pj.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://wl.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://vw.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://ph.yuexingan06.cn

[T14] Kotlin：循环
来源：http://xd.gzmigu.cn

for (i in 1..10) println(i)
来源：http://uq.hnjuh.cn

[T15] Kotlin：接口
来源：http://wr.colortex.cn

interface Shape { fun area(): Double }
来源：http://rn.yuexingan06.cn

[T16] Swift：Hello World
来源：http://iz.jctech888.com.cn

print("Hello")
来源：http://rt.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://qa.muxihuayi.cn

var a = 1;  let b = 2
来源：http://br.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://jy.yuntaijiaju.cn

"值: \(b)"
来源：http://fm.shxzskj.cn

[T19] Swift：可选绑定
来源：http://wm.huixiangedu.cn

if let n = opt { print(n) }
来源：http://fw.newstarts.cn

[T20] Swift：数组操作
来源：http://cy.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wa.lnxyls.cn

[T21] Swift：遍历
来源：http://hy.yuntaijiaju.cn

for x in a { print(x) }
来源：http://mw.nicolike.cn

[T22] Swift：字典
来源：http://am.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wk.bjjhwx.cn

[T23] Swift：函数
来源：http://mh.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mm.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://wm.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qx.bjjhwx.cn

[T25] Swift：结构体
来源：http://aj.shtwfgs.cn

struct P { var x: Int }
来源：http://dd.szxytkj.cn

[T26] Swift：类与重写
来源：http://fg.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://pd.lnxyls.cn

[T27] Swift：错误处理
来源：http://pp.9csxet.cn

do { try f() } catch { print(error) }
来源：http://pu.asd995.cn

[T28] Swift：枚举
来源：http://cc.bjjhwx.cn

enum Color { case red, green }
来源：http://hi.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://ud.521024.cn

guard let x = opt else { return }
来源：http://ew.huixiangedu.cn

[T30] Swift：协议
来源：http://xi.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ig.gzmigu.cn

[T31] Lua：Hello World
来源：http://og.hahajie.cn

print("Hello")
来源：http://mq.wgjwhj.cn

[T32] Lua：局部变量
来源：http://fz.jctech888.com.cn

local a = 1
来源：http://pb.hahajie.cn

[T33] Lua：表（数组）
来源：http://ms.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://er.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://hq.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vp.wgjwhj.cn

[T35] Lua：字典表
来源：http://fn.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://ni.yuntaijiaju.cn

[T36] Lua：函数
来源：http://oe.nicolike.cn

function add(a, b) return a + b end
来源：http://dj.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://rg.bjjhwx.cn

"a" .. "b"
来源：http://dt.shxzskj.cn

[T38] Lua：条件
来源：http://ax.panjiajie.cn

if x > 0 then print("正") end
来源：http://os.nszjky.cn

[T39] Lua：模式匹配
来源：http://gt.huixiangedu.cn

string.find(s, "%d+")
来源：http://dn.jianghongdianzi.cn

[T40] Lua：元表
来源：http://kn.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://zm.9csxet.cn

[T41] Perl：Hello World
来源：http://uz.521024.cn

print "Hello\n";
来源：http://kx.yuexingan06.cn

[T42] Perl：变量类型
来源：http://ih.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yb.newstarts.cn

[T43] Perl：字符串插值
来源：http://ql.colortex.cn

"值: $a"
来源：http://yk.newstarts.cn

[T44] Perl：条件
来源：http://ve.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://rp.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://co.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://pn.colortex.cn

[T46] Perl：哈希操作
来源：http://ev.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rl.panjiajie.cn

[T47] Perl：正则捕获
来源：http://gk.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pm.newstarts.cn

[T48] Perl：正则替换
来源：http://dh.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://nr.hahajie.cn

[T49] Perl：函数
来源：http://ru.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fh.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://tg.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rm.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://gc.gzmigu.cn

[T51] Scala：Hello World
来源：http://xw.hahajie.cn

println("Hello")
来源：http://bd.muxihuayi.cn

[T52] Scala：变量
来源：http://wm.shtwfgs.cn

val a = 1;  var b = 2
来源：http://op.hahajie.cn

[T53] Scala：字符串插值
来源：http://pg.szsharing.cn

s"值: $b"
来源：http://wm.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://ko.yuexingan06.cn


<!-- 参考信息 -->