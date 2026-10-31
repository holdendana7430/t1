代发 wailian999

cmd > out.log 2>&1
来源：http://fb.chemitech.net.cn

[R40] 追加写日志
来源：http://ly.huanxung.cn

echo "log" >> out.log
来源：http://ue.bjjhwx.cn

[R41] 丢弃输出
来源：http://az.huanxung.cn

cmd >/dev/null 2>&1
来源：http://bp.colortex.cn

[R42] 输入重定向
来源：http://yb.lnxyls.cn

wc -l < a.txt
来源：http://ot.jctech888.com.cn

[R43] 按名字查找文件
来源：http://nz.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://po.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://zx.chemitech.net.cn

find . -mtime -7 -type f
来源：http://as.lnxyls.cn

[R45] 批量删除
来源：http://qh.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://ao.hahajie.cn

[R46] 递归替换文件内容
来源：http://gr.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pf.hnjuh.cn

[R47] sed 单行替换
来源：http://ke.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://is.yuexingan06.cn

[R48] awk 取指定列
来源：http://po.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://ns.muxihuayi.cn

[R49] awk 带条件
来源：http://kz.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vj.huixinmuqiang.cn

[R50] awk 求和
来源：http://gg.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uj.gzmigu.cn

[R51] 排序去重取前几
来源：http://yf.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fv.szsharing.cn

[R52] 统计行数
来源：http://ed.yuexingan06.cn

wc -l a.txt
来源：http://td.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://fz.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ea.hnjuh.cn

[R54] 比较两个文件
来源：http://eg.colortex.cn

diff a.txt b.txt
来源：http://qb.colortex.cn

[R55] 压缩与解压
来源：http://ld.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xv.shtwfgs.cn

[R56] 远程拷贝
来源：http://qu.jianghongdianzi.cn

scp file user@host:/path/
来源：http://rx.jctech888.com.cn

[R57] 远程执行命令
来源：http://mf.lnxyls.cn

ssh user@host 'uptime'
来源：http://ej.yuntaijiaju.cn

[R58] 下载文件
来源：http://si.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mn.521024.cn

[R59] 发 POST JSON
来源：http://zd.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://td.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://ql.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fn.9csxet.cn

[R61] 磁盘占用
来源：http://px.nicolike.cn

df -h;  du -sh *
来源：http://ix.9csxet.cn

[R62] 找最占空间的文件
来源：http://ke.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://un.nicolike.cn

[R63] 内存与进程
来源：http://ca.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://my.szxytkj.cn

[R64] 结束进程
来源：http://oq.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://aj.muxihuayi.cn

[R65] 查看端口占用
来源：http://cn.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gw.colortex.cn

[R66] 定时任务
来源：http://yo.jctech888.com.cn

crontab -e;  crontab -l
来源：http://qr.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://lz.huixinmuqiang.cn

openssl rand -hex 16
来源：http://at.huixiangedu.cn

[R68] 计算文件校验值
来源：http://lt.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://en.bookmarksfly.cn

[R69] 生成随机密码
来源：http://do.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://zi.gzmigu.cn

[R70] 时间戳与互转
来源：http://xg.521024.cn

date +%s;  date -d @1700000000
来源：http://fk.huixiangedu.cn

[R71] 日期格式化
来源：http://gl.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vz.muxihuayi.cn

[R72] 等待端口就绪
来源：http://vd.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yn.bookmarksfly.cn

[R73] 分割大日志
来源：http://yt.hahajie.cn

split -l 1000 big.log part_
来源：http://ij.nszjky.cn

[R74] 批量重命名
来源：http://tw.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pq.shxzukj.cn

[R75] 导出环境变量
来源：http://md.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://il.lnxyls.cn

[R76] 使用临时文件
来源：http://gb.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ai.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://ss.shtwfgs.cn

read -rp "请输入: " ans
来源：http://be.haigaiapp.cn

[R78] 交互式菜单
来源：http://ur.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mk.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://hj.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ig.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ed.haigaiapp.cn

time ./run.sh
来源：http://kh.shxzskj.cn

================================================================================
来源：http://qs.szxytkj.cn

S. C / C++ 专题
来源：http://oq.lnxyls.cn

================================================================================
来源：http://qr.shxzskj.cn

[S01] C：Hello World
来源：http://bl.huixinmuqiang.cn

#include <stdio.h>
来源：http://sx.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xh.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://qj.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://cz.yuntaijiaju.cn

[S03] C：读入整数
来源：http://oh.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://sh.huixiangedu.cn

[S04] C：字符串复制
来源：http://gy.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rq.panjiajie.cn

[S05] C：字符串长度
来源：http://eb.chemitech.net.cn

strlen(s)
来源：http://tj.panjiajie.cn

[S06] C：字符串比较
来源：http://yr.hnjuh.cn

strcmp(a, b) == 0
来源：http://rg.shxzskj.cn

[S07] C：数组遍历求和
来源：http://hk.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yl.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://jg.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wv.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://zp.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nw.gzmigu.cn

[S10] C：指针与解引用
来源：http://zs.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://gp.521024.cn

[S11] C：逐行读文件
来源：http://xt.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ct.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mr.yuntaijiaju.cn

fclose(f);
来源：http://dr.shxzukj.cn

[S12] C：写文件
来源：http://db.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tc.huanxung.cn

[S13] C：宏定义
来源：http://wm.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ve.yuexingan06.cn

[S14] C：枚举
来源：http://qw.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://tv.nicolike.cn

[S15] C：类型转换
来源：http://dk.haigaiapp.cn

(double) a / b
来源：http://up.shtwfgs.cn

[S16] C：位操作置位
来源：http://ms.gzmigu.cn

x |= (1 << 3);
来源：http://xd.newstarts.cn

[S17] C：安全拼接字符串
来源：http://pw.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zn.shtwfgs.cn

[S18] C：命令行参数
来源：http://jr.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ss.521024.cn

[S19] C：快速排序
来源：http://vi.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cz.muxihuayi.cn

[S20] C：二分查找
来源：http://wf.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yq.huixiangedu.cn

[S21] C：字符类别判断
来源：http://mx.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yq.huixiangedu.cn

[S22] C：字符串转数字
来源：http://kl.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jk.colortex.cn

[S23] C：随机数
来源：http://bi.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qy.chemitech.net.cn

[S24] C：获取本地时间
来源：http://zy.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ym.shtwfgs.cn

[S25] C：内存拷贝
来源：http://we.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://vg.jctech888.com.cn

[S26] C：内存清零
来源：http://kb.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://gd.nszjky.cn

[S27] C：定义常量
来源：http://px.haigaiapp.cn

const double PI = 3.14159;
来源：http://oz.gzmigu.cn

[S28] C：静态变量
来源：http://ww.lnxyls.cn

static int counter = 0;
来源：http://ud.shtwfgs.cn

[S29] C：变参函数
来源：http://fm.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hb.panjiajie.cn

[S30] C：头文件保护
来源：http://yp.bookmarksfly.cn

#ifndef X_H
来源：http://kh.521024.cn

#define X_H
来源：http://qq.szxytkj.cn

#endif
来源：http://xi.asd995.cn

[S31] C++：Hello World
来源：http://rb.panjiajie.cn

#include <iostream>
来源：http://og.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://eq.nicolike.cn

[S32] C++：字符串
来源：http://da.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ur.muxihuayi.cn

[S33] C++：vector 增删
来源：http://cx.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xf.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://pg.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://xw.huixinmuqiang.cn

[S35] C++：map
来源：http://kf.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bh.wgjwhj.cn

[S36] C++：unordered_map
来源：http://yq.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nl.wgjwhj.cn

[S37] C++：set
来源：http://qc.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rt.hahajie.cn

[S38] C++：排序
来源：http://rx.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://rd.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://uu.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wc.szxytkj.cn

[S40] C++：查找元素
来源：http://uq.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rm.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://cy.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qx.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://mc.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://om.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://br.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://oy.hahajie.cn

[S44] C++：引用传参
来源：http://ig.huanxung.cn

void inc(int &x) { ++x; }
来源：http://nn.newstarts.cn

[S45] C++：lambda
来源：http://rt.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ag.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://pk.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rt.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://ks.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://el.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://qd.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rk.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://qw.newstarts.cn

[S49] C++：写文件
来源：http://dp.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xa.muxihuayi.cn

[S50] C++：格式化数字
来源：http://vt.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xt.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://rh.asd995.cn

static_cast<double>(a) / b
来源：http://fi.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://hj.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://kt.muxihuayi.cn

[S53] C++：移动语义
来源：http://pw.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://xa.yuexingan06.cn

[S54] C++：异常处理
来源：http://jg.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://or.nicolike.cn

[S55] C++：结构化绑定
来源：http://nn.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sq.yuexingan06.cn

[S56] C++：optional
来源：http://bq.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sv.hnjuh.cn

[S57] C++：编译期常量
来源：http://wi.jctech888.com.cn

constexpr int N = 10;
来源：http://vz.521024.cn

[S58] C++：命名空间
来源：http://yz.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://go.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://mx.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ya.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://gh.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uf.wgjwhj.cn

================================================================================
来源：http://ko.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zk.hnjuh.cn

================================================================================
来源：http://gn.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://qa.shtwfgs.cn

println("Hello")
来源：http://wp.asd995.cn

[T02] Kotlin：变量
来源：http://fb.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fo.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://gi.hahajie.cn

"值: $b"
来源：http://qx.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://ka.shxzskj.cn

val n: String? = null;  n?.length
来源：http://dw.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://if.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zj.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://rg.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eb.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://gn.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oy.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://kl.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://ah.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://le.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://xy.colortex.cn

[T10] Kotlin：默认参数
来源：http://tl.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ej.yuexingan06.cn

[T11] Kotlin：协程
来源：http://bv.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://go.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://ot.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://sz.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://xi.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://vs.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://yy.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://ji.jctech888.com.cn

[T15] Kotlin：接口
来源：http://xv.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://ss.asd995.cn

[T16] Swift：Hello World
来源：http://je.huixinmuqiang.cn

print("Hello")
来源：http://tm.lnxyls.cn

[T17] Swift：变量与常量
来源：http://qi.gzmigu.cn

var a = 1;  let b = 2
来源：http://mn.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://ji.haigaiapp.cn

"值: \(b)"
来源：http://be.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://fi.muxihuayi.cn

if let n = opt { print(n) }
来源：http://je.lnxyls.cn

[T20] Swift：数组操作
来源：http://tp.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qt.newstarts.cn

[T21] Swift：遍历
来源：http://jl.wgjwhj.cn

for x in a { print(x) }
来源：http://hq.colortex.cn

[T22] Swift：字典
来源：http://ik.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vn.newstarts.cn

[T23] Swift：函数
来源：http://lh.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kx.shxzukj.cn

[T24] Swift：闭包
来源：http://yz.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dg.newstarts.cn

[T25] Swift：结构体
来源：http://ig.huanxung.cn

struct P { var x: Int }
来源：http://vk.shtwfgs.cn

[T26] Swift：类与重写
来源：http://vt.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://lo.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://gr.asd995.cn

do { try f() } catch { print(error) }
来源：http://cs.panjiajie.cn

[T28] Swift：枚举
来源：http://mo.huanxung.cn

enum Color { case red, green }
来源：http://kk.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://uw.521024.cn

guard let x = opt else { return }
来源：http://at.jctech888.com.cn

[T30] Swift：协议
来源：http://jv.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://iw.szxytkj.cn

[T31] Lua：Hello World
来源：http://je.szsharing.cn

print("Hello")
来源：http://cs.shxzukj.cn

[T32] Lua：局部变量
来源：http://qq.muxihuayi.cn

local a = 1
来源：http://cr.hahajie.cn

[T33] Lua：表（数组）
来源：http://qq.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yk.asd995.cn

[T34] Lua：遍历表
来源：http://lb.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://re.asd995.cn

[T35] Lua：字典表
来源：http://ea.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://os.hnjuh.cn

[T36] Lua：函数
来源：http://fz.gzmigu.cn

function add(a, b) return a + b end
来源：http://my.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://fj.colortex.cn

"a" .. "b"
来源：http://io.asd995.cn

[T38] Lua：条件
来源：http://xh.shxzskj.cn

if x > 0 then print("正") end
来源：http://uk.lnxyls.cn

[T39] Lua：模式匹配
来源：http://ik.9csxet.cn

string.find(s, "%d+")
来源：http://cp.521024.cn

[T40] Lua：元表
来源：http://gh.9csxet.cn

setmetatable({}, { __index = base })
来源：http://yx.jctech888.com.cn

[T41] Perl：Hello World
来源：http://bs.muxihuayi.cn

print "Hello\n";
来源：http://yy.nszjky.cn

[T42] Perl：变量类型
来源：http://me.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://of.wgjwhj.cn


<!-- 参考信息 -->