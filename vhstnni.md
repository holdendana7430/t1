代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://xa.lnxyls.cn

[R26] 命令替换
来源：http://og.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://oy.chemitech.net.cn

[R27] 算术展开
来源：http://gs.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://ii.haigaiapp.cn

[R28] 浮点运算
来源：http://xk.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://dz.newstarts.cn

[R29] 定义函数
来源：http://gb.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gq.huixiangedu.cn

[R30] 函数返回状态码
来源：http://rd.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://fb.huixiangedu.cn

[R31] 局部变量
来源：http://gu.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://xq.gzmigu.cn

[R32] 参数个数校验
来源：http://rg.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://um.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://vx.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mk.lnxyls.cn

[R34] 退出时清理
来源：http://pe.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ci.521024.cn

[R35] 后台执行并等待
来源：http://nh.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zz.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://vg.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fb.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ri.huanxung.cn

files=$(ls -1)
来源：http://qq.bjjhwx.cn

[R38] 管道串联
来源：http://ux.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://lf.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://xj.newstarts.cn

cmd > out.log 2>&1
来源：http://vb.shxzskj.cn

[R40] 追加写日志
来源：http://xl.muxihuayi.cn

echo "log" >> out.log
来源：http://ff.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://ss.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://sb.wgjwhj.cn

[R42] 输入重定向
来源：http://ne.colortex.cn

wc -l < a.txt
来源：http://hq.colortex.cn

[R43] 按名字查找文件
来源：http://cv.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://vg.yuexingan06.cn

[R44] 按修改时间查找
来源：http://bg.lnxyls.cn

find . -mtime -7 -type f
来源：http://rp.bjjhwx.cn

[R45] 批量删除
来源：http://tn.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://gk.9csxet.cn

[R46] 递归替换文件内容
来源：http://kp.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ze.bookmarksfly.cn

[R47] sed 单行替换
来源：http://gb.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nn.shtwfgs.cn

[R48] awk 取指定列
来源：http://wb.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://it.panjiajie.cn

[R49] awk 带条件
来源：http://dx.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vm.jctech888.com.cn

[R50] awk 求和
来源：http://rg.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ej.9csxet.cn

[R51] 排序去重取前几
来源：http://ln.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lm.yuexingan06.cn

[R52] 统计行数
来源：http://ec.szsharing.cn

wc -l a.txt
来源：http://it.521024.cn

[R53] 查看文件头与实时尾
来源：http://oy.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://my.shxzukj.cn

[R54] 比较两个文件
来源：http://ij.hahajie.cn

diff a.txt b.txt
来源：http://yb.hnjuh.cn

[R55] 压缩与解压
来源：http://lo.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vf.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://ej.nicolike.cn

scp file user@host:/path/
来源：http://oh.gzmigu.cn

[R57] 远程执行命令
来源：http://nz.szsharing.cn

ssh user@host 'uptime'
来源：http://ja.yuntaijiaju.cn

[R58] 下载文件
来源：http://kf.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ys.wgjwhj.cn

[R59] 发 POST JSON
来源：http://la.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://en.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://xi.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sl.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://lh.panjiajie.cn

df -h;  du -sh *
来源：http://fp.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://fk.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://ey.9csxet.cn

[R63] 内存与进程
来源：http://fx.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://jn.chemitech.net.cn

[R64] 结束进程
来源：http://ma.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://ce.gzmigu.cn

[R65] 查看端口占用
来源：http://yc.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mg.hnjuh.cn

[R66] 定时任务
来源：http://dz.shxzukj.cn

crontab -e;  crontab -l
来源：http://sf.newstarts.cn

[R67] 生成随机十六进制串
来源：http://oy.nicolike.cn

openssl rand -hex 16
来源：http://ij.haigaiapp.cn

[R68] 计算文件校验值
来源：http://wf.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wf.hnjuh.cn

[R69] 生成随机密码
来源：http://vd.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://tb.muxihuayi.cn

[R70] 时间戳与互转
来源：http://sy.nszjky.cn

date +%s;  date -d @1700000000
来源：http://vw.shxzskj.cn

[R71] 日期格式化
来源：http://xo.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zq.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://ls.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yo.asd995.cn

[R73] 分割大日志
来源：http://zb.shxzukj.cn

split -l 1000 big.log part_
来源：http://gc.yuntaijiaju.cn

[R74] 批量重命名
来源：http://mf.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zu.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://vu.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://et.huixiangedu.cn

[R76] 使用临时文件
来源：http://vf.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ij.newstarts.cn

[R77] 读取用户输入
来源：http://xp.huanxung.cn

read -rp "请输入: " ans
来源：http://ve.newstarts.cn

[R78] 交互式菜单
来源：http://ti.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wx.szxytkj.cn

[R79] 解析命令行选项
来源：http://wv.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wz.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://wi.yuntaijiaju.cn

time ./run.sh
来源：http://ri.jctech888.com.cn

================================================================================
来源：http://iq.521024.cn

S. C / C++ 专题
来源：http://xy.huixiangedu.cn

================================================================================
来源：http://bo.wgjwhj.cn

[S01] C：Hello World
来源：http://il.szsharing.cn

#include <stdio.h>
来源：http://rs.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oa.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://nf.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://wq.newstarts.cn

[S03] C：读入整数
来源：http://wj.asd995.cn

int x; scanf("%d", &x);
来源：http://ou.nszjky.cn

[S04] C：字符串复制
来源：http://fp.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sv.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://vq.bjjhwx.cn

strlen(s)
来源：http://fl.gzmigu.cn

[S06] C：字符串比较
来源：http://bs.huanxung.cn

strcmp(a, b) == 0
来源：http://yr.shxzskj.cn

[S07] C：数组遍历求和
来源：http://cl.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://om.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://le.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kx.yuexingan06.cn

[S09] C：结构体定义与初始化
来源：http://wg.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nw.shxzukj.cn

[S10] C：指针与解引用
来源：http://mw.521024.cn

int *p = &a;  *p = 5;
来源：http://yl.jctech888.com.cn

[S11] C：逐行读文件
来源：http://od.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ys.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ej.asd995.cn

fclose(f);
来源：http://vp.newstarts.cn

[S12] C：写文件
来源：http://pn.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lk.hahajie.cn

[S13] C：宏定义
来源：http://kd.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oi.asd995.cn

[S14] C：枚举
来源：http://kv.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://ja.shxzukj.cn

[S15] C：类型转换
来源：http://ge.szsharing.cn

(double) a / b
来源：http://bc.asd995.cn

[S16] C：位操作置位
来源：http://lo.jctech888.com.cn

x |= (1 << 3);
来源：http://xu.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://sz.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://px.nicolike.cn

[S18] C：命令行参数
来源：http://lo.colortex.cn

int main(int argc, char **argv)
来源：http://rh.huixinmuqiang.cn

[S19] C：快速排序
来源：http://bz.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dg.bjjhwx.cn

[S20] C：二分查找
来源：http://ja.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fz.colortex.cn

[S21] C：字符类别判断
来源：http://nc.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ow.shtwfgs.cn

[S22] C：字符串转数字
来源：http://vp.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xy.panjiajie.cn

[S23] C：随机数
来源：http://mm.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://em.gzmigu.cn

[S24] C：获取本地时间
来源：http://xl.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iv.huanxung.cn

[S25] C：内存拷贝
来源：http://te.colortex.cn

memcpy(dst, src, n);
来源：http://vj.lnxyls.cn

[S26] C：内存清零
来源：http://up.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://mh.wgjwhj.cn

[S27] C：定义常量
来源：http://xq.bjjhwx.cn

const double PI = 3.14159;
来源：http://cf.muxihuayi.cn

[S28] C：静态变量
来源：http://wc.szxytkj.cn

static int counter = 0;
来源：http://ol.jctech888.com.cn

[S29] C：变参函数
来源：http://os.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ae.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://qj.bjjhwx.cn

#ifndef X_H
来源：http://xm.yuexingan06.cn

#define X_H
来源：http://te.newstarts.cn

#endif
来源：http://py.bjjhwx.cn

[S31] C++：Hello World
来源：http://rw.bookmarksfly.cn

#include <iostream>
来源：http://jj.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://dm.lnxyls.cn

[S32] C++：字符串
来源：http://bs.521024.cn

std::string s = "hi";  s += "!";
来源：http://qu.wgjwhj.cn

[S33] C++：vector 增删
来源：http://qh.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gn.521024.cn

[S34] C++：遍历 vector
来源：http://rf.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://rh.colortex.cn

[S35] C++：map
来源：http://mh.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iq.panjiajie.cn

[S36] C++：unordered_map
来源：http://zb.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rt.colortex.cn

[S37] C++：set
来源：http://ko.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tp.yuexingan06.cn

[S38] C++：排序
来源：http://qe.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://rs.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://mu.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mw.szsharing.cn

[S40] C++：查找元素
来源：http://sk.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ih.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://gd.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wi.521024.cn

[S42] C++：继承与虚函数
来源：http://qh.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ux.nicolike.cn

[S43] C++：智能指针
来源：http://og.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://kk.haigaiapp.cn

[S44] C++：引用传参
来源：http://wx.521024.cn

void inc(int &x) { ++x; }
来源：http://kl.muxihuayi.cn

[S45] C++：lambda
来源：http://wj.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hw.hnjuh.cn

[S46] C++：函数模板
来源：http://kq.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ea.521024.cn

[S47] C++：结构化绑定遍历
来源：http://sb.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://is.nszjky.cn

[S48] C++：逐行读文件
来源：http://ad.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hc.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://dq.bookmarksfly.cn

[S49] C++：写文件
来源：http://wj.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zy.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ck.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ce.huanxung.cn

[S51] C++：显式类型转换
来源：http://xg.jctech888.com.cn

static_cast<double>(a) / b
来源：http://nn.521024.cn

[S52] C++：const 与 noexcept
来源：http://fc.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://xl.shxzukj.cn

[S53] C++：移动语义
来源：http://ta.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://qx.9csxet.cn

[S54] C++：异常处理
来源：http://vn.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nk.huanxung.cn

[S55] C++：结构化绑定
来源：http://qo.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sq.bookmarksfly.cn

[S56] C++：optional
来源：http://wo.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vu.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ah.hnjuh.cn

constexpr int N = 10;
来源：http://pr.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://dv.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://xi.huixiangedu.cn

[S59] C++：静态断言
来源：http://yq.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ge.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://ae.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kv.521024.cn

================================================================================
来源：http://oi.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zn.shtwfgs.cn

================================================================================
来源：http://fm.colortex.cn

[T01] Kotlin：Hello World
来源：http://yt.hnjuh.cn

println("Hello")
来源：http://qn.huixiangedu.cn

[T02] Kotlin：变量
来源：http://zp.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://df.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://mh.jctech888.com.cn

"值: $b"
来源：http://hj.lnxyls.cn

[T04] Kotlin：空安全
来源：http://ex.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://hv.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://wf.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nf.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://hg.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://so.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://sz.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://io.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://xf.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://wh.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://wg.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://fb.521024.cn

[T10] Kotlin：默认参数
来源：http://lp.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gu.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://vm.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bw.huanxung.cn

[T12] Kotlin：解构声明
来源：http://bz.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://fj.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://rw.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://df.asd995.cn

[T14] Kotlin：循环
来源：http://pu.panjiajie.cn

for (i in 1..10) println(i)
来源：http://xn.newstarts.cn

[T15] Kotlin：接口
来源：http://xh.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://my.hnjuh.cn

[T16] Swift：Hello World
来源：http://ht.hahajie.cn

print("Hello")
来源：http://wq.9csxet.cn

[T17] Swift：变量与常量
来源：http://sy.wgjwhj.cn

var a = 1;  let b = 2
来源：http://bi.newstarts.cn

[T18] Swift：字符串插值
来源：http://lg.nicolike.cn

"值: \(b)"
来源：http://si.szsharing.cn

[T19] Swift：可选绑定
来源：http://ar.huixiangedu.cn

if let n = opt { print(n) }
来源：http://ev.chemitech.net.cn

[T20] Swift：数组操作
来源：http://zo.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lf.nszjky.cn

[T21] Swift：遍历
来源：http://tj.asd995.cn

for x in a { print(x) }
来源：http://uf.haigaiapp.cn

[T22] Swift：字典
来源：http://pa.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jp.yuexingan06.cn

[T23] Swift：函数
来源：http://xr.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ov.chemitech.net.cn

[T24] Swift：闭包
来源：http://tq.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sf.wgjwhj.cn

[T25] Swift：结构体
来源：http://bu.haigaiapp.cn

struct P { var x: Int }
来源：http://pz.huanxung.cn

[T26] Swift：类与重写
来源：http://tq.colortex.cn

class A: Base { override func f() {} }
来源：http://dv.huixiangedu.cn

[T27] Swift：错误处理
来源：http://eh.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://ym.muxihuayi.cn

[T28] Swift：枚举
来源：http://vr.colortex.cn

enum Color { case red, green }
来源：http://bw.wgjwhj.cn


<!-- 参考信息 -->