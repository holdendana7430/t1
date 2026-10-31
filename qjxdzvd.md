代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lk.jctech888.com.cn

[R24] 大小写转换
来源：http://qs.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qb.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://xb.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eh.szxytkj.cn

[R26] 命令替换
来源：http://vu.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://us.hnjuh.cn

[R27] 算术展开
来源：http://xg.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://sh.gzmigu.cn

[R28] 浮点运算
来源：http://en.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://uh.szsharing.cn

[R29] 定义函数
来源：http://tu.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ar.newstarts.cn

[R30] 函数返回状态码
来源：http://bb.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://gg.hnjuh.cn

[R31] 局部变量
来源：http://ew.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://rf.bjjhwx.cn

[R32] 参数个数校验
来源：http://xl.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gw.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://tz.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://os.chemitech.net.cn

[R34] 退出时清理
来源：http://dn.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dx.haigaiapp.cn

[R35] 后台执行并等待
来源：http://mh.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ev.nicolike.cn

[R36] 并发执行多个任务
来源：http://ah.jianghongdianzi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://te.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://ew.nicolike.cn

files=$(ls -1)
来源：http://jh.hnjuh.cn

[R38] 管道串联
来源：http://yo.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ak.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://mi.asd995.cn

cmd > out.log 2>&1
来源：http://az.panjiajie.cn

[R40] 追加写日志
来源：http://wm.yuexingan06.cn

echo "log" >> out.log
来源：http://jo.9csxet.cn

[R41] 丢弃输出
来源：http://uw.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://wd.9csxet.cn

[R42] 输入重定向
来源：http://pt.shxzskj.cn

wc -l < a.txt
来源：http://tl.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://zo.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://fv.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://nq.haigaiapp.cn

find . -mtime -7 -type f
来源：http://sm.shxzukj.cn

[R45] 批量删除
来源：http://ej.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://zi.nszjky.cn

[R46] 递归替换文件内容
来源：http://dl.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bm.521024.cn

[R47] sed 单行替换
来源：http://zy.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dp.yuexingan06.cn

[R48] awk 取指定列
来源：http://ty.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://xo.yuntaijiaju.cn

[R49] awk 带条件
来源：http://ps.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xm.shxzskj.cn

[R50] awk 求和
来源：http://mv.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mj.colortex.cn

[R51] 排序去重取前几
来源：http://sd.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wh.jianghongdianzi.cn

[R52] 统计行数
来源：http://qk.gzmigu.cn

wc -l a.txt
来源：http://wd.colortex.cn

[R53] 查看文件头与实时尾
来源：http://cx.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ua.colortex.cn

[R54] 比较两个文件
来源：http://df.jianghongdianzi.cn

diff a.txt b.txt
来源：http://ft.lnxyls.cn

[R55] 压缩与解压
来源：http://xj.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ee.hnjuh.cn

[R56] 远程拷贝
来源：http://ml.shtwfgs.cn

scp file user@host:/path/
来源：http://oc.huixiangedu.cn

[R57] 远程执行命令
来源：http://ms.nszjky.cn

ssh user@host 'uptime'
来源：http://tp.huanxung.cn

[R58] 下载文件
来源：http://vw.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vb.bjjhwx.cn

[R59] 发 POST JSON
来源：http://cl.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ho.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://jl.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ll.nszjky.cn

[R61] 磁盘占用
来源：http://ok.newstarts.cn

df -h;  du -sh *
来源：http://jm.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://ny.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ul.hnjuh.cn

[R63] 内存与进程
来源：http://jz.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://dt.asd995.cn

[R64] 结束进程
来源：http://ui.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://bm.jctech888.com.cn

[R65] 查看端口占用
来源：http://vk.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://af.bookmarksfly.cn

[R66] 定时任务
来源：http://dh.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://vm.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://xo.bookmarksfly.cn

openssl rand -hex 16
来源：http://aj.521024.cn

[R68] 计算文件校验值
来源：http://hj.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://di.panjiajie.cn

[R69] 生成随机密码
来源：http://iz.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://yh.chemitech.net.cn

[R70] 时间戳与互转
来源：http://pc.hahajie.cn

date +%s;  date -d @1700000000
来源：http://oh.hahajie.cn

[R71] 日期格式化
来源：http://et.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fc.asd995.cn

[R72] 等待端口就绪
来源：http://nm.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ec.jianghongdianzi.cn

[R73] 分割大日志
来源：http://xg.jctech888.com.cn

split -l 1000 big.log part_
来源：http://rg.huixiangedu.cn

[R74] 批量重命名
来源：http://ed.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dc.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ml.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://ne.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://th.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wf.jctech888.com.cn

[R77] 读取用户输入
来源：http://zv.bjjhwx.cn

read -rp "请输入: " ans
来源：http://sb.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://kt.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pj.huixiangedu.cn

[R79] 解析命令行选项
来源：http://as.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ey.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://lz.shxzukj.cn

time ./run.sh
来源：http://sg.521024.cn

================================================================================
来源：http://nt.jctech888.com.cn

S. C / C++ 专题
来源：http://rw.hnjuh.cn

================================================================================
来源：http://ki.haigaiapp.cn

[S01] C：Hello World
来源：http://po.newstarts.cn

#include <stdio.h>
来源：http://jf.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fu.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://na.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://hc.521024.cn

[S03] C：读入整数
来源：http://yw.521024.cn

int x; scanf("%d", &x);
来源：http://rv.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://yf.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://to.jctech888.com.cn

[S05] C：字符串长度
来源：http://zy.9csxet.cn

strlen(s)
来源：http://qn.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://zx.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://lu.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://wb.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://in.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://qa.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tc.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://fh.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rs.huanxung.cn

[S10] C：指针与解引用
来源：http://lj.huanxung.cn

int *p = &a;  *p = 5;
来源：http://hd.shtwfgs.cn

[S11] C：逐行读文件
来源：http://sj.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://sw.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://go.huixiangedu.cn

fclose(f);
来源：http://tg.szsharing.cn

[S12] C：写文件
来源：http://en.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ui.bjjhwx.cn

[S13] C：宏定义
来源：http://vr.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cq.szxytkj.cn

[S14] C：枚举
来源：http://jf.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://lf.asd995.cn

[S15] C：类型转换
来源：http://ej.shxzskj.cn

(double) a / b
来源：http://ez.wgjwhj.cn

[S16] C：位操作置位
来源：http://jg.shtwfgs.cn

x |= (1 << 3);
来源：http://vt.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://dh.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pr.yuexingan06.cn

[S18] C：命令行参数
来源：http://po.chemitech.net.cn

int main(int argc, char **argv)
来源：http://yv.shtwfgs.cn

[S19] C：快速排序
来源：http://md.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ot.muxihuayi.cn

[S20] C：二分查找
来源：http://wq.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://al.panjiajie.cn

[S21] C：字符类别判断
来源：http://nz.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xy.haigaiapp.cn

[S22] C：字符串转数字
来源：http://kt.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ta.gzmigu.cn

[S23] C：随机数
来源：http://qn.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ot.haigaiapp.cn

[S24] C：获取本地时间
来源：http://sy.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zq.521024.cn

[S25] C：内存拷贝
来源：http://em.haigaiapp.cn

memcpy(dst, src, n);
来源：http://nd.yuntaijiaju.cn

[S26] C：内存清零
来源：http://sr.newstarts.cn

memset(a, 0, sizeof a);
来源：http://ru.521024.cn

[S27] C：定义常量
来源：http://of.haigaiapp.cn

const double PI = 3.14159;
来源：http://pn.szxytkj.cn

[S28] C：静态变量
来源：http://tp.nszjky.cn

static int counter = 0;
来源：http://gq.hahajie.cn

[S29] C：变参函数
来源：http://xc.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jl.shxzskj.cn

[S30] C：头文件保护
来源：http://lc.muxihuayi.cn

#ifndef X_H
来源：http://to.bjjhwx.cn

#define X_H
来源：http://es.muxihuayi.cn

#endif
来源：http://se.asd995.cn

[S31] C++：Hello World
来源：http://an.huixiangedu.cn

#include <iostream>
来源：http://db.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://zz.yuntaijiaju.cn

[S32] C++：字符串
来源：http://bl.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://fz.lnxyls.cn

[S33] C++：vector 增删
来源：http://xj.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gm.szxytkj.cn

[S34] C++：遍历 vector
来源：http://ye.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://bi.shtwfgs.cn

[S35] C++：map
来源：http://td.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jv.hahajie.cn

[S36] C++：unordered_map
来源：http://qt.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tn.huixinmuqiang.cn

[S37] C++：set
来源：http://gb.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pq.nicolike.cn

[S38] C++：排序
来源：http://rb.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://wv.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://yh.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bb.muxihuayi.cn

[S40] C++：查找元素
来源：http://by.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qs.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://jm.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://er.521024.cn

[S42] C++：继承与虚函数
来源：http://os.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://fc.shxzskj.cn

[S43] C++：智能指针
来源：http://mc.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://dv.jctech888.com.cn

[S44] C++：引用传参
来源：http://cf.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://gi.newstarts.cn

[S45] C++：lambda
来源：http://xn.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zi.gzmigu.cn

[S46] C++：函数模板
来源：http://cy.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iz.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://ev.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qw.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://st.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tm.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://yi.huixinmuqiang.cn

[S49] C++：写文件
来源：http://on.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nq.lnxyls.cn

[S50] C++：格式化数字
来源：http://wa.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yr.shxzukj.cn

[S51] C++：显式类型转换
来源：http://zq.hnjuh.cn

static_cast<double>(a) / b
来源：http://kv.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://qn.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://cw.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://ua.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://sq.shxzskj.cn

[S54] C++：异常处理
来源：http://oc.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uu.521024.cn

[S55] C++：结构化绑定
来源：http://ak.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oa.nicolike.cn

[S56] C++：optional
来源：http://ab.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wn.asd995.cn

[S57] C++：编译期常量
来源：http://hj.gzmigu.cn

constexpr int N = 10;
来源：http://rx.huanxung.cn

[S58] C++：命名空间
来源：http://ja.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://cn.shxzukj.cn

[S59] C++：静态断言
来源：http://eb.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kg.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://xd.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wq.yuexingan06.cn

================================================================================
来源：http://up.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jc.jianghongdianzi.cn

================================================================================
来源：http://kp.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://fe.muxihuayi.cn

println("Hello")
来源：http://xn.9csxet.cn

[T02] Kotlin：变量
来源：http://xr.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ht.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://lc.chemitech.net.cn

"值: $b"
来源：http://fi.521024.cn

[T04] Kotlin：空安全
来源：http://ha.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://qb.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://wh.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zm.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://ny.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yd.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://vh.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vw.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://ae.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://lh.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://sn.colortex.cn

fun String.exclaim() = this + "!"
来源：http://hh.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://is.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gn.521024.cn

[T11] Kotlin：协程
来源：http://fi.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://az.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://fj.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://bs.shxzskj.cn

[T13] Kotlin：只读 Map
来源：http://sp.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://zw.szsharing.cn

[T14] Kotlin：循环
来源：http://nb.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://ef.9csxet.cn

[T15] Kotlin：接口
来源：http://pt.huanxung.cn

interface Shape { fun area(): Double }
来源：http://la.haigaiapp.cn

[T16] Swift：Hello World
来源：http://pm.bjjhwx.cn

print("Hello")
来源：http://hh.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://sk.szsharing.cn

var a = 1;  let b = 2
来源：http://mg.colortex.cn

[T18] Swift：字符串插值
来源：http://hj.muxihuayi.cn

"值: \(b)"
来源：http://le.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://wg.chemitech.net.cn

if let n = opt { print(n) }
来源：http://qw.wgjwhj.cn

[T20] Swift：数组操作
来源：http://fl.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kd.asd995.cn

[T21] Swift：遍历
来源：http://xf.nicolike.cn

for x in a { print(x) }
来源：http://ox.hnjuh.cn

[T22] Swift：字典
来源：http://gv.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://no.haigaiapp.cn

[T23] Swift：函数
来源：http://xt.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yl.shxzukj.cn

[T24] Swift：闭包
来源：http://vb.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xs.newstarts.cn

[T25] Swift：结构体
来源：http://nu.jianghongdianzi.cn

struct P { var x: Int }
来源：http://wu.9csxet.cn

[T26] Swift：类与重写
来源：http://qu.521024.cn

class A: Base { override func f() {} }
来源：http://at.gzmigu.cn


<!-- 参考信息 -->