代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zf.shxzskj.cn

[R50] awk 求和
来源：http://ju.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://by.521024.cn

[R51] 排序去重取前几
来源：http://yb.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ad.yuntaijiaju.cn

[R52] 统计行数
来源：http://ke.muxihuayi.cn

wc -l a.txt
来源：http://dv.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://kd.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gc.nszjky.cn

[R54] 比较两个文件
来源：http://ez.asd995.cn

diff a.txt b.txt
来源：http://lo.bjjhwx.cn

[R55] 压缩与解压
来源：http://hu.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ry.lnxyls.cn

[R56] 远程拷贝
来源：http://fe.muxihuayi.cn

scp file user@host:/path/
来源：http://vi.asd995.cn

[R57] 远程执行命令
来源：http://bt.chemitech.net.cn

ssh user@host 'uptime'
来源：http://xg.shxzukj.cn

[R58] 下载文件
来源：http://do.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xf.shxzukj.cn

[R59] 发 POST JSON
来源：http://fs.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oe.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://jp.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://up.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://mq.nszjky.cn

df -h;  du -sh *
来源：http://jz.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://ot.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://hf.9csxet.cn

[R63] 内存与进程
来源：http://wa.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://uv.bjjhwx.cn

[R64] 结束进程
来源：http://bf.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://kg.chemitech.net.cn

[R65] 查看端口占用
来源：http://st.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rv.nszjky.cn

[R66] 定时任务
来源：http://fm.nszjky.cn

crontab -e;  crontab -l
来源：http://fx.9csxet.cn

[R67] 生成随机十六进制串
来源：http://vj.shxzukj.cn

openssl rand -hex 16
来源：http://pq.newstarts.cn

[R68] 计算文件校验值
来源：http://vx.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ay.nicolike.cn

[R69] 生成随机密码
来源：http://pp.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://mu.shxzskj.cn

[R70] 时间戳与互转
来源：http://cc.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://ts.shxzukj.cn

[R71] 日期格式化
来源：http://ox.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vi.gzmigu.cn

[R72] 等待端口就绪
来源：http://zv.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://da.chemitech.net.cn

[R73] 分割大日志
来源：http://fk.nicolike.cn

split -l 1000 big.log part_
来源：http://pc.huixiangedu.cn

[R74] 批量重命名
来源：http://ke.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://px.yuexingan06.cn

[R75] 导出环境变量
来源：http://sp.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://jk.chemitech.net.cn

[R76] 使用临时文件
来源：http://do.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ab.szsharing.cn

[R77] 读取用户输入
来源：http://be.shxzukj.cn

read -rp "请输入: " ans
来源：http://yu.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://sd.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mr.nicolike.cn

[R79] 解析命令行选项
来源：http://ca.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kk.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://mu.panjiajie.cn

time ./run.sh
来源：http://ms.chemitech.net.cn

================================================================================
来源：http://zs.colortex.cn

S. C / C++ 专题
来源：http://no.nicolike.cn

================================================================================
来源：http://ks.shxzukj.cn

[S01] C：Hello World
来源：http://rv.yuntaijiaju.cn

#include <stdio.h>
来源：http://aq.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ak.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://mo.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://to.newstarts.cn

[S03] C：读入整数
来源：http://il.shxzskj.cn

int x; scanf("%d", &x);
来源：http://sn.shxzukj.cn

[S04] C：字符串复制
来源：http://ok.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fh.shtwfgs.cn

[S05] C：字符串长度
来源：http://dy.jctech888.com.cn

strlen(s)
来源：http://bk.shtwfgs.cn

[S06] C：字符串比较
来源：http://sj.huanxung.cn

strcmp(a, b) == 0
来源：http://mh.9csxet.cn

[S07] C：数组遍历求和
来源：http://ru.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uz.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://yt.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dm.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://bt.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xt.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://kn.nszjky.cn

int *p = &a;  *p = 5;
来源：http://om.chemitech.net.cn

[S11] C：逐行读文件
来源：http://uv.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://ka.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zp.hahajie.cn

fclose(f);
来源：http://sx.521024.cn

[S12] C：写文件
来源：http://io.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uv.huixinmuqiang.cn

[S13] C：宏定义
来源：http://ty.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://js.shxzskj.cn

[S14] C：枚举
来源：http://yo.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://ry.bjjhwx.cn

[S15] C：类型转换
来源：http://lr.yuntaijiaju.cn

(double) a / b
来源：http://dg.jctech888.com.cn

[S16] C：位操作置位
来源：http://xl.jianghongdianzi.cn

x |= (1 << 3);
来源：http://rx.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://bm.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zi.hahajie.cn

[S18] C：命令行参数
来源：http://db.huanxung.cn

int main(int argc, char **argv)
来源：http://yq.jianghongdianzi.cn

[S19] C：快速排序
来源：http://rt.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fn.hnjuh.cn

[S20] C：二分查找
来源：http://xu.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yd.colortex.cn

[S21] C：字符类别判断
来源：http://wo.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://js.chemitech.net.cn

[S22] C：字符串转数字
来源：http://kn.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ml.shxzukj.cn

[S23] C：随机数
来源：http://jf.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zv.szsharing.cn

[S24] C：获取本地时间
来源：http://hx.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ad.wgjwhj.cn

[S25] C：内存拷贝
来源：http://mv.szxytkj.cn

memcpy(dst, src, n);
来源：http://ma.521024.cn

[S26] C：内存清零
来源：http://ak.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://qv.wgjwhj.cn

[S27] C：定义常量
来源：http://tf.huanxung.cn

const double PI = 3.14159;
来源：http://lf.yuntaijiaju.cn

[S28] C：静态变量
来源：http://zn.asd995.cn

static int counter = 0;
来源：http://wi.521024.cn

[S29] C：变参函数
来源：http://yp.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wn.hnjuh.cn

[S30] C：头文件保护
来源：http://tq.asd995.cn

#ifndef X_H
来源：http://rl.yuexingan06.cn

#define X_H
来源：http://lc.panjiajie.cn

#endif
来源：http://dd.shxzukj.cn

[S31] C++：Hello World
来源：http://am.shtwfgs.cn

#include <iostream>
来源：http://eh.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://ui.521024.cn

[S32] C++：字符串
来源：http://ju.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://ew.shxzukj.cn

[S33] C++：vector 增删
来源：http://oj.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://al.szsharing.cn

[S34] C++：遍历 vector
来源：http://pa.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://yi.huixinmuqiang.cn

[S35] C++：map
来源：http://vw.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dr.shxzukj.cn

[S36] C++：unordered_map
来源：http://ln.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ku.yuntaijiaju.cn

[S37] C++：set
来源：http://uu.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jv.huixinmuqiang.cn

[S38] C++：排序
来源：http://vh.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://fk.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://sf.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vl.jctech888.com.cn

[S40] C++：查找元素
来源：http://go.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://do.asd995.cn

[S41] C++：类与构造函数
来源：http://fz.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://by.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://co.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://qf.shxzskj.cn

[S43] C++：智能指针
来源：http://xv.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://jq.9csxet.cn

[S44] C++：引用传参
来源：http://bj.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://qx.lnxyls.cn

[S45] C++：lambda
来源：http://rr.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gi.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://pz.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tu.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://kd.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tr.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://cu.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fo.newstarts.cn

while (std::getline(in, line)) { }
来源：http://dy.jctech888.com.cn

[S49] C++：写文件
来源：http://sh.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xx.newstarts.cn

[S50] C++：格式化数字
来源：http://jx.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ul.asd995.cn

[S51] C++：显式类型转换
来源：http://ii.9csxet.cn

static_cast<double>(a) / b
来源：http://ey.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://wl.colortex.cn

int size() const noexcept { return n_; }
来源：http://he.szxytkj.cn

[S53] C++：移动语义
来源：http://jl.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://kw.nicolike.cn

[S54] C++：异常处理
来源：http://lh.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nh.nszjky.cn

[S55] C++：结构化绑定
来源：http://qb.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://if.asd995.cn

[S56] C++：optional
来源：http://mv.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qw.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://gi.muxihuayi.cn

constexpr int N = 10;
来源：http://yb.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ph.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://na.panjiajie.cn

[S59] C++：静态断言
来源：http://js.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://st.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://uj.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ai.wgjwhj.cn

================================================================================
来源：http://zi.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sf.szsharing.cn

================================================================================
来源：http://rp.9csxet.cn

[T01] Kotlin：Hello World
来源：http://eo.wgjwhj.cn

println("Hello")
来源：http://wc.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://tn.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qj.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://kv.hnjuh.cn

"值: $b"
来源：http://cw.9csxet.cn

[T04] Kotlin：空安全
来源：http://cg.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://ia.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://hm.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://db.newstarts.cn

[T06] Kotlin：集合映射
来源：http://uv.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ct.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://qm.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xr.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://rk.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://fh.521024.cn

[T09] Kotlin：扩展函数
来源：http://ip.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://px.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://lt.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pb.colortex.cn

[T11] Kotlin：协程
来源：http://kx.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jj.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://rg.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://xn.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://wp.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://zc.lnxyls.cn

[T14] Kotlin：循环
来源：http://jf.asd995.cn

for (i in 1..10) println(i)
来源：http://fr.nszjky.cn

[T15] Kotlin：接口
来源：http://ih.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://fm.newstarts.cn

[T16] Swift：Hello World
来源：http://qf.9csxet.cn

print("Hello")
来源：http://ii.shxzukj.cn

[T17] Swift：变量与常量
来源：http://gs.nszjky.cn

var a = 1;  let b = 2
来源：http://jo.hahajie.cn

[T18] Swift：字符串插值
来源：http://id.szxytkj.cn

"值: \(b)"
来源：http://xq.newstarts.cn

[T19] Swift：可选绑定
来源：http://eg.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://ed.szxytkj.cn

[T20] Swift：数组操作
来源：http://tg.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zv.colortex.cn

[T21] Swift：遍历
来源：http://pi.9csxet.cn

for x in a { print(x) }
来源：http://dg.jctech888.com.cn

[T22] Swift：字典
来源：http://pl.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://an.yuntaijiaju.cn

[T23] Swift：函数
来源：http://xg.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ug.yuexingan06.cn

[T24] Swift：闭包
来源：http://vn.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cb.szxytkj.cn

[T25] Swift：结构体
来源：http://fm.shxzukj.cn

struct P { var x: Int }
来源：http://np.colortex.cn

[T26] Swift：类与重写
来源：http://ga.gzmigu.cn

class A: Base { override func f() {} }
来源：http://em.colortex.cn

[T27] Swift：错误处理
来源：http://zi.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://bm.hahajie.cn

[T28] Swift：枚举
来源：http://to.panjiajie.cn

enum Color { case red, green }
来源：http://lw.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://fm.wgjwhj.cn

guard let x = opt else { return }
来源：http://tp.nszjky.cn

[T30] Swift：协议
来源：http://bl.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://ds.521024.cn

[T31] Lua：Hello World
来源：http://na.hnjuh.cn

print("Hello")
来源：http://ii.9csxet.cn

[T32] Lua：局部变量
来源：http://zs.szsharing.cn

local a = 1
来源：http://ak.huanxung.cn

[T33] Lua：表（数组）
来源：http://fw.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qv.asd995.cn

[T34] Lua：遍历表
来源：http://yo.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vl.bjjhwx.cn

[T35] Lua：字典表
来源：http://mi.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://qj.huixiangedu.cn

[T36] Lua：函数
来源：http://ur.jctech888.com.cn

function add(a, b) return a + b end
来源：http://xb.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://qs.hahajie.cn

"a" .. "b"
来源：http://ov.huanxung.cn

[T38] Lua：条件
来源：http://nu.shxzukj.cn

if x > 0 then print("正") end
来源：http://ao.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://mo.gzmigu.cn

string.find(s, "%d+")
来源：http://km.haigaiapp.cn

[T40] Lua：元表
来源：http://hp.newstarts.cn

setmetatable({}, { __index = base })
来源：http://qo.9csxet.cn

[T41] Perl：Hello World
来源：http://cj.colortex.cn

print "Hello\n";
来源：http://hn.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://kp.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yq.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://fm.panjiajie.cn

"值: $a"
来源：http://om.huixiangedu.cn

[T44] Perl：条件
来源：http://gc.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://qu.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://kd.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://ls.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://en.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ha.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://lx.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ls.yuexingan06.cn

[T48] Perl：正则替换
来源：http://xg.nszjky.cn

$s =~ s/old/new/g;
来源：http://pb.hnjuh.cn

[T49] Perl：函数
来源：http://os.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zz.newstarts.cn

[T50] Perl：逐行读文件
来源：http://cn.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xl.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://gm.chemitech.net.cn

[T51] Scala：Hello World
来源：http://ob.szsharing.cn

println("Hello")
来源：http://pm.9csxet.cn

[T52] Scala：变量
来源：http://rl.muxihuayi.cn


<!-- 参考信息 -->