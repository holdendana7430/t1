代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iz.shtwfgs.cn

[R54] 比较两个文件
来源：http://lj.jctech888.com.cn

diff a.txt b.txt
来源：http://gv.colortex.cn

[R55] 压缩与解压
来源：http://wy.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uo.asd995.cn

[R56] 远程拷贝
来源：http://fq.jianghongdianzi.cn

scp file user@host:/path/
来源：http://lt.chemitech.net.cn

[R57] 远程执行命令
来源：http://dg.muxihuayi.cn

ssh user@host 'uptime'
来源：http://qb.szsharing.cn

[R58] 下载文件
来源：http://qd.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oz.muxihuayi.cn

[R59] 发 POST JSON
来源：http://sc.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cf.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://iu.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zq.chemitech.net.cn

[R61] 磁盘占用
来源：http://xe.szxytkj.cn

df -h;  du -sh *
来源：http://px.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://lg.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://jt.haigaiapp.cn

[R63] 内存与进程
来源：http://nd.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://hy.521024.cn

[R64] 结束进程
来源：http://qu.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://fa.muxihuayi.cn

[R65] 查看端口占用
来源：http://st.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ua.lnxyls.cn

[R66] 定时任务
来源：http://yu.szxytkj.cn

crontab -e;  crontab -l
来源：http://ba.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://dj.nicolike.cn

openssl rand -hex 16
来源：http://gy.wgjwhj.cn

[R68] 计算文件校验值
来源：http://ia.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lw.haigaiapp.cn

[R69] 生成随机密码
来源：http://za.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://zg.521024.cn

[R70] 时间戳与互转
来源：http://bz.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://rd.nszjky.cn

[R71] 日期格式化
来源：http://ea.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oh.huanxung.cn

[R72] 等待端口就绪
来源：http://vf.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ys.colortex.cn

[R73] 分割大日志
来源：http://rn.9csxet.cn

split -l 1000 big.log part_
来源：http://ae.panjiajie.cn

[R74] 批量重命名
来源：http://qu.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qp.colortex.cn

[R75] 导出环境变量
来源：http://wh.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://fx.shxzskj.cn

[R76] 使用临时文件
来源：http://cu.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://py.shxzskj.cn

[R77] 读取用户输入
来源：http://yc.wgjwhj.cn

read -rp "请输入: " ans
来源：http://xp.yuexingan06.cn

[R78] 交互式菜单
来源：http://mf.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kj.szxytkj.cn

[R79] 解析命令行选项
来源：http://kn.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zh.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://vm.asd995.cn

time ./run.sh
来源：http://ms.jianghongdianzi.cn

================================================================================
来源：http://cf.bjjhwx.cn

S. C / C++ 专题
来源：http://ok.gzmigu.cn

================================================================================
来源：http://ve.nicolike.cn

[S01] C：Hello World
来源：http://ob.panjiajie.cn

#include <stdio.h>
来源：http://po.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jf.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://gj.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://nb.muxihuayi.cn

[S03] C：读入整数
来源：http://ez.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://qv.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://mz.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ei.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://hv.muxihuayi.cn

strlen(s)
来源：http://mq.haigaiapp.cn

[S06] C：字符串比较
来源：http://ls.yuexingan06.cn

strcmp(a, b) == 0
来源：http://kd.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://pd.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gq.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://bh.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ro.colortex.cn

[S09] C：结构体定义与初始化
来源：http://vd.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ax.gzmigu.cn

[S10] C：指针与解引用
来源：http://ub.nicolike.cn

int *p = &a;  *p = 5;
来源：http://to.huixiangedu.cn

[S11] C：逐行读文件
来源：http://mq.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://ax.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jy.shxzukj.cn

fclose(f);
来源：http://ux.yuntaijiaju.cn

[S12] C：写文件
来源：http://du.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tj.nicolike.cn

[S13] C：宏定义
来源：http://uf.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zw.nicolike.cn

[S14] C：枚举
来源：http://sb.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://zi.chemitech.net.cn

[S15] C：类型转换
来源：http://tq.colortex.cn

(double) a / b
来源：http://as.haigaiapp.cn

[S16] C：位操作置位
来源：http://ub.shxzukj.cn

x |= (1 << 3);
来源：http://ln.9csxet.cn

[S17] C：安全拼接字符串
来源：http://hi.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jp.colortex.cn

[S18] C：命令行参数
来源：http://gj.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://ag.szxytkj.cn

[S19] C：快速排序
来源：http://qk.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ir.shxzskj.cn

[S20] C：二分查找
来源：http://eg.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zx.shtwfgs.cn

[S21] C：字符类别判断
来源：http://no.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://os.shxzukj.cn

[S22] C：字符串转数字
来源：http://ct.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sc.asd995.cn

[S23] C：随机数
来源：http://hf.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rp.huanxung.cn

[S24] C：获取本地时间
来源：http://ju.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://li.wgjwhj.cn

[S25] C：内存拷贝
来源：http://oh.haigaiapp.cn

memcpy(dst, src, n);
来源：http://xz.huixinmuqiang.cn

[S26] C：内存清零
来源：http://mn.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://id.chemitech.net.cn

[S27] C：定义常量
来源：http://yd.gzmigu.cn

const double PI = 3.14159;
来源：http://cl.asd995.cn

[S28] C：静态变量
来源：http://in.muxihuayi.cn

static int counter = 0;
来源：http://nv.shxzukj.cn

[S29] C：变参函数
来源：http://kx.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nm.muxihuayi.cn

[S30] C：头文件保护
来源：http://wg.colortex.cn

#ifndef X_H
来源：http://cb.szxytkj.cn

#define X_H
来源：http://ev.colortex.cn

#endif
来源：http://vw.lnxyls.cn

[S31] C++：Hello World
来源：http://yw.haigaiapp.cn

#include <iostream>
来源：http://se.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://dy.chemitech.net.cn

[S32] C++：字符串
来源：http://at.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://jm.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://qp.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rh.shxzskj.cn

[S34] C++：遍历 vector
来源：http://qg.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ys.9csxet.cn

[S35] C++：map
来源：http://rv.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fe.shxzskj.cn

[S36] C++：unordered_map
来源：http://xh.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://it.jianghongdianzi.cn

[S37] C++：set
来源：http://cf.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wm.asd995.cn

[S38] C++：排序
来源：http://mj.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://xj.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://me.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mo.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://wo.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ol.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://ii.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zy.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://fh.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://yl.asd995.cn

[S43] C++：智能指针
来源：http://pk.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://sb.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://nl.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://yu.yuexingan06.cn

[S45] C++：lambda
来源：http://xi.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hi.jctech888.com.cn

[S46] C++：函数模板
来源：http://hs.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vw.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://pt.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wa.nicolike.cn

[S48] C++：逐行读文件
来源：http://qc.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kc.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://bn.9csxet.cn

[S49] C++：写文件
来源：http://va.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iu.nicolike.cn

[S50] C++：格式化数字
来源：http://ub.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mj.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://ez.shxzskj.cn

static_cast<double>(a) / b
来源：http://xx.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://fu.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://oo.muxihuayi.cn

[S53] C++：移动语义
来源：http://ee.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://fs.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://pw.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nd.asd995.cn

[S55] C++：结构化绑定
来源：http://in.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pn.jctech888.com.cn

[S56] C++：optional
来源：http://uh.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ac.shtwfgs.cn

[S57] C++：编译期常量
来源：http://ir.colortex.cn

constexpr int N = 10;
来源：http://ay.colortex.cn

[S58] C++：命名空间
来源：http://rt.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://gt.shxzukj.cn

[S59] C++：静态断言
来源：http://jl.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nh.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://de.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bn.lnxyls.cn

================================================================================
来源：http://ti.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vo.nicolike.cn

================================================================================
来源：http://on.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://jt.newstarts.cn

println("Hello")
来源：http://oq.shxzukj.cn

[T02] Kotlin：变量
来源：http://ha.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mk.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://jt.shxzukj.cn

"值: $b"
来源：http://kk.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://xa.hnjuh.cn

val n: String? = null;  n?.length
来源：http://zh.521024.cn

[T05] Kotlin：when 表达式
来源：http://mu.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fn.colortex.cn

[T06] Kotlin：集合映射
来源：http://mx.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lv.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://bf.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pb.nicolike.cn

[T08] Kotlin：数据类
来源：http://rw.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://as.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://tg.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://kp.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://dv.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qf.shtwfgs.cn

[T11] Kotlin：协程
来源：http://fd.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://re.huanxung.cn

[T12] Kotlin：解构声明
来源：http://pf.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://kn.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://fb.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://vh.szsharing.cn

[T14] Kotlin：循环
来源：http://vj.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://dx.shxzukj.cn

[T15] Kotlin：接口
来源：http://ae.nszjky.cn

interface Shape { fun area(): Double }
来源：http://bl.hahajie.cn

[T16] Swift：Hello World
来源：http://nr.jctech888.com.cn

print("Hello")
来源：http://ba.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://ub.jctech888.com.cn

var a = 1;  let b = 2
来源：http://wf.newstarts.cn

[T18] Swift：字符串插值
来源：http://cw.9csxet.cn

"值: \(b)"
来源：http://uz.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://jh.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://wr.huixiangedu.cn

[T20] Swift：数组操作
来源：http://br.hahajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gk.shxzskj.cn

[T21] Swift：遍历
来源：http://ib.nicolike.cn

for x in a { print(x) }
来源：http://qo.szsharing.cn

[T22] Swift：字典
来源：http://an.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jy.haigaiapp.cn

[T23] Swift：函数
来源：http://xq.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ob.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://vp.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zc.szxytkj.cn

[T25] Swift：结构体
来源：http://uu.nicolike.cn

struct P { var x: Int }
来源：http://hh.haigaiapp.cn

[T26] Swift：类与重写
来源：http://qe.hahajie.cn

class A: Base { override func f() {} }
来源：http://yp.shxzukj.cn

[T27] Swift：错误处理
来源：http://vy.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://vt.gzmigu.cn

[T28] Swift：枚举
来源：http://aw.nicolike.cn

enum Color { case red, green }
来源：http://rp.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://xw.haigaiapp.cn

guard let x = opt else { return }
来源：http://hd.colortex.cn

[T30] Swift：协议
来源：http://wc.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://ih.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://jy.colortex.cn

print("Hello")
来源：http://fw.huanxung.cn

[T32] Lua：局部变量
来源：http://bo.hnjuh.cn

local a = 1
来源：http://je.9csxet.cn

[T33] Lua：表（数组）
来源：http://qu.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bp.hnjuh.cn

[T34] Lua：遍历表
来源：http://ld.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rc.lnxyls.cn

[T35] Lua：字典表
来源：http://rm.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://cd.shxzskj.cn

[T36] Lua：函数
来源：http://ql.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://zj.9csxet.cn

[T37] Lua：字符串拼接
来源：http://wo.huixiangedu.cn

"a" .. "b"
来源：http://zr.panjiajie.cn

[T38] Lua：条件
来源：http://pa.nszjky.cn

if x > 0 then print("正") end
来源：http://ub.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://iu.gzmigu.cn

string.find(s, "%d+")
来源：http://or.shxzukj.cn

[T40] Lua：元表
来源：http://cq.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://mg.jctech888.com.cn

[T41] Perl：Hello World
来源：http://cs.nszjky.cn

print "Hello\n";
来源：http://ua.shxzskj.cn

[T42] Perl：变量类型
来源：http://px.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rs.nszjky.cn

[T43] Perl：字符串插值
来源：http://gr.huanxung.cn

"值: $a"
来源：http://ja.huixiangedu.cn

[T44] Perl：条件
来源：http://lj.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://qo.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://qs.colortex.cn

for my $x (@arr) { print $x; }
来源：http://xh.szsharing.cn

[T46] Perl：哈希操作
来源：http://ks.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ru.nicolike.cn

[T47] Perl：正则捕获
来源：http://bf.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eh.wgjwhj.cn

[T48] Perl：正则替换
来源：http://dt.szsharing.cn

$s =~ s/old/new/g;
来源：http://ex.huanxung.cn

[T49] Perl：函数
来源：http://it.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qc.nicolike.cn

[T50] Perl：逐行读文件
来源：http://uu.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yl.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://li.shxzukj.cn

[T51] Scala：Hello World
来源：http://dr.haigaiapp.cn

println("Hello")
来源：http://kk.gzmigu.cn

[T52] Scala：变量
来源：http://my.gzmigu.cn

val a = 1;  var b = 2
来源：http://yl.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://cl.huixiangedu.cn

s"值: $b"
来源：http://vz.gzmigu.cn

[T54] Scala：集合映射
来源：http://qd.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://fd.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ul.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ej.szsharing.cn

[T56] Scala：样例类
来源：http://bq.9csxet.cn


<!-- 参考信息 -->