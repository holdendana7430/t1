代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://es.shxzukj.cn

[R36] 并发执行多个任务
来源：http://sm.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ak.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://wn.szsharing.cn

files=$(ls -1)
来源：http://ya.yuntaijiaju.cn

[R38] 管道串联
来源：http://xx.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://nf.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ct.nszjky.cn

cmd > out.log 2>&1
来源：http://ay.yuntaijiaju.cn

[R40] 追加写日志
来源：http://hx.yuexingan06.cn

echo "log" >> out.log
来源：http://jq.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://gj.9csxet.cn

cmd >/dev/null 2>&1
来源：http://aa.huanxung.cn

[R42] 输入重定向
来源：http://qp.shxzskj.cn

wc -l < a.txt
来源：http://cw.haigaiapp.cn

[R43] 按名字查找文件
来源：http://ca.nicolike.cn

find . -name "*.log" -type f
来源：http://qv.yuexingan06.cn

[R44] 按修改时间查找
来源：http://ya.9csxet.cn

find . -mtime -7 -type f
来源：http://ji.bjjhwx.cn

[R45] 批量删除
来源：http://yq.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://of.9csxet.cn

[R46] 递归替换文件内容
来源：http://ht.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cn.shxzukj.cn

[R47] sed 单行替换
来源：http://zn.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qf.bookmarksfly.cn

[R48] awk 取指定列
来源：http://cq.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://df.hahajie.cn

[R49] awk 带条件
来源：http://xy.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sl.nicolike.cn

[R50] awk 求和
来源：http://ic.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sw.haigaiapp.cn

[R51] 排序去重取前几
来源：http://xu.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rn.lnxyls.cn

[R52] 统计行数
来源：http://zl.9csxet.cn

wc -l a.txt
来源：http://rj.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://me.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ox.muxihuayi.cn

[R54] 比较两个文件
来源：http://fc.jianghongdianzi.cn

diff a.txt b.txt
来源：http://qo.haigaiapp.cn

[R55] 压缩与解压
来源：http://jz.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cx.9csxet.cn

[R56] 远程拷贝
来源：http://so.yuntaijiaju.cn

scp file user@host:/path/
来源：http://mj.bookmarksfly.cn

[R57] 远程执行命令
来源：http://vd.jctech888.com.cn

ssh user@host 'uptime'
来源：http://wr.nszjky.cn

[R58] 下载文件
来源：http://ua.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jb.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://eu.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ew.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://wu.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pj.yuexingan06.cn

[R61] 磁盘占用
来源：http://wk.huanxung.cn

df -h;  du -sh *
来源：http://qc.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://we.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://lq.haigaiapp.cn

[R63] 内存与进程
来源：http://sn.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://et.jianghongdianzi.cn

[R64] 结束进程
来源：http://xk.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://ng.jctech888.com.cn

[R65] 查看端口占用
来源：http://sh.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ts.yuexingan06.cn

[R66] 定时任务
来源：http://zn.szxytkj.cn

crontab -e;  crontab -l
来源：http://fo.9csxet.cn

[R67] 生成随机十六进制串
来源：http://aj.panjiajie.cn

openssl rand -hex 16
来源：http://ib.jctech888.com.cn

[R68] 计算文件校验值
来源：http://ms.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nl.panjiajie.cn

[R69] 生成随机密码
来源：http://gc.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://ye.asd995.cn

[R70] 时间戳与互转
来源：http://mn.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://it.newstarts.cn

[R71] 日期格式化
来源：http://tf.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zu.nicolike.cn

[R72] 等待端口就绪
来源：http://dg.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sm.lnxyls.cn

[R73] 分割大日志
来源：http://az.panjiajie.cn

split -l 1000 big.log part_
来源：http://lw.gzmigu.cn

[R74] 批量重命名
来源：http://eu.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sw.asd995.cn

[R75] 导出环境变量
来源：http://ya.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://yf.wgjwhj.cn

[R76] 使用临时文件
来源：http://qg.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bj.9csxet.cn

[R77] 读取用户输入
来源：http://iq.muxihuayi.cn

read -rp "请输入: " ans
来源：http://va.wgjwhj.cn

[R78] 交互式菜单
来源：http://ot.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vh.shxzukj.cn

[R79] 解析命令行选项
来源：http://yw.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://as.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://yq.panjiajie.cn

time ./run.sh
来源：http://dh.huanxung.cn

================================================================================
来源：http://we.nicolike.cn

S. C / C++ 专题
来源：http://ku.huanxung.cn

================================================================================
来源：http://fx.muxihuayi.cn

[S01] C：Hello World
来源：http://yc.panjiajie.cn

#include <stdio.h>
来源：http://mx.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cq.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://xh.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://oz.huixinmuqiang.cn

[S03] C：读入整数
来源：http://lm.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://ux.haigaiapp.cn

[S04] C：字符串复制
来源：http://do.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sy.haigaiapp.cn

[S05] C：字符串长度
来源：http://hz.jianghongdianzi.cn

strlen(s)
来源：http://at.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://tp.huixiangedu.cn

strcmp(a, b) == 0
来源：http://fd.nszjky.cn

[S07] C：数组遍历求和
来源：http://sd.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eq.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://zf.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lm.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://fy.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zk.chemitech.net.cn

[S10] C：指针与解引用
来源：http://kr.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://bl.colortex.cn

[S11] C：逐行读文件
来源：http://av.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://so.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eg.szxytkj.cn

fclose(f);
来源：http://nb.9csxet.cn

[S12] C：写文件
来源：http://yp.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://so.521024.cn

[S13] C：宏定义
来源：http://rz.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xt.yuntaijiaju.cn

[S14] C：枚举
来源：http://th.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ri.nicolike.cn

[S15] C：类型转换
来源：http://kr.huixiangedu.cn

(double) a / b
来源：http://xu.colortex.cn

[S16] C：位操作置位
来源：http://iw.chemitech.net.cn

x |= (1 << 3);
来源：http://cl.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://re.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://em.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://my.asd995.cn

int main(int argc, char **argv)
来源：http://fs.huanxung.cn

[S19] C：快速排序
来源：http://fb.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ca.gzmigu.cn

[S20] C：二分查找
来源：http://zp.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ok.szxytkj.cn

[S21] C：字符类别判断
来源：http://tm.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mu.hnjuh.cn

[S22] C：字符串转数字
来源：http://ik.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yo.szxytkj.cn

[S23] C：随机数
来源：http://fw.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zf.panjiajie.cn

[S24] C：获取本地时间
来源：http://np.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nl.haigaiapp.cn

[S25] C：内存拷贝
来源：http://cb.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://pb.shxzskj.cn

[S26] C：内存清零
来源：http://si.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://bj.hnjuh.cn

[S27] C：定义常量
来源：http://po.shtwfgs.cn

const double PI = 3.14159;
来源：http://vl.hahajie.cn

[S28] C：静态变量
来源：http://ob.huixinmuqiang.cn

static int counter = 0;
来源：http://mm.huixiangedu.cn

[S29] C：变参函数
来源：http://aq.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mh.huanxung.cn

[S30] C：头文件保护
来源：http://lb.huixiangedu.cn

#ifndef X_H
来源：http://vm.newstarts.cn

#define X_H
来源：http://by.521024.cn

#endif
来源：http://yb.muxihuayi.cn

[S31] C++：Hello World
来源：http://sv.huanxung.cn

#include <iostream>
来源：http://pv.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://xq.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ap.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://hs.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://kd.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ct.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://fp.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ez.yuntaijiaju.cn

[S35] C++：map
来源：http://lg.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cr.asd995.cn

[S36] C++：unordered_map
来源：http://mj.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mo.nicolike.cn

[S37] C++：set
来源：http://hy.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nf.huanxung.cn

[S38] C++：排序
来源：http://ac.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://rp.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://xd.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kj.szxytkj.cn

[S40] C++：查找元素
来源：http://as.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uc.colortex.cn

[S41] C++：类与构造函数
来源：http://lo.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dh.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://sp.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://sv.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://ac.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://hq.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://jm.nszjky.cn

void inc(int &x) { ++x; }
来源：http://xm.yuexingan06.cn

[S45] C++：lambda
来源：http://gl.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rw.bookmarksfly.cn

[S46] C++：函数模板
来源：http://eq.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://np.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://bg.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xy.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://ct.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xt.colortex.cn

while (std::getline(in, line)) { }
来源：http://ke.shtwfgs.cn

[S49] C++：写文件
来源：http://hw.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bf.shtwfgs.cn

[S50] C++：格式化数字
来源：http://po.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rv.szsharing.cn

[S51] C++：显式类型转换
来源：http://oy.haigaiapp.cn

static_cast<double>(a) / b
来源：http://jg.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://ul.szsharing.cn

int size() const noexcept { return n_; }
来源：http://oa.huanxung.cn

[S53] C++：移动语义
来源：http://oa.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://yu.lnxyls.cn

[S54] C++：异常处理
来源：http://hc.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ta.szsharing.cn

[S55] C++：结构化绑定
来源：http://kw.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pp.jctech888.com.cn

[S56] C++：optional
来源：http://gj.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dq.jctech888.com.cn

[S57] C++：编译期常量
来源：http://yt.szsharing.cn

constexpr int N = 10;
来源：http://fi.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://ts.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://dv.szsharing.cn

[S59] C++：静态断言
来源：http://zc.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bj.521024.cn

[S60] C++：遍历并删除元素
来源：http://th.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dt.szxytkj.cn

================================================================================
来源：http://kg.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sa.lnxyls.cn

================================================================================
来源：http://sl.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://cs.wgjwhj.cn

println("Hello")
来源：http://cq.shtwfgs.cn

[T02] Kotlin：变量
来源：http://by.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yw.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://vp.shxzukj.cn

"值: $b"
来源：http://ao.hahajie.cn

[T04] Kotlin：空安全
来源：http://xc.shxzskj.cn

val n: String? = null;  n?.length
来源：http://he.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://gs.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://my.szsharing.cn

[T06] Kotlin：集合映射
来源：http://rh.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ej.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ha.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fy.panjiajie.cn

[T08] Kotlin：数据类
来源：http://ys.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://pq.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://di.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://ae.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://gp.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vz.chemitech.net.cn

[T11] Kotlin：协程
来源：http://lc.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zm.colortex.cn

[T12] Kotlin：解构声明
来源：http://nl.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://zk.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://ax.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://sx.lnxyls.cn

[T14] Kotlin：循环
来源：http://rf.shxzukj.cn

for (i in 1..10) println(i)
来源：http://pj.huixiangedu.cn

[T15] Kotlin：接口
来源：http://vt.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://nl.nicolike.cn

[T16] Swift：Hello World
来源：http://zb.huixinmuqiang.cn

print("Hello")
来源：http://hl.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://uk.wgjwhj.cn

var a = 1;  let b = 2
来源：http://zg.hnjuh.cn

[T18] Swift：字符串插值
来源：http://zt.nicolike.cn

"值: \(b)"
来源：http://kf.shxzukj.cn

[T19] Swift：可选绑定
来源：http://hs.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://lx.newstarts.cn

[T20] Swift：数组操作
来源：http://ms.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xw.huixiangedu.cn

[T21] Swift：遍历
来源：http://dz.nszjky.cn

for x in a { print(x) }
来源：http://jj.szxytkj.cn

[T22] Swift：字典
来源：http://oi.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ki.colortex.cn

[T23] Swift：函数
来源：http://of.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vh.gzmigu.cn

[T24] Swift：闭包
来源：http://pi.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ep.hnjuh.cn

[T25] Swift：结构体
来源：http://lm.nicolike.cn

struct P { var x: Int }
来源：http://me.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://si.szxytkj.cn

class A: Base { override func f() {} }
来源：http://gs.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://pw.asd995.cn

do { try f() } catch { print(error) }
来源：http://bo.hnjuh.cn

[T28] Swift：枚举
来源：http://il.newstarts.cn

enum Color { case red, green }
来源：http://jy.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://sq.hahajie.cn

guard let x = opt else { return }
来源：http://yt.wgjwhj.cn

[T30] Swift：协议
来源：http://py.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://ds.huixiangedu.cn

[T31] Lua：Hello World
来源：http://xm.yuntaijiaju.cn

print("Hello")
来源：http://fr.nszjky.cn

[T32] Lua：局部变量
来源：http://xs.chemitech.net.cn

local a = 1
来源：http://jn.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://tk.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rr.gzmigu.cn

[T34] Lua：遍历表
来源：http://oe.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yx.nicolike.cn

[T35] Lua：字典表
来源：http://tt.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://pk.hnjuh.cn

[T36] Lua：函数
来源：http://qz.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://qo.colortex.cn

[T37] Lua：字符串拼接
来源：http://of.huixinmuqiang.cn

"a" .. "b"
来源：http://we.newstarts.cn

[T38] Lua：条件
来源：http://oi.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://hc.shtwfgs.cn


<!-- 参考信息 -->