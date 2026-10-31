代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tb.nicolike.cn

[R50] awk 求和
来源：http://wv.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zu.haigaiapp.cn

[R51] 排序去重取前几
来源：http://lm.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://np.huanxung.cn

[R52] 统计行数
来源：http://ni.haigaiapp.cn

wc -l a.txt
来源：http://wq.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://ga.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://io.yuexingan06.cn

[R54] 比较两个文件
来源：http://an.shtwfgs.cn

diff a.txt b.txt
来源：http://us.jctech888.com.cn

[R55] 压缩与解压
来源：http://nr.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ne.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://ka.jctech888.com.cn

scp file user@host:/path/
来源：http://kq.szxytkj.cn

[R57] 远程执行命令
来源：http://xc.asd995.cn

ssh user@host 'uptime'
来源：http://gs.jianghongdianzi.cn

[R58] 下载文件
来源：http://mu.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ya.colortex.cn

[R59] 发 POST JSON
来源：http://aq.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://na.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://pl.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tf.muxihuayi.cn

[R61] 磁盘占用
来源：http://as.521024.cn

df -h;  du -sh *
来源：http://zh.lnxyls.cn

[R62] 找最占空间的文件
来源：http://je.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://dc.wgjwhj.cn

[R63] 内存与进程
来源：http://yc.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://au.nicolike.cn

[R64] 结束进程
来源：http://eb.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://sg.shtwfgs.cn

[R65] 查看端口占用
来源：http://rm.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://du.shxzskj.cn

[R66] 定时任务
来源：http://xb.szsharing.cn

crontab -e;  crontab -l
来源：http://ze.521024.cn

[R67] 生成随机十六进制串
来源：http://pi.shtwfgs.cn

openssl rand -hex 16
来源：http://bc.nicolike.cn

[R68] 计算文件校验值
来源：http://yi.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dz.szxytkj.cn

[R69] 生成随机密码
来源：http://sg.521024.cn

head -c 16 /dev/urandom | base64
来源：http://wr.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://oo.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://uj.chemitech.net.cn

[R71] 日期格式化
来源：http://pt.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gc.szxytkj.cn

[R72] 等待端口就绪
来源：http://hn.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wm.shxzukj.cn

[R73] 分割大日志
来源：http://pl.hahajie.cn

split -l 1000 big.log part_
来源：http://xm.asd995.cn

[R74] 批量重命名
来源：http://hh.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jt.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ex.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://eb.jctech888.com.cn

[R76] 使用临时文件
来源：http://sj.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rz.hnjuh.cn

[R77] 读取用户输入
来源：http://fg.gzmigu.cn

read -rp "请输入: " ans
来源：http://vg.chemitech.net.cn

[R78] 交互式菜单
来源：http://ly.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pm.szxytkj.cn

[R79] 解析命令行选项
来源：http://wj.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cs.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://ab.asd995.cn

time ./run.sh
来源：http://nd.haigaiapp.cn

================================================================================
来源：http://lc.haigaiapp.cn

S. C / C++ 专题
来源：http://qz.yuntaijiaju.cn

================================================================================
来源：http://ok.huanxung.cn

[S01] C：Hello World
来源：http://no.huixinmuqiang.cn

#include <stdio.h>
来源：http://dx.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xk.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://kr.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://oa.huixiangedu.cn

[S03] C：读入整数
来源：http://kg.hnjuh.cn

int x; scanf("%d", &x);
来源：http://ni.chemitech.net.cn

[S04] C：字符串复制
来源：http://iz.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bz.panjiajie.cn

[S05] C：字符串长度
来源：http://ib.huixiangedu.cn

strlen(s)
来源：http://yn.9csxet.cn

[S06] C：字符串比较
来源：http://lf.asd995.cn

strcmp(a, b) == 0
来源：http://ds.newstarts.cn

[S07] C：数组遍历求和
来源：http://mx.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kv.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://kw.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://of.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://dx.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tl.szsharing.cn

[S10] C：指针与解引用
来源：http://at.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://kr.colortex.cn

[S11] C：逐行读文件
来源：http://yc.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://kd.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tf.newstarts.cn

fclose(f);
来源：http://ix.asd995.cn

[S12] C：写文件
来源：http://iy.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qu.bjjhwx.cn

[S13] C：宏定义
来源：http://tc.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xm.asd995.cn

[S14] C：枚举
来源：http://vq.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://ww.yuexingan06.cn

[S15] C：类型转换
来源：http://zg.bookmarksfly.cn

(double) a / b
来源：http://lh.asd995.cn

[S16] C：位操作置位
来源：http://sk.huixinmuqiang.cn

x |= (1 << 3);
来源：http://hp.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://cl.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oq.newstarts.cn

[S18] C：命令行参数
来源：http://bw.hnjuh.cn

int main(int argc, char **argv)
来源：http://rc.muxihuayi.cn

[S19] C：快速排序
来源：http://te.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tz.bjjhwx.cn

[S20] C：二分查找
来源：http://ea.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hj.hnjuh.cn

[S21] C：字符类别判断
来源：http://xr.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gf.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://yi.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://em.huanxung.cn

[S23] C：随机数
来源：http://qe.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pp.huanxung.cn

[S24] C：获取本地时间
来源：http://uk.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jl.bjjhwx.cn

[S25] C：内存拷贝
来源：http://km.9csxet.cn

memcpy(dst, src, n);
来源：http://ro.hnjuh.cn

[S26] C：内存清零
来源：http://lw.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://cj.shxzukj.cn

[S27] C：定义常量
来源：http://ty.asd995.cn

const double PI = 3.14159;
来源：http://kw.szxytkj.cn

[S28] C：静态变量
来源：http://uw.hahajie.cn

static int counter = 0;
来源：http://be.szsharing.cn

[S29] C：变参函数
来源：http://wb.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vw.yuexingan06.cn

[S30] C：头文件保护
来源：http://db.shxzukj.cn

#ifndef X_H
来源：http://uw.hahajie.cn

#define X_H
来源：http://yj.yuntaijiaju.cn

#endif
来源：http://dk.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://nl.newstarts.cn

#include <iostream>
来源：http://hc.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://bo.hahajie.cn

[S32] C++：字符串
来源：http://nj.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://ba.chemitech.net.cn

[S33] C++：vector 增删
来源：http://xz.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://no.szsharing.cn

[S34] C++：遍历 vector
来源：http://cw.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://dq.szxytkj.cn

[S35] C++：map
来源：http://zi.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mo.nszjky.cn

[S36] C++：unordered_map
来源：http://lr.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lf.asd995.cn

[S37] C++：set
来源：http://ra.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://an.chemitech.net.cn

[S38] C++：排序
来源：http://hc.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://ld.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://pd.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yf.nicolike.cn

[S40] C++：查找元素
来源：http://ud.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ma.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://vf.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://id.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://kr.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://wx.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://eq.521024.cn

auto p = std::make_unique<int>(5);
来源：http://rc.hahajie.cn

[S44] C++：引用传参
来源：http://nn.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://bz.nicolike.cn

[S45] C++：lambda
来源：http://jg.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mj.nszjky.cn

[S46] C++：函数模板
来源：http://du.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gr.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://gj.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bd.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ar.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mm.huanxung.cn

while (std::getline(in, line)) { }
来源：http://kq.szsharing.cn

[S49] C++：写文件
来源：http://uh.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wp.asd995.cn

[S50] C++：格式化数字
来源：http://af.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uv.shxzukj.cn

[S51] C++：显式类型转换
来源：http://ae.panjiajie.cn

static_cast<double>(a) / b
来源：http://on.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://ky.hahajie.cn

int size() const noexcept { return n_; }
来源：http://bo.shxzskj.cn

[S53] C++：移动语义
来源：http://li.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://ks.nicolike.cn

[S54] C++：异常处理
来源：http://as.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nr.szxytkj.cn

[S55] C++：结构化绑定
来源：http://cr.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ur.lnxyls.cn

[S56] C++：optional
来源：http://lf.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oi.shxzskj.cn

[S57] C++：编译期常量
来源：http://lw.panjiajie.cn

constexpr int N = 10;
来源：http://fl.lnxyls.cn

[S58] C++：命名空间
来源：http://ym.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://gg.muxihuayi.cn

[S59] C++：静态断言
来源：http://xn.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zn.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://kf.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://za.chemitech.net.cn

================================================================================
来源：http://it.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zu.nszjky.cn

================================================================================
来源：http://kz.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://lv.wgjwhj.cn

println("Hello")
来源：http://lr.jctech888.com.cn

[T02] Kotlin：变量
来源：http://vo.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fl.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://td.jctech888.com.cn

"值: $b"
来源：http://fs.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://ax.shxzukj.cn

val n: String? = null;  n?.length
来源：http://yq.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://uy.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nb.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://tg.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ji.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://as.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://br.colortex.cn

[T08] Kotlin：数据类
来源：http://wn.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://ba.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://qd.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://dx.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://np.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cu.wgjwhj.cn

[T11] Kotlin：协程
来源：http://ir.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tm.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://rd.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://gj.asd995.cn

[T13] Kotlin：只读 Map
来源：http://py.nicolike.cn

val m = mapOf("a" to 1)
来源：http://pi.9csxet.cn

[T14] Kotlin：循环
来源：http://gb.colortex.cn

for (i in 1..10) println(i)
来源：http://ae.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://az.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://ve.wgjwhj.cn

[T16] Swift：Hello World
来源：http://gk.bookmarksfly.cn

print("Hello")
来源：http://ti.panjiajie.cn

[T17] Swift：变量与常量
来源：http://ef.521024.cn

var a = 1;  let b = 2
来源：http://pn.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://dx.colortex.cn

"值: \(b)"
来源：http://az.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://qw.panjiajie.cn

if let n = opt { print(n) }
来源：http://ev.bjjhwx.cn

[T20] Swift：数组操作
来源：http://wf.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nl.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://wn.9csxet.cn

for x in a { print(x) }
来源：http://vx.colortex.cn

[T22] Swift：字典
来源：http://jr.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cx.521024.cn

[T23] Swift：函数
来源：http://rp.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kh.wgjwhj.cn

[T24] Swift：闭包
来源：http://xm.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pl.huanxung.cn

[T25] Swift：结构体
来源：http://fw.asd995.cn

struct P { var x: Int }
来源：http://cu.szxytkj.cn

[T26] Swift：类与重写
来源：http://sh.hahajie.cn

class A: Base { override func f() {} }
来源：http://ay.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://vd.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://nb.shtwfgs.cn

[T28] Swift：枚举
来源：http://gz.bookmarksfly.cn

enum Color { case red, green }
来源：http://tw.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://op.colortex.cn

guard let x = opt else { return }
来源：http://da.colortex.cn

[T30] Swift：协议
来源：http://va.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://sb.shtwfgs.cn

[T31] Lua：Hello World
来源：http://xs.gzmigu.cn

print("Hello")
来源：http://gl.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://tw.chemitech.net.cn

local a = 1
来源：http://lq.nszjky.cn

[T33] Lua：表（数组）
来源：http://wq.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kt.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://rg.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zz.9csxet.cn

[T35] Lua：字典表
来源：http://jy.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://ml.muxihuayi.cn

[T36] Lua：函数
来源：http://vz.521024.cn

function add(a, b) return a + b end
来源：http://ra.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://qe.bjjhwx.cn

"a" .. "b"
来源：http://kh.huanxung.cn

[T38] Lua：条件
来源：http://hb.9csxet.cn

if x > 0 then print("正") end
来源：http://ty.huanxung.cn

[T39] Lua：模式匹配
来源：http://an.shxzukj.cn

string.find(s, "%d+")
来源：http://sr.bookmarksfly.cn

[T40] Lua：元表
来源：http://fu.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://nf.bjjhwx.cn

[T41] Perl：Hello World
来源：http://oz.hnjuh.cn

print "Hello\n";
来源：http://er.panjiajie.cn

[T42] Perl：变量类型
来源：http://yo.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zo.huanxung.cn

[T43] Perl：字符串插值
来源：http://un.lnxyls.cn

"值: $a"
来源：http://xe.521024.cn

[T44] Perl：条件
来源：http://xf.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://zn.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://vg.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://zp.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://gl.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jb.hnjuh.cn

[T47] Perl：正则捕获
来源：http://qh.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ij.nicolike.cn

[T48] Perl：正则替换
来源：http://xd.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://br.jctech888.com.cn

[T49] Perl：函数
来源：http://kh.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fs.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://qz.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ob.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://sk.szxytkj.cn

[T51] Scala：Hello World
来源：http://mg.nicolike.cn

println("Hello")
来源：http://mt.yuexingan06.cn

[T52] Scala：变量
来源：http://ms.huixiangedu.cn


<!-- 参考信息 -->