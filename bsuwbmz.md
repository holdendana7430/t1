代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eh.shxzukj.cn

[R56] 远程拷贝
来源：http://kh.jianghongdianzi.cn

scp file user@host:/path/
来源：http://ik.shtwfgs.cn

[R57] 远程执行命令
来源：http://lh.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://mi.lnxyls.cn

[R58] 下载文件
来源：http://dl.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fv.yuexingan06.cn

[R59] 发 POST JSON
来源：http://va.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ar.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://kl.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ex.jctech888.com.cn

[R61] 磁盘占用
来源：http://ud.jianghongdianzi.cn

df -h;  du -sh *
来源：http://tz.nicolike.cn

[R62] 找最占空间的文件
来源：http://rs.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://gp.shxzskj.cn

[R63] 内存与进程
来源：http://fr.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://gc.hahajie.cn

[R64] 结束进程
来源：http://xf.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://ol.asd995.cn

[R65] 查看端口占用
来源：http://qw.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tc.szsharing.cn

[R66] 定时任务
来源：http://mn.9csxet.cn

crontab -e;  crontab -l
来源：http://cg.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://yn.nicolike.cn

openssl rand -hex 16
来源：http://ld.chemitech.net.cn

[R68] 计算文件校验值
来源：http://re.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wm.nicolike.cn

[R69] 生成随机密码
来源：http://bo.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://gs.shtwfgs.cn

[R70] 时间戳与互转
来源：http://cg.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ul.shxzskj.cn

[R71] 日期格式化
来源：http://ys.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mk.9csxet.cn

[R72] 等待端口就绪
来源：http://zb.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ji.gzmigu.cn

[R73] 分割大日志
来源：http://ap.huixiangedu.cn

split -l 1000 big.log part_
来源：http://ij.chemitech.net.cn

[R74] 批量重命名
来源：http://fs.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oj.colortex.cn

[R75] 导出环境变量
来源：http://uf.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://ci.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://am.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mq.chemitech.net.cn

[R77] 读取用户输入
来源：http://kl.jctech888.com.cn

read -rp "请输入: " ans
来源：http://sx.yuexingan06.cn

[R78] 交互式菜单
来源：http://sb.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yk.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://fp.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kb.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ea.huixiangedu.cn

time ./run.sh
来源：http://rn.nszjky.cn

================================================================================
来源：http://fc.jianghongdianzi.cn

S. C / C++ 专题
来源：http://pa.jianghongdianzi.cn

================================================================================
来源：http://kr.bjjhwx.cn

[S01] C：Hello World
来源：http://dp.yuntaijiaju.cn

#include <stdio.h>
来源：http://jv.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vd.newstarts.cn

[S02] C：变量与格式化输出
来源：http://gi.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://qi.shxzskj.cn

[S03] C：读入整数
来源：http://oq.newstarts.cn

int x; scanf("%d", &x);
来源：http://cj.chemitech.net.cn

[S04] C：字符串复制
来源：http://lm.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uv.shxzukj.cn

[S05] C：字符串长度
来源：http://ik.shxzukj.cn

strlen(s)
来源：http://xa.huanxung.cn

[S06] C：字符串比较
来源：http://sc.shtwfgs.cn

strcmp(a, b) == 0
来源：http://hk.szxytkj.cn

[S07] C：数组遍历求和
来源：http://av.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mg.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://zr.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gd.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://rn.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vb.szsharing.cn

[S10] C：指针与解引用
来源：http://lj.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://et.szxytkj.cn

[S11] C：逐行读文件
来源：http://nf.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://di.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ea.chemitech.net.cn

fclose(f);
来源：http://ug.panjiajie.cn

[S12] C：写文件
来源：http://xt.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eu.nszjky.cn

[S13] C：宏定义
来源：http://sx.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pg.hahajie.cn

[S14] C：枚举
来源：http://lb.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://qo.nicolike.cn

[S15] C：类型转换
来源：http://pu.shxzukj.cn

(double) a / b
来源：http://tw.szsharing.cn

[S16] C：位操作置位
来源：http://zk.huixinmuqiang.cn

x |= (1 << 3);
来源：http://lu.newstarts.cn

[S17] C：安全拼接字符串
来源：http://hq.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ws.jctech888.com.cn

[S18] C：命令行参数
来源：http://yo.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://jm.jctech888.com.cn

[S19] C：快速排序
来源：http://sl.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lo.yuexingan06.cn

[S20] C：二分查找
来源：http://fy.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lq.szxytkj.cn

[S21] C：字符类别判断
来源：http://gs.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://id.shtwfgs.cn

[S22] C：字符串转数字
来源：http://dt.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kv.newstarts.cn

[S23] C：随机数
来源：http://xy.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gx.yuexingan06.cn

[S24] C：获取本地时间
来源：http://qf.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gl.chemitech.net.cn

[S25] C：内存拷贝
来源：http://im.szsharing.cn

memcpy(dst, src, n);
来源：http://qq.haigaiapp.cn

[S26] C：内存清零
来源：http://qz.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://ku.bookmarksfly.cn

[S27] C：定义常量
来源：http://ig.521024.cn

const double PI = 3.14159;
来源：http://yt.szxytkj.cn

[S28] C：静态变量
来源：http://gx.jctech888.com.cn

static int counter = 0;
来源：http://sp.asd995.cn

[S29] C：变参函数
来源：http://fk.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uf.colortex.cn

[S30] C：头文件保护
来源：http://gj.huanxung.cn

#ifndef X_H
来源：http://bu.colortex.cn

#define X_H
来源：http://ur.bookmarksfly.cn

#endif
来源：http://xv.wgjwhj.cn

[S31] C++：Hello World
来源：http://vf.huixinmuqiang.cn

#include <iostream>
来源：http://bj.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://sc.newstarts.cn

[S32] C++：字符串
来源：http://cy.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://xb.muxihuayi.cn

[S33] C++：vector 增删
来源：http://ov.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kp.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://nz.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://ko.bjjhwx.cn

[S35] C++：map
来源：http://vf.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eg.9csxet.cn

[S36] C++：unordered_map
来源：http://gx.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cg.yuntaijiaju.cn

[S37] C++：set
来源：http://rg.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hl.yuntaijiaju.cn

[S38] C++：排序
来源：http://pi.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://by.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://lu.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ct.lnxyls.cn

[S40] C++：查找元素
来源：http://rt.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hf.lnxyls.cn

[S41] C++：类与构造函数
来源：http://nw.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ex.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://cz.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://zr.huanxung.cn

[S43] C++：智能指针
来源：http://rx.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://tb.nszjky.cn

[S44] C++：引用传参
来源：http://ax.9csxet.cn

void inc(int &x) { ++x; }
来源：http://mp.huixinmuqiang.cn

[S45] C++：lambda
来源：http://pb.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xk.newstarts.cn

[S46] C++：函数模板
来源：http://gr.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sw.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://sy.lnxyls.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ct.colortex.cn

[S48] C++：逐行读文件
来源：http://yx.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gt.nszjky.cn

while (std::getline(in, line)) { }
来源：http://dy.muxihuayi.cn

[S49] C++：写文件
来源：http://xs.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kr.hnjuh.cn

[S50] C++：格式化数字
来源：http://et.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://er.9csxet.cn

[S51] C++：显式类型转换
来源：http://qi.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://zd.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://zt.asd995.cn

int size() const noexcept { return n_; }
来源：http://os.nszjky.cn

[S53] C++：移动语义
来源：http://tq.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://nq.lnxyls.cn

[S54] C++：异常处理
来源：http://gu.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ih.panjiajie.cn

[S55] C++：结构化绑定
来源：http://kb.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bd.521024.cn

[S56] C++：optional
来源：http://ts.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ga.hahajie.cn

[S57] C++：编译期常量
来源：http://pu.haigaiapp.cn

constexpr int N = 10;
来源：http://ma.haigaiapp.cn

[S58] C++：命名空间
来源：http://on.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://qg.521024.cn

[S59] C++：静态断言
来源：http://qm.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wh.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://te.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ps.yuexingan06.cn

================================================================================
来源：http://fw.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wb.szsharing.cn

================================================================================
来源：http://ap.szsharing.cn

[T01] Kotlin：Hello World
来源：http://yw.nszjky.cn

println("Hello")
来源：http://bi.haigaiapp.cn

[T02] Kotlin：变量
来源：http://yq.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iy.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://oi.yuexingan06.cn

"值: $b"
来源：http://lk.asd995.cn

[T04] Kotlin：空安全
来源：http://qj.hahajie.cn

val n: String? = null;  n?.length
来源：http://qt.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://za.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vl.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://di.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nm.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://ri.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wv.shxzukj.cn

[T08] Kotlin：数据类
来源：http://oe.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://fi.asd995.cn

[T09] Kotlin：扩展函数
来源：http://xt.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://zx.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://ye.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://in.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://vx.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rt.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://sf.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://fe.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://nz.521024.cn

val m = mapOf("a" to 1)
来源：http://vn.panjiajie.cn

[T14] Kotlin：循环
来源：http://ao.huanxung.cn

for (i in 1..10) println(i)
来源：http://nk.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://bb.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://oh.9csxet.cn

[T16] Swift：Hello World
来源：http://hb.nszjky.cn

print("Hello")
来源：http://wb.nszjky.cn

[T17] Swift：变量与常量
来源：http://nb.bjjhwx.cn

var a = 1;  let b = 2
来源：http://kn.nicolike.cn

[T18] Swift：字符串插值
来源：http://un.szxytkj.cn

"值: \(b)"
来源：http://qs.shxzukj.cn

[T19] Swift：可选绑定
来源：http://kp.shxzukj.cn

if let n = opt { print(n) }
来源：http://tz.521024.cn

[T20] Swift：数组操作
来源：http://ch.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iu.szxytkj.cn

[T21] Swift：遍历
来源：http://nn.hnjuh.cn

for x in a { print(x) }
来源：http://nn.gzmigu.cn

[T22] Swift：字典
来源：http://nz.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bv.colortex.cn

[T23] Swift：函数
来源：http://do.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ip.bjjhwx.cn

[T24] Swift：闭包
来源：http://oh.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ze.shxzskj.cn

[T25] Swift：结构体
来源：http://mj.jianghongdianzi.cn

struct P { var x: Int }
来源：http://hz.shxzukj.cn

[T26] Swift：类与重写
来源：http://ag.shxzukj.cn

class A: Base { override func f() {} }
来源：http://yi.wgjwhj.cn

[T27] Swift：错误处理
来源：http://ap.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://mq.szxytkj.cn

[T28] Swift：枚举
来源：http://tu.huanxung.cn

enum Color { case red, green }
来源：http://fw.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://qz.gzmigu.cn

guard let x = opt else { return }
来源：http://ix.panjiajie.cn

[T30] Swift：协议
来源：http://pz.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://zi.shxzukj.cn

[T31] Lua：Hello World
来源：http://ol.shxzukj.cn

print("Hello")
来源：http://sk.521024.cn

[T32] Lua：局部变量
来源：http://vx.muxihuayi.cn

local a = 1
来源：http://kk.colortex.cn

[T33] Lua：表（数组）
来源：http://kk.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ud.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://pg.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qa.huixiangedu.cn

[T35] Lua：字典表
来源：http://hh.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://lq.hnjuh.cn

[T36] Lua：函数
来源：http://zf.gzmigu.cn

function add(a, b) return a + b end
来源：http://gh.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://wb.9csxet.cn

"a" .. "b"
来源：http://wq.jctech888.com.cn

[T38] Lua：条件
来源：http://lv.newstarts.cn

if x > 0 then print("正") end
来源：http://ap.shxzukj.cn

[T39] Lua：模式匹配
来源：http://jb.panjiajie.cn

string.find(s, "%d+")
来源：http://ig.chemitech.net.cn

[T40] Lua：元表
来源：http://ul.nicolike.cn

setmetatable({}, { __index = base })
来源：http://hl.hahajie.cn

[T41] Perl：Hello World
来源：http://zh.huanxung.cn

print "Hello\n";
来源：http://bf.haigaiapp.cn

[T42] Perl：变量类型
来源：http://ny.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fg.colortex.cn

[T43] Perl：字符串插值
来源：http://ao.wgjwhj.cn

"值: $a"
来源：http://tj.lnxyls.cn

[T44] Perl：条件
来源：http://rf.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://jo.huanxung.cn

[T45] Perl：数组遍历
来源：http://if.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://ig.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://st.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dh.nicolike.cn

[T47] Perl：正则捕获
来源：http://jt.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://en.jctech888.com.cn

[T48] Perl：正则替换
来源：http://fj.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://rw.muxihuayi.cn

[T49] Perl：函数
来源：http://md.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rw.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://gd.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cb.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://nw.9csxet.cn

[T51] Scala：Hello World
来源：http://zy.9csxet.cn

println("Hello")
来源：http://ss.bookmarksfly.cn

[T52] Scala：变量
来源：http://az.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://rh.asd995.cn

[T53] Scala：字符串插值
来源：http://pt.newstarts.cn

s"值: $b"
来源：http://xm.szsharing.cn

[T54] Scala：集合映射
来源：http://cl.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://iz.szsharing.cn

[T55] Scala：集合过滤
来源：http://ah.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yy.gzmigu.cn

[T56] Scala：样例类
来源：http://cc.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://kk.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://jv.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ex.panjiajie.cn

[T58] Scala：函数定义
来源：http://jj.bookmarksfly.cn


<!-- 参考信息 -->