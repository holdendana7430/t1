代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://qv.gzmigu.cn

[R52] 统计行数
来源：http://xu.szxytkj.cn

wc -l a.txt
来源：http://lu.asd995.cn

[R53] 查看文件头与实时尾
来源：http://cl.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kg.hahajie.cn

[R54] 比较两个文件
来源：http://on.521024.cn

diff a.txt b.txt
来源：http://zk.bookmarksfly.cn

[R55] 压缩与解压
来源：http://ch.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pz.bookmarksfly.cn

[R56] 远程拷贝
来源：http://si.521024.cn

scp file user@host:/path/
来源：http://qm.huanxung.cn

[R57] 远程执行命令
来源：http://wc.huixiangedu.cn

ssh user@host 'uptime'
来源：http://gy.muxihuayi.cn

[R58] 下载文件
来源：http://vt.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xh.lnxyls.cn

[R59] 发 POST JSON
来源：http://ti.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gr.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://xp.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rh.panjiajie.cn

[R61] 磁盘占用
来源：http://lg.asd995.cn

df -h;  du -sh *
来源：http://pe.nicolike.cn

[R62] 找最占空间的文件
来源：http://xk.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://sn.shxzukj.cn

[R63] 内存与进程
来源：http://sa.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://zy.shxzskj.cn

[R64] 结束进程
来源：http://pr.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://kz.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://tv.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nt.nszjky.cn

[R66] 定时任务
来源：http://wu.gzmigu.cn

crontab -e;  crontab -l
来源：http://ai.huanxung.cn

[R67] 生成随机十六进制串
来源：http://wp.newstarts.cn

openssl rand -hex 16
来源：http://gi.jctech888.com.cn

[R68] 计算文件校验值
来源：http://mn.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cl.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://al.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://vu.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://ce.newstarts.cn

date +%s;  date -d @1700000000
来源：http://jo.newstarts.cn

[R71] 日期格式化
来源：http://st.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tb.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://ql.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dg.jianghongdianzi.cn

[R73] 分割大日志
来源：http://gh.muxihuayi.cn

split -l 1000 big.log part_
来源：http://ok.huanxung.cn

[R74] 批量重命名
来源：http://nx.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yq.bjjhwx.cn

[R75] 导出环境变量
来源：http://hk.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ri.nicolike.cn

[R76] 使用临时文件
来源：http://ya.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ti.gzmigu.cn

[R77] 读取用户输入
来源：http://kv.hnjuh.cn

read -rp "请输入: " ans
来源：http://df.521024.cn

[R78] 交互式菜单
来源：http://mx.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qi.yuexingan06.cn

[R79] 解析命令行选项
来源：http://fj.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://it.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://zx.9csxet.cn

time ./run.sh
来源：http://ed.huanxung.cn

================================================================================
来源：http://yb.szxytkj.cn

S. C / C++ 专题
来源：http://td.szxytkj.cn

================================================================================
来源：http://jj.shtwfgs.cn

[S01] C：Hello World
来源：http://ar.yuntaijiaju.cn

#include <stdio.h>
来源：http://ij.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gx.newstarts.cn

[S02] C：变量与格式化输出
来源：http://qm.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://hq.nszjky.cn

[S03] C：读入整数
来源：http://wq.hahajie.cn

int x; scanf("%d", &x);
来源：http://zv.gzmigu.cn

[S04] C：字符串复制
来源：http://sn.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zd.haigaiapp.cn

[S05] C：字符串长度
来源：http://na.nszjky.cn

strlen(s)
来源：http://ft.hahajie.cn

[S06] C：字符串比较
来源：http://gc.szxytkj.cn

strcmp(a, b) == 0
来源：http://nv.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://jp.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ot.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://sz.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sn.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://lk.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jb.shxzskj.cn

[S10] C：指针与解引用
来源：http://qo.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://jy.shxzskj.cn

[S11] C：逐行读文件
来源：http://tv.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://jg.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://io.gzmigu.cn

fclose(f);
来源：http://pc.shxzskj.cn

[S12] C：写文件
来源：http://um.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xo.shtwfgs.cn

[S13] C：宏定义
来源：http://ah.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qb.yuexingan06.cn

[S14] C：枚举
来源：http://bi.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://nq.9csxet.cn

[S15] C：类型转换
来源：http://gp.nszjky.cn

(double) a / b
来源：http://ny.szxytkj.cn

[S16] C：位操作置位
来源：http://ev.huanxung.cn

x |= (1 << 3);
来源：http://iu.hahajie.cn

[S17] C：安全拼接字符串
来源：http://bi.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nt.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://bm.huanxung.cn

int main(int argc, char **argv)
来源：http://ik.muxihuayi.cn

[S19] C：快速排序
来源：http://kw.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uf.huixiangedu.cn

[S20] C：二分查找
来源：http://bh.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mz.hnjuh.cn

[S21] C：字符类别判断
来源：http://wv.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ow.hnjuh.cn

[S22] C：字符串转数字
来源：http://dp.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lb.muxihuayi.cn

[S23] C：随机数
来源：http://ta.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tz.yuexingan06.cn

[S24] C：获取本地时间
来源：http://gq.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://id.hahajie.cn

[S25] C：内存拷贝
来源：http://dw.muxihuayi.cn

memcpy(dst, src, n);
来源：http://bz.szxytkj.cn

[S26] C：内存清零
来源：http://hz.colortex.cn

memset(a, 0, sizeof a);
来源：http://rd.hnjuh.cn

[S27] C：定义常量
来源：http://rb.nszjky.cn

const double PI = 3.14159;
来源：http://xq.hnjuh.cn

[S28] C：静态变量
来源：http://uy.panjiajie.cn

static int counter = 0;
来源：http://ep.panjiajie.cn

[S29] C：变参函数
来源：http://dx.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jf.nicolike.cn

[S30] C：头文件保护
来源：http://dm.gzmigu.cn

#ifndef X_H
来源：http://tg.huanxung.cn

#define X_H
来源：http://nz.shxzskj.cn

#endif
来源：http://jm.asd995.cn

[S31] C++：Hello World
来源：http://oi.huixinmuqiang.cn

#include <iostream>
来源：http://os.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://ru.huixinmuqiang.cn

[S32] C++：字符串
来源：http://wk.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://hd.nszjky.cn

[S33] C++：vector 增删
来源：http://qb.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yc.9csxet.cn

[S34] C++：遍历 vector
来源：http://ex.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://kw.szxytkj.cn

[S35] C++：map
来源：http://pr.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sm.hahajie.cn

[S36] C++：unordered_map
来源：http://jd.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ca.asd995.cn

[S37] C++：set
来源：http://rx.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gv.panjiajie.cn

[S38] C++：排序
来源：http://wi.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://qr.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://sm.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://km.lnxyls.cn

[S40] C++：查找元素
来源：http://fx.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yu.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://xh.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jo.huanxung.cn

[S42] C++：继承与虚函数
来源：http://zi.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://sk.521024.cn

[S43] C++：智能指针
来源：http://bd.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://po.shtwfgs.cn

[S44] C++：引用传参
来源：http://pb.nszjky.cn

void inc(int &x) { ++x; }
来源：http://tx.wgjwhj.cn

[S45] C++：lambda
来源：http://li.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wu.bjjhwx.cn

[S46] C++：函数模板
来源：http://sy.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zy.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://or.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yf.hnjuh.cn

[S48] C++：逐行读文件
来源：http://tj.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://um.asd995.cn

while (std::getline(in, line)) { }
来源：http://uv.bookmarksfly.cn

[S49] C++：写文件
来源：http://xb.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://el.wgjwhj.cn

[S50] C++：格式化数字
来源：http://cr.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ht.asd995.cn

[S51] C++：显式类型转换
来源：http://qj.521024.cn

static_cast<double>(a) / b
来源：http://hn.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://fr.9csxet.cn

int size() const noexcept { return n_; }
来源：http://mm.lnxyls.cn

[S53] C++：移动语义
来源：http://yu.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://cm.bookmarksfly.cn

[S54] C++：异常处理
来源：http://bl.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://em.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://pi.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vi.szsharing.cn

[S56] C++：optional
来源：http://ih.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lc.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://rc.szsharing.cn

constexpr int N = 10;
来源：http://vo.shxzukj.cn

[S58] C++：命名空间
来源：http://nj.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://wr.muxihuayi.cn

[S59] C++：静态断言
来源：http://zo.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gq.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://pt.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ub.newstarts.cn

================================================================================
来源：http://is.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gz.yuntaijiaju.cn

================================================================================
来源：http://xa.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://bw.nszjky.cn

println("Hello")
来源：http://xl.szxytkj.cn

[T02] Kotlin：变量
来源：http://ab.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mw.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://ux.jianghongdianzi.cn

"值: $b"
来源：http://nz.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://iq.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://zw.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://nh.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hn.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://xq.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ub.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://us.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xg.newstarts.cn

[T08] Kotlin：数据类
来源：http://kd.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://ci.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://gq.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://db.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://sw.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iv.9csxet.cn

[T11] Kotlin：协程
来源：http://jj.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://af.colortex.cn

[T12] Kotlin：解构声明
来源：http://ye.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://ls.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://ne.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://vd.huanxung.cn

[T14] Kotlin：循环
来源：http://uv.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://ry.nszjky.cn

[T15] Kotlin：接口
来源：http://kx.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://ys.colortex.cn

[T16] Swift：Hello World
来源：http://qc.colortex.cn

print("Hello")
来源：http://xd.9csxet.cn

[T17] Swift：变量与常量
来源：http://ul.huanxung.cn

var a = 1;  let b = 2
来源：http://kf.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://km.wgjwhj.cn

"值: \(b)"
来源：http://hb.huanxung.cn

[T19] Swift：可选绑定
来源：http://ui.szsharing.cn

if let n = opt { print(n) }
来源：http://cv.asd995.cn

[T20] Swift：数组操作
来源：http://ur.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zn.nicolike.cn

[T21] Swift：遍历
来源：http://ch.szxytkj.cn

for x in a { print(x) }
来源：http://xf.huixiangedu.cn

[T22] Swift：字典
来源：http://sq.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hv.newstarts.cn

[T23] Swift：函数
来源：http://ch.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xy.gzmigu.cn

[T24] Swift：闭包
来源：http://ag.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ul.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://ni.nicolike.cn

struct P { var x: Int }
来源：http://ua.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://tb.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://sn.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://or.asd995.cn

do { try f() } catch { print(error) }
来源：http://tk.gzmigu.cn

[T28] Swift：枚举
来源：http://bi.jctech888.com.cn

enum Color { case red, green }
来源：http://kv.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://lt.nicolike.cn

guard let x = opt else { return }
来源：http://fo.yuntaijiaju.cn

[T30] Swift：协议
来源：http://hj.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://pw.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://xl.panjiajie.cn

print("Hello")
来源：http://hc.chemitech.net.cn

[T32] Lua：局部变量
来源：http://mg.shtwfgs.cn

local a = 1
来源：http://uo.shxzskj.cn

[T33] Lua：表（数组）
来源：http://we.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zr.nicolike.cn

[T34] Lua：遍历表
来源：http://et.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xk.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://ix.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://dk.nicolike.cn

[T36] Lua：函数
来源：http://id.colortex.cn

function add(a, b) return a + b end
来源：http://ly.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://nu.szsharing.cn

"a" .. "b"
来源：http://ba.gzmigu.cn

[T38] Lua：条件
来源：http://vd.huanxung.cn

if x > 0 then print("正") end
来源：http://ze.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://yt.nicolike.cn

string.find(s, "%d+")
来源：http://gx.wgjwhj.cn

[T40] Lua：元表
来源：http://ax.colortex.cn

setmetatable({}, { __index = base })
来源：http://ga.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://lo.9csxet.cn

print "Hello\n";
来源：http://zw.huixiangedu.cn

[T42] Perl：变量类型
来源：http://az.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tv.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://gl.muxihuayi.cn

"值: $a"
来源：http://xt.jctech888.com.cn

[T44] Perl：条件
来源：http://ra.asd995.cn

if ($a > 0) { print "正"; }
来源：http://ux.szsharing.cn

[T45] Perl：数组遍历
来源：http://ie.asd995.cn

for my $x (@arr) { print $x; }
来源：http://yh.huanxung.cn

[T46] Perl：哈希操作
来源：http://su.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ja.shxzskj.cn

[T47] Perl：正则捕获
来源：http://kv.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cf.nszjky.cn

[T48] Perl：正则替换
来源：http://ng.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://md.9csxet.cn

[T49] Perl：函数
来源：http://mk.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xq.521024.cn

[T50] Perl：逐行读文件
来源：http://di.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aj.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://ta.huanxung.cn

[T51] Scala：Hello World
来源：http://jv.521024.cn

println("Hello")
来源：http://du.jctech888.com.cn

[T52] Scala：变量
来源：http://wd.colortex.cn

val a = 1;  var b = 2
来源：http://zv.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://sf.colortex.cn

s"值: $b"
来源：http://wn.9csxet.cn

[T54] Scala：集合映射
来源：http://kg.9csxet.cn


<!-- 参考信息 -->