代发 wailian999

files=$(ls -1)
来源：http://dl.bookmarksfly.cn

[R38] 管道串联
来源：http://ha.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://fr.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://lr.521024.cn

cmd > out.log 2>&1
来源：http://lk.huixinmuqiang.cn

[R40] 追加写日志
来源：http://dp.bookmarksfly.cn

echo "log" >> out.log
来源：http://lc.huanxung.cn

[R41] 丢弃输出
来源：http://pe.521024.cn

cmd >/dev/null 2>&1
来源：http://bf.szxytkj.cn

[R42] 输入重定向
来源：http://xz.shxzskj.cn

wc -l < a.txt
来源：http://gf.muxihuayi.cn

[R43] 按名字查找文件
来源：http://eq.shxzskj.cn

find . -name "*.log" -type f
来源：http://ps.yuexingan06.cn

[R44] 按修改时间查找
来源：http://zt.newstarts.cn

find . -mtime -7 -type f
来源：http://ks.yuexingan06.cn

[R45] 批量删除
来源：http://ua.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://xd.lnxyls.cn

[R46] 递归替换文件内容
来源：http://os.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ya.shxzukj.cn

[R47] sed 单行替换
来源：http://vd.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://py.wgjwhj.cn

[R48] awk 取指定列
来源：http://kz.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://ep.521024.cn

[R49] awk 带条件
来源：http://ps.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uz.asd995.cn

[R50] awk 求和
来源：http://qb.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ig.szxytkj.cn

[R51] 排序去重取前几
来源：http://md.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qe.huixiangedu.cn

[R52] 统计行数
来源：http://dp.nszjky.cn

wc -l a.txt
来源：http://xa.521024.cn

[R53] 查看文件头与实时尾
来源：http://nt.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tn.colortex.cn

[R54] 比较两个文件
来源：http://ab.huanxung.cn

diff a.txt b.txt
来源：http://ap.gzmigu.cn

[R55] 压缩与解压
来源：http://oc.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wy.shxzskj.cn

[R56] 远程拷贝
来源：http://hx.521024.cn

scp file user@host:/path/
来源：http://nx.gzmigu.cn

[R57] 远程执行命令
来源：http://ss.chemitech.net.cn

ssh user@host 'uptime'
来源：http://vy.hahajie.cn

[R58] 下载文件
来源：http://xm.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bc.szsharing.cn

[R59] 发 POST JSON
来源：http://ms.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://th.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://ap.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gb.nicolike.cn

[R61] 磁盘占用
来源：http://lm.bookmarksfly.cn

df -h;  du -sh *
来源：http://se.hnjuh.cn

[R62] 找最占空间的文件
来源：http://ph.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://wf.colortex.cn

[R63] 内存与进程
来源：http://uz.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://nr.bookmarksfly.cn

[R64] 结束进程
来源：http://vx.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://wj.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://zv.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nz.szsharing.cn

[R66] 定时任务
来源：http://ie.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://fp.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://dp.wgjwhj.cn

openssl rand -hex 16
来源：http://fq.wgjwhj.cn

[R68] 计算文件校验值
来源：http://uz.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://al.szsharing.cn

[R69] 生成随机密码
来源：http://eo.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://cz.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://tw.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://jm.newstarts.cn

[R71] 日期格式化
来源：http://gr.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tp.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://zb.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zy.huixinmuqiang.cn

[R73] 分割大日志
来源：http://wp.huixiangedu.cn

split -l 1000 big.log part_
来源：http://cm.newstarts.cn

[R74] 批量重命名
来源：http://id.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://im.huanxung.cn

[R75] 导出环境变量
来源：http://yt.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://cn.521024.cn

[R76] 使用临时文件
来源：http://fz.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gp.shxzskj.cn

[R77] 读取用户输入
来源：http://dt.newstarts.cn

read -rp "请输入: " ans
来源：http://dp.bjjhwx.cn

[R78] 交互式菜单
来源：http://iy.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rg.9csxet.cn

[R79] 解析命令行选项
来源：http://yl.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gi.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://sg.chemitech.net.cn

time ./run.sh
来源：http://hv.haigaiapp.cn

================================================================================
来源：http://re.szsharing.cn

S. C / C++ 专题
来源：http://oz.shxzukj.cn

================================================================================
来源：http://ju.huixiangedu.cn

[S01] C：Hello World
来源：http://yw.yuntaijiaju.cn

#include <stdio.h>
来源：http://yx.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ja.nicolike.cn

[S02] C：变量与格式化输出
来源：http://ol.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://bu.bjjhwx.cn

[S03] C：读入整数
来源：http://pi.shxzukj.cn

int x; scanf("%d", &x);
来源：http://lh.yuexingan06.cn

[S04] C：字符串复制
来源：http://gf.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ff.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://kd.colortex.cn

strlen(s)
来源：http://hj.hahajie.cn

[S06] C：字符串比较
来源：http://bb.shxzskj.cn

strcmp(a, b) == 0
来源：http://wh.gzmigu.cn

[S07] C：数组遍历求和
来源：http://ej.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qj.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://mz.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ba.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://kx.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uk.yuexingan06.cn

[S10] C：指针与解引用
来源：http://du.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://gx.panjiajie.cn

[S11] C：逐行读文件
来源：http://sn.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://vn.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bj.huixinmuqiang.cn

fclose(f);
来源：http://ei.shxzukj.cn

[S12] C：写文件
来源：http://eg.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dr.colortex.cn

[S13] C：宏定义
来源：http://rn.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mh.haigaiapp.cn

[S14] C：枚举
来源：http://sc.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://oc.shxzskj.cn

[S15] C：类型转换
来源：http://sl.szxytkj.cn

(double) a / b
来源：http://st.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://uf.gzmigu.cn

x |= (1 << 3);
来源：http://dm.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://hf.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zi.lnxyls.cn

[S18] C：命令行参数
来源：http://gx.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://ew.yuexingan06.cn

[S19] C：快速排序
来源：http://go.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ch.yuexingan06.cn

[S20] C：二分查找
来源：http://fk.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://he.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://hf.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aa.shxzukj.cn

[S22] C：字符串转数字
来源：http://wi.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ng.huixiangedu.cn

[S23] C：随机数
来源：http://wg.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ss.huanxung.cn

[S24] C：获取本地时间
来源：http://zf.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dk.hahajie.cn

[S25] C：内存拷贝
来源：http://vv.huanxung.cn

memcpy(dst, src, n);
来源：http://kb.yuexingan06.cn

[S26] C：内存清零
来源：http://fa.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://yr.bookmarksfly.cn

[S27] C：定义常量
来源：http://ga.bookmarksfly.cn

const double PI = 3.14159;
来源：http://xb.szxytkj.cn

[S28] C：静态变量
来源：http://lj.huanxung.cn

static int counter = 0;
来源：http://rc.yuexingan06.cn

[S29] C：变参函数
来源：http://jl.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ki.wgjwhj.cn

[S30] C：头文件保护
来源：http://iq.chemitech.net.cn

#ifndef X_H
来源：http://uo.bjjhwx.cn

#define X_H
来源：http://tb.lnxyls.cn

#endif
来源：http://bg.szsharing.cn

[S31] C++：Hello World
来源：http://yu.hahajie.cn

#include <iostream>
来源：http://fe.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://rv.chemitech.net.cn

[S32] C++：字符串
来源：http://kp.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://jj.asd995.cn

[S33] C++：vector 增删
来源：http://xk.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sp.nicolike.cn

[S34] C++：遍历 vector
来源：http://mk.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://be.panjiajie.cn

[S35] C++：map
来源：http://cz.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fu.huanxung.cn

[S36] C++：unordered_map
来源：http://zs.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ix.wgjwhj.cn

[S37] C++：set
来源：http://gp.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gd.hahajie.cn

[S38] C++：排序
来源：http://fh.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://kx.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://pd.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://av.shtwfgs.cn

[S40] C++：查找元素
来源：http://kl.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ah.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://yk.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://og.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://bb.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://ik.521024.cn

[S43] C++：智能指针
来源：http://rv.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://yd.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://ck.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://mp.wgjwhj.cn

[S45] C++：lambda
来源：http://fd.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qd.muxihuayi.cn

[S46] C++：函数模板
来源：http://dw.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ko.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://eb.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iu.521024.cn

[S48] C++：逐行读文件
来源：http://sm.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wp.szsharing.cn

while (std::getline(in, line)) { }
来源：http://zb.huixiangedu.cn

[S49] C++：写文件
来源：http://gd.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pw.9csxet.cn

[S50] C++：格式化数字
来源：http://ms.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wf.nicolike.cn

[S51] C++：显式类型转换
来源：http://ya.colortex.cn

static_cast<double>(a) / b
来源：http://rz.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ny.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://iu.bjjhwx.cn

[S53] C++：移动语义
来源：http://kd.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://hm.szsharing.cn

[S54] C++：异常处理
来源：http://th.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sm.nszjky.cn

[S55] C++：结构化绑定
来源：http://nt.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ja.newstarts.cn

[S56] C++：optional
来源：http://kv.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dx.521024.cn

[S57] C++：编译期常量
来源：http://co.bookmarksfly.cn

constexpr int N = 10;
来源：http://lv.bjjhwx.cn

[S58] C++：命名空间
来源：http://tu.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://kl.huanxung.cn

[S59] C++：静态断言
来源：http://sx.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ki.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://ms.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://im.huixiangedu.cn

================================================================================
来源：http://pn.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yq.shxzukj.cn

================================================================================
来源：http://wy.nicolike.cn

[T01] Kotlin：Hello World
来源：http://zr.nicolike.cn

println("Hello")
来源：http://hx.haigaiapp.cn

[T02] Kotlin：变量
来源：http://jx.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mi.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://mf.chemitech.net.cn

"值: $b"
来源：http://kq.gzmigu.cn

[T04] Kotlin：空安全
来源：http://lm.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://iw.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://ik.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jo.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://wt.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xd.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://jn.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zf.szsharing.cn

[T08] Kotlin：数据类
来源：http://eg.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://sr.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://lg.colortex.cn

fun String.exclaim() = this + "!"
来源：http://it.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://ye.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gd.hahajie.cn

[T11] Kotlin：协程
来源：http://wy.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ze.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://bm.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://xm.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://jv.nicolike.cn

val m = mapOf("a" to 1)
来源：http://vv.panjiajie.cn

[T14] Kotlin：循环
来源：http://gj.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://qd.shtwfgs.cn

[T15] Kotlin：接口
来源：http://ys.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://cw.shxzukj.cn

[T16] Swift：Hello World
来源：http://id.shxzskj.cn

print("Hello")
来源：http://ub.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://ul.panjiajie.cn

var a = 1;  let b = 2
来源：http://yh.9csxet.cn

[T18] Swift：字符串插值
来源：http://zf.yuntaijiaju.cn

"值: \(b)"
来源：http://an.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://wa.gzmigu.cn

if let n = opt { print(n) }
来源：http://jm.521024.cn

[T20] Swift：数组操作
来源：http://kw.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fe.chemitech.net.cn

[T21] Swift：遍历
来源：http://yu.9csxet.cn

for x in a { print(x) }
来源：http://hl.lnxyls.cn

[T22] Swift：字典
来源：http://sn.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aw.wgjwhj.cn

[T23] Swift：函数
来源：http://kf.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xh.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://wj.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ou.yuexingan06.cn

[T25] Swift：结构体
来源：http://tg.muxihuayi.cn

struct P { var x: Int }
来源：http://cq.hahajie.cn

[T26] Swift：类与重写
来源：http://za.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://bv.colortex.cn

[T27] Swift：错误处理
来源：http://ir.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://bj.jctech888.com.cn

[T28] Swift：枚举
来源：http://jg.newstarts.cn

enum Color { case red, green }
来源：http://pq.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://yl.gzmigu.cn

guard let x = opt else { return }
来源：http://hg.chemitech.net.cn

[T30] Swift：协议
来源：http://qx.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://xq.9csxet.cn

[T31] Lua：Hello World
来源：http://vu.muxihuayi.cn

print("Hello")
来源：http://bc.panjiajie.cn

[T32] Lua：局部变量
来源：http://st.521024.cn

local a = 1
来源：http://nv.colortex.cn

[T33] Lua：表（数组）
来源：http://bf.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qi.nszjky.cn

[T34] Lua：遍历表
来源：http://nw.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tt.panjiajie.cn

[T35] Lua：字典表
来源：http://yn.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://xg.jctech888.com.cn

[T36] Lua：函数
来源：http://ag.hahajie.cn

function add(a, b) return a + b end
来源：http://hy.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://xc.yuntaijiaju.cn

"a" .. "b"
来源：http://ad.9csxet.cn

[T38] Lua：条件
来源：http://hl.shxzskj.cn

if x > 0 then print("正") end
来源：http://za.shxzskj.cn

[T39] Lua：模式匹配
来源：http://ff.gzmigu.cn

string.find(s, "%d+")
来源：http://fj.asd995.cn

[T40] Lua：元表
来源：http://yi.colortex.cn

setmetatable({}, { __index = base })
来源：http://qf.bookmarksfly.cn


<!-- 参考信息 -->