代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ms.lnxyls.cn

[R34] 退出时清理
来源：http://fy.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fv.hnjuh.cn

[R35] 后台执行并等待
来源：http://gw.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://go.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://oo.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nz.lnxyls.cn

[R37] 把输出赋给变量
来源：http://gx.521024.cn

files=$(ls -1)
来源：http://vt.bjjhwx.cn

[R38] 管道串联
来源：http://us.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://qf.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://zt.shxzukj.cn

cmd > out.log 2>&1
来源：http://wk.gzmigu.cn

[R40] 追加写日志
来源：http://wu.bjjhwx.cn

echo "log" >> out.log
来源：http://bt.bookmarksfly.cn

[R41] 丢弃输出
来源：http://ue.521024.cn

cmd >/dev/null 2>&1
来源：http://hq.muxihuayi.cn

[R42] 输入重定向
来源：http://of.colortex.cn

wc -l < a.txt
来源：http://oe.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://nb.shxzskj.cn

find . -name "*.log" -type f
来源：http://tw.chemitech.net.cn

[R44] 按修改时间查找
来源：http://xt.shxzukj.cn

find . -mtime -7 -type f
来源：http://uy.hahajie.cn

[R45] 批量删除
来源：http://ty.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://qa.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://bo.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://na.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://eg.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xi.huixiangedu.cn

[R48] awk 取指定列
来源：http://eh.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://vc.wgjwhj.cn

[R49] awk 带条件
来源：http://xw.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yd.huanxung.cn

[R50] awk 求和
来源：http://vc.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://op.yuexingan06.cn

[R51] 排序去重取前几
来源：http://mj.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mk.newstarts.cn

[R52] 统计行数
来源：http://ta.szxytkj.cn

wc -l a.txt
来源：http://kh.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://sa.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vc.huixiangedu.cn

[R54] 比较两个文件
来源：http://qh.hnjuh.cn

diff a.txt b.txt
来源：http://on.huanxung.cn

[R55] 压缩与解压
来源：http://cv.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bo.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ee.bookmarksfly.cn

scp file user@host:/path/
来源：http://ch.huixiangedu.cn

[R57] 远程执行命令
来源：http://df.haigaiapp.cn

ssh user@host 'uptime'
来源：http://gb.huanxung.cn

[R58] 下载文件
来源：http://yw.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sp.muxihuayi.cn

[R59] 发 POST JSON
来源：http://vb.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fq.521024.cn

[R60] 只看 HTTP 状态码
来源：http://af.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ro.szsharing.cn

[R61] 磁盘占用
来源：http://pe.jctech888.com.cn

df -h;  du -sh *
来源：http://of.colortex.cn

[R62] 找最占空间的文件
来源：http://zq.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://lz.9csxet.cn

[R63] 内存与进程
来源：http://so.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://cj.nszjky.cn

[R64] 结束进程
来源：http://sy.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://kz.szxytkj.cn

[R65] 查看端口占用
来源：http://ky.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gt.huixiangedu.cn

[R66] 定时任务
来源：http://by.colortex.cn

crontab -e;  crontab -l
来源：http://pv.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://qe.gzmigu.cn

openssl rand -hex 16
来源：http://ei.gzmigu.cn

[R68] 计算文件校验值
来源：http://qe.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aq.hahajie.cn

[R69] 生成随机密码
来源：http://ab.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://ke.wgjwhj.cn

[R70] 时间戳与互转
来源：http://yg.newstarts.cn

date +%s;  date -d @1700000000
来源：http://tx.wgjwhj.cn

[R71] 日期格式化
来源：http://wt.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ja.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://is.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kg.gzmigu.cn

[R73] 分割大日志
来源：http://fu.huanxung.cn

split -l 1000 big.log part_
来源：http://rc.hnjuh.cn

[R74] 批量重命名
来源：http://bj.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mm.nszjky.cn

[R75] 导出环境变量
来源：http://qd.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://zq.colortex.cn

[R76] 使用临时文件
来源：http://fx.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ll.newstarts.cn

[R77] 读取用户输入
来源：http://ug.hnjuh.cn

read -rp "请输入: " ans
来源：http://dr.szsharing.cn

[R78] 交互式菜单
来源：http://gn.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pe.szsharing.cn

[R79] 解析命令行选项
来源：http://ur.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ju.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://ll.9csxet.cn

time ./run.sh
来源：http://cj.szsharing.cn

================================================================================
来源：http://nz.szsharing.cn

S. C / C++ 专题
来源：http://ge.huanxung.cn

================================================================================
来源：http://iv.bjjhwx.cn

[S01] C：Hello World
来源：http://iu.asd995.cn

#include <stdio.h>
来源：http://ga.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://em.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://vy.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://lp.nszjky.cn

[S03] C：读入整数
来源：http://rs.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://se.hahajie.cn

[S04] C：字符串复制
来源：http://bl.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://aw.asd995.cn

[S05] C：字符串长度
来源：http://ej.huixiangedu.cn

strlen(s)
来源：http://kj.jctech888.com.cn

[S06] C：字符串比较
来源：http://jy.bjjhwx.cn

strcmp(a, b) == 0
来源：http://wc.9csxet.cn

[S07] C：数组遍历求和
来源：http://sj.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dk.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://cf.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mb.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://xw.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mg.szxytkj.cn

[S10] C：指针与解引用
来源：http://sp.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://en.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://qv.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://kd.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ye.bjjhwx.cn

fclose(f);
来源：http://wf.shxzskj.cn

[S12] C：写文件
来源：http://ac.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sw.huixiangedu.cn

[S13] C：宏定义
来源：http://wi.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zu.yuexingan06.cn

[S14] C：枚举
来源：http://oi.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://to.shxzskj.cn

[S15] C：类型转换
来源：http://ts.nicolike.cn

(double) a / b
来源：http://bu.jctech888.com.cn

[S16] C：位操作置位
来源：http://im.newstarts.cn

x |= (1 << 3);
来源：http://bk.nicolike.cn

[S17] C：安全拼接字符串
来源：http://nh.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xr.wgjwhj.cn

[S18] C：命令行参数
来源：http://pw.wgjwhj.cn

int main(int argc, char **argv)
来源：http://uo.newstarts.cn

[S19] C：快速排序
来源：http://xr.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pt.yuntaijiaju.cn

[S20] C：二分查找
来源：http://mt.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ie.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://fw.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zs.shxzskj.cn

[S22] C：字符串转数字
来源：http://cc.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rg.yuexingan06.cn

[S23] C：随机数
来源：http://jq.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vb.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://lx.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fx.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://rn.colortex.cn

memcpy(dst, src, n);
来源：http://qq.newstarts.cn

[S26] C：内存清零
来源：http://yk.521024.cn

memset(a, 0, sizeof a);
来源：http://ss.gzmigu.cn

[S27] C：定义常量
来源：http://vh.nszjky.cn

const double PI = 3.14159;
来源：http://we.huixiangedu.cn

[S28] C：静态变量
来源：http://rf.asd995.cn

static int counter = 0;
来源：http://cv.shtwfgs.cn

[S29] C：变参函数
来源：http://br.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ww.huanxung.cn

[S30] C：头文件保护
来源：http://ub.shxzukj.cn

#ifndef X_H
来源：http://iz.huixiangedu.cn

#define X_H
来源：http://dw.wgjwhj.cn

#endif
来源：http://nr.jctech888.com.cn

[S31] C++：Hello World
来源：http://ac.colortex.cn

#include <iostream>
来源：http://tu.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://wa.huanxung.cn

[S32] C++：字符串
来源：http://up.colortex.cn

std::string s = "hi";  s += "!";
来源：http://xu.szsharing.cn

[S33] C++：vector 增删
来源：http://wb.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qm.huanxung.cn

[S34] C++：遍历 vector
来源：http://sg.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wo.newstarts.cn

[S35] C++：map
来源：http://ev.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oo.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://mv.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zb.yuntaijiaju.cn

[S37] C++：set
来源：http://hh.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iw.haigaiapp.cn

[S38] C++：排序
来源：http://ct.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://vr.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://vm.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qj.szxytkj.cn

[S40] C++：查找元素
来源：http://zi.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cd.asd995.cn

[S41] C++：类与构造函数
来源：http://vi.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rb.newstarts.cn

[S42] C++：继承与虚函数
来源：http://ji.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://qe.szxytkj.cn

[S43] C++：智能指针
来源：http://ka.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://ud.jctech888.com.cn

[S44] C++：引用传参
来源：http://qk.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://fi.9csxet.cn

[S45] C++：lambda
来源：http://jd.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vi.colortex.cn

[S46] C++：函数模板
来源：http://gw.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zp.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://pk.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ga.newstarts.cn

[S48] C++：逐行读文件
来源：http://pv.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yy.521024.cn

while (std::getline(in, line)) { }
来源：http://mm.hahajie.cn

[S49] C++：写文件
来源：http://kq.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ju.haigaiapp.cn

[S50] C++：格式化数字
来源：http://wa.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://so.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://tm.nicolike.cn

static_cast<double>(a) / b
来源：http://oo.colortex.cn

[S52] C++：const 与 noexcept
来源：http://lc.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://nx.hnjuh.cn

[S53] C++：移动语义
来源：http://hc.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://ep.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://zx.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vw.9csxet.cn

[S55] C++：结构化绑定
来源：http://um.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hh.bookmarksfly.cn

[S56] C++：optional
来源：http://cp.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ql.hnjuh.cn

[S57] C++：编译期常量
来源：http://zc.nicolike.cn

constexpr int N = 10;
来源：http://ga.huanxung.cn

[S58] C++：命名空间
来源：http://yf.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://rq.chemitech.net.cn

[S59] C++：静态断言
来源：http://pv.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://do.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://ur.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xx.hnjuh.cn

================================================================================
来源：http://im.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rk.jianghongdianzi.cn

================================================================================
来源：http://td.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://tz.shxzukj.cn

println("Hello")
来源：http://gc.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://bo.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lb.colortex.cn

[T03] Kotlin：字符串模板
来源：http://hd.nszjky.cn

"值: $b"
来源：http://og.huanxung.cn

[T04] Kotlin：空安全
来源：http://pl.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://zf.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://lw.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sk.newstarts.cn

[T06] Kotlin：集合映射
来源：http://tj.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mn.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://ln.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ld.lnxyls.cn

[T08] Kotlin：数据类
来源：http://dt.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://ty.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://xs.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://ob.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://pn.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://er.lnxyls.cn

[T11] Kotlin：协程
来源：http://wo.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hi.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://ac.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://mv.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://ng.521024.cn

val m = mapOf("a" to 1)
来源：http://vc.szsharing.cn

[T14] Kotlin：循环
来源：http://ur.9csxet.cn

for (i in 1..10) println(i)
来源：http://xn.lnxyls.cn

[T15] Kotlin：接口
来源：http://mk.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://ed.huixiangedu.cn

[T16] Swift：Hello World
来源：http://tl.haigaiapp.cn

print("Hello")
来源：http://ve.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://jz.hahajie.cn

var a = 1;  let b = 2
来源：http://qc.521024.cn

[T18] Swift：字符串插值
来源：http://hk.bookmarksfly.cn

"值: \(b)"
来源：http://qg.shxzukj.cn

[T19] Swift：可选绑定
来源：http://gq.bjjhwx.cn

if let n = opt { print(n) }
来源：http://gr.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://ua.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ag.wgjwhj.cn

[T21] Swift：遍历
来源：http://ow.hnjuh.cn

for x in a { print(x) }
来源：http://dx.hnjuh.cn

[T22] Swift：字典
来源：http://oh.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cr.hahajie.cn

[T23] Swift：函数
来源：http://aa.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yg.lnxyls.cn

[T24] Swift：闭包
来源：http://ai.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eu.hnjuh.cn

[T25] Swift：结构体
来源：http://ja.bookmarksfly.cn

struct P { var x: Int }
来源：http://zo.huixiangedu.cn

[T26] Swift：类与重写
来源：http://te.9csxet.cn

class A: Base { override func f() {} }
来源：http://aq.newstarts.cn

[T27] Swift：错误处理
来源：http://zg.nszjky.cn

do { try f() } catch { print(error) }
来源：http://gl.szsharing.cn

[T28] Swift：枚举
来源：http://ox.9csxet.cn

enum Color { case red, green }
来源：http://mc.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://pt.hnjuh.cn

guard let x = opt else { return }
来源：http://dv.chemitech.net.cn

[T30] Swift：协议
来源：http://th.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://jl.newstarts.cn

[T31] Lua：Hello World
来源：http://zm.huanxung.cn

print("Hello")
来源：http://ns.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://lg.9csxet.cn

local a = 1
来源：http://fz.gzmigu.cn

[T33] Lua：表（数组）
来源：http://it.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sl.jctech888.com.cn

[T34] Lua：遍历表
来源：http://md.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dx.wgjwhj.cn

[T35] Lua：字典表
来源：http://jv.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://jq.yuexingan06.cn

[T36] Lua：函数
来源：http://kc.haigaiapp.cn

function add(a, b) return a + b end
来源：http://fx.shtwfgs.cn


<!-- 参考信息 -->