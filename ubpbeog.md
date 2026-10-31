代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rl.gzmigu.cn

[R50] awk 求和
来源：http://cr.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ro.colortex.cn

[R51] 排序去重取前几
来源：http://vk.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ht.521024.cn

[R52] 统计行数
来源：http://xs.jianghongdianzi.cn

wc -l a.txt
来源：http://ms.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://ja.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nn.bjjhwx.cn

[R54] 比较两个文件
来源：http://xb.lnxyls.cn

diff a.txt b.txt
来源：http://qd.szxytkj.cn

[R55] 压缩与解压
来源：http://to.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yh.bjjhwx.cn

[R56] 远程拷贝
来源：http://bh.yuntaijiaju.cn

scp file user@host:/path/
来源：http://wn.hahajie.cn

[R57] 远程执行命令
来源：http://xr.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://va.huanxung.cn

[R58] 下载文件
来源：http://me.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ps.shxzukj.cn

[R59] 发 POST JSON
来源：http://kn.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zr.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://np.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rg.asd995.cn

[R61] 磁盘占用
来源：http://vz.wgjwhj.cn

df -h;  du -sh *
来源：http://dt.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://cc.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://pl.jianghongdianzi.cn

[R63] 内存与进程
来源：http://it.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://yf.szsharing.cn

[R64] 结束进程
来源：http://qi.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://rf.jctech888.com.cn

[R65] 查看端口占用
来源：http://ny.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vw.chemitech.net.cn

[R66] 定时任务
来源：http://cq.huixiangedu.cn

crontab -e;  crontab -l
来源：http://hl.9csxet.cn

[R67] 生成随机十六进制串
来源：http://br.newstarts.cn

openssl rand -hex 16
来源：http://ur.huanxung.cn

[R68] 计算文件校验值
来源：http://qh.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zf.yuexingan06.cn

[R69] 生成随机密码
来源：http://gk.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://kj.wgjwhj.cn

[R70] 时间戳与互转
来源：http://ak.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://my.bjjhwx.cn

[R71] 日期格式化
来源：http://fm.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ac.gzmigu.cn

[R72] 等待端口就绪
来源：http://ia.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sc.bjjhwx.cn

[R73] 分割大日志
来源：http://yz.9csxet.cn

split -l 1000 big.log part_
来源：http://ht.gzmigu.cn

[R74] 批量重命名
来源：http://aj.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://as.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ps.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://nl.colortex.cn

[R76] 使用临时文件
来源：http://jl.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bo.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ue.asd995.cn

read -rp "请输入: " ans
来源：http://dp.chemitech.net.cn

[R78] 交互式菜单
来源：http://ey.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zt.huanxung.cn

[R79] 解析命令行选项
来源：http://sl.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jd.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://yt.newstarts.cn

time ./run.sh
来源：http://cz.chemitech.net.cn

================================================================================
来源：http://tw.521024.cn

S. C / C++ 专题
来源：http://xr.newstarts.cn

================================================================================
来源：http://an.9csxet.cn

[S01] C：Hello World
来源：http://he.szxytkj.cn

#include <stdio.h>
来源：http://zo.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jp.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://lx.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://ey.szxytkj.cn

[S03] C：读入整数
来源：http://vk.szxytkj.cn

int x; scanf("%d", &x);
来源：http://cu.jctech888.com.cn

[S04] C：字符串复制
来源：http://dm.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ft.lnxyls.cn

[S05] C：字符串长度
来源：http://bb.colortex.cn

strlen(s)
来源：http://gp.szxytkj.cn

[S06] C：字符串比较
来源：http://pc.chemitech.net.cn

strcmp(a, b) == 0
来源：http://qh.shxzskj.cn

[S07] C：数组遍历求和
来源：http://zg.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mk.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://jb.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ra.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://wp.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ys.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://tx.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://ij.nszjky.cn

[S11] C：逐行读文件
来源：http://va.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://mg.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zg.gzmigu.cn

fclose(f);
来源：http://kz.bjjhwx.cn

[S12] C：写文件
来源：http://wl.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bv.szsharing.cn

[S13] C：宏定义
来源：http://xy.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rx.huanxung.cn

[S14] C：枚举
来源：http://hl.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ck.huixinmuqiang.cn

[S15] C：类型转换
来源：http://vc.asd995.cn

(double) a / b
来源：http://dx.hahajie.cn

[S16] C：位操作置位
来源：http://yk.hnjuh.cn

x |= (1 << 3);
来源：http://qd.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://rh.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zx.yuexingan06.cn

[S18] C：命令行参数
来源：http://jp.szxytkj.cn

int main(int argc, char **argv)
来源：http://xe.jctech888.com.cn

[S19] C：快速排序
来源：http://sf.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vz.muxihuayi.cn

[S20] C：二分查找
来源：http://ky.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pv.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://yr.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aa.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://yi.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bv.chemitech.net.cn

[S23] C：随机数
来源：http://gz.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rn.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://eo.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zu.gzmigu.cn

[S25] C：内存拷贝
来源：http://up.panjiajie.cn

memcpy(dst, src, n);
来源：http://ob.panjiajie.cn

[S26] C：内存清零
来源：http://hy.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://ua.huixinmuqiang.cn

[S27] C：定义常量
来源：http://jw.nicolike.cn

const double PI = 3.14159;
来源：http://vp.nszjky.cn

[S28] C：静态变量
来源：http://yr.asd995.cn

static int counter = 0;
来源：http://wa.newstarts.cn

[S29] C：变参函数
来源：http://nc.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zs.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://fl.jctech888.com.cn

#ifndef X_H
来源：http://bk.yuexingan06.cn

#define X_H
来源：http://wh.shtwfgs.cn

#endif
来源：http://if.haigaiapp.cn

[S31] C++：Hello World
来源：http://vu.521024.cn

#include <iostream>
来源：http://lu.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://al.shxzukj.cn

[S32] C++：字符串
来源：http://ff.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://df.newstarts.cn

[S33] C++：vector 增删
来源：http://wx.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wm.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://px.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://qc.lnxyls.cn

[S35] C++：map
来源：http://xr.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hf.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://eb.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tq.panjiajie.cn

[S37] C++：set
来源：http://ka.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ly.chemitech.net.cn

[S38] C++：排序
来源：http://qp.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://mn.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://qx.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zh.521024.cn

[S40] C++：查找元素
来源：http://ae.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gs.szsharing.cn

[S41] C++：类与构造函数
来源：http://ay.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gr.521024.cn

[S42] C++：继承与虚函数
来源：http://ms.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://lz.shxzskj.cn

[S43] C++：智能指针
来源：http://rv.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://rq.jctech888.com.cn

[S44] C++：引用传参
来源：http://pp.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://df.shxzskj.cn

[S45] C++：lambda
来源：http://uj.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ff.jctech888.com.cn

[S46] C++：函数模板
来源：http://qi.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hl.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://zw.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://re.asd995.cn

[S48] C++：逐行读文件
来源：http://mw.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://or.asd995.cn

while (std::getline(in, line)) { }
来源：http://ed.shxzskj.cn

[S49] C++：写文件
来源：http://et.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yh.nicolike.cn

[S50] C++：格式化数字
来源：http://km.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zu.9csxet.cn

[S51] C++：显式类型转换
来源：http://lx.szsharing.cn

static_cast<double>(a) / b
来源：http://lt.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://me.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://uw.huanxung.cn

[S53] C++：移动语义
来源：http://lm.muxihuayi.cn

std::vector<int> w = std::move(v);
来源：http://cv.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://qh.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yj.szxytkj.cn

[S55] C++：结构化绑定
来源：http://ia.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ff.bjjhwx.cn

[S56] C++：optional
来源：http://qv.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yq.jctech888.com.cn

[S57] C++：编译期常量
来源：http://yw.lnxyls.cn

constexpr int N = 10;
来源：http://nj.shxzskj.cn

[S58] C++：命名空间
来源：http://bq.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://sr.chemitech.net.cn

[S59] C++：静态断言
来源：http://fx.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eo.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://fo.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kn.jctech888.com.cn

================================================================================
来源：http://nl.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wt.shtwfgs.cn

================================================================================
来源：http://yq.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://rl.asd995.cn

println("Hello")
来源：http://wf.wgjwhj.cn

[T02] Kotlin：变量
来源：http://ru.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rb.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://vn.bookmarksfly.cn

"值: $b"
来源：http://he.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://hv.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ij.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://is.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://td.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://iu.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://th.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ou.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wj.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://dc.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://jb.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://ku.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://jh.nszjky.cn

[T10] Kotlin：默认参数
来源：http://zc.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ks.huanxung.cn

[T11] Kotlin：协程
来源：http://xf.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nq.asd995.cn

[T12] Kotlin：解构声明
来源：http://bl.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://ig.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://fu.9csxet.cn

val m = mapOf("a" to 1)
来源：http://mo.asd995.cn

[T14] Kotlin：循环
来源：http://yj.9csxet.cn

for (i in 1..10) println(i)
来源：http://go.muxihuayi.cn

[T15] Kotlin：接口
来源：http://ah.9csxet.cn

interface Shape { fun area(): Double }
来源：http://fs.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://hc.asd995.cn

print("Hello")
来源：http://vs.szsharing.cn

[T17] Swift：变量与常量
来源：http://cf.szsharing.cn

var a = 1;  let b = 2
来源：http://gk.521024.cn

[T18] Swift：字符串插值
来源：http://cg.shxzskj.cn

"值: \(b)"
来源：http://yz.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://ds.chemitech.net.cn

if let n = opt { print(n) }
来源：http://na.haigaiapp.cn

[T20] Swift：数组操作
来源：http://dz.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://os.gzmigu.cn

[T21] Swift：遍历
来源：http://wg.hnjuh.cn

for x in a { print(x) }
来源：http://ep.shtwfgs.cn

[T22] Swift：字典
来源：http://on.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fx.nszjky.cn

[T23] Swift：函数
来源：http://ix.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xo.newstarts.cn

[T24] Swift：闭包
来源：http://ny.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://va.szsharing.cn

[T25] Swift：结构体
来源：http://oj.nszjky.cn

struct P { var x: Int }
来源：http://cj.szsharing.cn

[T26] Swift：类与重写
来源：http://bw.newstarts.cn

class A: Base { override func f() {} }
来源：http://rp.9csxet.cn

[T27] Swift：错误处理
来源：http://mg.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://ce.panjiajie.cn

[T28] Swift：枚举
来源：http://pq.chemitech.net.cn

enum Color { case red, green }
来源：http://ji.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://jo.lnxyls.cn

guard let x = opt else { return }
来源：http://uf.huanxung.cn

[T30] Swift：协议
来源：http://rr.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://pl.newstarts.cn

[T31] Lua：Hello World
来源：http://dk.asd995.cn

print("Hello")
来源：http://bt.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://ii.nicolike.cn

local a = 1
来源：http://pz.9csxet.cn

[T33] Lua：表（数组）
来源：http://vo.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://az.lnxyls.cn

[T34] Lua：遍历表
来源：http://gd.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cl.shxzukj.cn

[T35] Lua：字典表
来源：http://zl.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://gs.colortex.cn

[T36] Lua：函数
来源：http://mi.szxytkj.cn

function add(a, b) return a + b end
来源：http://qb.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://bz.jctech888.com.cn

"a" .. "b"
来源：http://fi.521024.cn

[T38] Lua：条件
来源：http://yw.yuexingan06.cn

if x > 0 then print("正") end
来源：http://id.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://ct.bjjhwx.cn

string.find(s, "%d+")
来源：http://tu.bjjhwx.cn

[T40] Lua：元表
来源：http://zk.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ke.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://gx.huanxung.cn

print "Hello\n";
来源：http://fa.yuexingan06.cn

[T42] Perl：变量类型
来源：http://pf.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nb.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://xx.asd995.cn

"值: $a"
来源：http://qs.newstarts.cn

[T44] Perl：条件
来源：http://nm.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://sz.asd995.cn

[T45] Perl：数组遍历
来源：http://qa.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://cu.hnjuh.cn

[T46] Perl：哈希操作
来源：http://fo.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yh.panjiajie.cn

[T47] Perl：正则捕获
来源：http://wm.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://di.huanxung.cn

[T48] Perl：正则替换
来源：http://ne.szsharing.cn

$s =~ s/old/new/g;
来源：http://qs.yuntaijiaju.cn

[T49] Perl：函数
来源：http://di.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ad.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://le.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gx.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://vf.szxytkj.cn

[T51] Scala：Hello World
来源：http://so.panjiajie.cn

println("Hello")
来源：http://ez.shtwfgs.cn

[T52] Scala：变量
来源：http://kj.asd995.cn


<!-- 参考信息 -->