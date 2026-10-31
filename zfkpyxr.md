代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://xp.shxzskj.cn

[R52] 统计行数
来源：http://oy.hnjuh.cn

wc -l a.txt
来源：http://cu.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://qr.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qz.521024.cn

[R54] 比较两个文件
来源：http://vn.huanxung.cn

diff a.txt b.txt
来源：http://cl.9csxet.cn

[R55] 压缩与解压
来源：http://il.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hw.szxytkj.cn

[R56] 远程拷贝
来源：http://km.szxytkj.cn

scp file user@host:/path/
来源：http://wc.szxytkj.cn

[R57] 远程执行命令
来源：http://wv.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://ip.lnxyls.cn

[R58] 下载文件
来源：http://gj.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tr.colortex.cn

[R59] 发 POST JSON
来源：http://md.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nd.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://aa.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xk.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://wt.muxihuayi.cn

df -h;  du -sh *
来源：http://bk.521024.cn

[R62] 找最占空间的文件
来源：http://bm.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://lc.yuntaijiaju.cn

[R63] 内存与进程
来源：http://vj.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://rl.asd995.cn

[R64] 结束进程
来源：http://ey.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://iv.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://ae.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mb.gzmigu.cn

[R66] 定时任务
来源：http://kr.huanxung.cn

crontab -e;  crontab -l
来源：http://qr.nicolike.cn

[R67] 生成随机十六进制串
来源：http://tl.huixiangedu.cn

openssl rand -hex 16
来源：http://fw.yuexingan06.cn

[R68] 计算文件校验值
来源：http://of.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fr.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://hh.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://vi.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://pi.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://sh.shtwfgs.cn

[R71] 日期格式化
来源：http://cb.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kk.lnxyls.cn

[R72] 等待端口就绪
来源：http://zt.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://at.jctech888.com.cn

[R73] 分割大日志
来源：http://wr.shtwfgs.cn

split -l 1000 big.log part_
来源：http://fy.shxzukj.cn

[R74] 批量重命名
来源：http://hg.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aj.nicolike.cn

[R75] 导出环境变量
来源：http://dl.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ko.jctech888.com.cn

[R76] 使用临时文件
来源：http://ih.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xw.panjiajie.cn

[R77] 读取用户输入
来源：http://fs.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ox.huanxung.cn

[R78] 交互式菜单
来源：http://ep.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ia.nszjky.cn

[R79] 解析命令行选项
来源：http://qz.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://db.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://in.521024.cn

time ./run.sh
来源：http://hi.hnjuh.cn

================================================================================
来源：http://td.szsharing.cn

S. C / C++ 专题
来源：http://ak.bjjhwx.cn

================================================================================
来源：http://dk.huanxung.cn

[S01] C：Hello World
来源：http://qy.chemitech.net.cn

#include <stdio.h>
来源：http://ah.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mj.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://by.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://uh.9csxet.cn

[S03] C：读入整数
来源：http://oz.szsharing.cn

int x; scanf("%d", &x);
来源：http://jv.hahajie.cn

[S04] C：字符串复制
来源：http://tw.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://si.shtwfgs.cn

[S05] C：字符串长度
来源：http://nl.colortex.cn

strlen(s)
来源：http://fw.szxytkj.cn

[S06] C：字符串比较
来源：http://py.chemitech.net.cn

strcmp(a, b) == 0
来源：http://qv.521024.cn

[S07] C：数组遍历求和
来源：http://rt.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eu.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://lg.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xe.521024.cn

[S09] C：结构体定义与初始化
来源：http://it.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bn.hahajie.cn

[S10] C：指针与解引用
来源：http://xz.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://xm.shxzskj.cn

[S11] C：逐行读文件
来源：http://rl.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://fk.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ai.yuntaijiaju.cn

fclose(f);
来源：http://vb.9csxet.cn

[S12] C：写文件
来源：http://wm.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cr.shtwfgs.cn

[S13] C：宏定义
来源：http://ln.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://js.jianghongdianzi.cn

[S14] C：枚举
来源：http://ed.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://ko.szxytkj.cn

[S15] C：类型转换
来源：http://mv.huanxung.cn

(double) a / b
来源：http://kg.szsharing.cn

[S16] C：位操作置位
来源：http://br.huixiangedu.cn

x |= (1 << 3);
来源：http://is.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://ua.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://on.gzmigu.cn

[S18] C：命令行参数
来源：http://cb.shxzukj.cn

int main(int argc, char **argv)
来源：http://ea.szsharing.cn

[S19] C：快速排序
来源：http://ne.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cq.bjjhwx.cn

[S20] C：二分查找
来源：http://ae.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://in.colortex.cn

[S21] C：字符类别判断
来源：http://is.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zw.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://mr.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rs.huixiangedu.cn

[S23] C：随机数
来源：http://nu.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gx.9csxet.cn

[S24] C：获取本地时间
来源：http://kz.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hv.shxzukj.cn

[S25] C：内存拷贝
来源：http://iq.newstarts.cn

memcpy(dst, src, n);
来源：http://bb.yuexingan06.cn

[S26] C：内存清零
来源：http://fl.newstarts.cn

memset(a, 0, sizeof a);
来源：http://qd.colortex.cn

[S27] C：定义常量
来源：http://jn.huanxung.cn

const double PI = 3.14159;
来源：http://ba.hahajie.cn

[S28] C：静态变量
来源：http://zk.newstarts.cn

static int counter = 0;
来源：http://as.huixiangedu.cn

[S29] C：变参函数
来源：http://oc.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kg.wgjwhj.cn

[S30] C：头文件保护
来源：http://xr.asd995.cn

#ifndef X_H
来源：http://ov.gzmigu.cn

#define X_H
来源：http://du.nicolike.cn

#endif
来源：http://ah.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://en.szxytkj.cn

#include <iostream>
来源：http://ir.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://lm.shxzukj.cn

[S32] C++：字符串
来源：http://cz.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://ad.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ea.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ff.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://kl.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://lu.yuexingan06.cn

[S35] C++：map
来源：http://ka.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rf.9csxet.cn

[S36] C++：unordered_map
来源：http://jm.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xk.wgjwhj.cn

[S37] C++：set
来源：http://fl.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://co.hahajie.cn

[S38] C++：排序
来源：http://vh.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://kp.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://pc.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fs.9csxet.cn

[S40] C++：查找元素
来源：http://hh.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lh.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://ym.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yi.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://dd.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://uc.colortex.cn

[S43] C++：智能指针
来源：http://on.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://li.lnxyls.cn

[S44] C++：引用传参
来源：http://sw.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://xl.muxihuayi.cn

[S45] C++：lambda
来源：http://ls.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pv.wgjwhj.cn

[S46] C++：函数模板
来源：http://pt.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sz.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://yq.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mz.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://uw.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rg.asd995.cn

while (std::getline(in, line)) { }
来源：http://oi.yuntaijiaju.cn

[S49] C++：写文件
来源：http://ww.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oi.huixiangedu.cn

[S50] C++：格式化数字
来源：http://or.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nv.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://ms.shxzskj.cn

static_cast<double>(a) / b
来源：http://cn.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://wv.9csxet.cn

int size() const noexcept { return n_; }
来源：http://yz.nicolike.cn

[S53] C++：移动语义
来源：http://si.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://rm.hahajie.cn

[S54] C++：异常处理
来源：http://sn.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vs.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://fc.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qq.lnxyls.cn

[S56] C++：optional
来源：http://fh.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fb.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://xa.huixinmuqiang.cn

constexpr int N = 10;
来源：http://ya.yuexingan06.cn

[S58] C++：命名空间
来源：http://jl.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://ne.szxytkj.cn

[S59] C++：静态断言
来源：http://cg.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rk.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://bd.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hl.nszjky.cn

================================================================================
来源：http://lk.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jr.bookmarksfly.cn

================================================================================
来源：http://nl.521024.cn

[T01] Kotlin：Hello World
来源：http://mu.huixiangedu.cn

println("Hello")
来源：http://do.jctech888.com.cn

[T02] Kotlin：变量
来源：http://qh.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nx.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://tf.hnjuh.cn

"值: $b"
来源：http://af.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://nn.lnxyls.cn

val n: String? = null;  n?.length
来源：http://py.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://qh.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gw.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://ug.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qq.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://xe.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mm.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://ri.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://ls.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://ed.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://sc.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://uy.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rz.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://xq.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gn.colortex.cn

[T12] Kotlin：解构声明
来源：http://eq.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://yj.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://gr.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://za.yuexingan06.cn

[T14] Kotlin：循环
来源：http://ix.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://fm.muxihuayi.cn

[T15] Kotlin：接口
来源：http://mw.nszjky.cn

interface Shape { fun area(): Double }
来源：http://ur.nszjky.cn

[T16] Swift：Hello World
来源：http://uj.chemitech.net.cn

print("Hello")
来源：http://ab.hahajie.cn

[T17] Swift：变量与常量
来源：http://ke.panjiajie.cn

var a = 1;  let b = 2
来源：http://pv.gzmigu.cn

[T18] Swift：字符串插值
来源：http://jl.hahajie.cn

"值: \(b)"
来源：http://ug.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://ow.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://us.szxytkj.cn

[T20] Swift：数组操作
来源：http://mi.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kp.9csxet.cn

[T21] Swift：遍历
来源：http://rt.huixinmuqiang.cn

for x in a { print(x) }
来源：http://kq.nicolike.cn

[T22] Swift：字典
来源：http://co.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fm.yuexingan06.cn

[T23] Swift：函数
来源：http://dl.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vk.shxzukj.cn

[T24] Swift：闭包
来源：http://wq.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ry.newstarts.cn

[T25] Swift：结构体
来源：http://fo.wgjwhj.cn

struct P { var x: Int }
来源：http://pg.wgjwhj.cn

[T26] Swift：类与重写
来源：http://xe.shxzukj.cn

class A: Base { override func f() {} }
来源：http://ju.jctech888.com.cn

[T27] Swift：错误处理
来源：http://qx.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://iv.newstarts.cn

[T28] Swift：枚举
来源：http://mx.hahajie.cn

enum Color { case red, green }
来源：http://um.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://of.yuexingan06.cn

guard let x = opt else { return }
来源：http://vn.chemitech.net.cn

[T30] Swift：协议
来源：http://bl.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://kf.yuexingan06.cn

[T31] Lua：Hello World
来源：http://ka.wgjwhj.cn

print("Hello")
来源：http://kg.huixiangedu.cn

[T32] Lua：局部变量
来源：http://pc.huixiangedu.cn

local a = 1
来源：http://bv.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://xn.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cx.shxzukj.cn

[T34] Lua：遍历表
来源：http://zd.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ui.muxihuayi.cn

[T35] Lua：字典表
来源：http://dc.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://bc.521024.cn

[T36] Lua：函数
来源：http://tc.shxzukj.cn

function add(a, b) return a + b end
来源：http://zu.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://wt.haigaiapp.cn

"a" .. "b"
来源：http://hi.huixiangedu.cn

[T38] Lua：条件
来源：http://fa.wgjwhj.cn

if x > 0 then print("正") end
来源：http://vp.lnxyls.cn

[T39] Lua：模式匹配
来源：http://on.muxihuayi.cn

string.find(s, "%d+")
来源：http://eo.huixiangedu.cn

[T40] Lua：元表
来源：http://ei.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://vz.yuexingan06.cn

[T41] Perl：Hello World
来源：http://tk.gzmigu.cn

print "Hello\n";
来源：http://di.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://se.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ks.gzmigu.cn

[T43] Perl：字符串插值
来源：http://ov.colortex.cn

"值: $a"
来源：http://lh.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ei.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://oo.colortex.cn

[T45] Perl：数组遍历
来源：http://lk.colortex.cn

for my $x (@arr) { print $x; }
来源：http://qz.gzmigu.cn

[T46] Perl：哈希操作
来源：http://ra.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jm.szxytkj.cn

[T47] Perl：正则捕获
来源：http://ob.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tj.wgjwhj.cn

[T48] Perl：正则替换
来源：http://xb.9csxet.cn

$s =~ s/old/new/g;
来源：http://lb.szxytkj.cn

[T49] Perl：函数
来源：http://jb.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kl.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://rh.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://br.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vy.shxzukj.cn

[T51] Scala：Hello World
来源：http://nw.yuexingan06.cn

println("Hello")
来源：http://fg.muxihuayi.cn

[T52] Scala：变量
来源：http://mn.jctech888.com.cn

val a = 1;  var b = 2
来源：http://kj.panjiajie.cn

[T53] Scala：字符串插值
来源：http://ik.newstarts.cn

s"值: $b"
来源：http://ik.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://xb.szxytkj.cn


<!-- 参考信息 -->