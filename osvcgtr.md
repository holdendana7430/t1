代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://ad.jctech888.com.cn

[R32] 参数个数校验
来源：http://rq.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eb.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://fr.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ph.muxihuayi.cn

[R34] 退出时清理
来源：http://uu.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ik.huixiangedu.cn

[R35] 后台执行并等待
来源：http://sh.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ib.hnjuh.cn

[R36] 并发执行多个任务
来源：http://cg.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ct.panjiajie.cn

[R37] 把输出赋给变量
来源：http://xg.asd995.cn

files=$(ls -1)
来源：http://ys.gzmigu.cn

[R38] 管道串联
来源：http://dm.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ab.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://oi.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://pu.shxzukj.cn

[R40] 追加写日志
来源：http://fi.haigaiapp.cn

echo "log" >> out.log
来源：http://me.shxzskj.cn

[R41] 丢弃输出
来源：http://ak.newstarts.cn

cmd >/dev/null 2>&1
来源：http://rz.nszjky.cn

[R42] 输入重定向
来源：http://ni.asd995.cn

wc -l < a.txt
来源：http://do.521024.cn

[R43] 按名字查找文件
来源：http://xd.gzmigu.cn

find . -name "*.log" -type f
来源：http://kt.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://ai.haigaiapp.cn

find . -mtime -7 -type f
来源：http://zp.jctech888.com.cn

[R45] 批量删除
来源：http://jp.szsharing.cn

find . -name "*.tmp" -delete
来源：http://tz.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://cr.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uk.szxytkj.cn

[R47] sed 单行替换
来源：http://je.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sl.colortex.cn

[R48] awk 取指定列
来源：http://ce.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://ct.szsharing.cn

[R49] awk 带条件
来源：http://rp.hnjuh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qk.szsharing.cn

[R50] awk 求和
来源：http://xl.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ry.newstarts.cn

[R51] 排序去重取前几
来源：http://vd.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bx.haigaiapp.cn

[R52] 统计行数
来源：http://kz.shxzskj.cn

wc -l a.txt
来源：http://cw.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://jm.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://id.haigaiapp.cn

[R54] 比较两个文件
来源：http://cr.panjiajie.cn

diff a.txt b.txt
来源：http://dl.lnxyls.cn

[R55] 压缩与解压
来源：http://gu.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oo.hahajie.cn

[R56] 远程拷贝
来源：http://sn.chemitech.net.cn

scp file user@host:/path/
来源：http://if.asd995.cn

[R57] 远程执行命令
来源：http://ua.colortex.cn

ssh user@host 'uptime'
来源：http://zl.hnjuh.cn

[R58] 下载文件
来源：http://qa.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qw.521024.cn

[R59] 发 POST JSON
来源：http://vq.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wx.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://wv.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cw.haigaiapp.cn

[R61] 磁盘占用
来源：http://vx.nicolike.cn

df -h;  du -sh *
来源：http://pq.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://us.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ru.yuexingan06.cn

[R63] 内存与进程
来源：http://ad.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://gy.yuexingan06.cn

[R64] 结束进程
来源：http://ib.chemitech.net.cn

kill -9 $(pgrep -f app.py)
来源：http://ut.hnjuh.cn

[R65] 查看端口占用
来源：http://ok.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yq.shtwfgs.cn

[R66] 定时任务
来源：http://jv.hahajie.cn

crontab -e;  crontab -l
来源：http://hr.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://qd.huanxung.cn

openssl rand -hex 16
来源：http://vd.huixiangedu.cn

[R68] 计算文件校验值
来源：http://ck.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bn.gzmigu.cn

[R69] 生成随机密码
来源：http://jl.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://er.wgjwhj.cn

[R70] 时间戳与互转
来源：http://pv.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://yv.huixiangedu.cn

[R71] 日期格式化
来源：http://nc.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://py.nszjky.cn

[R72] 等待端口就绪
来源：http://ie.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ge.hnjuh.cn

[R73] 分割大日志
来源：http://li.hahajie.cn

split -l 1000 big.log part_
来源：http://ct.huanxung.cn

[R74] 批量重命名
来源：http://ac.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wn.wgjwhj.cn

[R75] 导出环境变量
来源：http://hx.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://lx.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://rf.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gt.muxihuayi.cn

[R77] 读取用户输入
来源：http://wp.huixiangedu.cn

read -rp "请输入: " ans
来源：http://jd.yuexingan06.cn

[R78] 交互式菜单
来源：http://xg.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mg.gzmigu.cn

[R79] 解析命令行选项
来源：http://gd.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yf.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://fs.huixiangedu.cn

time ./run.sh
来源：http://ek.9csxet.cn

================================================================================
来源：http://rs.bookmarksfly.cn

S. C / C++ 专题
来源：http://cz.shxzskj.cn

================================================================================
来源：http://yr.nicolike.cn

[S01] C：Hello World
来源：http://la.shxzukj.cn

#include <stdio.h>
来源：http://yq.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sd.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://xg.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://eu.haigaiapp.cn

[S03] C：读入整数
来源：http://sf.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://zq.colortex.cn

[S04] C：字符串复制
来源：http://ww.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wt.chemitech.net.cn

[S05] C：字符串长度
来源：http://or.huixiangedu.cn

strlen(s)
来源：http://ti.9csxet.cn

[S06] C：字符串比较
来源：http://pa.nicolike.cn

strcmp(a, b) == 0
来源：http://uj.szsharing.cn

[S07] C：数组遍历求和
来源：http://jj.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://se.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://ra.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hg.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://gs.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ff.nszjky.cn

[S10] C：指针与解引用
来源：http://px.newstarts.cn

int *p = &a;  *p = 5;
来源：http://qz.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://zu.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://bl.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wc.asd995.cn

fclose(f);
来源：http://hj.asd995.cn

[S12] C：写文件
来源：http://ve.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rg.newstarts.cn

[S13] C：宏定义
来源：http://nr.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nh.jctech888.com.cn

[S14] C：枚举
来源：http://cb.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://dt.lnxyls.cn

[S15] C：类型转换
来源：http://py.huanxung.cn

(double) a / b
来源：http://lq.bookmarksfly.cn

[S16] C：位操作置位
来源：http://yp.521024.cn

x |= (1 << 3);
来源：http://ia.nszjky.cn

[S17] C：安全拼接字符串
来源：http://us.521024.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rm.huanxung.cn

[S18] C：命令行参数
来源：http://py.nicolike.cn

int main(int argc, char **argv)
来源：http://eg.yuntaijiaju.cn

[S19] C：快速排序
来源：http://fy.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ar.nszjky.cn

[S20] C：二分查找
来源：http://gj.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bz.asd995.cn

[S21] C：字符类别判断
来源：http://ej.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://do.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://mq.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uo.521024.cn

[S23] C：随机数
来源：http://rc.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fo.gzmigu.cn

[S24] C：获取本地时间
来源：http://pz.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://je.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://kb.hahajie.cn

memcpy(dst, src, n);
来源：http://yf.asd995.cn

[S26] C：内存清零
来源：http://wd.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://rt.asd995.cn

[S27] C：定义常量
来源：http://vl.panjiajie.cn

const double PI = 3.14159;
来源：http://go.shtwfgs.cn

[S28] C：静态变量
来源：http://nt.yuntaijiaju.cn

static int counter = 0;
来源：http://sr.hahajie.cn

[S29] C：变参函数
来源：http://xp.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gz.haigaiapp.cn

[S30] C：头文件保护
来源：http://mx.panjiajie.cn

#ifndef X_H
来源：http://wa.asd995.cn

#define X_H
来源：http://yi.huixinmuqiang.cn

#endif
来源：http://on.9csxet.cn

[S31] C++：Hello World
来源：http://yb.shxzskj.cn

#include <iostream>
来源：http://vx.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://xt.yuexingan06.cn

[S32] C++：字符串
来源：http://aa.521024.cn

std::string s = "hi";  s += "!";
来源：http://nt.szsharing.cn

[S33] C++：vector 增删
来源：http://qj.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fk.hahajie.cn

[S34] C++：遍历 vector
来源：http://mh.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://hj.hnjuh.cn

[S35] C++：map
来源：http://bp.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fy.shxzukj.cn

[S36] C++：unordered_map
来源：http://yj.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ip.shtwfgs.cn

[S37] C++：set
来源：http://ep.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nu.521024.cn

[S38] C++：排序
来源：http://st.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://xl.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://ic.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hf.shxzukj.cn

[S40] C++：查找元素
来源：http://hj.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ye.szxytkj.cn

[S41] C++：类与构造函数
来源：http://je.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eo.nszjky.cn

[S42] C++：继承与虚函数
来源：http://bs.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ln.newstarts.cn

[S43] C++：智能指针
来源：http://fd.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://wb.chemitech.net.cn

[S44] C++：引用传参
来源：http://lw.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://hj.shxzskj.cn

[S45] C++：lambda
来源：http://cb.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zs.muxihuayi.cn

[S46] C++：函数模板
来源：http://vh.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ua.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://hn.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ix.asd995.cn

[S48] C++：逐行读文件
来源：http://hg.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bb.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://gv.colortex.cn

[S49] C++：写文件
来源：http://fq.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qp.yuexingan06.cn

[S50] C++：格式化数字
来源：http://nw.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zt.shxzskj.cn

[S51] C++：显式类型转换
来源：http://jf.haigaiapp.cn

static_cast<double>(a) / b
来源：http://td.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://ic.521024.cn

int size() const noexcept { return n_; }
来源：http://tu.nicolike.cn

[S53] C++：移动语义
来源：http://sh.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://kt.shxzukj.cn

[S54] C++：异常处理
来源：http://gx.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qz.hnjuh.cn

[S55] C++：结构化绑定
来源：http://vx.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xy.huixinmuqiang.cn

[S56] C++：optional
来源：http://dd.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vk.bjjhwx.cn

[S57] C++：编译期常量
来源：http://ng.chemitech.net.cn

constexpr int N = 10;
来源：http://uw.lnxyls.cn

[S58] C++：命名空间
来源：http://kc.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://bw.nicolike.cn

[S59] C++：静态断言
来源：http://ps.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://it.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://hu.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yw.521024.cn

================================================================================
来源：http://om.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vb.haigaiapp.cn

================================================================================
来源：http://gz.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://xr.huixinmuqiang.cn

println("Hello")
来源：http://wi.lnxyls.cn

[T02] Kotlin：变量
来源：http://ts.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ks.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://jp.nicolike.cn

"值: $b"
来源：http://yr.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://fz.asd995.cn

val n: String? = null;  n?.length
来源：http://ov.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://ut.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kn.nicolike.cn

[T06] Kotlin：集合映射
来源：http://aj.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ns.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://he.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rv.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://gb.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://zb.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://ik.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://kn.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://an.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qi.haigaiapp.cn

[T11] Kotlin：协程
来源：http://fc.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uv.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://ig.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://so.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://ss.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://ha.szxytkj.cn

[T14] Kotlin：循环
来源：http://xv.nszjky.cn

for (i in 1..10) println(i)
来源：http://xr.nicolike.cn

[T15] Kotlin：接口
来源：http://rk.hahajie.cn

interface Shape { fun area(): Double }
来源：http://sa.hahajie.cn

[T16] Swift：Hello World
来源：http://gy.shtwfgs.cn

print("Hello")
来源：http://aw.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ij.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://pb.szxytkj.cn

[T18] Swift：字符串插值
来源：http://af.bookmarksfly.cn

"值: \(b)"
来源：http://hn.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://cu.huanxung.cn

if let n = opt { print(n) }
来源：http://ap.huixiangedu.cn

[T20] Swift：数组操作
来源：http://le.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://am.521024.cn

[T21] Swift：遍历
来源：http://sk.newstarts.cn

for x in a { print(x) }
来源：http://km.newstarts.cn

[T22] Swift：字典
来源：http://rv.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://li.chemitech.net.cn

[T23] Swift：函数
来源：http://yr.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://je.haigaiapp.cn

[T24] Swift：闭包
来源：http://yt.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rm.hahajie.cn

[T25] Swift：结构体
来源：http://rx.huixinmuqiang.cn

struct P { var x: Int }
来源：http://wg.muxihuayi.cn

[T26] Swift：类与重写
来源：http://lk.shxzukj.cn

class A: Base { override func f() {} }
来源：http://jd.hahajie.cn

[T27] Swift：错误处理
来源：http://ou.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://xs.panjiajie.cn

[T28] Swift：枚举
来源：http://mu.szsharing.cn

enum Color { case red, green }
来源：http://rr.colortex.cn

[T29] Swift：guard 提前返回
来源：http://kw.9csxet.cn

guard let x = opt else { return }
来源：http://bm.shxzukj.cn

[T30] Swift：协议
来源：http://yb.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://xc.shxzukj.cn

[T31] Lua：Hello World
来源：http://ac.wgjwhj.cn

print("Hello")
来源：http://vw.shxzukj.cn

[T32] Lua：局部变量
来源：http://xr.bookmarksfly.cn

local a = 1
来源：http://rg.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://df.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zh.huanxung.cn

[T34] Lua：遍历表
来源：http://sk.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oy.hahajie.cn


<!-- 参考信息 -->