代发 wailian999

echo $((1 + 2 * 3))
来源：http://po.yuexingan06.cn

[R28] 浮点运算
来源：http://vb.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://xm.jianghongdianzi.cn

[R29] 定义函数
来源：http://ow.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vx.asd995.cn

[R30] 函数返回状态码
来源：http://cr.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://bz.nicolike.cn

[R31] 局部变量
来源：http://mq.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://nx.colortex.cn

[R32] 参数个数校验
来源：http://tf.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://my.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://rx.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tz.muxihuayi.cn

[R34] 退出时清理
来源：http://cl.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gy.nicolike.cn

[R35] 后台执行并等待
来源：http://ea.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yo.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://kt.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ob.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://ee.nicolike.cn

files=$(ls -1)
来源：http://kb.colortex.cn

[R38] 管道串联
来源：http://jp.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://xl.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://hn.jctech888.com.cn

cmd > out.log 2>&1
来源：http://sk.bjjhwx.cn

[R40] 追加写日志
来源：http://bo.jctech888.com.cn

echo "log" >> out.log
来源：http://yz.newstarts.cn

[R41] 丢弃输出
来源：http://ag.newstarts.cn

cmd >/dev/null 2>&1
来源：http://in.asd995.cn

[R42] 输入重定向
来源：http://gd.gzmigu.cn

wc -l < a.txt
来源：http://sn.huanxung.cn

[R43] 按名字查找文件
来源：http://oo.colortex.cn

find . -name "*.log" -type f
来源：http://xm.wgjwhj.cn

[R44] 按修改时间查找
来源：http://md.gzmigu.cn

find . -mtime -7 -type f
来源：http://ei.huixinmuqiang.cn

[R45] 批量删除
来源：http://ot.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://aa.lnxyls.cn

[R46] 递归替换文件内容
来源：http://wk.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yz.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://cn.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hr.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://ef.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://lr.bjjhwx.cn

[R49] awk 带条件
来源：http://nm.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cw.gzmigu.cn

[R50] awk 求和
来源：http://lb.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mv.asd995.cn

[R51] 排序去重取前几
来源：http://th.nicolike.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gs.521024.cn

[R52] 统计行数
来源：http://fo.wgjwhj.cn

wc -l a.txt
来源：http://nf.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://nz.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wk.panjiajie.cn

[R54] 比较两个文件
来源：http://ig.yuntaijiaju.cn

diff a.txt b.txt
来源：http://mb.szsharing.cn

[R55] 压缩与解压
来源：http://mr.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bn.panjiajie.cn

[R56] 远程拷贝
来源：http://oy.asd995.cn

scp file user@host:/path/
来源：http://jy.asd995.cn

[R57] 远程执行命令
来源：http://yw.chemitech.net.cn

ssh user@host 'uptime'
来源：http://ar.9csxet.cn

[R58] 下载文件
来源：http://oa.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qp.yuexingan06.cn

[R59] 发 POST JSON
来源：http://ft.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wb.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ay.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zw.shtwfgs.cn

[R61] 磁盘占用
来源：http://ak.haigaiapp.cn

df -h;  du -sh *
来源：http://vl.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://yc.asd995.cn

du -ah . | sort -rh | head -10
来源：http://pv.shtwfgs.cn

[R63] 内存与进程
来源：http://mz.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://az.huixiangedu.cn

[R64] 结束进程
来源：http://gm.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://ei.huixiangedu.cn

[R65] 查看端口占用
来源：http://gy.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ae.jianghongdianzi.cn

[R66] 定时任务
来源：http://go.asd995.cn

crontab -e;  crontab -l
来源：http://lg.9csxet.cn

[R67] 生成随机十六进制串
来源：http://jz.bjjhwx.cn

openssl rand -hex 16
来源：http://rw.asd995.cn

[R68] 计算文件校验值
来源：http://dg.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gb.gzmigu.cn

[R69] 生成随机密码
来源：http://hc.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://px.chemitech.net.cn

[R70] 时间戳与互转
来源：http://tt.asd995.cn

date +%s;  date -d @1700000000
来源：http://tj.lnxyls.cn

[R71] 日期格式化
来源：http://bj.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bj.huanxung.cn

[R72] 等待端口就绪
来源：http://wk.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wy.szsharing.cn

[R73] 分割大日志
来源：http://hz.szxytkj.cn

split -l 1000 big.log part_
来源：http://lk.panjiajie.cn

[R74] 批量重命名
来源：http://zu.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yg.521024.cn

[R75] 导出环境变量
来源：http://px.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://qw.shxzskj.cn

[R76] 使用临时文件
来源：http://df.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sp.nicolike.cn

[R77] 读取用户输入
来源：http://nv.newstarts.cn

read -rp "请输入: " ans
来源：http://om.nicolike.cn

[R78] 交互式菜单
来源：http://kq.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sr.521024.cn

[R79] 解析命令行选项
来源：http://vy.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ng.colortex.cn

[R80] 查看脚本执行耗时
来源：http://ox.muxihuayi.cn

time ./run.sh
来源：http://wu.nicolike.cn

================================================================================
来源：http://ga.huixiangedu.cn

S. C / C++ 专题
来源：http://lo.hahajie.cn

================================================================================
来源：http://bk.chemitech.net.cn

[S01] C：Hello World
来源：http://me.shxzskj.cn

#include <stdio.h>
来源：http://jc.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hj.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://ai.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://wj.yuntaijiaju.cn

[S03] C：读入整数
来源：http://jw.newstarts.cn

int x; scanf("%d", &x);
来源：http://jk.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://wg.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sf.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://uy.521024.cn

strlen(s)
来源：http://vn.bjjhwx.cn

[S06] C：字符串比较
来源：http://kc.szsharing.cn

strcmp(a, b) == 0
来源：http://zj.szsharing.cn

[S07] C：数组遍历求和
来源：http://oe.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://to.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://wy.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yr.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://rz.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ii.gzmigu.cn

[S10] C：指针与解引用
来源：http://sc.nicolike.cn

int *p = &a;  *p = 5;
来源：http://oj.huixiangedu.cn

[S11] C：逐行读文件
来源：http://sx.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://kh.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fj.yuexingan06.cn

fclose(f);
来源：http://ps.wgjwhj.cn

[S12] C：写文件
来源：http://re.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gp.huixiangedu.cn

[S13] C：宏定义
来源：http://ew.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://at.szxytkj.cn

[S14] C：枚举
来源：http://fx.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://ow.gzmigu.cn

[S15] C：类型转换
来源：http://bt.szsharing.cn

(double) a / b
来源：http://pf.shxzskj.cn

[S16] C：位操作置位
来源：http://rh.gzmigu.cn

x |= (1 << 3);
来源：http://xp.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://bs.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gg.bookmarksfly.cn

[S18] C：命令行参数
来源：http://rc.yuexingan06.cn

int main(int argc, char **argv)
来源：http://mn.yuntaijiaju.cn

[S19] C：快速排序
来源：http://wj.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tj.bjjhwx.cn

[S20] C：二分查找
来源：http://rr.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ds.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://vu.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ip.shtwfgs.cn

[S22] C：字符串转数字
来源：http://ac.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ue.szxytkj.cn

[S23] C：随机数
来源：http://ze.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ml.muxihuayi.cn

[S24] C：获取本地时间
来源：http://zv.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://un.hnjuh.cn

[S25] C：内存拷贝
来源：http://su.hnjuh.cn

memcpy(dst, src, n);
来源：http://jc.bjjhwx.cn

[S26] C：内存清零
来源：http://sk.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://um.nicolike.cn

[S27] C：定义常量
来源：http://ji.panjiajie.cn

const double PI = 3.14159;
来源：http://iq.newstarts.cn

[S28] C：静态变量
来源：http://vn.yuntaijiaju.cn

static int counter = 0;
来源：http://aa.shxzukj.cn

[S29] C：变参函数
来源：http://sp.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oc.huanxung.cn

[S30] C：头文件保护
来源：http://lm.huanxung.cn

#ifndef X_H
来源：http://in.lnxyls.cn

#define X_H
来源：http://db.lnxyls.cn

#endif
来源：http://gk.newstarts.cn

[S31] C++：Hello World
来源：http://km.hahajie.cn

#include <iostream>
来源：http://vk.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://rj.chemitech.net.cn

[S32] C++：字符串
来源：http://ab.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://ky.chemitech.net.cn

[S33] C++：vector 增删
来源：http://sv.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sn.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://xg.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://eq.gzmigu.cn

[S35] C++：map
来源：http://ur.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tb.huanxung.cn

[S36] C++：unordered_map
来源：http://tx.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zm.yuntaijiaju.cn

[S37] C++：set
来源：http://js.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ec.521024.cn

[S38] C++：排序
来源：http://ne.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://mk.521024.cn

[S39] C++：自定义比较器排序
来源：http://mi.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ok.9csxet.cn

[S40] C++：查找元素
来源：http://md.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ge.hahajie.cn

[S41] C++：类与构造函数
来源：http://fg.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qx.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://qc.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://hv.wgjwhj.cn

[S43] C++：智能指针
来源：http://wk.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://nn.szxytkj.cn

[S44] C++：引用传参
来源：http://od.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://uw.huixinmuqiang.cn

[S45] C++：lambda
来源：http://ej.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nj.bjjhwx.cn

[S46] C++：函数模板
来源：http://wp.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zd.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://mi.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uf.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://ns.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ze.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://pk.bjjhwx.cn

[S49] C++：写文件
来源：http://rm.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gc.asd995.cn

[S50] C++：格式化数字
来源：http://nn.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lj.hahajie.cn

[S51] C++：显式类型转换
来源：http://gj.szxytkj.cn

static_cast<double>(a) / b
来源：http://mi.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://ua.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://in.wgjwhj.cn

[S53] C++：移动语义
来源：http://wz.asd995.cn

std::vector<int> w = std::move(v);
来源：http://pq.jctech888.com.cn

[S54] C++：异常处理
来源：http://vm.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ls.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://rm.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ev.gzmigu.cn

[S56] C++：optional
来源：http://ty.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lf.9csxet.cn

[S57] C++：编译期常量
来源：http://bs.lnxyls.cn

constexpr int N = 10;
来源：http://cy.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://sn.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://gu.521024.cn

[S59] C++：静态断言
来源：http://da.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://em.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://ve.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gw.gzmigu.cn

================================================================================
来源：http://ff.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zs.wgjwhj.cn

================================================================================
来源：http://ww.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://oy.muxihuayi.cn

println("Hello")
来源：http://tg.nszjky.cn

[T02] Kotlin：变量
来源：http://vl.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uu.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://jw.yuexingan06.cn

"值: $b"
来源：http://lz.colortex.cn

[T04] Kotlin：空安全
来源：http://ft.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ez.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://ks.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vm.nszjky.cn

[T06] Kotlin：集合映射
来源：http://su.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gk.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://ym.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wf.newstarts.cn

[T08] Kotlin：数据类
来源：http://nf.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://ns.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://rz.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://hv.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://wt.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://et.hahajie.cn

[T11] Kotlin：协程
来源：http://hm.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jd.521024.cn

[T12] Kotlin：解构声明
来源：http://ch.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://pj.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://ee.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://gv.szxytkj.cn

[T14] Kotlin：循环
来源：http://ns.shxzskj.cn

for (i in 1..10) println(i)
来源：http://rt.panjiajie.cn

[T15] Kotlin：接口
来源：http://kn.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://ce.9csxet.cn

[T16] Swift：Hello World
来源：http://vr.jctech888.com.cn

print("Hello")
来源：http://zj.szsharing.cn

[T17] Swift：变量与常量
来源：http://hr.szxytkj.cn

var a = 1;  let b = 2
来源：http://ip.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://uj.szsharing.cn

"值: \(b)"
来源：http://yi.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://tk.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://ha.bjjhwx.cn

[T20] Swift：数组操作
来源：http://lu.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pm.wgjwhj.cn

[T21] Swift：遍历
来源：http://ib.newstarts.cn

for x in a { print(x) }
来源：http://tb.shxzskj.cn

[T22] Swift：字典
来源：http://em.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iw.panjiajie.cn

[T23] Swift：函数
来源：http://qh.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fi.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://yk.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oo.shxzukj.cn

[T25] Swift：结构体
来源：http://tc.szxytkj.cn

struct P { var x: Int }
来源：http://qz.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://wi.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://rj.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://ra.nszjky.cn

do { try f() } catch { print(error) }
来源：http://fu.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://md.szxytkj.cn

enum Color { case red, green }
来源：http://hu.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://qu.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://hf.huixiangedu.cn

[T30] Swift：协议
来源：http://pk.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://ly.shtwfgs.cn


<!-- 参考信息 -->