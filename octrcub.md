代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ff.9csxet.cn

[R34] 退出时清理
来源：http://gt.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mk.shxzskj.cn

[R35] 后台执行并等待
来源：http://ja.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bc.nszjky.cn

[R36] 并发执行多个任务
来源：http://so.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dr.hahajie.cn

[R37] 把输出赋给变量
来源：http://ab.muxihuayi.cn

files=$(ls -1)
来源：http://ua.asd995.cn

[R38] 管道串联
来源：http://oi.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://hp.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://na.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://bu.9csxet.cn

[R40] 追加写日志
来源：http://vp.chemitech.net.cn

echo "log" >> out.log
来源：http://wk.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://gy.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://ti.lnxyls.cn

[R42] 输入重定向
来源：http://hv.huixiangedu.cn

wc -l < a.txt
来源：http://ft.nicolike.cn

[R43] 按名字查找文件
来源：http://oo.nicolike.cn

find . -name "*.log" -type f
来源：http://zx.wgjwhj.cn

[R44] 按修改时间查找
来源：http://ob.asd995.cn

find . -mtime -7 -type f
来源：http://hu.yuntaijiaju.cn

[R45] 批量删除
来源：http://xh.jianghongdianzi.cn

find . -name "*.tmp" -delete
来源：http://ay.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://qa.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://us.nicolike.cn

[R47] sed 单行替换
来源：http://hw.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xf.yuexingan06.cn

[R48] awk 取指定列
来源：http://zs.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://rc.hnjuh.cn

[R49] awk 带条件
来源：http://yd.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pf.gzmigu.cn

[R50] awk 求和
来源：http://av.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pz.jctech888.com.cn

[R51] 排序去重取前几
来源：http://al.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ru.szxytkj.cn

[R52] 统计行数
来源：http://td.nszjky.cn

wc -l a.txt
来源：http://pq.521024.cn

[R53] 查看文件头与实时尾
来源：http://uv.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zp.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://on.chemitech.net.cn

diff a.txt b.txt
来源：http://hz.haigaiapp.cn

[R55] 压缩与解压
来源：http://ko.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mb.haigaiapp.cn

[R56] 远程拷贝
来源：http://aa.haigaiapp.cn

scp file user@host:/path/
来源：http://sv.huixiangedu.cn

[R57] 远程执行命令
来源：http://yf.colortex.cn

ssh user@host 'uptime'
来源：http://zh.szsharing.cn

[R58] 下载文件
来源：http://hg.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gd.shxzskj.cn

[R59] 发 POST JSON
来源：http://sx.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ma.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://nw.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qp.chemitech.net.cn

[R61] 磁盘占用
来源：http://ht.haigaiapp.cn

df -h;  du -sh *
来源：http://ri.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://yk.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://gz.hnjuh.cn

[R63] 内存与进程
来源：http://hi.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://ce.shxzukj.cn

[R64] 结束进程
来源：http://pa.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://ws.bjjhwx.cn

[R65] 查看端口占用
来源：http://nq.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wa.521024.cn

[R66] 定时任务
来源：http://bg.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://yv.huanxung.cn

[R67] 生成随机十六进制串
来源：http://th.hnjuh.cn

openssl rand -hex 16
来源：http://ye.521024.cn

[R68] 计算文件校验值
来源：http://tj.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hr.hnjuh.cn

[R69] 生成随机密码
来源：http://ov.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://au.wgjwhj.cn

[R70] 时间戳与互转
来源：http://lf.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://gn.nszjky.cn

[R71] 日期格式化
来源：http://il.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wc.521024.cn

[R72] 等待端口就绪
来源：http://mw.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oh.wgjwhj.cn

[R73] 分割大日志
来源：http://di.jctech888.com.cn

split -l 1000 big.log part_
来源：http://nm.asd995.cn

[R74] 批量重命名
来源：http://ee.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lb.panjiajie.cn

[R75] 导出环境变量
来源：http://rv.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://yc.colortex.cn

[R76] 使用临时文件
来源：http://mt.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ok.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://tj.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://jc.newstarts.cn

[R78] 交互式菜单
来源：http://vk.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ls.nicolike.cn

[R79] 解析命令行选项
来源：http://ja.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vt.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://zw.colortex.cn

time ./run.sh
来源：http://iw.hahajie.cn

================================================================================
来源：http://ab.nszjky.cn

S. C / C++ 专题
来源：http://el.9csxet.cn

================================================================================
来源：http://ak.panjiajie.cn

[S01] C：Hello World
来源：http://wx.huixiangedu.cn

#include <stdio.h>
来源：http://ns.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qy.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://zf.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://oi.shtwfgs.cn

[S03] C：读入整数
来源：http://kf.gzmigu.cn

int x; scanf("%d", &x);
来源：http://ga.huixiangedu.cn

[S04] C：字符串复制
来源：http://jc.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xu.szsharing.cn

[S05] C：字符串长度
来源：http://en.huixiangedu.cn

strlen(s)
来源：http://wc.huixiangedu.cn

[S06] C：字符串比较
来源：http://vz.shxzukj.cn

strcmp(a, b) == 0
来源：http://gn.szxytkj.cn

[S07] C：数组遍历求和
来源：http://mw.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cn.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://hy.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mq.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://xk.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bm.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://gr.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://es.9csxet.cn

[S11] C：逐行读文件
来源：http://ld.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://tm.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iq.bookmarksfly.cn

fclose(f);
来源：http://zr.shxzukj.cn

[S12] C：写文件
来源：http://eg.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ez.shxzskj.cn

[S13] C：宏定义
来源：http://hd.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jc.nicolike.cn

[S14] C：枚举
来源：http://jn.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://gk.huixinmuqiang.cn

[S15] C：类型转换
来源：http://my.shtwfgs.cn

(double) a / b
来源：http://jy.nszjky.cn

[S16] C：位操作置位
来源：http://ek.muxihuayi.cn

x |= (1 << 3);
来源：http://lm.nicolike.cn

[S17] C：安全拼接字符串
来源：http://fv.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bt.gzmigu.cn

[S18] C：命令行参数
来源：http://zo.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://sa.hahajie.cn

[S19] C：快速排序
来源：http://ff.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ty.haigaiapp.cn

[S20] C：二分查找
来源：http://xs.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xa.nicolike.cn

[S21] C：字符类别判断
来源：http://ce.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jl.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://cs.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://km.colortex.cn

[S23] C：随机数
来源：http://gd.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.yuexingan06.cn

[S24] C：获取本地时间
来源：http://nr.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ts.colortex.cn

[S25] C：内存拷贝
来源：http://vn.nicolike.cn

memcpy(dst, src, n);
来源：http://ze.bjjhwx.cn

[S26] C：内存清零
来源：http://lj.huanxung.cn

memset(a, 0, sizeof a);
来源：http://lx.huanxung.cn

[S27] C：定义常量
来源：http://ch.9csxet.cn

const double PI = 3.14159;
来源：http://bs.newstarts.cn

[S28] C：静态变量
来源：http://nd.bookmarksfly.cn

static int counter = 0;
来源：http://qi.nicolike.cn

[S29] C：变参函数
来源：http://gu.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qw.szxytkj.cn

[S30] C：头文件保护
来源：http://kd.haigaiapp.cn

#ifndef X_H
来源：http://go.shxzukj.cn

#define X_H
来源：http://qx.gzmigu.cn

#endif
来源：http://wg.nicolike.cn

[S31] C++：Hello World
来源：http://ti.szsharing.cn

#include <iostream>
来源：http://rd.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://sx.newstarts.cn

[S32] C++：字符串
来源：http://hb.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://tm.szxytkj.cn

[S33] C++：vector 增删
来源：http://fm.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fy.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://da.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://ug.nicolike.cn

[S35] C++：map
来源：http://pa.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cx.szxytkj.cn

[S36] C++：unordered_map
来源：http://mv.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vj.wgjwhj.cn

[S37] C++：set
来源：http://or.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ac.huanxung.cn

[S38] C++：排序
来源：http://nk.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://hb.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://wr.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gp.chemitech.net.cn

[S40] C++：查找元素
来源：http://go.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wl.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://zi.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zo.hahajie.cn

[S42] C++：继承与虚函数
来源：http://qk.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://pn.shtwfgs.cn

[S43] C++：智能指针
来源：http://bw.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://lu.newstarts.cn

[S44] C++：引用传参
来源：http://kv.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://fp.panjiajie.cn

[S45] C++：lambda
来源：http://gj.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ui.bjjhwx.cn

[S46] C++：函数模板
来源：http://kx.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ti.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://zx.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wm.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://hz.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xd.huanxung.cn

while (std::getline(in, line)) { }
来源：http://xl.muxihuayi.cn

[S49] C++：写文件
来源：http://yl.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tf.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://li.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zr.newstarts.cn

[S51] C++：显式类型转换
来源：http://ea.nszjky.cn

static_cast<double>(a) / b
来源：http://kn.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://fx.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://wk.wgjwhj.cn

[S53] C++：移动语义
来源：http://sw.asd995.cn

std::vector<int> w = std::move(v);
来源：http://eu.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://rk.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cx.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://pg.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yh.yuntaijiaju.cn

[S56] C++：optional
来源：http://oj.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mr.hnjuh.cn

[S57] C++：编译期常量
来源：http://iz.shxzukj.cn

constexpr int N = 10;
来源：http://gi.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://hi.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://yh.nszjky.cn

[S59] C++：静态断言
来源：http://sb.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jj.asd995.cn

[S60] C++：遍历并删除元素
来源：http://fy.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://of.asd995.cn

================================================================================
来源：http://ip.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ab.szsharing.cn

================================================================================
来源：http://mk.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://nf.haigaiapp.cn

println("Hello")
来源：http://vm.szsharing.cn

[T02] Kotlin：变量
来源：http://at.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wa.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://wi.hahajie.cn

"值: $b"
来源：http://sz.gzmigu.cn

[T04] Kotlin：空安全
来源：http://ah.panjiajie.cn

val n: String? = null;  n?.length
来源：http://vl.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://xj.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fp.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://oe.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eb.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://qy.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sn.huanxung.cn

[T08] Kotlin：数据类
来源：http://ii.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://np.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://xo.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://la.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://th.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ra.hahajie.cn

[T11] Kotlin：协程
来源：http://fh.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cw.hahajie.cn

[T12] Kotlin：解构声明
来源：http://za.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://vu.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://up.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://tk.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://mm.shxzskj.cn

for (i in 1..10) println(i)
来源：http://du.521024.cn

[T15] Kotlin：接口
来源：http://vy.nszjky.cn

interface Shape { fun area(): Double }
来源：http://nf.shxzukj.cn

[T16] Swift：Hello World
来源：http://lm.nszjky.cn

print("Hello")
来源：http://sm.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://qx.9csxet.cn

var a = 1;  let b = 2
来源：http://pt.nszjky.cn

[T18] Swift：字符串插值
来源：http://fk.panjiajie.cn

"值: \(b)"
来源：http://ee.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://cl.asd995.cn

if let n = opt { print(n) }
来源：http://ew.muxihuayi.cn

[T20] Swift：数组操作
来源：http://aq.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tz.colortex.cn

[T21] Swift：遍历
来源：http://rr.nszjky.cn

for x in a { print(x) }
来源：http://kg.muxihuayi.cn

[T22] Swift：字典
来源：http://qe.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xw.haigaiapp.cn

[T23] Swift：函数
来源：http://cj.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fc.shxzskj.cn

[T24] Swift：闭包
来源：http://xq.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ov.szxytkj.cn

[T25] Swift：结构体
来源：http://yi.newstarts.cn

struct P { var x: Int }
来源：http://uf.shxzukj.cn

[T26] Swift：类与重写
来源：http://cg.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://lc.wgjwhj.cn

[T27] Swift：错误处理
来源：http://wk.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://tf.gzmigu.cn

[T28] Swift：枚举
来源：http://cf.hnjuh.cn

enum Color { case red, green }
来源：http://ew.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://lc.wgjwhj.cn

guard let x = opt else { return }
来源：http://tt.muxihuayi.cn

[T30] Swift：协议
来源：http://be.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://ko.shxzukj.cn

[T31] Lua：Hello World
来源：http://ur.szsharing.cn

print("Hello")
来源：http://hk.panjiajie.cn

[T32] Lua：局部变量
来源：http://gk.huixiangedu.cn

local a = 1
来源：http://zp.newstarts.cn

[T33] Lua：表（数组）
来源：http://vw.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qh.shtwfgs.cn

[T34] Lua：遍历表
来源：http://ux.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aq.nicolike.cn

[T35] Lua：字典表
来源：http://yy.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://yd.shxzskj.cn

[T36] Lua：函数
来源：http://vu.shxzukj.cn

function add(a, b) return a + b end
来源：http://pa.521024.cn


<!-- 参考信息 -->