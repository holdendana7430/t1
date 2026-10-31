代发 wailian999

cmd > out.log 2>&1
来源：http://gv.shtwfgs.cn

[R40] 追加写日志
来源：http://dv.gzmigu.cn

echo "log" >> out.log
来源：http://yu.wgjwhj.cn

[R41] 丢弃输出
来源：http://wm.yuntaijiaju.cn

cmd >/dev/null 2>&1
来源：http://jw.szxytkj.cn

[R42] 输入重定向
来源：http://it.yuexingan06.cn

wc -l < a.txt
来源：http://ka.shtwfgs.cn

[R43] 按名字查找文件
来源：http://iy.muxihuayi.cn

find . -name "*.log" -type f
来源：http://re.haigaiapp.cn

[R44] 按修改时间查找
来源：http://up.haigaiapp.cn

find . -mtime -7 -type f
来源：http://kk.lnxyls.cn

[R45] 批量删除
来源：http://cf.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://qs.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://jx.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://da.yuexingan06.cn

[R47] sed 单行替换
来源：http://od.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mg.bjjhwx.cn

[R48] awk 取指定列
来源：http://oj.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://bf.shtwfgs.cn

[R49] awk 带条件
来源：http://ds.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sx.muxihuayi.cn

[R50] awk 求和
来源：http://og.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ck.lnxyls.cn

[R51] 排序去重取前几
来源：http://wu.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://se.shtwfgs.cn

[R52] 统计行数
来源：http://xs.wgjwhj.cn

wc -l a.txt
来源：http://dl.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://yj.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kb.bookmarksfly.cn

[R54] 比较两个文件
来源：http://uq.hnjuh.cn

diff a.txt b.txt
来源：http://ei.nszjky.cn

[R55] 压缩与解压
来源：http://wr.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://po.huanxung.cn

[R56] 远程拷贝
来源：http://au.panjiajie.cn

scp file user@host:/path/
来源：http://xa.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://xe.asd995.cn

ssh user@host 'uptime'
来源：http://ej.muxihuayi.cn

[R58] 下载文件
来源：http://us.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://to.hahajie.cn

[R59] 发 POST JSON
来源：http://qd.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nv.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://ip.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://th.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://zb.chemitech.net.cn

df -h;  du -sh *
来源：http://lt.hnjuh.cn

[R62] 找最占空间的文件
来源：http://gm.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://og.hahajie.cn

[R63] 内存与进程
来源：http://zd.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://zq.gzmigu.cn

[R64] 结束进程
来源：http://kq.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://ys.asd995.cn

[R65] 查看端口占用
来源：http://bk.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xj.nicolike.cn

[R66] 定时任务
来源：http://yl.gzmigu.cn

crontab -e;  crontab -l
来源：http://og.szsharing.cn

[R67] 生成随机十六进制串
来源：http://qy.huixiangedu.cn

openssl rand -hex 16
来源：http://sw.szsharing.cn

[R68] 计算文件校验值
来源：http://hs.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wf.szxytkj.cn

[R69] 生成随机密码
来源：http://lw.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://xg.wgjwhj.cn

[R70] 时间戳与互转
来源：http://rw.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://pa.jctech888.com.cn

[R71] 日期格式化
来源：http://wn.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sv.shxzukj.cn

[R72] 等待端口就绪
来源：http://la.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fo.jianghongdianzi.cn

[R73] 分割大日志
来源：http://th.szsharing.cn

split -l 1000 big.log part_
来源：http://sl.bookmarksfly.cn

[R74] 批量重命名
来源：http://rm.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yn.chemitech.net.cn

[R75] 导出环境变量
来源：http://vl.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://oi.muxihuayi.cn

[R76] 使用临时文件
来源：http://vl.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cg.521024.cn

[R77] 读取用户输入
来源：http://sp.shxzukj.cn

read -rp "请输入: " ans
来源：http://yb.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://eu.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hq.lnxyls.cn

[R79] 解析命令行选项
来源：http://hc.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nx.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://dd.gzmigu.cn

time ./run.sh
来源：http://zk.hnjuh.cn

================================================================================
来源：http://px.huixinmuqiang.cn

S. C / C++ 专题
来源：http://pf.szsharing.cn

================================================================================
来源：http://on.jctech888.com.cn

[S01] C：Hello World
来源：http://ex.haigaiapp.cn

#include <stdio.h>
来源：http://tb.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ds.colortex.cn

[S02] C：变量与格式化输出
来源：http://ej.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://ya.muxihuayi.cn

[S03] C：读入整数
来源：http://hc.huixiangedu.cn

int x; scanf("%d", &x);
来源：http://rp.asd995.cn

[S04] C：字符串复制
来源：http://rw.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ow.shxzukj.cn

[S05] C：字符串长度
来源：http://lt.nszjky.cn

strlen(s)
来源：http://pl.huixiangedu.cn

[S06] C：字符串比较
来源：http://lc.panjiajie.cn

strcmp(a, b) == 0
来源：http://el.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://hh.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kc.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://dk.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://go.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://hb.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yo.nszjky.cn

[S10] C：指针与解引用
来源：http://ez.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://ri.shxzukj.cn

[S11] C：逐行读文件
来源：http://tb.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://vq.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vw.muxihuayi.cn

fclose(f);
来源：http://oc.9csxet.cn

[S12] C：写文件
来源：http://ey.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ik.huixinmuqiang.cn

[S13] C：宏定义
来源：http://wr.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jf.shxzskj.cn

[S14] C：枚举
来源：http://st.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://zy.9csxet.cn

[S15] C：类型转换
来源：http://jb.panjiajie.cn

(double) a / b
来源：http://my.shxzukj.cn

[S16] C：位操作置位
来源：http://hg.hahajie.cn

x |= (1 << 3);
来源：http://ef.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://pd.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://al.asd995.cn

[S18] C：命令行参数
来源：http://fn.szsharing.cn

int main(int argc, char **argv)
来源：http://ec.newstarts.cn

[S19] C：快速排序
来源：http://lb.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ry.shxzukj.cn

[S20] C：二分查找
来源：http://ve.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wf.panjiajie.cn

[S21] C：字符类别判断
来源：http://bn.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ov.hnjuh.cn

[S22] C：字符串转数字
来源：http://oe.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ox.nicolike.cn

[S23] C：随机数
来源：http://vy.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ns.szxytkj.cn

[S24] C：获取本地时间
来源：http://th.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wl.lnxyls.cn

[S25] C：内存拷贝
来源：http://fi.nszjky.cn

memcpy(dst, src, n);
来源：http://hq.521024.cn

[S26] C：内存清零
来源：http://dh.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ag.chemitech.net.cn

[S27] C：定义常量
来源：http://ns.panjiajie.cn

const double PI = 3.14159;
来源：http://lz.nicolike.cn

[S28] C：静态变量
来源：http://zj.panjiajie.cn

static int counter = 0;
来源：http://jz.szsharing.cn

[S29] C：变参函数
来源：http://sd.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ln.asd995.cn

[S30] C：头文件保护
来源：http://ir.bookmarksfly.cn

#ifndef X_H
来源：http://vz.lnxyls.cn

#define X_H
来源：http://ke.newstarts.cn

#endif
来源：http://rr.nicolike.cn

[S31] C++：Hello World
来源：http://vc.yuexingan06.cn

#include <iostream>
来源：http://vq.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ny.shxzskj.cn

[S32] C++：字符串
来源：http://cr.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://ki.yuexingan06.cn

[S33] C++：vector 增删
来源：http://fb.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ie.nicolike.cn

[S34] C++：遍历 vector
来源：http://ha.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://td.shtwfgs.cn

[S35] C++：map
来源：http://vu.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gf.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://ar.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sh.huanxung.cn

[S37] C++：set
来源：http://aw.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jg.shxzukj.cn

[S38] C++：排序
来源：http://ss.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://xo.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://qx.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://po.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://uu.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ws.lnxyls.cn

[S41] C++：类与构造函数
来源：http://hh.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cl.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://fd.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://if.9csxet.cn

[S43] C++：智能指针
来源：http://gw.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://ik.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://bb.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://fy.shtwfgs.cn

[S45] C++：lambda
来源：http://yf.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://om.shxzukj.cn

[S46] C++：函数模板
来源：http://yr.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vk.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://wz.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qr.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://al.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://et.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ll.gzmigu.cn

[S49] C++：写文件
来源：http://li.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ic.huanxung.cn

[S50] C++：格式化数字
来源：http://bq.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ka.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://ll.haigaiapp.cn

static_cast<double>(a) / b
来源：http://ng.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://gd.szsharing.cn

int size() const noexcept { return n_; }
来源：http://fe.bookmarksfly.cn

[S53] C++：移动语义
来源：http://hh.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://nj.wgjwhj.cn

[S54] C++：异常处理
来源：http://xu.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ud.szxytkj.cn

[S55] C++：结构化绑定
来源：http://la.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zi.shtwfgs.cn

[S56] C++：optional
来源：http://jt.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://di.chemitech.net.cn

[S57] C++：编译期常量
来源：http://yq.haigaiapp.cn

constexpr int N = 10;
来源：http://hb.huanxung.cn

[S58] C++：命名空间
来源：http://rh.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://ku.bookmarksfly.cn

[S59] C++：静态断言
来源：http://xm.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cc.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://pv.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://at.muxihuayi.cn

================================================================================
来源：http://xh.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pn.huanxung.cn

================================================================================
来源：http://ci.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://ss.gzmigu.cn

println("Hello")
来源：http://vb.nicolike.cn

[T02] Kotlin：变量
来源：http://ae.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hl.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://wx.szxytkj.cn

"值: $b"
来源：http://uq.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://it.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://oz.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://ji.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xw.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://gr.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zl.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ca.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rk.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://bl.521024.cn

data class User(val name: String, val age: Int)
来源：http://ay.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ov.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://eh.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://ej.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bf.newstarts.cn

[T11] Kotlin：协程
来源：http://wc.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dx.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://uq.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://qi.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://ij.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://eo.shxzukj.cn

[T14] Kotlin：循环
来源：http://bl.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://qq.asd995.cn

[T15] Kotlin：接口
来源：http://md.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://dp.shxzskj.cn

[T16] Swift：Hello World
来源：http://ai.newstarts.cn

print("Hello")
来源：http://lo.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://fx.9csxet.cn

var a = 1;  let b = 2
来源：http://hq.hahajie.cn

[T18] Swift：字符串插值
来源：http://bi.huanxung.cn

"值: \(b)"
来源：http://yq.gzmigu.cn

[T19] Swift：可选绑定
来源：http://mk.gzmigu.cn

if let n = opt { print(n) }
来源：http://wy.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://cj.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lv.lnxyls.cn

[T21] Swift：遍历
来源：http://il.panjiajie.cn

for x in a { print(x) }
来源：http://an.521024.cn

[T22] Swift：字典
来源：http://fz.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cd.bookmarksfly.cn

[T23] Swift：函数
来源：http://kd.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dz.asd995.cn

[T24] Swift：闭包
来源：http://ht.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cj.gzmigu.cn

[T25] Swift：结构体
来源：http://jn.hahajie.cn

struct P { var x: Int }
来源：http://ha.chemitech.net.cn

[T26] Swift：类与重写
来源：http://qt.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://lf.bjjhwx.cn

[T27] Swift：错误处理
来源：http://ug.newstarts.cn

do { try f() } catch { print(error) }
来源：http://lb.shxzukj.cn

[T28] Swift：枚举
来源：http://wu.shxzukj.cn

enum Color { case red, green }
来源：http://qq.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://vl.haigaiapp.cn

guard let x = opt else { return }
来源：http://we.panjiajie.cn

[T30] Swift：协议
来源：http://zt.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://cs.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://pp.chemitech.net.cn

print("Hello")
来源：http://un.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://uw.huixiangedu.cn

local a = 1
来源：http://jp.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://ou.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xt.nicolike.cn

[T34] Lua：遍历表
来源：http://dn.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mj.huixiangedu.cn

[T35] Lua：字典表
来源：http://ub.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://sg.huanxung.cn

[T36] Lua：函数
来源：http://xa.colortex.cn

function add(a, b) return a + b end
来源：http://iq.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://ox.shxzukj.cn

"a" .. "b"
来源：http://wr.gzmigu.cn

[T38] Lua：条件
来源：http://vr.521024.cn

if x > 0 then print("正") end
来源：http://do.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://dm.wgjwhj.cn

string.find(s, "%d+")
来源：http://oj.huixinmuqiang.cn

[T40] Lua：元表
来源：http://bu.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://qi.9csxet.cn

[T41] Perl：Hello World
来源：http://qw.wgjwhj.cn

print "Hello\n";
来源：http://nz.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://rz.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ne.jianghongdianzi.cn


<!-- 参考信息 -->