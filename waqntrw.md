代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ib.asd995.cn

[R34] 退出时清理
来源：http://yx.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wv.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://hi.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mv.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://mo.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tb.huanxung.cn

[R37] 把输出赋给变量
来源：http://uw.colortex.cn

files=$(ls -1)
来源：http://ic.9csxet.cn

[R38] 管道串联
来源：http://mn.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://fm.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://yo.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://vy.gzmigu.cn

[R40] 追加写日志
来源：http://kf.bookmarksfly.cn

echo "log" >> out.log
来源：http://rj.nicolike.cn

[R41] 丢弃输出
来源：http://kj.asd995.cn

cmd >/dev/null 2>&1
来源：http://lg.yuntaijiaju.cn

[R42] 输入重定向
来源：http://lb.haigaiapp.cn

wc -l < a.txt
来源：http://iw.9csxet.cn

[R43] 按名字查找文件
来源：http://lj.521024.cn

find . -name "*.log" -type f
来源：http://sh.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://hh.huixiangedu.cn

find . -mtime -7 -type f
来源：http://vx.haigaiapp.cn

[R45] 批量删除
来源：http://bd.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://lf.nicolike.cn

[R46] 递归替换文件内容
来源：http://ei.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pd.huixiangedu.cn

[R47] sed 单行替换
来源：http://ee.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cz.newstarts.cn

[R48] awk 取指定列
来源：http://kp.521024.cn

awk '{print $1, $3}' a.txt
来源：http://ct.colortex.cn

[R49] awk 带条件
来源：http://ih.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qh.szsharing.cn

[R50] awk 求和
来源：http://el.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fm.gzmigu.cn

[R51] 排序去重取前几
来源：http://yt.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wk.lnxyls.cn

[R52] 统计行数
来源：http://bz.yuntaijiaju.cn

wc -l a.txt
来源：http://vj.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://jt.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://am.szxytkj.cn

[R54] 比较两个文件
来源：http://cv.szsharing.cn

diff a.txt b.txt
来源：http://zl.nszjky.cn

[R55] 压缩与解压
来源：http://tq.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wl.haigaiapp.cn

[R56] 远程拷贝
来源：http://uz.shtwfgs.cn

scp file user@host:/path/
来源：http://rh.nicolike.cn

[R57] 远程执行命令
来源：http://wl.panjiajie.cn

ssh user@host 'uptime'
来源：http://lq.9csxet.cn

[R58] 下载文件
来源：http://og.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ek.szsharing.cn

[R59] 发 POST JSON
来源：http://eb.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uo.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://sb.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hw.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://cl.shxzukj.cn

df -h;  du -sh *
来源：http://ga.hnjuh.cn

[R62] 找最占空间的文件
来源：http://de.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://ck.shxzukj.cn

[R63] 内存与进程
来源：http://dc.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://mw.colortex.cn

[R64] 结束进程
来源：http://am.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://mk.gzmigu.cn

[R65] 查看端口占用
来源：http://fl.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wj.nszjky.cn

[R66] 定时任务
来源：http://eb.asd995.cn

crontab -e;  crontab -l
来源：http://tv.521024.cn

[R67] 生成随机十六进制串
来源：http://bn.panjiajie.cn

openssl rand -hex 16
来源：http://fh.shtwfgs.cn

[R68] 计算文件校验值
来源：http://eu.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cr.hnjuh.cn

[R69] 生成随机密码
来源：http://zd.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://kw.huanxung.cn

[R70] 时间戳与互转
来源：http://tg.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://kn.huixiangedu.cn

[R71] 日期格式化
来源：http://jg.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://di.shtwfgs.cn

[R72] 等待端口就绪
来源：http://jq.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nt.lnxyls.cn

[R73] 分割大日志
来源：http://sc.shxzskj.cn

split -l 1000 big.log part_
来源：http://sw.panjiajie.cn

[R74] 批量重命名
来源：http://eb.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ki.9csxet.cn

[R75] 导出环境变量
来源：http://js.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://dj.panjiajie.cn

[R76] 使用临时文件
来源：http://wn.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://la.yuexingan06.cn

[R77] 读取用户输入
来源：http://ia.yuexingan06.cn

read -rp "请输入: " ans
来源：http://au.nszjky.cn

[R78] 交互式菜单
来源：http://mi.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wu.hahajie.cn

[R79] 解析命令行选项
来源：http://bv.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wo.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://kt.nicolike.cn

time ./run.sh
来源：http://wn.bookmarksfly.cn

================================================================================
来源：http://qz.muxihuayi.cn

S. C / C++ 专题
来源：http://aw.hnjuh.cn

================================================================================
来源：http://st.chemitech.net.cn

[S01] C：Hello World
来源：http://bt.newstarts.cn

#include <stdio.h>
来源：http://ez.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xg.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://el.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://jg.huixinmuqiang.cn

[S03] C：读入整数
来源：http://gq.szxytkj.cn

int x; scanf("%d", &x);
来源：http://mk.bjjhwx.cn

[S04] C：字符串复制
来源：http://vm.panjiajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hc.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://hn.nszjky.cn

strlen(s)
来源：http://uh.newstarts.cn

[S06] C：字符串比较
来源：http://ui.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://xb.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://qo.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sz.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://tr.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lu.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://jm.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ju.newstarts.cn

[S10] C：指针与解引用
来源：http://wd.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://xa.521024.cn

[S11] C：逐行读文件
来源：http://mj.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://fq.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zm.colortex.cn

fclose(f);
来源：http://qf.huixinmuqiang.cn

[S12] C：写文件
来源：http://fr.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://se.chemitech.net.cn

[S13] C：宏定义
来源：http://ah.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hh.gzmigu.cn

[S14] C：枚举
来源：http://wu.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://bb.bookmarksfly.cn

[S15] C：类型转换
来源：http://or.haigaiapp.cn

(double) a / b
来源：http://yf.muxihuayi.cn

[S16] C：位操作置位
来源：http://ra.huixinmuqiang.cn

x |= (1 << 3);
来源：http://pr.huanxung.cn

[S17] C：安全拼接字符串
来源：http://yt.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mj.haigaiapp.cn

[S18] C：命令行参数
来源：http://ni.huanxung.cn

int main(int argc, char **argv)
来源：http://bd.jctech888.com.cn

[S19] C：快速排序
来源：http://pf.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gh.yuntaijiaju.cn

[S20] C：二分查找
来源：http://cm.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dv.asd995.cn

[S21] C：字符类别判断
来源：http://yz.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fo.szsharing.cn

[S22] C：字符串转数字
来源：http://jr.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ag.jctech888.com.cn

[S23] C：随机数
来源：http://jn.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zs.asd995.cn

[S24] C：获取本地时间
来源：http://pj.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://un.asd995.cn

[S25] C：内存拷贝
来源：http://hi.gzmigu.cn

memcpy(dst, src, n);
来源：http://rj.newstarts.cn

[S26] C：内存清零
来源：http://vs.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://ei.521024.cn

[S27] C：定义常量
来源：http://mz.shxzskj.cn

const double PI = 3.14159;
来源：http://od.panjiajie.cn

[S28] C：静态变量
来源：http://zk.colortex.cn

static int counter = 0;
来源：http://dt.bjjhwx.cn

[S29] C：变参函数
来源：http://tg.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yy.panjiajie.cn

[S30] C：头文件保护
来源：http://jr.bjjhwx.cn

#ifndef X_H
来源：http://je.shtwfgs.cn

#define X_H
来源：http://vb.521024.cn

#endif
来源：http://ej.huanxung.cn

[S31] C++：Hello World
来源：http://cr.nszjky.cn

#include <iostream>
来源：http://bf.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://rf.huixinmuqiang.cn

[S32] C++：字符串
来源：http://rh.hahajie.cn

std::string s = "hi";  s += "!";
来源：http://jg.shtwfgs.cn

[S33] C++：vector 增删
来源：http://jb.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ml.521024.cn

[S34] C++：遍历 vector
来源：http://ha.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://xk.shxzskj.cn

[S35] C++：map
来源：http://sz.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qd.huixiangedu.cn

[S36] C++：unordered_map
来源：http://qj.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ta.nszjky.cn

[S37] C++：set
来源：http://zc.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pg.szsharing.cn

[S38] C++：排序
来源：http://zp.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://aq.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://oh.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ju.hahajie.cn

[S40] C++：查找元素
来源：http://wb.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kv.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://ol.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mn.nszjky.cn

[S42] C++：继承与虚函数
来源：http://eu.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://wj.shxzukj.cn

[S43] C++：智能指针
来源：http://xw.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://vf.521024.cn

[S44] C++：引用传参
来源：http://cq.newstarts.cn

void inc(int &x) { ++x; }
来源：http://me.wgjwhj.cn

[S45] C++：lambda
来源：http://pn.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wc.nicolike.cn

[S46] C++：函数模板
来源：http://fu.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rv.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://zm.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nj.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://tz.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ds.szsharing.cn

while (std::getline(in, line)) { }
来源：http://ra.huanxung.cn

[S49] C++：写文件
来源：http://mq.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pg.haigaiapp.cn

[S50] C++：格式化数字
来源：http://ft.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nc.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://uk.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://od.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://zx.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://zb.bookmarksfly.cn

[S53] C++：移动语义
来源：http://dl.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://bh.shxzukj.cn

[S54] C++：异常处理
来源：http://go.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://et.521024.cn

[S55] C++：结构化绑定
来源：http://gx.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qc.hnjuh.cn

[S56] C++：optional
来源：http://kx.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uc.bjjhwx.cn

[S57] C++：编译期常量
来源：http://xx.shxzukj.cn

constexpr int N = 10;
来源：http://hy.hnjuh.cn

[S58] C++：命名空间
来源：http://vx.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://qp.hnjuh.cn

[S59] C++：静态断言
来源：http://kh.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oz.asd995.cn

[S60] C++：遍历并删除元素
来源：http://pq.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bb.jctech888.com.cn

================================================================================
来源：http://lx.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fc.haigaiapp.cn

================================================================================
来源：http://hk.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://wm.colortex.cn

println("Hello")
来源：http://na.shtwfgs.cn

[T02] Kotlin：变量
来源：http://yr.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ue.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://vi.shxzukj.cn

"值: $b"
来源：http://rf.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://rc.hnjuh.cn

val n: String? = null;  n?.length
来源：http://ps.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://pl.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ti.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://cv.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://es.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://lw.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fc.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://jd.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://ld.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://jk.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://hx.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://so.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iu.wgjwhj.cn

[T11] Kotlin：协程
来源：http://gp.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lj.colortex.cn

[T12] Kotlin：解构声明
来源：http://nf.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://of.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://kl.newstarts.cn

val m = mapOf("a" to 1)
来源：http://et.muxihuayi.cn

[T14] Kotlin：循环
来源：http://mt.nszjky.cn

for (i in 1..10) println(i)
来源：http://ny.chemitech.net.cn

[T15] Kotlin：接口
来源：http://hl.nicolike.cn

interface Shape { fun area(): Double }
来源：http://ds.shtwfgs.cn

[T16] Swift：Hello World
来源：http://ci.chemitech.net.cn

print("Hello")
来源：http://fr.colortex.cn

[T17] Swift：变量与常量
来源：http://xd.haigaiapp.cn

var a = 1;  let b = 2
来源：http://lf.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://cb.9csxet.cn

"值: \(b)"
来源：http://ob.hnjuh.cn

[T19] Swift：可选绑定
来源：http://ge.huixiangedu.cn

if let n = opt { print(n) }
来源：http://tu.shtwfgs.cn

[T20] Swift：数组操作
来源：http://si.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zb.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://rm.hnjuh.cn

for x in a { print(x) }
来源：http://lj.huixiangedu.cn

[T22] Swift：字典
来源：http://sr.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xi.shxzukj.cn

[T23] Swift：函数
来源：http://ri.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qz.asd995.cn

[T24] Swift：闭包
来源：http://qd.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zz.huanxung.cn

[T25] Swift：结构体
来源：http://mr.bjjhwx.cn

struct P { var x: Int }
来源：http://on.wgjwhj.cn

[T26] Swift：类与重写
来源：http://uj.huanxung.cn

class A: Base { override func f() {} }
来源：http://tn.521024.cn

[T27] Swift：错误处理
来源：http://lc.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://zw.haigaiapp.cn

[T28] Swift：枚举
来源：http://jq.nicolike.cn

enum Color { case red, green }
来源：http://lo.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://zs.asd995.cn

guard let x = opt else { return }
来源：http://mu.hahajie.cn

[T30] Swift：协议
来源：http://dp.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://af.asd995.cn

[T31] Lua：Hello World
来源：http://mi.colortex.cn

print("Hello")
来源：http://lt.haigaiapp.cn

[T32] Lua：局部变量
来源：http://jt.shtwfgs.cn

local a = 1
来源：http://qd.nszjky.cn

[T33] Lua：表（数组）
来源：http://im.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ip.szxytkj.cn

[T34] Lua：遍历表
来源：http://td.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ma.wgjwhj.cn

[T35] Lua：字典表
来源：http://kp.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://er.shxzukj.cn

[T36] Lua：函数
来源：http://wf.lnxyls.cn

function add(a, b) return a + b end
来源：http://ys.szxytkj.cn


<!-- 参考信息 -->