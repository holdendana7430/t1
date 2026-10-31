代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://jd.yuntaijiaju.cn

[R52] 统计行数
来源：http://zc.huanxung.cn

wc -l a.txt
来源：http://el.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://re.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gq.lnxyls.cn

[R54] 比较两个文件
来源：http://fo.shxzukj.cn

diff a.txt b.txt
来源：http://wm.gzmigu.cn

[R55] 压缩与解压
来源：http://mw.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ys.shtwfgs.cn

[R56] 远程拷贝
来源：http://lh.9csxet.cn

scp file user@host:/path/
来源：http://nl.bjjhwx.cn

[R57] 远程执行命令
来源：http://gz.bjjhwx.cn

ssh user@host 'uptime'
来源：http://hn.9csxet.cn

[R58] 下载文件
来源：http://jj.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rt.shxzukj.cn

[R59] 发 POST JSON
来源：http://zz.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tq.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://tb.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ck.szxytkj.cn

[R61] 磁盘占用
来源：http://nd.yuntaijiaju.cn

df -h;  du -sh *
来源：http://ix.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://iq.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://vj.hahajie.cn

[R63] 内存与进程
来源：http://qx.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://zz.haigaiapp.cn

[R64] 结束进程
来源：http://kk.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://qb.chemitech.net.cn

[R65] 查看端口占用
来源：http://rx.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lp.nszjky.cn

[R66] 定时任务
来源：http://zy.szsharing.cn

crontab -e;  crontab -l
来源：http://jf.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ec.yuexingan06.cn

openssl rand -hex 16
来源：http://aw.9csxet.cn

[R68] 计算文件校验值
来源：http://ng.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ef.szxytkj.cn

[R69] 生成随机密码
来源：http://rh.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://sj.yuexingan06.cn

[R70] 时间戳与互转
来源：http://df.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://mp.yuntaijiaju.cn

[R71] 日期格式化
来源：http://li.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mh.asd995.cn

[R72] 等待端口就绪
来源：http://az.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://da.521024.cn

[R73] 分割大日志
来源：http://ls.shxzskj.cn

split -l 1000 big.log part_
来源：http://lv.nszjky.cn

[R74] 批量重命名
来源：http://sj.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ze.bjjhwx.cn

[R75] 导出环境变量
来源：http://gs.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://ol.chemitech.net.cn

[R76] 使用临时文件
来源：http://gq.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ej.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://lu.szxytkj.cn

read -rp "请输入: " ans
来源：http://bd.jctech888.com.cn

[R78] 交互式菜单
来源：http://hv.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pk.chemitech.net.cn

[R79] 解析命令行选项
来源：http://zz.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pl.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://kd.muxihuayi.cn

time ./run.sh
来源：http://xx.newstarts.cn

================================================================================
来源：http://zt.huixinmuqiang.cn

S. C / C++ 专题
来源：http://se.colortex.cn

================================================================================
来源：http://vd.huixinmuqiang.cn

[S01] C：Hello World
来源：http://xc.asd995.cn

#include <stdio.h>
来源：http://yb.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sw.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://sv.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://qj.huixiangedu.cn

[S03] C：读入整数
来源：http://qg.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://hk.chemitech.net.cn

[S04] C：字符串复制
来源：http://cx.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tc.yuexingan06.cn

[S05] C：字符串长度
来源：http://jw.huanxung.cn

strlen(s)
来源：http://hm.huixiangedu.cn

[S06] C：字符串比较
来源：http://up.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://jh.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://hl.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zx.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://hs.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xx.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://wa.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lu.521024.cn

[S10] C：指针与解引用
来源：http://gu.asd995.cn

int *p = &a;  *p = 5;
来源：http://xq.nicolike.cn

[S11] C：逐行读文件
来源：http://wt.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://si.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fe.jctech888.com.cn

fclose(f);
来源：http://tl.hahajie.cn

[S12] C：写文件
来源：http://jn.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fo.bjjhwx.cn

[S13] C：宏定义
来源：http://pb.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uf.szsharing.cn

[S14] C：枚举
来源：http://ko.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://zo.hnjuh.cn

[S15] C：类型转换
来源：http://br.huixinmuqiang.cn

(double) a / b
来源：http://sz.9csxet.cn

[S16] C：位操作置位
来源：http://ne.yuntaijiaju.cn

x |= (1 << 3);
来源：http://mo.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://qu.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sw.szxytkj.cn

[S18] C：命令行参数
来源：http://kz.521024.cn

int main(int argc, char **argv)
来源：http://gr.huanxung.cn

[S19] C：快速排序
来源：http://ei.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cc.jctech888.com.cn

[S20] C：二分查找
来源：http://me.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kb.shtwfgs.cn

[S21] C：字符类别判断
来源：http://oi.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pl.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://ed.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bl.gzmigu.cn

[S23] C：随机数
来源：http://aq.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sp.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://fb.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kl.nicolike.cn

[S25] C：内存拷贝
来源：http://bm.shxzskj.cn

memcpy(dst, src, n);
来源：http://sb.nszjky.cn

[S26] C：内存清零
来源：http://yu.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://go.szsharing.cn

[S27] C：定义常量
来源：http://za.shtwfgs.cn

const double PI = 3.14159;
来源：http://iu.colortex.cn

[S28] C：静态变量
来源：http://sl.nicolike.cn

static int counter = 0;
来源：http://ko.huixinmuqiang.cn

[S29] C：变参函数
来源：http://gf.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ep.muxihuayi.cn

[S30] C：头文件保护
来源：http://ki.szxytkj.cn

#ifndef X_H
来源：http://hv.asd995.cn

#define X_H
来源：http://rz.panjiajie.cn

#endif
来源：http://pb.shxzskj.cn

[S31] C++：Hello World
来源：http://ww.jctech888.com.cn

#include <iostream>
来源：http://vd.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://vh.hnjuh.cn

[S32] C++：字符串
来源：http://hm.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://ay.shtwfgs.cn

[S33] C++：vector 增删
来源：http://di.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xs.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://fj.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ie.gzmigu.cn

[S35] C++：map
来源：http://xh.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bg.szxytkj.cn

[S36] C++：unordered_map
来源：http://wr.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mc.newstarts.cn

[S37] C++：set
来源：http://bk.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rh.jianghongdianzi.cn

[S38] C++：排序
来源：http://jj.asd995.cn

std::sort(v.begin(), v.end());
来源：http://hd.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://jo.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bg.nszjky.cn

[S40] C++：查找元素
来源：http://jb.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cn.nszjky.cn

[S41] C++：类与构造函数
来源：http://mo.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zb.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://rj.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://pt.chemitech.net.cn

[S43] C++：智能指针
来源：http://xt.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://sz.521024.cn

[S44] C++：引用传参
来源：http://qr.asd995.cn

void inc(int &x) { ++x; }
来源：http://gz.jianghongdianzi.cn

[S45] C++：lambda
来源：http://bs.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bv.bookmarksfly.cn

[S46] C++：函数模板
来源：http://dj.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ug.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://kn.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tf.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://jh.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vj.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://rf.wgjwhj.cn

[S49] C++：写文件
来源：http://re.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ca.asd995.cn

[S50] C++：格式化数字
来源：http://zn.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ts.szxytkj.cn

[S51] C++：显式类型转换
来源：http://ja.huanxung.cn

static_cast<double>(a) / b
来源：http://nn.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://qn.521024.cn

int size() const noexcept { return n_; }
来源：http://cd.newstarts.cn

[S53] C++：移动语义
来源：http://bx.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://mm.hahajie.cn

[S54] C++：异常处理
来源：http://dv.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xy.nicolike.cn

[S55] C++：结构化绑定
来源：http://vh.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jv.huixinmuqiang.cn

[S56] C++：optional
来源：http://uk.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hu.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://vc.shtwfgs.cn

constexpr int N = 10;
来源：http://oq.colortex.cn

[S58] C++：命名空间
来源：http://ci.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://hw.colortex.cn

[S59] C++：静态断言
来源：http://mo.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ax.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://ep.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hc.hahajie.cn

================================================================================
来源：http://tr.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://km.hnjuh.cn

================================================================================
来源：http://hx.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://sb.yuexingan06.cn

println("Hello")
来源：http://wz.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ue.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ny.colortex.cn

[T03] Kotlin：字符串模板
来源：http://kj.shxzukj.cn

"值: $b"
来源：http://sv.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://fe.panjiajie.cn

val n: String? = null;  n?.length
来源：http://mp.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://gh.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xf.newstarts.cn

[T06] Kotlin：集合映射
来源：http://cj.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cz.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://jt.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jj.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://hf.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://bg.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://ut.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://xh.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://ti.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sw.hahajie.cn

[T11] Kotlin：协程
来源：http://pe.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ou.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://yv.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://cx.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://vl.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://dn.huanxung.cn

[T14] Kotlin：循环
来源：http://ex.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://kp.nicolike.cn

[T15] Kotlin：接口
来源：http://xu.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://dv.lnxyls.cn

[T16] Swift：Hello World
来源：http://ic.9csxet.cn

print("Hello")
来源：http://yu.panjiajie.cn

[T17] Swift：变量与常量
来源：http://lq.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://ny.szsharing.cn

[T18] Swift：字符串插值
来源：http://gp.asd995.cn

"值: \(b)"
来源：http://vr.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://ec.shtwfgs.cn

if let n = opt { print(n) }
来源：http://sd.521024.cn

[T20] Swift：数组操作
来源：http://ul.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://et.shtwfgs.cn

[T21] Swift：遍历
来源：http://fj.shxzukj.cn

for x in a { print(x) }
来源：http://rl.nicolike.cn

[T22] Swift：字典
来源：http://ee.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ks.shxzukj.cn

[T23] Swift：函数
来源：http://xk.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lb.szxytkj.cn

[T24] Swift：闭包
来源：http://ce.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qc.chemitech.net.cn

[T25] Swift：结构体
来源：http://fc.521024.cn

struct P { var x: Int }
来源：http://wv.521024.cn

[T26] Swift：类与重写
来源：http://kz.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://ts.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://gd.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://wj.chemitech.net.cn

[T28] Swift：枚举
来源：http://nh.jctech888.com.cn

enum Color { case red, green }
来源：http://uc.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://li.hnjuh.cn

guard let x = opt else { return }
来源：http://fr.haigaiapp.cn

[T30] Swift：协议
来源：http://jv.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://zl.szsharing.cn

[T31] Lua：Hello World
来源：http://my.shxzukj.cn

print("Hello")
来源：http://pt.asd995.cn

[T32] Lua：局部变量
来源：http://kn.shtwfgs.cn

local a = 1
来源：http://rg.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://db.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ef.asd995.cn

[T34] Lua：遍历表
来源：http://ly.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ru.haigaiapp.cn

[T35] Lua：字典表
来源：http://ry.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://wb.szxytkj.cn

[T36] Lua：函数
来源：http://wg.huixiangedu.cn

function add(a, b) return a + b end
来源：http://vq.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://id.gzmigu.cn

"a" .. "b"
来源：http://fg.9csxet.cn

[T38] Lua：条件
来源：http://dj.haigaiapp.cn

if x > 0 then print("正") end
来源：http://lb.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://pa.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://gp.lnxyls.cn

[T40] Lua：元表
来源：http://zt.nicolike.cn

setmetatable({}, { __index = base })
来源：http://om.yuexingan06.cn

[T41] Perl：Hello World
来源：http://tw.shxzukj.cn

print "Hello\n";
来源：http://qx.shtwfgs.cn

[T42] Perl：变量类型
来源：http://lp.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jw.newstarts.cn

[T43] Perl：字符串插值
来源：http://fx.hnjuh.cn

"值: $a"
来源：http://zo.szxytkj.cn

[T44] Perl：条件
来源：http://de.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://pi.szsharing.cn

[T45] Perl：数组遍历
来源：http://do.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://qv.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://op.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cf.nszjky.cn

[T47] Perl：正则捕获
来源：http://dk.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lb.huanxung.cn

[T48] Perl：正则替换
来源：http://gd.panjiajie.cn

$s =~ s/old/new/g;
来源：http://wy.huixinmuqiang.cn

[T49] Perl：函数
来源：http://vv.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ad.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://op.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xw.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://hz.shxzskj.cn

[T51] Scala：Hello World
来源：http://rv.shxzukj.cn

println("Hello")
来源：http://wx.nszjky.cn

[T52] Scala：变量
来源：http://hx.huixiangedu.cn

val a = 1;  var b = 2
来源：http://hn.panjiajie.cn

[T53] Scala：字符串插值
来源：http://lo.jianghongdianzi.cn

s"值: $b"
来源：http://ww.huixiangedu.cn

[T54] Scala：集合映射
来源：http://pa.shxzukj.cn


<!-- 参考信息 -->