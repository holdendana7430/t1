代发 wailian999

echo $((1 + 2 * 3))
来源：http://gp.nicolike.cn

[R28] 浮点运算
来源：http://wd.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://dp.huixiangedu.cn

[R29] 定义函数
来源：http://vk.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ca.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://dv.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://cg.lnxyls.cn

[R31] 局部变量
来源：http://tk.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://vo.huanxung.cn

[R32] 参数个数校验
来源：http://jo.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ms.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://sx.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tb.wgjwhj.cn

[R34] 退出时清理
来源：http://eg.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jz.lnxyls.cn

[R35] 后台执行并等待
来源：http://iy.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tb.newstarts.cn

[R36] 并发执行多个任务
来源：http://id.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ks.9csxet.cn

[R37] 把输出赋给变量
来源：http://kb.hahajie.cn

files=$(ls -1)
来源：http://fr.jctech888.com.cn

[R38] 管道串联
来源：http://kc.panjiajie.cn

cat a.txt | grep -i error | wc -l
来源：http://xy.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://fz.shtwfgs.cn

cmd > out.log 2>&1
来源：http://fr.newstarts.cn

[R40] 追加写日志
来源：http://po.wgjwhj.cn

echo "log" >> out.log
来源：http://eb.newstarts.cn

[R41] 丢弃输出
来源：http://ul.hahajie.cn

cmd >/dev/null 2>&1
来源：http://zt.shtwfgs.cn

[R42] 输入重定向
来源：http://pr.jianghongdianzi.cn

wc -l < a.txt
来源：http://fw.shxzskj.cn

[R43] 按名字查找文件
来源：http://ul.nszjky.cn

find . -name "*.log" -type f
来源：http://lg.hahajie.cn

[R44] 按修改时间查找
来源：http://sc.shxzskj.cn

find . -mtime -7 -type f
来源：http://wr.szxytkj.cn

[R45] 批量删除
来源：http://yj.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://xi.huanxung.cn

[R46] 递归替换文件内容
来源：http://ku.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ay.bjjhwx.cn

[R47] sed 单行替换
来源：http://ni.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ou.jctech888.com.cn

[R48] awk 取指定列
来源：http://qm.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://yx.shxzukj.cn

[R49] awk 带条件
来源：http://dk.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dp.bookmarksfly.cn

[R50] awk 求和
来源：http://ni.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://db.gzmigu.cn

[R51] 排序去重取前几
来源：http://yy.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qa.wgjwhj.cn

[R52] 统计行数
来源：http://ns.asd995.cn

wc -l a.txt
来源：http://or.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://qg.nszjky.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wr.521024.cn

[R54] 比较两个文件
来源：http://jz.huixinmuqiang.cn

diff a.txt b.txt
来源：http://ji.chemitech.net.cn

[R55] 压缩与解压
来源：http://hf.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yi.jctech888.com.cn

[R56] 远程拷贝
来源：http://dg.521024.cn

scp file user@host:/path/
来源：http://cs.huixiangedu.cn

[R57] 远程执行命令
来源：http://uu.hnjuh.cn

ssh user@host 'uptime'
来源：http://ew.chemitech.net.cn

[R58] 下载文件
来源：http://vg.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fm.nicolike.cn

[R59] 发 POST JSON
来源：http://pc.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dw.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://ju.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pz.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://nw.hnjuh.cn

df -h;  du -sh *
来源：http://qx.lnxyls.cn

[R62] 找最占空间的文件
来源：http://la.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ss.szsharing.cn

[R63] 内存与进程
来源：http://gv.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://hp.huanxung.cn

[R64] 结束进程
来源：http://zn.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://xd.shtwfgs.cn

[R65] 查看端口占用
来源：http://pl.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rl.huanxung.cn

[R66] 定时任务
来源：http://gr.panjiajie.cn

crontab -e;  crontab -l
来源：http://qx.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://mm.yuexingan06.cn

openssl rand -hex 16
来源：http://md.panjiajie.cn

[R68] 计算文件校验值
来源：http://gc.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ni.newstarts.cn

[R69] 生成随机密码
来源：http://ig.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://rt.haigaiapp.cn

[R70] 时间戳与互转
来源：http://qz.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://vw.asd995.cn

[R71] 日期格式化
来源：http://lt.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://on.szsharing.cn

[R72] 等待端口就绪
来源：http://hv.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jy.huixinmuqiang.cn

[R73] 分割大日志
来源：http://ea.chemitech.net.cn

split -l 1000 big.log part_
来源：http://qo.muxihuayi.cn

[R74] 批量重命名
来源：http://wt.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ef.panjiajie.cn

[R75] 导出环境变量
来源：http://fu.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://jw.muxihuayi.cn

[R76] 使用临时文件
来源：http://iw.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jb.521024.cn

[R77] 读取用户输入
来源：http://cy.asd995.cn

read -rp "请输入: " ans
来源：http://pj.yuexingan06.cn

[R78] 交互式菜单
来源：http://js.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nn.521024.cn

[R79] 解析命令行选项
来源：http://yw.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hx.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ws.nicolike.cn

time ./run.sh
来源：http://tg.huixinmuqiang.cn

================================================================================
来源：http://ax.shxzukj.cn

S. C / C++ 专题
来源：http://xx.521024.cn

================================================================================
来源：http://uk.shxzskj.cn

[S01] C：Hello World
来源：http://wm.bookmarksfly.cn

#include <stdio.h>
来源：http://xj.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qw.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://tx.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://qd.huixiangedu.cn

[S03] C：读入整数
来源：http://fb.newstarts.cn

int x; scanf("%d", &x);
来源：http://tg.haigaiapp.cn

[S04] C：字符串复制
来源：http://wk.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qc.bjjhwx.cn

[S05] C：字符串长度
来源：http://jr.colortex.cn

strlen(s)
来源：http://qa.shxzukj.cn

[S06] C：字符串比较
来源：http://kk.newstarts.cn

strcmp(a, b) == 0
来源：http://kp.gzmigu.cn

[S07] C：数组遍历求和
来源：http://lm.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qp.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://la.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vg.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://bl.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ty.shxzukj.cn

[S10] C：指针与解引用
来源：http://wf.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://lu.bjjhwx.cn

[S11] C：逐行读文件
来源：http://lz.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://hm.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cc.yuntaijiaju.cn

fclose(f);
来源：http://nf.newstarts.cn

[S12] C：写文件
来源：http://pv.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://er.hahajie.cn

[S13] C：宏定义
来源：http://uw.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uw.wgjwhj.cn

[S14] C：枚举
来源：http://em.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ja.hahajie.cn

[S15] C：类型转换
来源：http://bf.521024.cn

(double) a / b
来源：http://nx.shxzukj.cn

[S16] C：位操作置位
来源：http://mx.shxzukj.cn

x |= (1 << 3);
来源：http://zq.muxihuayi.cn

[S17] C：安全拼接字符串
来源：http://jy.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zy.szsharing.cn

[S18] C：命令行参数
来源：http://fg.yuexingan06.cn

int main(int argc, char **argv)
来源：http://lt.lnxyls.cn

[S19] C：快速排序
来源：http://xl.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sk.shxzskj.cn

[S20] C：二分查找
来源：http://pw.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ta.nicolike.cn

[S21] C：字符类别判断
来源：http://ab.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://di.521024.cn

[S22] C：字符串转数字
来源：http://qc.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tx.muxihuayi.cn

[S23] C：随机数
来源：http://qx.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qw.hahajie.cn

[S24] C：获取本地时间
来源：http://ex.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ky.huanxung.cn

[S25] C：内存拷贝
来源：http://wf.jctech888.com.cn

memcpy(dst, src, n);
来源：http://lw.shtwfgs.cn

[S26] C：内存清零
来源：http://lh.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://zf.huixiangedu.cn

[S27] C：定义常量
来源：http://jl.gzmigu.cn

const double PI = 3.14159;
来源：http://ah.huixinmuqiang.cn

[S28] C：静态变量
来源：http://hb.yuexingan06.cn

static int counter = 0;
来源：http://rk.nicolike.cn

[S29] C：变参函数
来源：http://jp.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jn.szsharing.cn

[S30] C：头文件保护
来源：http://ug.bookmarksfly.cn

#ifndef X_H
来源：http://qq.huixinmuqiang.cn

#define X_H
来源：http://bg.colortex.cn

#endif
来源：http://et.shxzskj.cn

[S31] C++：Hello World
来源：http://ps.jctech888.com.cn

#include <iostream>
来源：http://ip.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://op.bjjhwx.cn

[S32] C++：字符串
来源：http://qv.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://zm.asd995.cn

[S33] C++：vector 增删
来源：http://vv.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xi.asd995.cn

[S34] C++：遍历 vector
来源：http://rn.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://wd.yuntaijiaju.cn

[S35] C++：map
来源：http://do.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hi.lnxyls.cn

[S36] C++：unordered_map
来源：http://lt.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wi.nszjky.cn

[S37] C++：set
来源：http://ti.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ng.521024.cn

[S38] C++：排序
来源：http://wx.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://rm.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://hm.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ak.haigaiapp.cn

[S40] C++：查找元素
来源：http://dx.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sm.panjiajie.cn

[S41] C++：类与构造函数
来源：http://rv.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nc.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://sv.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://dw.colortex.cn

[S43] C++：智能指针
来源：http://ra.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://pk.panjiajie.cn

[S44] C++：引用传参
来源：http://au.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://vh.haigaiapp.cn

[S45] C++：lambda
来源：http://gb.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://un.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://il.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bh.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://zo.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://py.nszjky.cn

[S48] C++：逐行读文件
来源：http://ry.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ps.9csxet.cn

while (std::getline(in, line)) { }
来源：http://qj.shtwfgs.cn

[S49] C++：写文件
来源：http://hn.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ve.colortex.cn

[S50] C++：格式化数字
来源：http://iv.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jh.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://yp.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://no.asd995.cn

[S52] C++：const 与 noexcept
来源：http://hy.newstarts.cn

int size() const noexcept { return n_; }
来源：http://vj.gzmigu.cn

[S53] C++：移动语义
来源：http://tz.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://vd.newstarts.cn

[S54] C++：异常处理
来源：http://yv.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fr.szxytkj.cn

[S55] C++：结构化绑定
来源：http://sr.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wf.nicolike.cn

[S56] C++：optional
来源：http://to.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hr.hnjuh.cn

[S57] C++：编译期常量
来源：http://jq.huixinmuqiang.cn

constexpr int N = 10;
来源：http://ni.muxihuayi.cn

[S58] C++：命名空间
来源：http://es.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://nt.shxzskj.cn

[S59] C++：静态断言
来源：http://kv.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rs.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://ke.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nv.huixiangedu.cn

================================================================================
来源：http://rk.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qh.asd995.cn

================================================================================
来源：http://ru.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://hs.haigaiapp.cn

println("Hello")
来源：http://vk.521024.cn

[T02] Kotlin：变量
来源：http://hc.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gk.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://tx.szsharing.cn

"值: $b"
来源：http://yf.shxzukj.cn

[T04] Kotlin：空安全
来源：http://mz.asd995.cn

val n: String? = null;  n?.length
来源：http://mq.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://xm.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wp.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://sj.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xr.521024.cn

[T07] Kotlin：集合过滤
来源：http://wz.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iz.colortex.cn

[T08] Kotlin：数据类
来源：http://bn.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://gp.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://ct.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://hp.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://re.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gj.huixiangedu.cn

[T11] Kotlin：协程
来源：http://tu.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wg.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://bp.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://zf.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://sg.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://wa.9csxet.cn

[T14] Kotlin：循环
来源：http://yg.szsharing.cn

for (i in 1..10) println(i)
来源：http://qo.521024.cn

[T15] Kotlin：接口
来源：http://dp.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://fw.haigaiapp.cn

[T16] Swift：Hello World
来源：http://ze.jianghongdianzi.cn

print("Hello")
来源：http://mc.hnjuh.cn

[T17] Swift：变量与常量
来源：http://ci.gzmigu.cn

var a = 1;  let b = 2
来源：http://lm.521024.cn

[T18] Swift：字符串插值
来源：http://xf.jctech888.com.cn

"值: \(b)"
来源：http://ek.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://pe.521024.cn

if let n = opt { print(n) }
来源：http://go.newstarts.cn

[T20] Swift：数组操作
来源：http://yb.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ee.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://tm.bookmarksfly.cn

for x in a { print(x) }
来源：http://ni.jctech888.com.cn

[T22] Swift：字典
来源：http://xy.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gg.asd995.cn

[T23] Swift：函数
来源：http://op.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bq.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://aj.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jm.gzmigu.cn

[T25] Swift：结构体
来源：http://pl.hnjuh.cn

struct P { var x: Int }
来源：http://bc.newstarts.cn

[T26] Swift：类与重写
来源：http://zp.nszjky.cn

class A: Base { override func f() {} }
来源：http://km.huixiangedu.cn

[T27] Swift：错误处理
来源：http://fx.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://ku.lnxyls.cn

[T28] Swift：枚举
来源：http://uq.hnjuh.cn

enum Color { case red, green }
来源：http://za.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://ou.wgjwhj.cn

guard let x = opt else { return }
来源：http://io.wgjwhj.cn

[T30] Swift：协议
来源：http://an.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://aq.haigaiapp.cn


<!-- 参考信息 -->