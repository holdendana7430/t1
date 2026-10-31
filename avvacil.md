代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yv.gzmigu.cn

[R34] 退出时清理
来源：http://nd.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rc.shxzskj.cn

[R35] 后台执行并等待
来源：http://ff.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nx.colortex.cn

[R36] 并发执行多个任务
来源：http://de.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yg.gzmigu.cn

[R37] 把输出赋给变量
来源：http://yr.chemitech.net.cn

files=$(ls -1)
来源：http://hy.gzmigu.cn

[R38] 管道串联
来源：http://hm.newstarts.cn

cat a.txt | grep -i error | wc -l
来源：http://tp.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://fk.nicolike.cn

cmd > out.log 2>&1
来源：http://co.nszjky.cn

[R40] 追加写日志
来源：http://hi.chemitech.net.cn

echo "log" >> out.log
来源：http://ml.9csxet.cn

[R41] 丢弃输出
来源：http://rp.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://ew.colortex.cn

[R42] 输入重定向
来源：http://dq.nicolike.cn

wc -l < a.txt
来源：http://xn.9csxet.cn

[R43] 按名字查找文件
来源：http://vu.9csxet.cn

find . -name "*.log" -type f
来源：http://gc.szxytkj.cn

[R44] 按修改时间查找
来源：http://fc.nicolike.cn

find . -mtime -7 -type f
来源：http://yn.panjiajie.cn

[R45] 批量删除
来源：http://me.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://go.hnjuh.cn

[R46] 递归替换文件内容
来源：http://aw.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kk.shtwfgs.cn

[R47] sed 单行替换
来源：http://ac.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xi.nszjky.cn

[R48] awk 取指定列
来源：http://wt.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://iz.newstarts.cn

[R49] awk 带条件
来源：http://jj.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fu.nicolike.cn

[R50] awk 求和
来源：http://ai.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bq.gzmigu.cn

[R51] 排序去重取前几
来源：http://cn.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://on.asd995.cn

[R52] 统计行数
来源：http://tp.wgjwhj.cn

wc -l a.txt
来源：http://uj.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://jf.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wq.panjiajie.cn

[R54] 比较两个文件
来源：http://wj.bjjhwx.cn

diff a.txt b.txt
来源：http://fi.hnjuh.cn

[R55] 压缩与解压
来源：http://ny.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xf.gzmigu.cn

[R56] 远程拷贝
来源：http://ka.szsharing.cn

scp file user@host:/path/
来源：http://xv.bjjhwx.cn

[R57] 远程执行命令
来源：http://ub.newstarts.cn

ssh user@host 'uptime'
来源：http://ck.9csxet.cn

[R58] 下载文件
来源：http://xm.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cv.shxzskj.cn

[R59] 发 POST JSON
来源：http://et.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xc.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://cd.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kl.szsharing.cn

[R61] 磁盘占用
来源：http://km.bjjhwx.cn

df -h;  du -sh *
来源：http://ur.lnxyls.cn

[R62] 找最占空间的文件
来源：http://eq.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://uc.huixiangedu.cn

[R63] 内存与进程
来源：http://mu.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://pv.bookmarksfly.cn

[R64] 结束进程
来源：http://zu.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://vm.newstarts.cn

[R65] 查看端口占用
来源：http://lc.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://av.shxzukj.cn

[R66] 定时任务
来源：http://db.bjjhwx.cn

crontab -e;  crontab -l
来源：http://pe.huanxung.cn

[R67] 生成随机十六进制串
来源：http://be.szxytkj.cn

openssl rand -hex 16
来源：http://bt.panjiajie.cn

[R68] 计算文件校验值
来源：http://tq.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vf.huixiangedu.cn

[R69] 生成随机密码
来源：http://ex.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://jh.jctech888.com.cn

[R70] 时间戳与互转
来源：http://wa.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://mj.9csxet.cn

[R71] 日期格式化
来源：http://bb.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zw.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://ha.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ru.jianghongdianzi.cn

[R73] 分割大日志
来源：http://ea.huixiangedu.cn

split -l 1000 big.log part_
来源：http://we.haigaiapp.cn

[R74] 批量重命名
来源：http://ny.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ca.huixiangedu.cn

[R75] 导出环境变量
来源：http://zc.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://xt.huanxung.cn

[R76] 使用临时文件
来源：http://xt.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cx.shxzukj.cn

[R77] 读取用户输入
来源：http://hm.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://vn.wgjwhj.cn

[R78] 交互式菜单
来源：http://lq.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wg.521024.cn

[R79] 解析命令行选项
来源：http://gx.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vm.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://kc.haigaiapp.cn

time ./run.sh
来源：http://sl.521024.cn

================================================================================
来源：http://vd.shtwfgs.cn

S. C / C++ 专题
来源：http://fi.huanxung.cn

================================================================================
来源：http://eo.bjjhwx.cn

[S01] C：Hello World
来源：http://vx.bookmarksfly.cn

#include <stdio.h>
来源：http://nl.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lw.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://zh.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://ji.bookmarksfly.cn

[S03] C：读入整数
来源：http://ka.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://ne.szxytkj.cn

[S04] C：字符串复制
来源：http://bi.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oa.asd995.cn

[S05] C：字符串长度
来源：http://ih.nszjky.cn

strlen(s)
来源：http://lj.nicolike.cn

[S06] C：字符串比较
来源：http://qd.chemitech.net.cn

strcmp(a, b) == 0
来源：http://aj.lnxyls.cn

[S07] C：数组遍历求和
来源：http://fy.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mf.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://qt.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ae.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://om.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kv.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://yg.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://nk.yuexingan06.cn

[S11] C：逐行读文件
来源：http://md.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://jc.hahajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kr.lnxyls.cn

fclose(f);
来源：http://gm.szxytkj.cn

[S12] C：写文件
来源：http://zh.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://my.nicolike.cn

[S13] C：宏定义
来源：http://hk.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dd.wgjwhj.cn

[S14] C：枚举
来源：http://wo.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://au.jctech888.com.cn

[S15] C：类型转换
来源：http://wi.huixiangedu.cn

(double) a / b
来源：http://ml.shxzukj.cn

[S16] C：位操作置位
来源：http://uv.hahajie.cn

x |= (1 << 3);
来源：http://xp.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://wm.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xu.colortex.cn

[S18] C：命令行参数
来源：http://dh.szxytkj.cn

int main(int argc, char **argv)
来源：http://yf.shxzskj.cn

[S19] C：快速排序
来源：http://jo.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://il.huixinmuqiang.cn

[S20] C：二分查找
来源：http://km.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xt.hnjuh.cn

[S21] C：字符类别判断
来源：http://fz.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ln.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://xu.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ce.gzmigu.cn

[S23] C：随机数
来源：http://ck.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jz.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://th.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://le.521024.cn

[S25] C：内存拷贝
来源：http://kg.9csxet.cn

memcpy(dst, src, n);
来源：http://qb.yuntaijiaju.cn

[S26] C：内存清零
来源：http://ds.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://ty.haigaiapp.cn

[S27] C：定义常量
来源：http://jx.hnjuh.cn

const double PI = 3.14159;
来源：http://cg.shtwfgs.cn

[S28] C：静态变量
来源：http://dy.yuexingan06.cn

static int counter = 0;
来源：http://dg.szsharing.cn

[S29] C：变参函数
来源：http://mg.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yg.newstarts.cn

[S30] C：头文件保护
来源：http://ct.bookmarksfly.cn

#ifndef X_H
来源：http://ad.jianghongdianzi.cn

#define X_H
来源：http://pn.asd995.cn

#endif
来源：http://ux.bjjhwx.cn

[S31] C++：Hello World
来源：http://xb.szsharing.cn

#include <iostream>
来源：http://cp.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://gm.hnjuh.cn

[S32] C++：字符串
来源：http://vq.asd995.cn

std::string s = "hi";  s += "!";
来源：http://km.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ec.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hq.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://jl.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://sk.szxytkj.cn

[S35] C++：map
来源：http://cm.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sm.lnxyls.cn

[S36] C++：unordered_map
来源：http://bq.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rk.yuntaijiaju.cn

[S37] C++：set
来源：http://gt.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hk.hahajie.cn

[S38] C++：排序
来源：http://it.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://fl.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://fc.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qn.szxytkj.cn

[S40] C++：查找元素
来源：http://ig.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fd.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://fo.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qp.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://ph.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://uq.chemitech.net.cn

[S43] C++：智能指针
来源：http://dj.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://ry.yuntaijiaju.cn

[S44] C++：引用传参
来源：http://ch.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://mx.newstarts.cn

[S45] C++：lambda
来源：http://al.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dr.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://qj.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gf.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://te.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://va.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://yq.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ov.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://lc.shxzukj.cn

[S49] C++：写文件
来源：http://bh.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wa.haigaiapp.cn

[S50] C++：格式化数字
来源：http://rk.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ey.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://po.521024.cn

static_cast<double>(a) / b
来源：http://ao.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://wi.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://gr.huanxung.cn

[S53] C++：移动语义
来源：http://my.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://ux.muxihuayi.cn

[S54] C++：异常处理
来源：http://hw.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yj.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://fw.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yn.yuntaijiaju.cn

[S56] C++：optional
来源：http://rs.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mh.shxzukj.cn

[S57] C++：编译期常量
来源：http://mt.yuexingan06.cn

constexpr int N = 10;
来源：http://in.nicolike.cn

[S58] C++：命名空间
来源：http://ut.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://br.gzmigu.cn

[S59] C++：静态断言
来源：http://df.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ai.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://zf.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ag.colortex.cn

================================================================================
来源：http://gb.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://if.nszjky.cn

================================================================================
来源：http://mf.9csxet.cn

[T01] Kotlin：Hello World
来源：http://ig.shxzukj.cn

println("Hello")
来源：http://pg.muxihuayi.cn

[T02] Kotlin：变量
来源：http://sp.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sy.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://de.muxihuayi.cn

"值: $b"
来源：http://bf.9csxet.cn

[T04] Kotlin：空安全
来源：http://dr.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://wl.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://zl.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cy.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://ek.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ew.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://us.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xf.asd995.cn

[T08] Kotlin：数据类
来源：http://in.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://bx.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://zb.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://se.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ef.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eg.shxzskj.cn

[T11] Kotlin：协程
来源：http://zs.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ua.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://dh.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://bt.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://wi.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://mq.newstarts.cn

[T14] Kotlin：循环
来源：http://ch.szsharing.cn

for (i in 1..10) println(i)
来源：http://yf.nszjky.cn

[T15] Kotlin：接口
来源：http://fg.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://ta.9csxet.cn

[T16] Swift：Hello World
来源：http://hb.shxzukj.cn

print("Hello")
来源：http://sl.9csxet.cn

[T17] Swift：变量与常量
来源：http://at.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://mj.huanxung.cn

[T18] Swift：字符串插值
来源：http://da.szsharing.cn

"值: \(b)"
来源：http://il.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://po.asd995.cn

if let n = opt { print(n) }
来源：http://ia.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://th.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sj.lnxyls.cn

[T21] Swift：遍历
来源：http://ua.9csxet.cn

for x in a { print(x) }
来源：http://oe.nicolike.cn

[T22] Swift：字典
来源：http://sd.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tp.bookmarksfly.cn

[T23] Swift：函数
来源：http://zc.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xt.panjiajie.cn

[T24] Swift：闭包
来源：http://uo.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sz.chemitech.net.cn

[T25] Swift：结构体
来源：http://bm.panjiajie.cn

struct P { var x: Int }
来源：http://hp.newstarts.cn

[T26] Swift：类与重写
来源：http://nb.shxzukj.cn

class A: Base { override func f() {} }
来源：http://pv.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://wr.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://di.hahajie.cn

[T28] Swift：枚举
来源：http://br.gzmigu.cn

enum Color { case red, green }
来源：http://nm.asd995.cn

[T29] Swift：guard 提前返回
来源：http://es.chemitech.net.cn

guard let x = opt else { return }
来源：http://vp.gzmigu.cn

[T30] Swift：协议
来源：http://us.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://bg.521024.cn

[T31] Lua：Hello World
来源：http://dx.jctech888.com.cn

print("Hello")
来源：http://kb.muxihuayi.cn

[T32] Lua：局部变量
来源：http://tu.huanxung.cn

local a = 1
来源：http://ae.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://en.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mh.huanxung.cn

[T34] Lua：遍历表
来源：http://wi.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://de.newstarts.cn

[T35] Lua：字典表
来源：http://iq.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://gw.huixinmuqiang.cn

[T36] Lua：函数
来源：http://hj.wgjwhj.cn

function add(a, b) return a + b end
来源：http://lg.chemitech.net.cn


<!-- 参考信息 -->