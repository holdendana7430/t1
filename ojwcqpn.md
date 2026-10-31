代发 wailian999

echo "${#s}"
来源：http://po.521024.cn

[R22] 截取子串
来源：http://hb.hahajie.cn

echo "${s:0:5}"
来源：http://zn.colortex.cn

[R23] 字符串替换
来源：http://hq.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yx.newstarts.cn

[R24] 大小写转换
来源：http://ew.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iv.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://vn.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cu.9csxet.cn

[R26] 命令替换
来源：http://jn.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://bi.9csxet.cn

[R27] 算术展开
来源：http://yu.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://ga.bookmarksfly.cn

[R28] 浮点运算
来源：http://xh.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://hu.lnxyls.cn

[R29] 定义函数
来源：http://ay.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aw.gzmigu.cn

[R30] 函数返回状态码
来源：http://eq.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://vq.colortex.cn

[R31] 局部变量
来源：http://ee.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://zf.szxytkj.cn

[R32] 参数个数校验
来源：http://tl.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fc.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://gv.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yr.shxzukj.cn

[R34] 退出时清理
来源：http://bw.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tn.muxihuayi.cn

[R35] 后台执行并等待
来源：http://rn.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qq.szsharing.cn

[R36] 并发执行多个任务
来源：http://qp.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ap.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://uw.huanxung.cn

files=$(ls -1)
来源：http://jm.bookmarksfly.cn

[R38] 管道串联
来源：http://ir.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://tx.hnjuh.cn

[R39] 重定向标准输出与错误
来源：http://bv.gzmigu.cn

cmd > out.log 2>&1
来源：http://zk.hnjuh.cn

[R40] 追加写日志
来源：http://dn.bjjhwx.cn

echo "log" >> out.log
来源：http://sb.nszjky.cn

[R41] 丢弃输出
来源：http://nb.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://es.szxytkj.cn

[R42] 输入重定向
来源：http://vq.chemitech.net.cn

wc -l < a.txt
来源：http://tz.szxytkj.cn

[R43] 按名字查找文件
来源：http://if.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://eo.nszjky.cn

[R44] 按修改时间查找
来源：http://qu.521024.cn

find . -mtime -7 -type f
来源：http://ai.bjjhwx.cn

[R45] 批量删除
来源：http://pa.asd995.cn

find . -name "*.tmp" -delete
来源：http://aj.szxytkj.cn

[R46] 递归替换文件内容
来源：http://ni.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rn.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://xp.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jk.nszjky.cn

[R48] awk 取指定列
来源：http://qk.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://uw.gzmigu.cn

[R49] awk 带条件
来源：http://mo.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jn.hnjuh.cn

[R50] awk 求和
来源：http://yp.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bs.newstarts.cn

[R51] 排序去重取前几
来源：http://vp.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://re.huixiangedu.cn

[R52] 统计行数
来源：http://ku.nicolike.cn

wc -l a.txt
来源：http://br.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://pp.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kw.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://bo.huixinmuqiang.cn

diff a.txt b.txt
来源：http://gm.muxihuayi.cn

[R55] 压缩与解压
来源：http://xl.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vv.nicolike.cn

[R56] 远程拷贝
来源：http://xm.shxzskj.cn

scp file user@host:/path/
来源：http://ko.shxzskj.cn

[R57] 远程执行命令
来源：http://dd.shtwfgs.cn

ssh user@host 'uptime'
来源：http://vr.yuntaijiaju.cn

[R58] 下载文件
来源：http://nr.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://md.shxzukj.cn

[R59] 发 POST JSON
来源：http://ya.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://la.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://ha.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xo.bookmarksfly.cn

[R61] 磁盘占用
来源：http://xt.yuntaijiaju.cn

df -h;  du -sh *
来源：http://ud.newstarts.cn

[R62] 找最占空间的文件
来源：http://ii.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ey.nicolike.cn

[R63] 内存与进程
来源：http://fh.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://fs.lnxyls.cn

[R64] 结束进程
来源：http://ye.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://ev.yuexingan06.cn

[R65] 查看端口占用
来源：http://ui.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qw.nicolike.cn

[R66] 定时任务
来源：http://eb.wgjwhj.cn

crontab -e;  crontab -l
来源：http://vx.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://ht.lnxyls.cn

openssl rand -hex 16
来源：http://bl.lnxyls.cn

[R68] 计算文件校验值
来源：http://xn.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tt.panjiajie.cn

[R69] 生成随机密码
来源：http://zh.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://dz.jctech888.com.cn

[R70] 时间戳与互转
来源：http://ir.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://lx.yuntaijiaju.cn

[R71] 日期格式化
来源：http://ur.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ys.521024.cn

[R72] 等待端口就绪
来源：http://zd.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zc.nszjky.cn

[R73] 分割大日志
来源：http://bq.shxzskj.cn

split -l 1000 big.log part_
来源：http://va.jianghongdianzi.cn

[R74] 批量重命名
来源：http://gf.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pf.haigaiapp.cn

[R75] 导出环境变量
来源：http://rb.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://uz.jctech888.com.cn

[R76] 使用临时文件
来源：http://jb.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://em.nicolike.cn

[R77] 读取用户输入
来源：http://as.szxytkj.cn

read -rp "请输入: " ans
来源：http://hg.bjjhwx.cn

[R78] 交互式菜单
来源：http://xv.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fz.521024.cn

[R79] 解析命令行选项
来源：http://ad.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nf.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://cv.shxzukj.cn

time ./run.sh
来源：http://gx.muxihuayi.cn

================================================================================
来源：http://tw.jctech888.com.cn

S. C / C++ 专题
来源：http://wl.lnxyls.cn

================================================================================
来源：http://da.chemitech.net.cn

[S01] C：Hello World
来源：http://ry.gzmigu.cn

#include <stdio.h>
来源：http://lo.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cz.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://gc.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://hc.panjiajie.cn

[S03] C：读入整数
来源：http://qb.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ml.huanxung.cn

[S04] C：字符串复制
来源：http://xm.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kg.521024.cn

[S05] C：字符串长度
来源：http://me.9csxet.cn

strlen(s)
来源：http://iy.szxytkj.cn

[S06] C：字符串比较
来源：http://zd.hahajie.cn

strcmp(a, b) == 0
来源：http://gq.9csxet.cn

[S07] C：数组遍历求和
来源：http://iu.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pu.asd995.cn

[S08] C：动态内存分配与释放
来源：http://vw.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vc.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://kq.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dg.huixiangedu.cn

[S10] C：指针与解引用
来源：http://op.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://fh.521024.cn

[S11] C：逐行读文件
来源：http://mz.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ab.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ks.chemitech.net.cn

fclose(f);
来源：http://ws.jctech888.com.cn

[S12] C：写文件
来源：http://xk.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://va.nszjky.cn

[S13] C：宏定义
来源：http://fl.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bd.colortex.cn

[S14] C：枚举
来源：http://le.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://xr.gzmigu.cn

[S15] C：类型转换
来源：http://kb.szxytkj.cn

(double) a / b
来源：http://qd.haigaiapp.cn

[S16] C：位操作置位
来源：http://dy.hahajie.cn

x |= (1 << 3);
来源：http://zg.nicolike.cn

[S17] C：安全拼接字符串
来源：http://ys.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zk.lnxyls.cn

[S18] C：命令行参数
来源：http://lj.lnxyls.cn

int main(int argc, char **argv)
来源：http://na.521024.cn

[S19] C：快速排序
来源：http://sz.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qx.newstarts.cn

[S20] C：二分查找
来源：http://uq.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wa.nicolike.cn

[S21] C：字符类别判断
来源：http://zs.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://su.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://ss.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vv.panjiajie.cn

[S23] C：随机数
来源：http://dd.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ba.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://oc.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://go.haigaiapp.cn

[S25] C：内存拷贝
来源：http://gj.newstarts.cn

memcpy(dst, src, n);
来源：http://xq.jianghongdianzi.cn

[S26] C：内存清零
来源：http://nz.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://ay.jctech888.com.cn

[S27] C：定义常量
来源：http://ao.gzmigu.cn

const double PI = 3.14159;
来源：http://xe.nicolike.cn

[S28] C：静态变量
来源：http://jy.jctech888.com.cn

static int counter = 0;
来源：http://pu.panjiajie.cn

[S29] C：变参函数
来源：http://xv.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xc.9csxet.cn

[S30] C：头文件保护
来源：http://yb.huixiangedu.cn

#ifndef X_H
来源：http://go.wgjwhj.cn

#define X_H
来源：http://jc.haigaiapp.cn

#endif
来源：http://eb.haigaiapp.cn

[S31] C++：Hello World
来源：http://qo.9csxet.cn

#include <iostream>
来源：http://ba.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://uy.shxzskj.cn

[S32] C++：字符串
来源：http://bq.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://nl.huanxung.cn

[S33] C++：vector 增删
来源：http://se.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hq.nszjky.cn

[S34] C++：遍历 vector
来源：http://nj.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://cx.jianghongdianzi.cn

[S35] C++：map
来源：http://hm.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rk.yuexingan06.cn

[S36] C++：unordered_map
来源：http://tg.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://km.9csxet.cn

[S37] C++：set
来源：http://le.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jv.hahajie.cn

[S38] C++：排序
来源：http://fa.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://jl.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://id.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kv.shxzukj.cn

[S40] C++：查找元素
来源：http://wj.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aa.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://un.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bq.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://vz.521024.cn

class B : public Base { public: void f() override {} };
来源：http://kx.shxzukj.cn

[S43] C++：智能指针
来源：http://pn.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://ps.muxihuayi.cn

[S44] C++：引用传参
来源：http://ql.nszjky.cn

void inc(int &x) { ++x; }
来源：http://ea.hnjuh.cn

[S45] C++：lambda
来源：http://ot.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wj.muxihuayi.cn

[S46] C++：函数模板
来源：http://jd.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wg.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://tw.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fa.gzmigu.cn

[S48] C++：逐行读文件
来源：http://cr.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ys.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://wd.muxihuayi.cn

[S49] C++：写文件
来源：http://vz.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xp.chemitech.net.cn

[S50] C++：格式化数字
来源：http://oa.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gb.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://ns.jctech888.com.cn

static_cast<double>(a) / b
来源：http://io.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://ia.huanxung.cn

int size() const noexcept { return n_; }
来源：http://yk.hnjuh.cn

[S53] C++：移动语义
来源：http://mw.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://qo.shxzskj.cn

[S54] C++：异常处理
来源：http://la.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bh.newstarts.cn

[S55] C++：结构化绑定
来源：http://ww.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lb.huanxung.cn

[S56] C++：optional
来源：http://cv.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ij.haigaiapp.cn

[S57] C++：编译期常量
来源：http://ar.newstarts.cn

constexpr int N = 10;
来源：http://ke.bjjhwx.cn

[S58] C++：命名空间
来源：http://tn.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://vx.huixiangedu.cn

[S59] C++：静态断言
来源：http://ox.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wv.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://hx.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yj.yuexingan06.cn

================================================================================
来源：http://bg.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pg.panjiajie.cn

================================================================================
来源：http://zq.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://qz.newstarts.cn

println("Hello")
来源：http://ql.521024.cn

[T02] Kotlin：变量
来源：http://ac.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wd.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://gx.yuntaijiaju.cn

"值: $b"
来源：http://xs.huanxung.cn

[T04] Kotlin：空安全
来源：http://vx.hnjuh.cn

val n: String? = null;  n?.length
来源：http://ij.521024.cn

[T05] Kotlin：when 表达式
来源：http://ht.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bn.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://yt.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://df.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://tw.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fv.panjiajie.cn

[T08] Kotlin：数据类
来源：http://mi.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://lr.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://ux.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://jh.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://st.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mo.szsharing.cn

[T11] Kotlin：协程
来源：http://iw.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dh.nszjky.cn

[T12] Kotlin：解构声明
来源：http://jv.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://hr.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://qy.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://dt.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://uj.szsharing.cn

for (i in 1..10) println(i)
来源：http://nw.shtwfgs.cn

[T15] Kotlin：接口
来源：http://ld.hahajie.cn

interface Shape { fun area(): Double }
来源：http://sz.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://jg.bjjhwx.cn

print("Hello")
来源：http://is.hahajie.cn

[T17] Swift：变量与常量
来源：http://pf.szsharing.cn

var a = 1;  let b = 2
来源：http://iq.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://xd.jianghongdianzi.cn

"值: \(b)"
来源：http://eu.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://sf.panjiajie.cn

if let n = opt { print(n) }
来源：http://ew.haigaiapp.cn

[T20] Swift：数组操作
来源：http://tx.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ai.chemitech.net.cn

[T21] Swift：遍历
来源：http://yy.nszjky.cn

for x in a { print(x) }
来源：http://be.yuexingan06.cn

[T22] Swift：字典
来源：http://li.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mx.gzmigu.cn

[T23] Swift：函数
来源：http://oi.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ez.521024.cn

[T24] Swift：闭包
来源：http://cz.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wx.szsharing.cn


<!-- 参考信息 -->