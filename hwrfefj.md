代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fp.shxzukj.cn

[R34] 退出时清理
来源：http://yo.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zd.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://uh.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vm.nicolike.cn

[R36] 并发执行多个任务
来源：http://nv.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aw.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://fx.nszjky.cn

files=$(ls -1)
来源：http://ni.huanxung.cn

[R38] 管道串联
来源：http://gv.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://gg.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://xt.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://gx.huixinmuqiang.cn

[R40] 追加写日志
来源：http://yi.hnjuh.cn

echo "log" >> out.log
来源：http://jo.nicolike.cn

[R41] 丢弃输出
来源：http://ly.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://ao.colortex.cn

[R42] 输入重定向
来源：http://rx.lnxyls.cn

wc -l < a.txt
来源：http://qz.chemitech.net.cn

[R43] 按名字查找文件
来源：http://fz.muxihuayi.cn

find . -name "*.log" -type f
来源：http://rl.huixiangedu.cn

[R44] 按修改时间查找
来源：http://lh.hnjuh.cn

find . -mtime -7 -type f
来源：http://qy.newstarts.cn

[R45] 批量删除
来源：http://mx.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://ft.hahajie.cn

[R46] 递归替换文件内容
来源：http://ey.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mg.521024.cn

[R47] sed 单行替换
来源：http://ty.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tu.colortex.cn

[R48] awk 取指定列
来源：http://ts.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://ex.newstarts.cn

[R49] awk 带条件
来源：http://vs.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vz.huixinmuqiang.cn

[R50] awk 求和
来源：http://qg.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xn.lnxyls.cn

[R51] 排序去重取前几
来源：http://ui.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hj.yuntaijiaju.cn

[R52] 统计行数
来源：http://vg.wgjwhj.cn

wc -l a.txt
来源：http://ma.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://ys.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nl.colortex.cn

[R54] 比较两个文件
来源：http://zb.wgjwhj.cn

diff a.txt b.txt
来源：http://xf.haigaiapp.cn

[R55] 压缩与解压
来源：http://wk.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tj.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://cj.hahajie.cn

scp file user@host:/path/
来源：http://vq.panjiajie.cn

[R57] 远程执行命令
来源：http://ts.shtwfgs.cn

ssh user@host 'uptime'
来源：http://nk.haigaiapp.cn

[R58] 下载文件
来源：http://ed.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vh.nszjky.cn

[R59] 发 POST JSON
来源：http://tj.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vt.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://ou.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://or.wgjwhj.cn

[R61] 磁盘占用
来源：http://xa.hahajie.cn

df -h;  du -sh *
来源：http://ll.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://ag.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://ig.panjiajie.cn

[R63] 内存与进程
来源：http://id.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://pk.nszjky.cn

[R64] 结束进程
来源：http://et.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://xp.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://ih.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nj.521024.cn

[R66] 定时任务
来源：http://jb.shxzukj.cn

crontab -e;  crontab -l
来源：http://uz.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://jw.huixinmuqiang.cn

openssl rand -hex 16
来源：http://wv.hnjuh.cn

[R68] 计算文件校验值
来源：http://ln.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hh.gzmigu.cn

[R69] 生成随机密码
来源：http://kg.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://af.szsharing.cn

[R70] 时间戳与互转
来源：http://xe.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://bz.jctech888.com.cn

[R71] 日期格式化
来源：http://sb.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yg.panjiajie.cn

[R72] 等待端口就绪
来源：http://ho.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qp.9csxet.cn

[R73] 分割大日志
来源：http://yb.huanxung.cn

split -l 1000 big.log part_
来源：http://ka.szsharing.cn

[R74] 批量重命名
来源：http://dt.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rt.asd995.cn

[R75] 导出环境变量
来源：http://ke.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://wv.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://bh.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://it.newstarts.cn

[R77] 读取用户输入
来源：http://oe.huixiangedu.cn

read -rp "请输入: " ans
来源：http://db.szxytkj.cn

[R78] 交互式菜单
来源：http://pe.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zi.szxytkj.cn

[R79] 解析命令行选项
来源：http://vs.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aj.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://hr.9csxet.cn

time ./run.sh
来源：http://qn.lnxyls.cn

================================================================================
来源：http://bv.jctech888.com.cn

S. C / C++ 专题
来源：http://ej.yuexingan06.cn

================================================================================
来源：http://es.hnjuh.cn

[S01] C：Hello World
来源：http://wr.newstarts.cn

#include <stdio.h>
来源：http://pb.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nm.521024.cn

[S02] C：变量与格式化输出
来源：http://en.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://fd.wgjwhj.cn

[S03] C：读入整数
来源：http://eu.lnxyls.cn

int x; scanf("%d", &x);
来源：http://fy.bookmarksfly.cn

[S04] C：字符串复制
来源：http://bn.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://st.muxihuayi.cn

[S05] C：字符串长度
来源：http://qv.colortex.cn

strlen(s)
来源：http://de.shxzukj.cn

[S06] C：字符串比较
来源：http://kf.hnjuh.cn

strcmp(a, b) == 0
来源：http://mb.lnxyls.cn

[S07] C：数组遍历求和
来源：http://jp.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eb.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://hl.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ic.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://fy.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xu.yuexingan06.cn

[S10] C：指针与解引用
来源：http://zi.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://ti.521024.cn

[S11] C：逐行读文件
来源：http://ix.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://zd.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qi.asd995.cn

fclose(f);
来源：http://of.newstarts.cn

[S12] C：写文件
来源：http://kg.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xm.colortex.cn

[S13] C：宏定义
来源：http://nt.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ed.9csxet.cn

[S14] C：枚举
来源：http://vm.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://yg.haigaiapp.cn

[S15] C：类型转换
来源：http://wn.huixiangedu.cn

(double) a / b
来源：http://wd.lnxyls.cn

[S16] C：位操作置位
来源：http://ft.nicolike.cn

x |= (1 << 3);
来源：http://qy.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://mq.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iq.asd995.cn

[S18] C：命令行参数
来源：http://gx.bjjhwx.cn

int main(int argc, char **argv)
来源：http://di.521024.cn

[S19] C：快速排序
来源：http://mn.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mv.muxihuayi.cn

[S20] C：二分查找
来源：http://px.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iq.newstarts.cn

[S21] C：字符类别判断
来源：http://ll.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cm.newstarts.cn

[S22] C：字符串转数字
来源：http://fd.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kw.bookmarksfly.cn

[S23] C：随机数
来源：http://fe.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zl.jctech888.com.cn

[S24] C：获取本地时间
来源：http://vm.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jp.9csxet.cn

[S25] C：内存拷贝
来源：http://sv.nszjky.cn

memcpy(dst, src, n);
来源：http://ok.colortex.cn

[S26] C：内存清零
来源：http://za.newstarts.cn

memset(a, 0, sizeof a);
来源：http://ky.jctech888.com.cn

[S27] C：定义常量
来源：http://jc.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://iz.bjjhwx.cn

[S28] C：静态变量
来源：http://cv.521024.cn

static int counter = 0;
来源：http://qb.szxytkj.cn

[S29] C：变参函数
来源：http://qw.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zq.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://se.newstarts.cn

#ifndef X_H
来源：http://he.bookmarksfly.cn

#define X_H
来源：http://pt.huanxung.cn

#endif
来源：http://rt.szsharing.cn

[S31] C++：Hello World
来源：http://sz.lnxyls.cn

#include <iostream>
来源：http://mb.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://jg.huixiangedu.cn

[S32] C++：字符串
来源：http://nx.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://dp.newstarts.cn

[S33] C++：vector 增删
来源：http://ta.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tg.shxzukj.cn

[S34] C++：遍历 vector
来源：http://zv.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://go.shxzskj.cn

[S35] C++：map
来源：http://ns.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ij.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://yu.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://di.jctech888.com.cn

[S37] C++：set
来源：http://jr.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tr.9csxet.cn

[S38] C++：排序
来源：http://qc.colortex.cn

std::sort(v.begin(), v.end());
来源：http://ly.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://pd.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://el.nicolike.cn

[S40] C++：查找元素
来源：http://el.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xj.shxzskj.cn

[S41] C++：类与构造函数
来源：http://ct.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dc.521024.cn

[S42] C++：继承与虚函数
来源：http://si.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://tw.521024.cn

[S43] C++：智能指针
来源：http://ve.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ad.shxzskj.cn

[S44] C++：引用传参
来源：http://ww.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://hh.wgjwhj.cn

[S45] C++：lambda
来源：http://of.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vw.bookmarksfly.cn

[S46] C++：函数模板
来源：http://xo.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fr.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://mo.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ib.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://qn.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qd.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://ag.lnxyls.cn

[S49] C++：写文件
来源：http://jx.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sf.newstarts.cn

[S50] C++：格式化数字
来源：http://nm.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ug.szxytkj.cn

[S51] C++：显式类型转换
来源：http://zm.hahajie.cn

static_cast<double>(a) / b
来源：http://rq.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://au.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://lk.szxytkj.cn

[S53] C++：移动语义
来源：http://sd.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://av.nicolike.cn

[S54] C++：异常处理
来源：http://pn.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://er.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://jp.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fp.muxihuayi.cn

[S56] C++：optional
来源：http://rd.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ju.hahajie.cn

[S57] C++：编译期常量
来源：http://ez.shtwfgs.cn

constexpr int N = 10;
来源：http://mv.521024.cn

[S58] C++：命名空间
来源：http://zm.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://iw.9csxet.cn

[S59] C++：静态断言
来源：http://uf.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ve.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://ux.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lm.yuexingan06.cn

================================================================================
来源：http://ml.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ro.jctech888.com.cn

================================================================================
来源：http://kb.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://aj.9csxet.cn

println("Hello")
来源：http://jb.wgjwhj.cn

[T02] Kotlin：变量
来源：http://dr.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://af.521024.cn

[T03] Kotlin：字符串模板
来源：http://rg.yuexingan06.cn

"值: $b"
来源：http://hd.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://qo.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://mp.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://dl.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zl.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://hn.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xd.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://qc.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ir.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ls.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://fs.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://gx.asd995.cn

fun String.exclaim() = this + "!"
来源：http://ko.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://dc.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://he.hahajie.cn

[T11] Kotlin：协程
来源：http://gw.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dx.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://js.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://fj.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://ty.asd995.cn

val m = mapOf("a" to 1)
来源：http://ip.nszjky.cn

[T14] Kotlin：循环
来源：http://kh.9csxet.cn

for (i in 1..10) println(i)
来源：http://ww.hahajie.cn

[T15] Kotlin：接口
来源：http://uw.hahajie.cn

interface Shape { fun area(): Double }
来源：http://lv.nicolike.cn

[T16] Swift：Hello World
来源：http://wh.muxihuayi.cn

print("Hello")
来源：http://qv.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://vw.szsharing.cn

var a = 1;  let b = 2
来源：http://vl.asd995.cn

[T18] Swift：字符串插值
来源：http://dd.gzmigu.cn

"值: \(b)"
来源：http://st.lnxyls.cn

[T19] Swift：可选绑定
来源：http://zq.huanxung.cn

if let n = opt { print(n) }
来源：http://ho.nszjky.cn

[T20] Swift：数组操作
来源：http://gy.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gk.chemitech.net.cn

[T21] Swift：遍历
来源：http://xq.shxzukj.cn

for x in a { print(x) }
来源：http://ox.haigaiapp.cn

[T22] Swift：字典
来源：http://so.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zh.chemitech.net.cn

[T23] Swift：函数
来源：http://vz.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nw.colortex.cn

[T24] Swift：闭包
来源：http://ah.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cy.chemitech.net.cn

[T25] Swift：结构体
来源：http://gd.nszjky.cn

struct P { var x: Int }
来源：http://bq.huanxung.cn

[T26] Swift：类与重写
来源：http://kx.lnxyls.cn

class A: Base { override func f() {} }
来源：http://kp.chemitech.net.cn

[T27] Swift：错误处理
来源：http://jn.521024.cn

do { try f() } catch { print(error) }
来源：http://tg.colortex.cn

[T28] Swift：枚举
来源：http://ns.hahajie.cn

enum Color { case red, green }
来源：http://fc.521024.cn

[T29] Swift：guard 提前返回
来源：http://af.nszjky.cn

guard let x = opt else { return }
来源：http://eq.shxzskj.cn

[T30] Swift：协议
来源：http://gq.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://bx.shxzskj.cn

[T31] Lua：Hello World
来源：http://mn.hnjuh.cn

print("Hello")
来源：http://ht.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://kc.521024.cn

local a = 1
来源：http://kl.shxzskj.cn

[T33] Lua：表（数组）
来源：http://jn.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://op.yuexingan06.cn

[T34] Lua：遍历表
来源：http://bz.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rz.shtwfgs.cn

[T35] Lua：字典表
来源：http://fc.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://od.hahajie.cn

[T36] Lua：函数
来源：http://nx.huanxung.cn

function add(a, b) return a + b end
来源：http://ek.bjjhwx.cn


<!-- 参考信息 -->