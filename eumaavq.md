代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://lo.bookmarksfly.cn

[R26] 命令替换
来源：http://zo.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://rj.521024.cn

[R27] 算术展开
来源：http://dq.nszjky.cn

echo $((1 + 2 * 3))
来源：http://eh.shtwfgs.cn

[R28] 浮点运算
来源：http://cx.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://tp.szxytkj.cn

[R29] 定义函数
来源：http://bv.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ub.szsharing.cn

[R30] 函数返回状态码
来源：http://tf.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://an.huanxung.cn

[R31] 局部变量
来源：http://oy.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://zy.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://ou.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pq.muxihuayi.cn

[R33] 捕获错误并提示行号
来源：http://xd.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vi.huixiangedu.cn

[R34] 退出时清理
来源：http://hh.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cm.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://lu.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zj.nszjky.cn

[R36] 并发执行多个任务
来源：http://jw.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xp.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://rc.hahajie.cn

files=$(ls -1)
来源：http://ji.wgjwhj.cn

[R38] 管道串联
来源：http://bm.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://ys.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://ls.szsharing.cn

cmd > out.log 2>&1
来源：http://oe.yuntaijiaju.cn

[R40] 追加写日志
来源：http://lo.shxzskj.cn

echo "log" >> out.log
来源：http://cn.nicolike.cn

[R41] 丢弃输出
来源：http://uj.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://kx.chemitech.net.cn

[R42] 输入重定向
来源：http://wf.jianghongdianzi.cn

wc -l < a.txt
来源：http://ls.panjiajie.cn

[R43] 按名字查找文件
来源：http://ua.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://rw.wgjwhj.cn

[R44] 按修改时间查找
来源：http://yr.shxzukj.cn

find . -mtime -7 -type f
来源：http://zo.jianghongdianzi.cn

[R45] 批量删除
来源：http://ho.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://mv.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://km.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yg.szsharing.cn

[R47] sed 单行替换
来源：http://wm.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vt.bjjhwx.cn

[R48] awk 取指定列
来源：http://ec.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://og.9csxet.cn

[R49] awk 带条件
来源：http://kq.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eo.shtwfgs.cn

[R50] awk 求和
来源：http://of.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cb.shtwfgs.cn

[R51] 排序去重取前几
来源：http://qn.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dy.szxytkj.cn

[R52] 统计行数
来源：http://qj.hahajie.cn

wc -l a.txt
来源：http://zf.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://jb.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ne.bookmarksfly.cn

[R54] 比较两个文件
来源：http://ne.shxzskj.cn

diff a.txt b.txt
来源：http://mc.szxytkj.cn

[R55] 压缩与解压
来源：http://dy.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hh.haigaiapp.cn

[R56] 远程拷贝
来源：http://iy.lnxyls.cn

scp file user@host:/path/
来源：http://sc.chemitech.net.cn

[R57] 远程执行命令
来源：http://if.shxzukj.cn

ssh user@host 'uptime'
来源：http://wr.bjjhwx.cn

[R58] 下载文件
来源：http://xg.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ti.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ke.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uy.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://mj.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rl.newstarts.cn

[R61] 磁盘占用
来源：http://gl.newstarts.cn

df -h;  du -sh *
来源：http://mp.lnxyls.cn

[R62] 找最占空间的文件
来源：http://nl.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://se.bjjhwx.cn

[R63] 内存与进程
来源：http://fw.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://kz.bookmarksfly.cn

[R64] 结束进程
来源：http://wn.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://oj.gzmigu.cn

[R65] 查看端口占用
来源：http://nj.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://no.chemitech.net.cn

[R66] 定时任务
来源：http://ik.hahajie.cn

crontab -e;  crontab -l
来源：http://na.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://md.haigaiapp.cn

openssl rand -hex 16
来源：http://xv.szsharing.cn

[R68] 计算文件校验值
来源：http://ys.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qn.bjjhwx.cn

[R69] 生成随机密码
来源：http://vj.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://yh.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://qk.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://mn.szxytkj.cn

[R71] 日期格式化
来源：http://ie.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aw.yuexingan06.cn

[R72] 等待端口就绪
来源：http://sk.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ql.huanxung.cn

[R73] 分割大日志
来源：http://vp.hnjuh.cn

split -l 1000 big.log part_
来源：http://dp.jctech888.com.cn

[R74] 批量重命名
来源：http://gu.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cg.shxzukj.cn

[R75] 导出环境变量
来源：http://xh.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://en.wgjwhj.cn

[R76] 使用临时文件
来源：http://dh.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cv.nicolike.cn

[R77] 读取用户输入
来源：http://zs.521024.cn

read -rp "请输入: " ans
来源：http://gh.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://om.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fr.9csxet.cn

[R79] 解析命令行选项
来源：http://ai.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lf.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://th.huixiangedu.cn

time ./run.sh
来源：http://mq.521024.cn

================================================================================
来源：http://rz.shxzukj.cn

S. C / C++ 专题
来源：http://ye.colortex.cn

================================================================================
来源：http://mi.9csxet.cn

[S01] C：Hello World
来源：http://ko.521024.cn

#include <stdio.h>
来源：http://ad.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zf.521024.cn

[S02] C：变量与格式化输出
来源：http://gc.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://ir.haigaiapp.cn

[S03] C：读入整数
来源：http://bg.szxytkj.cn

int x; scanf("%d", &x);
来源：http://fm.chemitech.net.cn

[S04] C：字符串复制
来源：http://ej.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fr.szxytkj.cn

[S05] C：字符串长度
来源：http://vm.bjjhwx.cn

strlen(s)
来源：http://ny.huanxung.cn

[S06] C：字符串比较
来源：http://eq.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://uq.newstarts.cn

[S07] C：数组遍历求和
来源：http://wc.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cf.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://lm.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ul.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://jx.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ow.wgjwhj.cn

[S10] C：指针与解引用
来源：http://bj.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://kk.yuexingan06.cn

[S11] C：逐行读文件
来源：http://xu.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://wn.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xo.yuexingan06.cn

fclose(f);
来源：http://ee.yuexingan06.cn

[S12] C：写文件
来源：http://lb.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mj.shxzukj.cn

[S13] C：宏定义
来源：http://pp.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ii.huixiangedu.cn

[S14] C：枚举
来源：http://ei.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://ll.hahajie.cn

[S15] C：类型转换
来源：http://id.9csxet.cn

(double) a / b
来源：http://da.nicolike.cn

[S16] C：位操作置位
来源：http://zy.nicolike.cn

x |= (1 << 3);
来源：http://rr.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://lp.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tx.9csxet.cn

[S18] C：命令行参数
来源：http://am.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://qk.hnjuh.cn

[S19] C：快速排序
来源：http://le.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ry.huixiangedu.cn

[S20] C：二分查找
来源：http://qp.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eu.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://vc.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wk.lnxyls.cn

[S22] C：字符串转数字
来源：http://po.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ej.newstarts.cn

[S23] C：随机数
来源：http://nt.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://no.521024.cn

[S24] C：获取本地时间
来源：http://ea.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ip.haigaiapp.cn

[S25] C：内存拷贝
来源：http://yn.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://gk.bjjhwx.cn

[S26] C：内存清零
来源：http://qz.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://gg.colortex.cn

[S27] C：定义常量
来源：http://cg.shxzukj.cn

const double PI = 3.14159;
来源：http://ua.chemitech.net.cn

[S28] C：静态变量
来源：http://bl.huixinmuqiang.cn

static int counter = 0;
来源：http://wv.szsharing.cn

[S29] C：变参函数
来源：http://wg.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yx.hnjuh.cn

[S30] C：头文件保护
来源：http://mc.bjjhwx.cn

#ifndef X_H
来源：http://yw.muxihuayi.cn

#define X_H
来源：http://lh.szsharing.cn

#endif
来源：http://rg.yuexingan06.cn

[S31] C++：Hello World
来源：http://fg.nicolike.cn

#include <iostream>
来源：http://sm.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://uq.wgjwhj.cn

[S32] C++：字符串
来源：http://rz.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://iz.muxihuayi.cn

[S33] C++：vector 增删
来源：http://fg.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iq.lnxyls.cn

[S34] C++：遍历 vector
来源：http://lu.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://of.shtwfgs.cn

[S35] C++：map
来源：http://ai.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://on.muxihuayi.cn

[S36] C++：unordered_map
来源：http://dy.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zb.hnjuh.cn

[S37] C++：set
来源：http://qc.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gd.panjiajie.cn

[S38] C++：排序
来源：http://wx.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://vs.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://mz.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ta.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://dl.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ae.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://bx.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fx.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://yi.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ll.hnjuh.cn

[S43] C++：智能指针
来源：http://se.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://mn.newstarts.cn

[S44] C++：引用传参
来源：http://pf.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://rh.huixinmuqiang.cn

[S45] C++：lambda
来源：http://bq.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ts.lnxyls.cn

[S46] C++：函数模板
来源：http://bl.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://py.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://cc.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qu.hnjuh.cn

[S48] C++：逐行读文件
来源：http://sl.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bp.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://sd.huixiangedu.cn

[S49] C++：写文件
来源：http://gn.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uj.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://iq.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iv.nicolike.cn

[S51] C++：显式类型转换
来源：http://qw.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://sa.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://ra.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ck.chemitech.net.cn

[S53] C++：移动语义
来源：http://ha.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://ee.szxytkj.cn

[S54] C++：异常处理
来源：http://lh.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nd.szxytkj.cn

[S55] C++：结构化绑定
来源：http://rw.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lq.huixiangedu.cn

[S56] C++：optional
来源：http://gu.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://if.shxzukj.cn

[S57] C++：编译期常量
来源：http://kl.haigaiapp.cn

constexpr int N = 10;
来源：http://iw.nicolike.cn

[S58] C++：命名空间
来源：http://vn.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://vv.huanxung.cn

[S59] C++：静态断言
来源：http://sh.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jp.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://ul.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ro.huixinmuqiang.cn

================================================================================
来源：http://dz.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pq.shxzukj.cn

================================================================================
来源：http://dn.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://oc.chemitech.net.cn

println("Hello")
来源：http://lx.hnjuh.cn

[T02] Kotlin：变量
来源：http://gk.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ym.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://gm.jianghongdianzi.cn

"值: $b"
来源：http://oo.9csxet.cn

[T04] Kotlin：空安全
来源：http://wp.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://rr.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://dq.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ja.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://aj.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://if.szsharing.cn

[T07] Kotlin：集合过滤
来源：http://cs.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uo.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://rg.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://eb.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://gq.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://oh.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ae.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ls.chemitech.net.cn

[T11] Kotlin：协程
来源：http://qr.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://om.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://ck.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://pl.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://qq.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://gv.nicolike.cn

[T14] Kotlin：循环
来源：http://dn.shxzukj.cn

for (i in 1..10) println(i)
来源：http://cn.nszjky.cn

[T15] Kotlin：接口
来源：http://nw.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://bb.bjjhwx.cn

[T16] Swift：Hello World
来源：http://yi.yuntaijiaju.cn

print("Hello")
来源：http://yo.colortex.cn

[T17] Swift：变量与常量
来源：http://cg.hahajie.cn

var a = 1;  let b = 2
来源：http://cd.asd995.cn

[T18] Swift：字符串插值
来源：http://wn.hahajie.cn

"值: \(b)"
来源：http://mu.newstarts.cn

[T19] Swift：可选绑定
来源：http://yi.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://hu.shtwfgs.cn

[T20] Swift：数组操作
来源：http://jd.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qo.lnxyls.cn

[T21] Swift：遍历
来源：http://xj.huanxung.cn

for x in a { print(x) }
来源：http://eu.yuexingan06.cn

[T22] Swift：字典
来源：http://kn.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dm.bjjhwx.cn

[T23] Swift：函数
来源：http://en.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gk.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://ch.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lp.bookmarksfly.cn

[T25] Swift：结构体
来源：http://yc.gzmigu.cn

struct P { var x: Int }
来源：http://cu.szsharing.cn

[T26] Swift：类与重写
来源：http://ey.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://jg.shxzskj.cn

[T27] Swift：错误处理
来源：http://qf.szsharing.cn

do { try f() } catch { print(error) }
来源：http://qa.shxzskj.cn

[T28] Swift：枚举
来源：http://oe.hnjuh.cn

enum Color { case red, green }
来源：http://jc.jctech888.com.cn


<!-- 参考信息 -->