代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://fl.yuexingan06.cn

[R52] 统计行数
来源：http://vm.521024.cn

wc -l a.txt
来源：http://fq.asd995.cn

[R53] 查看文件头与实时尾
来源：http://jx.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ga.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://qn.chemitech.net.cn

diff a.txt b.txt
来源：http://mq.wgjwhj.cn

[R55] 压缩与解压
来源：http://vw.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xa.nszjky.cn

[R56] 远程拷贝
来源：http://tq.lnxyls.cn

scp file user@host:/path/
来源：http://uo.gzmigu.cn

[R57] 远程执行命令
来源：http://re.huanxung.cn

ssh user@host 'uptime'
来源：http://pd.yuexingan06.cn

[R58] 下载文件
来源：http://kx.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xo.gzmigu.cn

[R59] 发 POST JSON
来源：http://bp.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rl.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://br.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mf.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://my.shxzskj.cn

df -h;  du -sh *
来源：http://ha.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://iw.asd995.cn

du -ah . | sort -rh | head -10
来源：http://gv.9csxet.cn

[R63] 内存与进程
来源：http://fb.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://xy.521024.cn

[R64] 结束进程
来源：http://ts.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://km.lnxyls.cn

[R65] 查看端口占用
来源：http://ic.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lm.yuntaijiaju.cn

[R66] 定时任务
来源：http://sn.newstarts.cn

crontab -e;  crontab -l
来源：http://jx.nszjky.cn

[R67] 生成随机十六进制串
来源：http://fv.huixinmuqiang.cn

openssl rand -hex 16
来源：http://nl.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://ri.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ed.muxihuayi.cn

[R69] 生成随机密码
来源：http://on.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://vv.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://xh.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://xn.szxytkj.cn

[R71] 日期格式化
来源：http://ei.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wx.bjjhwx.cn

[R72] 等待端口就绪
来源：http://sx.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dv.jianghongdianzi.cn

[R73] 分割大日志
来源：http://tb.9csxet.cn

split -l 1000 big.log part_
来源：http://vc.521024.cn

[R74] 批量重命名
来源：http://vu.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nj.hahajie.cn

[R75] 导出环境变量
来源：http://qu.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://sv.nicolike.cn

[R76] 使用临时文件
来源：http://cb.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ql.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://gv.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://ry.nicolike.cn

[R78] 交互式菜单
来源：http://nb.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bi.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ax.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fk.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://ev.wgjwhj.cn

time ./run.sh
来源：http://jo.jianghongdianzi.cn

================================================================================
来源：http://jw.gzmigu.cn

S. C / C++ 专题
来源：http://zx.panjiajie.cn

================================================================================
来源：http://qz.shtwfgs.cn

[S01] C：Hello World
来源：http://wq.9csxet.cn

#include <stdio.h>
来源：http://bw.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yh.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://wx.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://tk.shtwfgs.cn

[S03] C：读入整数
来源：http://aj.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://fc.shxzukj.cn

[S04] C：字符串复制
来源：http://ou.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xn.huixiangedu.cn

[S05] C：字符串长度
来源：http://dg.colortex.cn

strlen(s)
来源：http://qw.shxzukj.cn

[S06] C：字符串比较
来源：http://sh.muxihuayi.cn

strcmp(a, b) == 0
来源：http://mx.huanxung.cn

[S07] C：数组遍历求和
来源：http://dg.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hg.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://oa.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nl.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://py.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://km.hahajie.cn

[S10] C：指针与解引用
来源：http://fp.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://kx.newstarts.cn

[S11] C：逐行读文件
来源：http://lt.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://gq.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yt.muxihuayi.cn

fclose(f);
来源：http://me.bookmarksfly.cn

[S12] C：写文件
来源：http://ri.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nz.yuntaijiaju.cn

[S13] C：宏定义
来源：http://ot.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ss.shxzukj.cn

[S14] C：枚举
来源：http://eg.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://dt.colortex.cn

[S15] C：类型转换
来源：http://sc.hahajie.cn

(double) a / b
来源：http://kg.chemitech.net.cn

[S16] C：位操作置位
来源：http://ff.chemitech.net.cn

x |= (1 << 3);
来源：http://zj.huanxung.cn

[S17] C：安全拼接字符串
来源：http://kp.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bw.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://gc.nicolike.cn

int main(int argc, char **argv)
来源：http://vl.huanxung.cn

[S19] C：快速排序
来源：http://ys.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bf.muxihuayi.cn

[S20] C：二分查找
来源：http://te.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gw.huixiangedu.cn

[S21] C：字符类别判断
来源：http://kk.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nv.huixiangedu.cn

[S22] C：字符串转数字
来源：http://ou.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xm.szxytkj.cn

[S23] C：随机数
来源：http://lf.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yv.huanxung.cn

[S24] C：获取本地时间
来源：http://rd.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://os.shxzukj.cn

[S25] C：内存拷贝
来源：http://xs.nszjky.cn

memcpy(dst, src, n);
来源：http://pf.9csxet.cn

[S26] C：内存清零
来源：http://ky.hahajie.cn

memset(a, 0, sizeof a);
来源：http://zl.asd995.cn

[S27] C：定义常量
来源：http://lk.colortex.cn

const double PI = 3.14159;
来源：http://vv.huixinmuqiang.cn

[S28] C：静态变量
来源：http://hw.szxytkj.cn

static int counter = 0;
来源：http://hj.bjjhwx.cn

[S29] C：变参函数
来源：http://ci.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iv.shtwfgs.cn

[S30] C：头文件保护
来源：http://bg.newstarts.cn

#ifndef X_H
来源：http://gu.lnxyls.cn

#define X_H
来源：http://kd.bjjhwx.cn

#endif
来源：http://rr.hahajie.cn

[S31] C++：Hello World
来源：http://tf.panjiajie.cn

#include <iostream>
来源：http://fh.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://cn.jianghongdianzi.cn

[S32] C++：字符串
来源：http://yq.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://kc.shtwfgs.cn

[S33] C++：vector 增删
来源：http://wc.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xe.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://ww.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ss.asd995.cn

[S35] C++：map
来源：http://er.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xk.szsharing.cn

[S36] C++：unordered_map
来源：http://ic.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ec.szxytkj.cn

[S37] C++：set
来源：http://ha.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ar.shxzukj.cn

[S38] C++：排序
来源：http://eb.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://me.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://st.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jl.shtwfgs.cn

[S40] C++：查找元素
来源：http://wg.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dp.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://wx.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tm.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://nr.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://az.newstarts.cn

[S43] C++：智能指针
来源：http://gs.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://hy.newstarts.cn

[S44] C++：引用传参
来源：http://bw.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://nl.jianghongdianzi.cn

[S45] C++：lambda
来源：http://us.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tx.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://vi.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xz.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://jt.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hi.panjiajie.cn

[S48] C++：逐行读文件
来源：http://de.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://te.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://kz.nszjky.cn

[S49] C++：写文件
来源：http://gd.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yq.asd995.cn

[S50] C++：格式化数字
来源：http://ih.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sh.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://cc.lnxyls.cn

static_cast<double>(a) / b
来源：http://rf.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://fo.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://yq.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://bo.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://af.bjjhwx.cn

[S54] C++：异常处理
来源：http://zb.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://od.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://pk.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sb.yuntaijiaju.cn

[S56] C++：optional
来源：http://rw.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rm.muxihuayi.cn

[S57] C++：编译期常量
来源：http://qn.newstarts.cn

constexpr int N = 10;
来源：http://yn.shxzukj.cn

[S58] C++：命名空间
来源：http://no.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://rh.521024.cn

[S59] C++：静态断言
来源：http://di.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yg.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://ng.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://va.lnxyls.cn

================================================================================
来源：http://qb.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bz.bookmarksfly.cn

================================================================================
来源：http://ka.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://se.gzmigu.cn

println("Hello")
来源：http://qi.lnxyls.cn

[T02] Kotlin：变量
来源：http://vn.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dl.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://hz.gzmigu.cn

"值: $b"
来源：http://gx.521024.cn

[T04] Kotlin：空安全
来源：http://ik.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://br.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://ht.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gi.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://eh.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bo.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://bt.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xq.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://bb.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://pz.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://hg.colortex.cn

fun String.exclaim() = this + "!"
来源：http://da.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://bs.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ex.9csxet.cn

[T11] Kotlin：协程
来源：http://dr.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fy.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://yj.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://nq.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://ve.asd995.cn

val m = mapOf("a" to 1)
来源：http://pt.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://yj.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://eo.asd995.cn

[T15] Kotlin：接口
来源：http://zi.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://uf.newstarts.cn

[T16] Swift：Hello World
来源：http://pj.bjjhwx.cn

print("Hello")
来源：http://nm.nszjky.cn

[T17] Swift：变量与常量
来源：http://ny.nicolike.cn

var a = 1;  let b = 2
来源：http://lo.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://ji.colortex.cn

"值: \(b)"
来源：http://xe.nszjky.cn

[T19] Swift：可选绑定
来源：http://yh.gzmigu.cn

if let n = opt { print(n) }
来源：http://np.yuexingan06.cn

[T20] Swift：数组操作
来源：http://ai.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uz.colortex.cn

[T21] Swift：遍历
来源：http://jt.huixiangedu.cn

for x in a { print(x) }
来源：http://ja.shtwfgs.cn

[T22] Swift：字典
来源：http://lk.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hw.hahajie.cn

[T23] Swift：函数
来源：http://ac.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://re.bookmarksfly.cn

[T24] Swift：闭包
来源：http://ta.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fr.hnjuh.cn

[T25] Swift：结构体
来源：http://re.nicolike.cn

struct P { var x: Int }
来源：http://ta.szxytkj.cn

[T26] Swift：类与重写
来源：http://qj.asd995.cn

class A: Base { override func f() {} }
来源：http://ta.muxihuayi.cn

[T27] Swift：错误处理
来源：http://jc.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://xk.shtwfgs.cn

[T28] Swift：枚举
来源：http://uo.muxihuayi.cn

enum Color { case red, green }
来源：http://en.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://gz.asd995.cn

guard let x = opt else { return }
来源：http://nl.gzmigu.cn

[T30] Swift：协议
来源：http://yg.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://gz.9csxet.cn

[T31] Lua：Hello World
来源：http://jw.chemitech.net.cn

print("Hello")
来源：http://xx.szsharing.cn

[T32] Lua：局部变量
来源：http://kh.gzmigu.cn

local a = 1
来源：http://nz.9csxet.cn

[T33] Lua：表（数组）
来源：http://fo.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sv.9csxet.cn

[T34] Lua：遍历表
来源：http://fr.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mz.nszjky.cn

[T35] Lua：字典表
来源：http://vb.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://an.bjjhwx.cn

[T36] Lua：函数
来源：http://or.asd995.cn

function add(a, b) return a + b end
来源：http://mr.colortex.cn

[T37] Lua：字符串拼接
来源：http://gq.jianghongdianzi.cn

"a" .. "b"
来源：http://nw.521024.cn

[T38] Lua：条件
来源：http://et.hnjuh.cn

if x > 0 then print("正") end
来源：http://lz.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://xb.shtwfgs.cn

string.find(s, "%d+")
来源：http://mf.lnxyls.cn

[T40] Lua：元表
来源：http://gk.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://gr.panjiajie.cn

[T41] Perl：Hello World
来源：http://mu.muxihuayi.cn

print "Hello\n";
来源：http://jd.colortex.cn

[T42] Perl：变量类型
来源：http://bd.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kj.shxzskj.cn

[T43] Perl：字符串插值
来源：http://ae.bjjhwx.cn

"值: $a"
来源：http://rf.nszjky.cn

[T44] Perl：条件
来源：http://jb.asd995.cn

if ($a > 0) { print "正"; }
来源：http://uy.szsharing.cn

[T45] Perl：数组遍历
来源：http://io.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://qb.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://ud.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bt.szsharing.cn

[T47] Perl：正则捕获
来源：http://kq.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ya.haigaiapp.cn

[T48] Perl：正则替换
来源：http://wr.asd995.cn

$s =~ s/old/new/g;
来源：http://vg.haigaiapp.cn

[T49] Perl：函数
来源：http://xm.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ub.nszjky.cn

[T50] Perl：逐行读文件
来源：http://xy.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ga.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://wh.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://sk.panjiajie.cn

println("Hello")
来源：http://hu.bookmarksfly.cn

[T52] Scala：变量
来源：http://ys.colortex.cn

val a = 1;  var b = 2
来源：http://rg.huanxung.cn

[T53] Scala：字符串插值
来源：http://vy.huixinmuqiang.cn

s"值: $b"
来源：http://mi.shtwfgs.cn

[T54] Scala：集合映射
来源：http://jh.yuexingan06.cn


<!-- 参考信息 -->