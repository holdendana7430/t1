代发 wailian999

echo "${#s}"
来源：http://ie.panjiajie.cn

[R22] 截取子串
来源：http://su.muxihuayi.cn

echo "${s:0:5}"
来源：http://zn.gzmigu.cn

[R23] 字符串替换
来源：http://ll.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mx.muxihuayi.cn

[R24] 大小写转换
来源：http://hu.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ra.521024.cn

[R25] 去后缀 / 去前缀
来源：http://yi.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tx.colortex.cn

[R26] 命令替换
来源：http://py.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://ot.colortex.cn

[R27] 算术展开
来源：http://yi.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://ts.shtwfgs.cn

[R28] 浮点运算
来源：http://wp.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://yn.521024.cn

[R29] 定义函数
来源：http://kj.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tx.szsharing.cn

[R30] 函数返回状态码
来源：http://og.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://dw.muxihuayi.cn

[R31] 局部变量
来源：http://et.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://ef.wgjwhj.cn

[R32] 参数个数校验
来源：http://cx.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rx.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://id.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qa.muxihuayi.cn

[R34] 退出时清理
来源：http://kh.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xo.jctech888.com.cn

[R35] 后台执行并等待
来源：http://se.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xt.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://hb.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bw.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://vk.huixinmuqiang.cn

files=$(ls -1)
来源：http://jw.chemitech.net.cn

[R38] 管道串联
来源：http://lb.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://ja.521024.cn

[R39] 重定向标准输出与错误
来源：http://as.panjiajie.cn

cmd > out.log 2>&1
来源：http://zk.shtwfgs.cn

[R40] 追加写日志
来源：http://vt.szxytkj.cn

echo "log" >> out.log
来源：http://bf.bjjhwx.cn

[R41] 丢弃输出
来源：http://gs.colortex.cn

cmd >/dev/null 2>&1
来源：http://ko.huanxung.cn

[R42] 输入重定向
来源：http://hc.colortex.cn

wc -l < a.txt
来源：http://rd.haigaiapp.cn

[R43] 按名字查找文件
来源：http://xg.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://zy.nicolike.cn

[R44] 按修改时间查找
来源：http://ud.colortex.cn

find . -mtime -7 -type f
来源：http://io.nszjky.cn

[R45] 批量删除
来源：http://hq.nicolike.cn

find . -name "*.tmp" -delete
来源：http://zf.lnxyls.cn

[R46] 递归替换文件内容
来源：http://fy.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hv.panjiajie.cn

[R47] sed 单行替换
来源：http://qx.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jr.muxihuayi.cn

[R48] awk 取指定列
来源：http://fb.521024.cn

awk '{print $1, $3}' a.txt
来源：http://ft.gzmigu.cn

[R49] awk 带条件
来源：http://ws.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://is.jctech888.com.cn

[R50] awk 求和
来源：http://ga.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jr.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://yw.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gy.jctech888.com.cn

[R52] 统计行数
来源：http://ly.muxihuayi.cn

wc -l a.txt
来源：http://zh.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://nt.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fh.haigaiapp.cn

[R54] 比较两个文件
来源：http://zv.lnxyls.cn

diff a.txt b.txt
来源：http://nj.nicolike.cn

[R55] 压缩与解压
来源：http://ly.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uz.shtwfgs.cn

[R56] 远程拷贝
来源：http://km.hahajie.cn

scp file user@host:/path/
来源：http://au.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://ti.hahajie.cn

ssh user@host 'uptime'
来源：http://zp.huanxung.cn

[R58] 下载文件
来源：http://oy.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vi.521024.cn

[R59] 发 POST JSON
来源：http://ft.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://os.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://jd.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rl.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://cm.nicolike.cn

df -h;  du -sh *
来源：http://nr.nicolike.cn

[R62] 找最占空间的文件
来源：http://jx.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://wm.521024.cn

[R63] 内存与进程
来源：http://jr.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://ww.asd995.cn

[R64] 结束进程
来源：http://ke.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://ar.panjiajie.cn

[R65] 查看端口占用
来源：http://lf.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ht.shxzukj.cn

[R66] 定时任务
来源：http://qj.szxytkj.cn

crontab -e;  crontab -l
来源：http://kb.szsharing.cn

[R67] 生成随机十六进制串
来源：http://tn.szxytkj.cn

openssl rand -hex 16
来源：http://mi.shxzukj.cn

[R68] 计算文件校验值
来源：http://ep.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qh.lnxyls.cn

[R69] 生成随机密码
来源：http://no.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://ce.nicolike.cn

[R70] 时间戳与互转
来源：http://zk.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://kj.jianghongdianzi.cn

[R71] 日期格式化
来源：http://el.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lk.521024.cn

[R72] 等待端口就绪
来源：http://ci.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eq.szsharing.cn

[R73] 分割大日志
来源：http://iz.huixiangedu.cn

split -l 1000 big.log part_
来源：http://fd.bjjhwx.cn

[R74] 批量重命名
来源：http://jh.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gy.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://gd.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://ck.haigaiapp.cn

[R76] 使用临时文件
来源：http://xf.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tu.lnxyls.cn

[R77] 读取用户输入
来源：http://ph.colortex.cn

read -rp "请输入: " ans
来源：http://um.szsharing.cn

[R78] 交互式菜单
来源：http://ux.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zt.bjjhwx.cn

[R79] 解析命令行选项
来源：http://bw.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tq.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://nb.jianghongdianzi.cn

time ./run.sh
来源：http://fq.bjjhwx.cn

================================================================================
来源：http://ru.gzmigu.cn

S. C / C++ 专题
来源：http://db.bjjhwx.cn

================================================================================
来源：http://rp.colortex.cn

[S01] C：Hello World
来源：http://fm.szxytkj.cn

#include <stdio.h>
来源：http://ae.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bj.asd995.cn

[S02] C：变量与格式化输出
来源：http://md.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://sj.huixinmuqiang.cn

[S03] C：读入整数
来源：http://oi.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://nu.bjjhwx.cn

[S04] C：字符串复制
来源：http://mg.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dy.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://oh.szxytkj.cn

strlen(s)
来源：http://um.colortex.cn

[S06] C：字符串比较
来源：http://nw.lnxyls.cn

strcmp(a, b) == 0
来源：http://so.huanxung.cn

[S07] C：数组遍历求和
来源：http://rx.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zp.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://st.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ni.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://hk.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yt.szsharing.cn

[S10] C：指针与解引用
来源：http://rz.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ny.newstarts.cn

[S11] C：逐行读文件
来源：http://zl.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://jn.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uu.lnxyls.cn

fclose(f);
来源：http://gn.panjiajie.cn

[S12] C：写文件
来源：http://xp.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ge.lnxyls.cn

[S13] C：宏定义
来源：http://hr.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ip.gzmigu.cn

[S14] C：枚举
来源：http://td.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://yz.shxzukj.cn

[S15] C：类型转换
来源：http://zo.shtwfgs.cn

(double) a / b
来源：http://qx.521024.cn

[S16] C：位操作置位
来源：http://oa.huixinmuqiang.cn

x |= (1 << 3);
来源：http://su.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://qh.bjjhwx.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wz.jctech888.com.cn

[S18] C：命令行参数
来源：http://rb.chemitech.net.cn

int main(int argc, char **argv)
来源：http://ta.yuntaijiaju.cn

[S19] C：快速排序
来源：http://un.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ik.hnjuh.cn

[S20] C：二分查找
来源：http://ic.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gzmigu.cn

[S21] C：字符类别判断
来源：http://rr.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uw.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://mu.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qe.newstarts.cn

[S23] C：随机数
来源：http://xc.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kp.9csxet.cn

[S24] C：获取本地时间
来源：http://gh.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ut.shxzukj.cn

[S25] C：内存拷贝
来源：http://go.chemitech.net.cn

memcpy(dst, src, n);
来源：http://cg.521024.cn

[S26] C：内存清零
来源：http://kg.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://de.bjjhwx.cn

[S27] C：定义常量
来源：http://gd.hahajie.cn

const double PI = 3.14159;
来源：http://ug.gzmigu.cn

[S28] C：静态变量
来源：http://db.shxzskj.cn

static int counter = 0;
来源：http://bs.bookmarksfly.cn

[S29] C：变参函数
来源：http://rw.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lz.szsharing.cn

[S30] C：头文件保护
来源：http://pz.shxzskj.cn

#ifndef X_H
来源：http://cr.colortex.cn

#define X_H
来源：http://ry.szsharing.cn

#endif
来源：http://uo.hahajie.cn

[S31] C++：Hello World
来源：http://ba.521024.cn

#include <iostream>
来源：http://fk.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ml.panjiajie.cn

[S32] C++：字符串
来源：http://jh.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://vk.hahajie.cn

[S33] C++：vector 增删
来源：http://ll.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ys.nicolike.cn

[S34] C++：遍历 vector
来源：http://qo.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://po.colortex.cn

[S35] C++：map
来源：http://uc.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ln.szxytkj.cn

[S36] C++：unordered_map
来源：http://yb.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lm.haigaiapp.cn

[S37] C++：set
来源：http://mj.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xr.lnxyls.cn

[S38] C++：排序
来源：http://uj.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://xb.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://su.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nb.9csxet.cn

[S40] C++：查找元素
来源：http://hu.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sm.hnjuh.cn

[S41] C++：类与构造函数
来源：http://bh.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qt.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://vm.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://sd.colortex.cn

[S43] C++：智能指针
来源：http://dp.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://sd.haigaiapp.cn

[S44] C++：引用传参
来源：http://xn.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://nx.shxzukj.cn

[S45] C++：lambda
来源：http://vi.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xu.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://ol.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xx.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://rs.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sz.hahajie.cn

[S48] C++：逐行读文件
来源：http://qe.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lo.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://ll.colortex.cn

[S49] C++：写文件
来源：http://oj.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dz.shtwfgs.cn

[S50] C++：格式化数字
来源：http://ph.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oy.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://xk.hnjuh.cn

static_cast<double>(a) / b
来源：http://yv.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://yt.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://mm.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://ie.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://hf.newstarts.cn

[S54] C++：异常处理
来源：http://fc.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fl.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://dk.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zy.shxzskj.cn

[S56] C++：optional
来源：http://qm.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ze.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://tt.shxzukj.cn

constexpr int N = 10;
来源：http://ya.9csxet.cn

[S58] C++：命名空间
来源：http://la.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://xj.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ig.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ym.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://ls.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://no.haigaiapp.cn

================================================================================
来源：http://vy.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ex.huanxung.cn

================================================================================
来源：http://fc.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://rd.shtwfgs.cn

println("Hello")
来源：http://fd.chemitech.net.cn

[T02] Kotlin：变量
来源：http://po.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uk.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://vd.jianghongdianzi.cn

"值: $b"
来源：http://yv.asd995.cn

[T04] Kotlin：空安全
来源：http://eo.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://zv.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://cu.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ug.nszjky.cn

[T06] Kotlin：集合映射
来源：http://zj.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hp.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://ft.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zx.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://fr.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://za.521024.cn

[T09] Kotlin：扩展函数
来源：http://on.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://qo.newstarts.cn

[T10] Kotlin：默认参数
来源：http://kz.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xy.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ny.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oh.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://ay.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://ql.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://mq.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://aw.gzmigu.cn

[T14] Kotlin：循环
来源：http://xa.panjiajie.cn

for (i in 1..10) println(i)
来源：http://jw.9csxet.cn

[T15] Kotlin：接口
来源：http://tq.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://mb.yuexingan06.cn

[T16] Swift：Hello World
来源：http://bw.szxytkj.cn

print("Hello")
来源：http://nw.hahajie.cn

[T17] Swift：变量与常量
来源：http://sv.panjiajie.cn

var a = 1;  let b = 2
来源：http://ze.nicolike.cn

[T18] Swift：字符串插值
来源：http://dc.chemitech.net.cn

"值: \(b)"
来源：http://nk.9csxet.cn

[T19] Swift：可选绑定
来源：http://rv.szsharing.cn

if let n = opt { print(n) }
来源：http://fk.nszjky.cn

[T20] Swift：数组操作
来源：http://vn.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://il.haigaiapp.cn

[T21] Swift：遍历
来源：http://wy.szxytkj.cn

for x in a { print(x) }
来源：http://cv.yuntaijiaju.cn

[T22] Swift：字典
来源：http://gj.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nd.newstarts.cn

[T23] Swift：函数
来源：http://jk.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ye.shtwfgs.cn

[T24] Swift：闭包
来源：http://qp.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://un.hahajie.cn


<!-- 参考信息 -->