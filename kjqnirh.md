代发 wailian999

echo "${#arr[@]}"
来源：http://nn.nicolike.cn

[R20] 关联数组（字典）
来源：http://fy.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rk.shxzukj.cn

[R21] 字符串长度
来源：http://js.nicolike.cn

echo "${#s}"
来源：http://uu.521024.cn

[R22] 截取子串
来源：http://rv.panjiajie.cn

echo "${s:0:5}"
来源：http://rc.shxzukj.cn

[R23] 字符串替换
来源：http://jc.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rs.chemitech.net.cn

[R24] 大小写转换
来源：http://hg.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ec.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://qk.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hy.gzmigu.cn

[R26] 命令替换
来源：http://lp.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://tg.jianghongdianzi.cn

[R27] 算术展开
来源：http://lt.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://zr.yuntaijiaju.cn

[R28] 浮点运算
来源：http://ze.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://ad.nszjky.cn

[R29] 定义函数
来源：http://ti.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ya.asd995.cn

[R30] 函数返回状态码
来源：http://pl.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://qh.huixiangedu.cn

[R31] 局部变量
来源：http://sm.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://pw.szsharing.cn

[R32] 参数个数校验
来源：http://xp.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eq.521024.cn

[R33] 捕获错误并提示行号
来源：http://hd.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zu.9csxet.cn

[R34] 退出时清理
来源：http://xb.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tg.colortex.cn

[R35] 后台执行并等待
来源：http://qn.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qh.huanxung.cn

[R36] 并发执行多个任务
来源：http://ls.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qu.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://cp.chemitech.net.cn

files=$(ls -1)
来源：http://zo.bjjhwx.cn

[R38] 管道串联
来源：http://nu.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://pu.521024.cn

[R39] 重定向标准输出与错误
来源：http://xy.yuexingan06.cn

cmd > out.log 2>&1
来源：http://ed.huixiangedu.cn

[R40] 追加写日志
来源：http://mv.yuntaijiaju.cn

echo "log" >> out.log
来源：http://im.hnjuh.cn

[R41] 丢弃输出
来源：http://br.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://jd.gzmigu.cn

[R42] 输入重定向
来源：http://xo.gzmigu.cn

wc -l < a.txt
来源：http://cj.hnjuh.cn

[R43] 按名字查找文件
来源：http://vy.wgjwhj.cn

find . -name "*.log" -type f
来源：http://lv.muxihuayi.cn

[R44] 按修改时间查找
来源：http://yp.nszjky.cn

find . -mtime -7 -type f
来源：http://xz.jctech888.com.cn

[R45] 批量删除
来源：http://nf.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://ol.asd995.cn

[R46] 递归替换文件内容
来源：http://oa.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mj.gzmigu.cn

[R47] sed 单行替换
来源：http://xv.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gt.bjjhwx.cn

[R48] awk 取指定列
来源：http://kd.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://ua.lnxyls.cn

[R49] awk 带条件
来源：http://ja.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wc.hnjuh.cn

[R50] awk 求和
来源：http://ai.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ui.muxihuayi.cn

[R51] 排序去重取前几
来源：http://rx.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xf.jianghongdianzi.cn

[R52] 统计行数
来源：http://gf.shxzskj.cn

wc -l a.txt
来源：http://mb.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://xt.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qk.asd995.cn

[R54] 比较两个文件
来源：http://rf.lnxyls.cn

diff a.txt b.txt
来源：http://xi.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://sm.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mz.szsharing.cn

[R56] 远程拷贝
来源：http://tz.hnjuh.cn

scp file user@host:/path/
来源：http://qk.szxytkj.cn

[R57] 远程执行命令
来源：http://wc.shtwfgs.cn

ssh user@host 'uptime'
来源：http://lt.521024.cn

[R58] 下载文件
来源：http://lt.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xs.jctech888.com.cn

[R59] 发 POST JSON
来源：http://qd.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jk.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://mr.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uf.9csxet.cn

[R61] 磁盘占用
来源：http://vm.newstarts.cn

df -h;  du -sh *
来源：http://ee.521024.cn

[R62] 找最占空间的文件
来源：http://vj.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://fv.jctech888.com.cn

[R63] 内存与进程
来源：http://ko.colortex.cn

free -h;  ps aux | grep nginx
来源：http://uu.bjjhwx.cn

[R64] 结束进程
来源：http://fh.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://aj.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://gf.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ve.muxihuayi.cn

[R66] 定时任务
来源：http://el.yuexingan06.cn

crontab -e;  crontab -l
来源：http://md.colortex.cn

[R67] 生成随机十六进制串
来源：http://om.nszjky.cn

openssl rand -hex 16
来源：http://sc.wgjwhj.cn

[R68] 计算文件校验值
来源：http://ne.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gn.colortex.cn

[R69] 生成随机密码
来源：http://ec.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://al.muxihuayi.cn

[R70] 时间戳与互转
来源：http://pd.nicolike.cn

date +%s;  date -d @1700000000
来源：http://ro.newstarts.cn

[R71] 日期格式化
来源：http://hm.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bv.haigaiapp.cn

[R72] 等待端口就绪
来源：http://io.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nm.panjiajie.cn

[R73] 分割大日志
来源：http://cl.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://nc.521024.cn

[R74] 批量重命名
来源：http://fo.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ds.521024.cn

[R75] 导出环境变量
来源：http://ap.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://ou.panjiajie.cn

[R76] 使用临时文件
来源：http://av.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nx.nszjky.cn

[R77] 读取用户输入
来源：http://hv.nicolike.cn

read -rp "请输入: " ans
来源：http://ok.521024.cn

[R78] 交互式菜单
来源：http://yb.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vs.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ij.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fr.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://nb.hnjuh.cn

time ./run.sh
来源：http://eo.gzmigu.cn

================================================================================
来源：http://ik.shxzukj.cn

S. C / C++ 专题
来源：http://ws.gzmigu.cn

================================================================================
来源：http://yy.521024.cn

[S01] C：Hello World
来源：http://dg.wgjwhj.cn

#include <stdio.h>
来源：http://pc.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ft.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://fx.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://ky.chemitech.net.cn

[S03] C：读入整数
来源：http://np.szxytkj.cn

int x; scanf("%d", &x);
来源：http://vt.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://ii.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sq.szxytkj.cn

[S05] C：字符串长度
来源：http://me.huanxung.cn

strlen(s)
来源：http://ei.szsharing.cn

[S06] C：字符串比较
来源：http://mb.521024.cn

strcmp(a, b) == 0
来源：http://qs.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://gr.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yo.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://pk.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zv.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://yr.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pz.lnxyls.cn

[S10] C：指针与解引用
来源：http://bm.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://ix.huanxung.cn

[S11] C：逐行读文件
来源：http://hm.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://un.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ch.colortex.cn

fclose(f);
来源：http://lm.chemitech.net.cn

[S12] C：写文件
来源：http://ll.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fn.wgjwhj.cn

[S13] C：宏定义
来源：http://kw.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yb.asd995.cn

[S14] C：枚举
来源：http://lq.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://qn.wgjwhj.cn

[S15] C：类型转换
来源：http://md.hnjuh.cn

(double) a / b
来源：http://wg.shxzskj.cn

[S16] C：位操作置位
来源：http://vb.panjiajie.cn

x |= (1 << 3);
来源：http://nq.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ab.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oj.jctech888.com.cn

[S18] C：命令行参数
来源：http://up.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://wx.nicolike.cn

[S19] C：快速排序
来源：http://mu.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lm.huanxung.cn

[S20] C：二分查找
来源：http://lo.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qo.shxzukj.cn

[S21] C：字符类别判断
来源：http://kg.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cm.haigaiapp.cn

[S22] C：字符串转数字
来源：http://rn.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kj.bjjhwx.cn

[S23] C：随机数
来源：http://gf.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zt.yuexingan06.cn

[S24] C：获取本地时间
来源：http://dy.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://er.shxzukj.cn

[S25] C：内存拷贝
来源：http://xo.huanxung.cn

memcpy(dst, src, n);
来源：http://tv.panjiajie.cn

[S26] C：内存清零
来源：http://hq.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://tl.chemitech.net.cn

[S27] C：定义常量
来源：http://cg.shxzskj.cn

const double PI = 3.14159;
来源：http://jk.hahajie.cn

[S28] C：静态变量
来源：http://rk.wgjwhj.cn

static int counter = 0;
来源：http://uh.colortex.cn

[S29] C：变参函数
来源：http://cs.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bq.nszjky.cn

[S30] C：头文件保护
来源：http://pb.yuntaijiaju.cn

#ifndef X_H
来源：http://vf.wgjwhj.cn

#define X_H
来源：http://kl.521024.cn

#endif
来源：http://rh.wgjwhj.cn

[S31] C++：Hello World
来源：http://te.9csxet.cn

#include <iostream>
来源：http://lj.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://dq.muxihuayi.cn

[S32] C++：字符串
来源：http://wd.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://mr.hnjuh.cn

[S33] C++：vector 增删
来源：http://zq.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ix.huanxung.cn

[S34] C++：遍历 vector
来源：http://rq.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://gv.huixiangedu.cn

[S35] C++：map
来源：http://hy.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vx.521024.cn

[S36] C++：unordered_map
来源：http://tg.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fm.shxzukj.cn

[S37] C++：set
来源：http://ki.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uo.bookmarksfly.cn

[S38] C++：排序
来源：http://gz.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://xl.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ym.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eu.9csxet.cn

[S40] C++：查找元素
来源：http://es.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yg.9csxet.cn

[S41] C++：类与构造函数
来源：http://wk.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qe.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://eu.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://ga.hahajie.cn

[S43] C++：智能指针
来源：http://nf.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://yu.gzmigu.cn

[S44] C++：引用传参
来源：http://jy.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://ep.lnxyls.cn

[S45] C++：lambda
来源：http://sj.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jn.huanxung.cn

[S46] C++：函数模板
来源：http://ty.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uz.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://bg.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gp.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ak.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wn.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://ol.bookmarksfly.cn

[S49] C++：写文件
来源：http://bn.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nu.hnjuh.cn

[S50] C++：格式化数字
来源：http://og.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pu.521024.cn

[S51] C++：显式类型转换
来源：http://kv.haigaiapp.cn

static_cast<double>(a) / b
来源：http://dq.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://fs.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://ic.9csxet.cn

[S53] C++：移动语义
来源：http://ml.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://nv.lnxyls.cn

[S54] C++：异常处理
来源：http://yh.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bh.szxytkj.cn

[S55] C++：结构化绑定
来源：http://zt.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ys.yuexingan06.cn

[S56] C++：optional
来源：http://en.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://om.shxzskj.cn

[S57] C++：编译期常量
来源：http://gp.bookmarksfly.cn

constexpr int N = 10;
来源：http://hv.wgjwhj.cn

[S58] C++：命名空间
来源：http://sj.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://xi.hahajie.cn

[S59] C++：静态断言
来源：http://ng.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vo.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://di.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jc.szxytkj.cn

================================================================================
来源：http://ns.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bc.bjjhwx.cn

================================================================================
来源：http://hn.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://df.nicolike.cn

println("Hello")
来源：http://sc.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://xb.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cv.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://iq.yuntaijiaju.cn

"值: $b"
来源：http://en.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ib.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://jy.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://es.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kg.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://kn.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oe.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ry.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ri.nszjky.cn

[T08] Kotlin：数据类
来源：http://sz.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://gv.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://xa.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://ys.hahajie.cn

[T10] Kotlin：默认参数
来源：http://te.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sl.bjjhwx.cn

[T11] Kotlin：协程
来源：http://sf.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nv.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://nu.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://qu.colortex.cn

[T13] Kotlin：只读 Map
来源：http://rz.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://kx.muxihuayi.cn

[T14] Kotlin：循环
来源：http://zo.asd995.cn

for (i in 1..10) println(i)
来源：http://ve.colortex.cn

[T15] Kotlin：接口
来源：http://bl.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://lk.hnjuh.cn

[T16] Swift：Hello World
来源：http://ty.szsharing.cn

print("Hello")
来源：http://dn.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://sh.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://mq.colortex.cn

[T18] Swift：字符串插值
来源：http://gx.asd995.cn

"值: \(b)"
来源：http://wa.huanxung.cn

[T19] Swift：可选绑定
来源：http://pz.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://dn.panjiajie.cn

[T20] Swift：数组操作
来源：http://dn.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xd.szxytkj.cn

[T21] Swift：遍历
来源：http://ai.shxzukj.cn

for x in a { print(x) }
来源：http://yz.bookmarksfly.cn

[T22] Swift：字典
来源：http://gc.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zh.wgjwhj.cn


<!-- 参考信息 -->