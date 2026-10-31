代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eg.9csxet.cn

[R30] 函数返回状态码
来源：http://zq.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://op.szxytkj.cn

[R31] 局部变量
来源：http://gr.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://wp.yuexingan06.cn

[R32] 参数个数校验
来源：http://pm.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://su.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://wq.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pu.shxzskj.cn

[R34] 退出时清理
来源：http://im.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ya.haigaiapp.cn

[R35] 后台执行并等待
来源：http://ms.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ws.szsharing.cn

[R36] 并发执行多个任务
来源：http://fp.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vp.shxzskj.cn

[R37] 把输出赋给变量
来源：http://hm.chemitech.net.cn

files=$(ls -1)
来源：http://sp.colortex.cn

[R38] 管道串联
来源：http://ma.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://kc.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://na.szsharing.cn

cmd > out.log 2>&1
来源：http://bw.yuexingan06.cn

[R40] 追加写日志
来源：http://tv.gzmigu.cn

echo "log" >> out.log
来源：http://cf.muxihuayi.cn

[R41] 丢弃输出
来源：http://ta.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://ox.yuexingan06.cn

[R42] 输入重定向
来源：http://lc.521024.cn

wc -l < a.txt
来源：http://qz.wgjwhj.cn

[R43] 按名字查找文件
来源：http://mi.colortex.cn

find . -name "*.log" -type f
来源：http://pc.huixiangedu.cn

[R44] 按修改时间查找
来源：http://wd.huanxung.cn

find . -mtime -7 -type f
来源：http://bn.szsharing.cn

[R45] 批量删除
来源：http://iz.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://oz.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://jy.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iq.bjjhwx.cn

[R47] sed 单行替换
来源：http://xj.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://af.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ub.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://wt.shxzukj.cn

[R49] awk 带条件
来源：http://ke.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://em.lnxyls.cn

[R50] awk 求和
来源：http://zv.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pp.colortex.cn

[R51] 排序去重取前几
来源：http://jq.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vl.gzmigu.cn

[R52] 统计行数
来源：http://ec.yuntaijiaju.cn

wc -l a.txt
来源：http://tm.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://jk.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vw.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://fz.nicolike.cn

diff a.txt b.txt
来源：http://tg.nszjky.cn

[R55] 压缩与解压
来源：http://fb.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cx.newstarts.cn

[R56] 远程拷贝
来源：http://ft.shtwfgs.cn

scp file user@host:/path/
来源：http://yl.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://zz.szsharing.cn

ssh user@host 'uptime'
来源：http://mb.panjiajie.cn

[R58] 下载文件
来源：http://cc.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iv.9csxet.cn

[R59] 发 POST JSON
来源：http://vz.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pa.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://ux.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yg.jctech888.com.cn

[R61] 磁盘占用
来源：http://gw.shxzskj.cn

df -h;  du -sh *
来源：http://va.szsharing.cn

[R62] 找最占空间的文件
来源：http://lu.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://ro.gzmigu.cn

[R63] 内存与进程
来源：http://eg.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://me.nicolike.cn

[R64] 结束进程
来源：http://cg.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://hm.jctech888.com.cn

[R65] 查看端口占用
来源：http://xz.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fa.yuexingan06.cn

[R66] 定时任务
来源：http://en.gzmigu.cn

crontab -e;  crontab -l
来源：http://cg.hahajie.cn

[R67] 生成随机十六进制串
来源：http://sx.yuntaijiaju.cn

openssl rand -hex 16
来源：http://zu.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://xf.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fj.shxzukj.cn

[R69] 生成随机密码
来源：http://is.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://jy.shtwfgs.cn

[R70] 时间戳与互转
来源：http://hm.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://pf.yuntaijiaju.cn

[R71] 日期格式化
来源：http://em.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sz.chemitech.net.cn

[R72] 等待端口就绪
来源：http://uy.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://th.chemitech.net.cn

[R73] 分割大日志
来源：http://nk.muxihuayi.cn

split -l 1000 big.log part_
来源：http://fh.nszjky.cn

[R74] 批量重命名
来源：http://yh.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bg.nszjky.cn

[R75] 导出环境变量
来源：http://hs.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://lf.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://px.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ij.hnjuh.cn

[R77] 读取用户输入
来源：http://by.lnxyls.cn

read -rp "请输入: " ans
来源：http://jj.yuexingan06.cn

[R78] 交互式菜单
来源：http://us.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pt.hnjuh.cn

[R79] 解析命令行选项
来源：http://fo.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://st.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://nk.shtwfgs.cn

time ./run.sh
来源：http://nb.shxzskj.cn

================================================================================
来源：http://ul.huanxung.cn

S. C / C++ 专题
来源：http://ll.nicolike.cn

================================================================================
来源：http://nd.huixinmuqiang.cn

[S01] C：Hello World
来源：http://fb.521024.cn

#include <stdio.h>
来源：http://xf.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hh.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://ga.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://yy.huixinmuqiang.cn

[S03] C：读入整数
来源：http://lo.huanxung.cn

int x; scanf("%d", &x);
来源：http://oz.shxzukj.cn

[S04] C：字符串复制
来源：http://ox.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oj.muxihuayi.cn

[S05] C：字符串长度
来源：http://yj.wgjwhj.cn

strlen(s)
来源：http://gx.shxzukj.cn

[S06] C：字符串比较
来源：http://km.hahajie.cn

strcmp(a, b) == 0
来源：http://fd.szxytkj.cn

[S07] C：数组遍历求和
来源：http://bl.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qo.colortex.cn

[S08] C：动态内存分配与释放
来源：http://dl.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hu.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://lj.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://od.hnjuh.cn

[S10] C：指针与解引用
来源：http://zi.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://ch.haigaiapp.cn

[S11] C：逐行读文件
来源：http://ma.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://gy.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fr.bjjhwx.cn

fclose(f);
来源：http://sa.jianghongdianzi.cn

[S12] C：写文件
来源：http://my.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dc.jctech888.com.cn

[S13] C：宏定义
来源：http://yx.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ts.asd995.cn

[S14] C：枚举
来源：http://pt.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://ks.haigaiapp.cn

[S15] C：类型转换
来源：http://zf.szxytkj.cn

(double) a / b
来源：http://km.szsharing.cn

[S16] C：位操作置位
来源：http://mq.jianghongdianzi.cn

x |= (1 << 3);
来源：http://ec.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://ul.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vd.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://ju.huanxung.cn

int main(int argc, char **argv)
来源：http://ei.nszjky.cn

[S19] C：快速排序
来源：http://rr.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://os.gzmigu.cn

[S20] C：二分查找
来源：http://dp.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bm.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://zg.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ad.bjjhwx.cn

[S22] C：字符串转数字
来源：http://er.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://id.jctech888.com.cn

[S23] C：随机数
来源：http://to.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rv.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://sb.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yy.haigaiapp.cn

[S25] C：内存拷贝
来源：http://dr.haigaiapp.cn

memcpy(dst, src, n);
来源：http://ce.9csxet.cn

[S26] C：内存清零
来源：http://ti.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://bh.yuntaijiaju.cn

[S27] C：定义常量
来源：http://bz.wgjwhj.cn

const double PI = 3.14159;
来源：http://el.nicolike.cn

[S28] C：静态变量
来源：http://pj.huanxung.cn

static int counter = 0;
来源：http://ul.szsharing.cn

[S29] C：变参函数
来源：http://mi.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lw.shxzskj.cn

[S30] C：头文件保护
来源：http://kn.shxzskj.cn

#ifndef X_H
来源：http://xg.yuexingan06.cn

#define X_H
来源：http://tj.panjiajie.cn

#endif
来源：http://wv.lnxyls.cn

[S31] C++：Hello World
来源：http://jo.shtwfgs.cn

#include <iostream>
来源：http://bh.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://jt.yuexingan06.cn

[S32] C++：字符串
来源：http://wj.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://vj.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://ty.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gb.nicolike.cn

[S34] C++：遍历 vector
来源：http://zt.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://jk.lnxyls.cn

[S35] C++：map
来源：http://ms.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cx.wgjwhj.cn

[S36] C++：unordered_map
来源：http://nf.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tl.hahajie.cn

[S37] C++：set
来源：http://nt.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nw.huixinmuqiang.cn

[S38] C++：排序
来源：http://bb.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://fh.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://om.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eo.szsharing.cn

[S40] C++：查找元素
来源：http://hm.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gl.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://dj.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kv.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://nd.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://wp.gzmigu.cn

[S43] C++：智能指针
来源：http://ee.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://zw.shtwfgs.cn

[S44] C++：引用传参
来源：http://nq.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://ju.huanxung.cn

[S45] C++：lambda
来源：http://ap.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ma.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://xx.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uy.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://ev.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pu.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://su.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://in.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://sh.newstarts.cn

[S49] C++：写文件
来源：http://nh.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dp.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://mr.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cf.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://tr.muxihuayi.cn

static_cast<double>(a) / b
来源：http://uy.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://gm.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://vr.asd995.cn

[S53] C++：移动语义
来源：http://fb.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://ld.bookmarksfly.cn

[S54] C++：异常处理
来源：http://ev.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pg.lnxyls.cn

[S55] C++：结构化绑定
来源：http://uh.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yt.521024.cn

[S56] C++：optional
来源：http://qu.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://in.521024.cn

[S57] C++：编译期常量
来源：http://st.521024.cn

constexpr int N = 10;
来源：http://hu.nszjky.cn

[S58] C++：命名空间
来源：http://vk.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://pv.shxzukj.cn

[S59] C++：静态断言
来源：http://fi.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sm.asd995.cn

[S60] C++：遍历并删除元素
来源：http://kb.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zp.huixinmuqiang.cn

================================================================================
来源：http://fu.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kl.lnxyls.cn

================================================================================
来源：http://hy.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://lf.szsharing.cn

println("Hello")
来源：http://fr.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://lp.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jv.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://pu.yuntaijiaju.cn

"值: $b"
来源：http://wx.asd995.cn

[T04] Kotlin：空安全
来源：http://qe.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://ky.asd995.cn

[T05] Kotlin：when 表达式
来源：http://op.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wp.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://ft.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zu.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://ef.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jd.hahajie.cn

[T08] Kotlin：数据类
来源：http://xf.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://lf.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://sn.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://as.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://lc.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hl.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://lr.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wo.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://nf.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://nt.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://ck.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ee.muxihuayi.cn

[T14] Kotlin：循环
来源：http://kh.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://tb.9csxet.cn

[T15] Kotlin：接口
来源：http://xi.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://mf.hnjuh.cn

[T16] Swift：Hello World
来源：http://ts.hnjuh.cn

print("Hello")
来源：http://us.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://lf.shxzukj.cn

var a = 1;  let b = 2
来源：http://lp.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://yb.hahajie.cn

"值: \(b)"
来源：http://do.gzmigu.cn

[T19] Swift：可选绑定
来源：http://ms.nszjky.cn

if let n = opt { print(n) }
来源：http://nm.nszjky.cn

[T20] Swift：数组操作
来源：http://gt.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oj.wgjwhj.cn

[T21] Swift：遍历
来源：http://jd.nicolike.cn

for x in a { print(x) }
来源：http://qz.gzmigu.cn

[T22] Swift：字典
来源：http://iq.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://su.shxzskj.cn

[T23] Swift：函数
来源：http://pa.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xo.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://su.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ch.szxytkj.cn

[T25] Swift：结构体
来源：http://lv.muxihuayi.cn

struct P { var x: Int }
来源：http://on.newstarts.cn

[T26] Swift：类与重写
来源：http://ui.huanxung.cn

class A: Base { override func f() {} }
来源：http://yw.shxzukj.cn

[T27] Swift：错误处理
来源：http://ch.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://yd.9csxet.cn

[T28] Swift：枚举
来源：http://gv.huixiangedu.cn

enum Color { case red, green }
来源：http://zj.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://bv.szsharing.cn

guard let x = opt else { return }
来源：http://yd.wgjwhj.cn

[T30] Swift：协议
来源：http://gl.asd995.cn

protocol Shape { func area() -> Double }
来源：http://tb.wgjwhj.cn

[T31] Lua：Hello World
来源：http://je.nszjky.cn

print("Hello")
来源：http://hu.shxzskj.cn

[T32] Lua：局部变量
来源：http://ah.bookmarksfly.cn

local a = 1
来源：http://ll.jctech888.com.cn


<!-- 参考信息 -->