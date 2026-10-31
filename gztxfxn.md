代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://qc.huixiangedu.cn

[R26] 命令替换
来源：http://oe.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://ys.shxzskj.cn

[R27] 算术展开
来源：http://ga.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://jc.huixiangedu.cn

[R28] 浮点运算
来源：http://ao.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://dl.chemitech.net.cn

[R29] 定义函数
来源：http://we.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ll.hnjuh.cn

[R30] 函数返回状态码
来源：http://wq.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://mi.asd995.cn

[R31] 局部变量
来源：http://zx.521024.cn

f() { local x=1; echo "$x"; }
来源：http://gb.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://kr.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fj.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://zi.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://af.gzmigu.cn

[R34] 退出时清理
来源：http://sf.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iq.bjjhwx.cn

[R35] 后台执行并等待
来源：http://dt.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xu.9csxet.cn

[R36] 并发执行多个任务
来源：http://nk.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yx.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://ez.nszjky.cn

files=$(ls -1)
来源：http://jl.huixiangedu.cn

[R38] 管道串联
来源：http://ru.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://lz.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://qn.hnjuh.cn

cmd > out.log 2>&1
来源：http://bw.hnjuh.cn

[R40] 追加写日志
来源：http://xq.haigaiapp.cn

echo "log" >> out.log
来源：http://jl.colortex.cn

[R41] 丢弃输出
来源：http://wb.521024.cn

cmd >/dev/null 2>&1
来源：http://yi.shxzukj.cn

[R42] 输入重定向
来源：http://zk.huixinmuqiang.cn

wc -l < a.txt
来源：http://fr.shtwfgs.cn

[R43] 按名字查找文件
来源：http://fz.hnjuh.cn

find . -name "*.log" -type f
来源：http://wh.muxihuayi.cn

[R44] 按修改时间查找
来源：http://at.9csxet.cn

find . -mtime -7 -type f
来源：http://sq.lnxyls.cn

[R45] 批量删除
来源：http://zi.9csxet.cn

find . -name "*.tmp" -delete
来源：http://ip.hahajie.cn

[R46] 递归替换文件内容
来源：http://fz.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uu.bookmarksfly.cn

[R47] sed 单行替换
来源：http://hd.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tc.newstarts.cn

[R48] awk 取指定列
来源：http://na.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://qg.yuntaijiaju.cn

[R49] awk 带条件
来源：http://pc.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uw.wgjwhj.cn

[R50] awk 求和
来源：http://re.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sf.chemitech.net.cn

[R51] 排序去重取前几
来源：http://bc.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nq.jctech888.com.cn

[R52] 统计行数
来源：http://dh.lnxyls.cn

wc -l a.txt
来源：http://yt.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ly.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xj.asd995.cn

[R54] 比较两个文件
来源：http://pe.huixiangedu.cn

diff a.txt b.txt
来源：http://ch.huixiangedu.cn

[R55] 压缩与解压
来源：http://it.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ly.huanxung.cn

[R56] 远程拷贝
来源：http://qx.yuexingan06.cn

scp file user@host:/path/
来源：http://th.jctech888.com.cn

[R57] 远程执行命令
来源：http://wz.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ty.haigaiapp.cn

[R58] 下载文件
来源：http://sw.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dl.muxihuayi.cn

[R59] 发 POST JSON
来源：http://nd.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://km.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://fh.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vf.colortex.cn

[R61] 磁盘占用
来源：http://yp.hnjuh.cn

df -h;  du -sh *
来源：http://iw.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://jk.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://ys.colortex.cn

[R63] 内存与进程
来源：http://jz.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://si.huixiangedu.cn

[R64] 结束进程
来源：http://zm.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://hn.huanxung.cn

[R65] 查看端口占用
来源：http://ua.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ak.nszjky.cn

[R66] 定时任务
来源：http://lq.nszjky.cn

crontab -e;  crontab -l
来源：http://dp.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://kh.521024.cn

openssl rand -hex 16
来源：http://xp.chemitech.net.cn

[R68] 计算文件校验值
来源：http://hi.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://re.gzmigu.cn

[R69] 生成随机密码
来源：http://he.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://tg.nszjky.cn

[R70] 时间戳与互转
来源：http://fq.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://bn.haigaiapp.cn

[R71] 日期格式化
来源：http://sp.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vg.huixiangedu.cn

[R72] 等待端口就绪
来源：http://ie.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mo.chemitech.net.cn

[R73] 分割大日志
来源：http://vm.hnjuh.cn

split -l 1000 big.log part_
来源：http://ro.asd995.cn

[R74] 批量重命名
来源：http://vk.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mi.wgjwhj.cn

[R75] 导出环境变量
来源：http://sj.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://xq.bjjhwx.cn

[R76] 使用临时文件
来源：http://nc.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ts.wgjwhj.cn

[R77] 读取用户输入
来源：http://xw.huanxung.cn

read -rp "请输入: " ans
来源：http://qx.huixiangedu.cn

[R78] 交互式菜单
来源：http://xh.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://de.szsharing.cn

[R79] 解析命令行选项
来源：http://uo.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fy.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://xg.hnjuh.cn

time ./run.sh
来源：http://bw.jianghongdianzi.cn

================================================================================
来源：http://ef.shxzukj.cn

S. C / C++ 专题
来源：http://vs.bookmarksfly.cn

================================================================================
来源：http://cl.bjjhwx.cn

[S01] C：Hello World
来源：http://qc.shtwfgs.cn

#include <stdio.h>
来源：http://kb.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ak.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://nh.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://gf.9csxet.cn

[S03] C：读入整数
来源：http://bu.szsharing.cn

int x; scanf("%d", &x);
来源：http://vs.colortex.cn

[S04] C：字符串复制
来源：http://cf.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lq.gzmigu.cn

[S05] C：字符串长度
来源：http://pv.bjjhwx.cn

strlen(s)
来源：http://na.hahajie.cn

[S06] C：字符串比较
来源：http://rz.haigaiapp.cn

strcmp(a, b) == 0
来源：http://ph.9csxet.cn

[S07] C：数组遍历求和
来源：http://rw.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ye.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://rb.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xx.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://yc.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wy.szxytkj.cn

[S10] C：指针与解引用
来源：http://ok.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://wf.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://tw.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://oi.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uo.nicolike.cn

fclose(f);
来源：http://hj.yuexingan06.cn

[S12] C：写文件
来源：http://hj.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sr.panjiajie.cn

[S13] C：宏定义
来源：http://jb.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qe.huixiangedu.cn

[S14] C：枚举
来源：http://jq.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://yj.shtwfgs.cn

[S15] C：类型转换
来源：http://ah.huixiangedu.cn

(double) a / b
来源：http://us.panjiajie.cn

[S16] C：位操作置位
来源：http://eh.huixinmuqiang.cn

x |= (1 << 3);
来源：http://yp.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://ty.huixiangedu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uh.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://rd.szsharing.cn

int main(int argc, char **argv)
来源：http://lm.yuexingan06.cn

[S19] C：快速排序
来源：http://bi.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://se.shxzukj.cn

[S20] C：二分查找
来源：http://me.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gq.jctech888.com.cn

[S21] C：字符类别判断
来源：http://ka.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://il.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://hy.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cb.szsharing.cn

[S23] C：随机数
来源：http://yj.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hg.yuexingan06.cn

[S24] C：获取本地时间
来源：http://uj.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://me.szsharing.cn

[S25] C：内存拷贝
来源：http://qw.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://wa.gzmigu.cn

[S26] C：内存清零
来源：http://bx.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://et.newstarts.cn

[S27] C：定义常量
来源：http://qa.szxytkj.cn

const double PI = 3.14159;
来源：http://iv.shxzskj.cn

[S28] C：静态变量
来源：http://sd.yuexingan06.cn

static int counter = 0;
来源：http://tb.bookmarksfly.cn

[S29] C：变参函数
来源：http://et.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jc.yuexingan06.cn

[S30] C：头文件保护
来源：http://tb.bookmarksfly.cn

#ifndef X_H
来源：http://uf.muxihuayi.cn

#define X_H
来源：http://kb.shxzskj.cn

#endif
来源：http://dj.chemitech.net.cn

[S31] C++：Hello World
来源：http://cf.shxzukj.cn

#include <iostream>
来源：http://zu.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://tz.bjjhwx.cn

[S32] C++：字符串
来源：http://zc.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://ri.shtwfgs.cn

[S33] C++：vector 增删
来源：http://gn.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kt.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://vr.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://tf.lnxyls.cn

[S35] C++：map
来源：http://lp.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ux.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://uh.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vh.yuntaijiaju.cn

[S37] C++：set
来源：http://tp.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uj.bjjhwx.cn

[S38] C++：排序
来源：http://tl.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://ks.521024.cn

[S39] C++：自定义比较器排序
来源：http://np.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ee.shxzskj.cn

[S40] C++：查找元素
来源：http://uo.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vl.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://vw.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wk.szsharing.cn

[S42] C++：继承与虚函数
来源：http://as.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://dw.haigaiapp.cn

[S43] C++：智能指针
来源：http://wu.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://bx.szxytkj.cn

[S44] C++：引用传参
来源：http://gs.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://gz.shxzukj.cn

[S45] C++：lambda
来源：http://rl.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bq.muxihuayi.cn

[S46] C++：函数模板
来源：http://un.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fw.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://sz.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uv.shxzukj.cn

[S48] C++：逐行读文件
来源：http://ts.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kd.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://qq.chemitech.net.cn

[S49] C++：写文件
来源：http://ub.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ez.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://ft.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sl.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://bg.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://vn.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://ue.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://oq.bookmarksfly.cn

[S53] C++：移动语义
来源：http://mq.521024.cn

std::vector<int> w = std::move(v);
来源：http://yc.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://qx.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bs.hnjuh.cn

[S55] C++：结构化绑定
来源：http://kk.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nx.lnxyls.cn

[S56] C++：optional
来源：http://bg.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hh.chemitech.net.cn

[S57] C++：编译期常量
来源：http://fw.huanxung.cn

constexpr int N = 10;
来源：http://xm.bjjhwx.cn

[S58] C++：命名空间
来源：http://br.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://ak.asd995.cn

[S59] C++：静态断言
来源：http://zb.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sk.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://nv.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xc.shxzukj.cn

================================================================================
来源：http://kt.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wg.shtwfgs.cn

================================================================================
来源：http://in.nszjky.cn

[T01] Kotlin：Hello World
来源：http://vj.jctech888.com.cn

println("Hello")
来源：http://ur.gzmigu.cn

[T02] Kotlin：变量
来源：http://hg.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dr.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://vc.huixiangedu.cn

"值: $b"
来源：http://nb.huanxung.cn

[T04] Kotlin：空安全
来源：http://xg.szxytkj.cn

val n: String? = null;  n?.length
来源：http://ia.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ln.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ji.nszjky.cn

[T06] Kotlin：集合映射
来源：http://ik.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xz.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://co.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jj.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://yl.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://nh.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://vm.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://wv.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://tr.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jr.lnxyls.cn

[T11] Kotlin：协程
来源：http://jt.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nv.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://rp.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://hs.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://cu.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://nx.haigaiapp.cn

[T14] Kotlin：循环
来源：http://zl.asd995.cn

for (i in 1..10) println(i)
来源：http://io.szxytkj.cn

[T15] Kotlin：接口
来源：http://nj.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://li.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://xd.yuntaijiaju.cn

print("Hello")
来源：http://ge.hahajie.cn

[T17] Swift：变量与常量
来源：http://wz.521024.cn

var a = 1;  let b = 2
来源：http://zh.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://gz.shxzukj.cn

"值: \(b)"
来源：http://so.nszjky.cn

[T19] Swift：可选绑定
来源：http://pj.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://fp.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://mk.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vm.gzmigu.cn

[T21] Swift：遍历
来源：http://zn.jianghongdianzi.cn

for x in a { print(x) }
来源：http://kp.szsharing.cn

[T22] Swift：字典
来源：http://ea.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qz.hnjuh.cn

[T23] Swift：函数
来源：http://hh.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oh.bookmarksfly.cn

[T24] Swift：闭包
来源：http://dg.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ni.521024.cn

[T25] Swift：结构体
来源：http://sa.yuntaijiaju.cn

struct P { var x: Int }
来源：http://dh.lnxyls.cn

[T26] Swift：类与重写
来源：http://cx.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://wk.haigaiapp.cn

[T27] Swift：错误处理
来源：http://aa.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://lz.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://lv.newstarts.cn

enum Color { case red, green }
来源：http://de.hahajie.cn


<!-- 参考信息 -->