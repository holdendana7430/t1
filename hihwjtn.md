代发 wailian999

echo "${#s}"
来源：http://dr.yuexingan06.cn

[R22] 截取子串
来源：http://ad.hnjuh.cn

echo "${s:0:5}"
来源：http://xc.shxzukj.cn

[R23] 字符串替换
来源：http://du.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qz.521024.cn

[R24] 大小写转换
来源：http://ck.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mx.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://dz.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zk.bookmarksfly.cn

[R26] 命令替换
来源：http://qu.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://qk.wgjwhj.cn

[R27] 算术展开
来源：http://zg.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://yh.newstarts.cn

[R28] 浮点运算
来源：http://dh.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://ip.bookmarksfly.cn

[R29] 定义函数
来源：http://oo.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bc.hnjuh.cn

[R30] 函数返回状态码
来源：http://vb.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://hy.yuntaijiaju.cn

[R31] 局部变量
来源：http://tz.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://sx.shxzukj.cn

[R32] 参数个数校验
来源：http://pv.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yt.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://lm.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ql.huanxung.cn

[R34] 退出时清理
来源：http://ey.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nc.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://ba.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yc.newstarts.cn

[R36] 并发执行多个任务
来源：http://uz.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ms.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://ee.shxzskj.cn

files=$(ls -1)
来源：http://gj.szsharing.cn

[R38] 管道串联
来源：http://fq.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://mz.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://mp.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://tb.muxihuayi.cn

[R40] 追加写日志
来源：http://zu.huanxung.cn

echo "log" >> out.log
来源：http://et.szxytkj.cn

[R41] 丢弃输出
来源：http://py.nszjky.cn

cmd >/dev/null 2>&1
来源：http://tm.hnjuh.cn

[R42] 输入重定向
来源：http://ya.jianghongdianzi.cn

wc -l < a.txt
来源：http://ff.shtwfgs.cn

[R43] 按名字查找文件
来源：http://cd.szsharing.cn

find . -name "*.log" -type f
来源：http://fj.lnxyls.cn

[R44] 按修改时间查找
来源：http://ff.bjjhwx.cn

find . -mtime -7 -type f
来源：http://gq.wgjwhj.cn

[R45] 批量删除
来源：http://ky.szsharing.cn

find . -name "*.tmp" -delete
来源：http://qs.panjiajie.cn

[R46] 递归替换文件内容
来源：http://pl.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://um.gzmigu.cn

[R47] sed 单行替换
来源：http://xh.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ji.szxytkj.cn

[R48] awk 取指定列
来源：http://kl.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://cm.shtwfgs.cn

[R49] awk 带条件
来源：http://iv.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sp.jctech888.com.cn

[R50] awk 求和
来源：http://vb.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fu.panjiajie.cn

[R51] 排序去重取前几
来源：http://gk.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qa.szsharing.cn

[R52] 统计行数
来源：http://en.nszjky.cn

wc -l a.txt
来源：http://jl.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://wc.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://of.haigaiapp.cn

[R54] 比较两个文件
来源：http://xr.gzmigu.cn

diff a.txt b.txt
来源：http://kn.bookmarksfly.cn

[R55] 压缩与解压
来源：http://yv.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kn.szsharing.cn

[R56] 远程拷贝
来源：http://rr.szxytkj.cn

scp file user@host:/path/
来源：http://bg.asd995.cn

[R57] 远程执行命令
来源：http://uc.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://cd.haigaiapp.cn

[R58] 下载文件
来源：http://cw.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ej.yuexingan06.cn

[R59] 发 POST JSON
来源：http://oc.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nv.521024.cn

[R60] 只看 HTTP 状态码
来源：http://xd.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://re.huixiangedu.cn

[R61] 磁盘占用
来源：http://cu.muxihuayi.cn

df -h;  du -sh *
来源：http://rl.asd995.cn

[R62] 找最占空间的文件
来源：http://uy.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://sz.szsharing.cn

[R63] 内存与进程
来源：http://su.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://sv.jianghongdianzi.cn

[R64] 结束进程
来源：http://ca.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://jq.hnjuh.cn

[R65] 查看端口占用
来源：http://kd.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zs.shtwfgs.cn

[R66] 定时任务
来源：http://hm.hahajie.cn

crontab -e;  crontab -l
来源：http://jv.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://ht.yuexingan06.cn

openssl rand -hex 16
来源：http://zr.newstarts.cn

[R68] 计算文件校验值
来源：http://xm.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ta.lnxyls.cn

[R69] 生成随机密码
来源：http://cv.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://xb.bjjhwx.cn

[R70] 时间戳与互转
来源：http://bq.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ed.521024.cn

[R71] 日期格式化
来源：http://vl.shxzskj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://il.panjiajie.cn

[R72] 等待端口就绪
来源：http://ny.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tt.nicolike.cn

[R73] 分割大日志
来源：http://wc.nszjky.cn

split -l 1000 big.log part_
来源：http://bb.shxzukj.cn

[R74] 批量重命名
来源：http://be.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ia.shxzukj.cn

[R75] 导出环境变量
来源：http://it.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://hz.bookmarksfly.cn

[R76] 使用临时文件
来源：http://la.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://so.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://vh.newstarts.cn

read -rp "请输入: " ans
来源：http://xo.szsharing.cn

[R78] 交互式菜单
来源：http://te.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tc.panjiajie.cn

[R79] 解析命令行选项
来源：http://nr.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qm.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://vi.szsharing.cn

time ./run.sh
来源：http://op.nicolike.cn

================================================================================
来源：http://gp.shtwfgs.cn

S. C / C++ 专题
来源：http://fc.yuntaijiaju.cn

================================================================================
来源：http://rj.huixiangedu.cn

[S01] C：Hello World
来源：http://tz.szxytkj.cn

#include <stdio.h>
来源：http://ym.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wf.521024.cn

[S02] C：变量与格式化输出
来源：http://jx.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://ke.shxzukj.cn

[S03] C：读入整数
来源：http://fj.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://wt.chemitech.net.cn

[S04] C：字符串复制
来源：http://gy.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ew.lnxyls.cn

[S05] C：字符串长度
来源：http://xn.huanxung.cn

strlen(s)
来源：http://jn.gzmigu.cn

[S06] C：字符串比较
来源：http://to.newstarts.cn

strcmp(a, b) == 0
来源：http://yx.colortex.cn

[S07] C：数组遍历求和
来源：http://gl.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vt.asd995.cn

[S08] C：动态内存分配与释放
来源：http://eq.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oo.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://mp.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qd.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://vm.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://no.huanxung.cn

[S11] C：逐行读文件
来源：http://ji.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://uj.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lv.haigaiapp.cn

fclose(f);
来源：http://lc.haigaiapp.cn

[S12] C：写文件
来源：http://sx.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oc.gzmigu.cn

[S13] C：宏定义
来源：http://ga.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vi.newstarts.cn

[S14] C：枚举
来源：http://wy.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://vy.szsharing.cn

[S15] C：类型转换
来源：http://is.nicolike.cn

(double) a / b
来源：http://ba.bookmarksfly.cn

[S16] C：位操作置位
来源：http://sf.bookmarksfly.cn

x |= (1 << 3);
来源：http://az.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://ow.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rl.shxzskj.cn

[S18] C：命令行参数
来源：http://fy.9csxet.cn

int main(int argc, char **argv)
来源：http://ma.yuexingan06.cn

[S19] C：快速排序
来源：http://ph.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dj.szxytkj.cn

[S20] C：二分查找
来源：http://lb.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wn.newstarts.cn

[S21] C：字符类别判断
来源：http://oq.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cr.haigaiapp.cn

[S22] C：字符串转数字
来源：http://fj.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ax.hnjuh.cn

[S23] C：随机数
来源：http://sd.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lb.panjiajie.cn

[S24] C：获取本地时间
来源：http://tl.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wz.haigaiapp.cn

[S25] C：内存拷贝
来源：http://jn.szxytkj.cn

memcpy(dst, src, n);
来源：http://we.jianghongdianzi.cn

[S26] C：内存清零
来源：http://ra.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://mg.nicolike.cn

[S27] C：定义常量
来源：http://qs.haigaiapp.cn

const double PI = 3.14159;
来源：http://ll.huixinmuqiang.cn

[S28] C：静态变量
来源：http://ly.huixinmuqiang.cn

static int counter = 0;
来源：http://wn.huanxung.cn

[S29] C：变参函数
来源：http://wf.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bg.521024.cn

[S30] C：头文件保护
来源：http://lh.huixinmuqiang.cn

#ifndef X_H
来源：http://up.shtwfgs.cn

#define X_H
来源：http://ff.hnjuh.cn

#endif
来源：http://fz.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://vb.huixinmuqiang.cn

#include <iostream>
来源：http://ec.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://te.huanxung.cn

[S32] C++：字符串
来源：http://gn.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://da.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ai.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dx.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://is.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://ha.bookmarksfly.cn

[S35] C++：map
来源：http://zc.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ty.shxzukj.cn

[S36] C++：unordered_map
来源：http://qz.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jn.521024.cn

[S37] C++：set
来源：http://am.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yz.haigaiapp.cn

[S38] C++：排序
来源：http://mu.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://hc.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://fa.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gl.shxzskj.cn

[S40] C++：查找元素
来源：http://oy.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://am.hnjuh.cn

[S41] C++：类与构造函数
来源：http://vt.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hq.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://zw.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://dn.9csxet.cn

[S43] C++：智能指针
来源：http://zl.521024.cn

auto p = std::make_unique<int>(5);
来源：http://um.chemitech.net.cn

[S44] C++：引用传参
来源：http://rs.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://qe.yuntaijiaju.cn

[S45] C++：lambda
来源：http://mp.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ab.panjiajie.cn

[S46] C++：函数模板
来源：http://tu.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jn.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://bh.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yy.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://om.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tb.nszjky.cn

while (std::getline(in, line)) { }
来源：http://hk.yuntaijiaju.cn

[S49] C++：写文件
来源：http://dj.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bh.asd995.cn

[S50] C++：格式化数字
来源：http://nn.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rl.521024.cn

[S51] C++：显式类型转换
来源：http://yp.huanxung.cn

static_cast<double>(a) / b
来源：http://sn.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://jd.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://am.nicolike.cn

[S53] C++：移动语义
来源：http://yo.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://cp.bookmarksfly.cn

[S54] C++：异常处理
来源：http://qd.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hh.lnxyls.cn

[S55] C++：结构化绑定
来源：http://hj.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yk.gzmigu.cn

[S56] C++：optional
来源：http://wy.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jt.panjiajie.cn

[S57] C++：编译期常量
来源：http://zi.nszjky.cn

constexpr int N = 10;
来源：http://bu.shxzukj.cn

[S58] C++：命名空间
来源：http://kl.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://cc.hnjuh.cn

[S59] C++：静态断言
来源：http://ip.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rb.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://nq.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://io.shxzskj.cn

================================================================================
来源：http://in.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ei.huanxung.cn

================================================================================
来源：http://ui.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://kl.jctech888.com.cn

println("Hello")
来源：http://xu.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://qt.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zb.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://gz.bjjhwx.cn

"值: $b"
来源：http://hd.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://mb.gzmigu.cn

val n: String? = null;  n?.length
来源：http://rh.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://td.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://as.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://xb.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wd.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://uc.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zg.gzmigu.cn

[T08] Kotlin：数据类
来源：http://ly.hnjuh.cn

data class User(val name: String, val age: Int)
来源：http://fl.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://gr.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://xt.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://hx.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ft.huanxung.cn

[T11] Kotlin：协程
来源：http://nm.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hf.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://xn.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://km.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://uo.hahajie.cn

val m = mapOf("a" to 1)
来源：http://ek.chemitech.net.cn

[T14] Kotlin：循环
来源：http://vc.colortex.cn

for (i in 1..10) println(i)
来源：http://pu.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://yl.huanxung.cn

interface Shape { fun area(): Double }
来源：http://dd.newstarts.cn

[T16] Swift：Hello World
来源：http://bm.newstarts.cn

print("Hello")
来源：http://pw.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://ox.lnxyls.cn

var a = 1;  let b = 2
来源：http://uq.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://xg.lnxyls.cn

"值: \(b)"
来源：http://ji.521024.cn

[T19] Swift：可选绑定
来源：http://bl.9csxet.cn

if let n = opt { print(n) }
来源：http://it.gzmigu.cn

[T20] Swift：数组操作
来源：http://xb.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xk.bjjhwx.cn

[T21] Swift：遍历
来源：http://sh.521024.cn

for x in a { print(x) }
来源：http://ak.chemitech.net.cn

[T22] Swift：字典
来源：http://qy.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://go.shxzukj.cn

[T23] Swift：函数
来源：http://fg.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gd.nszjky.cn

[T24] Swift：闭包
来源：http://sk.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mq.hnjuh.cn


<!-- 参考信息 -->