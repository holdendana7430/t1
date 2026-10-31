代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wq.panjiajie.cn

[R30] 函数返回状态码
来源：http://ei.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://sg.shxzskj.cn

[R31] 局部变量
来源：http://kc.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://th.hnjuh.cn

[R32] 参数个数校验
来源：http://kw.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eh.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://if.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yz.muxihuayi.cn

[R34] 退出时清理
来源：http://xj.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ex.chemitech.net.cn

[R35] 后台执行并等待
来源：http://en.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cy.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://yz.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qv.hahajie.cn

[R37] 把输出赋给变量
来源：http://fr.panjiajie.cn

files=$(ls -1)
来源：http://kd.nicolike.cn

[R38] 管道串联
来源：http://du.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://tf.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://ht.gzmigu.cn

cmd > out.log 2>&1
来源：http://ry.huixiangedu.cn

[R40] 追加写日志
来源：http://ox.bookmarksfly.cn

echo "log" >> out.log
来源：http://bk.shtwfgs.cn

[R41] 丢弃输出
来源：http://fi.newstarts.cn

cmd >/dev/null 2>&1
来源：http://au.haigaiapp.cn

[R42] 输入重定向
来源：http://hq.wgjwhj.cn

wc -l < a.txt
来源：http://hq.muxihuayi.cn

[R43] 按名字查找文件
来源：http://vc.shxzukj.cn

find . -name "*.log" -type f
来源：http://af.asd995.cn

[R44] 按修改时间查找
来源：http://rn.chemitech.net.cn

find . -mtime -7 -type f
来源：http://uw.haigaiapp.cn

[R45] 批量删除
来源：http://ry.asd995.cn

find . -name "*.tmp" -delete
来源：http://lb.asd995.cn

[R46] 递归替换文件内容
来源：http://xx.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wl.bookmarksfly.cn

[R47] sed 单行替换
来源：http://jo.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dv.shxzskj.cn

[R48] awk 取指定列
来源：http://qj.521024.cn

awk '{print $1, $3}' a.txt
来源：http://gp.hnjuh.cn

[R49] awk 带条件
来源：http://hz.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xn.huixinmuqiang.cn

[R50] awk 求和
来源：http://uo.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xf.jctech888.com.cn

[R51] 排序去重取前几
来源：http://hu.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ce.521024.cn

[R52] 统计行数
来源：http://ry.9csxet.cn

wc -l a.txt
来源：http://vm.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://am.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sc.hnjuh.cn

[R54] 比较两个文件
来源：http://gn.newstarts.cn

diff a.txt b.txt
来源：http://xt.wgjwhj.cn

[R55] 压缩与解压
来源：http://oo.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://st.szsharing.cn

[R56] 远程拷贝
来源：http://yq.bjjhwx.cn

scp file user@host:/path/
来源：http://it.asd995.cn

[R57] 远程执行命令
来源：http://lx.yuexingan06.cn

ssh user@host 'uptime'
来源：http://lx.hnjuh.cn

[R58] 下载文件
来源：http://fa.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bp.shxzskj.cn

[R59] 发 POST JSON
来源：http://gb.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://br.jctech888.com.cn

[R60] 只看 HTTP 状态码
来源：http://zp.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://of.yuexingan06.cn

[R61] 磁盘占用
来源：http://tz.yuexingan06.cn

df -h;  du -sh *
来源：http://sv.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://xk.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://vt.yuntaijiaju.cn

[R63] 内存与进程
来源：http://xx.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://sn.colortex.cn

[R64] 结束进程
来源：http://uk.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://wy.yuexingan06.cn

[R65] 查看端口占用
来源：http://kc.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tr.9csxet.cn

[R66] 定时任务
来源：http://pr.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ti.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://bf.yuexingan06.cn

openssl rand -hex 16
来源：http://fl.panjiajie.cn

[R68] 计算文件校验值
来源：http://um.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yy.haigaiapp.cn

[R69] 生成随机密码
来源：http://zc.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://je.yuexingan06.cn

[R70] 时间戳与互转
来源：http://jt.szsharing.cn

date +%s;  date -d @1700000000
来源：http://sf.huanxung.cn

[R71] 日期格式化
来源：http://hg.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mv.huixiangedu.cn

[R72] 等待端口就绪
来源：http://ma.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kg.panjiajie.cn

[R73] 分割大日志
来源：http://yl.gzmigu.cn

split -l 1000 big.log part_
来源：http://yc.asd995.cn

[R74] 批量重命名
来源：http://mk.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jh.521024.cn

[R75] 导出环境变量
来源：http://st.bookmarksfly.cn

export PATH="$HOME/bin:$PATH"
来源：http://wn.hnjuh.cn

[R76] 使用临时文件
来源：http://ln.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ty.bjjhwx.cn

[R77] 读取用户输入
来源：http://bi.hnjuh.cn

read -rp "请输入: " ans
来源：http://co.gzmigu.cn

[R78] 交互式菜单
来源：http://pa.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://el.huixiangedu.cn

[R79] 解析命令行选项
来源：http://ds.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tk.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://bd.hahajie.cn

time ./run.sh
来源：http://mu.wgjwhj.cn

================================================================================
来源：http://on.yuexingan06.cn

S. C / C++ 专题
来源：http://qt.jctech888.com.cn

================================================================================
来源：http://qn.huixinmuqiang.cn

[S01] C：Hello World
来源：http://ho.yuntaijiaju.cn

#include <stdio.h>
来源：http://oo.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iz.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://im.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://zh.yuexingan06.cn

[S03] C：读入整数
来源：http://dl.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://nq.wgjwhj.cn

[S04] C：字符串复制
来源：http://so.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hq.jctech888.com.cn

[S05] C：字符串长度
来源：http://ki.gzmigu.cn

strlen(s)
来源：http://gg.shxzukj.cn

[S06] C：字符串比较
来源：http://mn.szsharing.cn

strcmp(a, b) == 0
来源：http://xc.huanxung.cn

[S07] C：数组遍历求和
来源：http://wa.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ch.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://fg.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ng.colortex.cn

[S09] C：结构体定义与初始化
来源：http://za.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ft.asd995.cn

[S10] C：指针与解引用
来源：http://pw.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://nx.gzmigu.cn

[S11] C：逐行读文件
来源：http://zl.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://ri.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rq.jianghongdianzi.cn

fclose(f);
来源：http://kh.yuntaijiaju.cn

[S12] C：写文件
来源：http://wv.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ug.szxytkj.cn

[S13] C：宏定义
来源：http://le.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sr.bookmarksfly.cn

[S14] C：枚举
来源：http://fx.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://in.szsharing.cn

[S15] C：类型转换
来源：http://oq.asd995.cn

(double) a / b
来源：http://ot.lnxyls.cn

[S16] C：位操作置位
来源：http://ut.bookmarksfly.cn

x |= (1 << 3);
来源：http://vx.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://ks.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rj.shtwfgs.cn

[S18] C：命令行参数
来源：http://et.asd995.cn

int main(int argc, char **argv)
来源：http://dl.jctech888.com.cn

[S19] C：快速排序
来源：http://cj.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oo.hahajie.cn

[S20] C：二分查找
来源：http://gj.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xt.colortex.cn

[S21] C：字符类别判断
来源：http://px.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xl.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://kq.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kl.bjjhwx.cn

[S23] C：随机数
来源：http://em.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tl.szsharing.cn

[S24] C：获取本地时间
来源：http://gq.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yy.gzmigu.cn

[S25] C：内存拷贝
来源：http://fw.gzmigu.cn

memcpy(dst, src, n);
来源：http://fc.hahajie.cn

[S26] C：内存清零
来源：http://yp.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://pv.yuntaijiaju.cn

[S27] C：定义常量
来源：http://sz.gzmigu.cn

const double PI = 3.14159;
来源：http://fd.haigaiapp.cn

[S28] C：静态变量
来源：http://ps.bjjhwx.cn

static int counter = 0;
来源：http://mp.huixinmuqiang.cn

[S29] C：变参函数
来源：http://rt.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fn.bjjhwx.cn

[S30] C：头文件保护
来源：http://rt.lnxyls.cn

#ifndef X_H
来源：http://uu.haigaiapp.cn

#define X_H
来源：http://cn.panjiajie.cn

#endif
来源：http://og.asd995.cn

[S31] C++：Hello World
来源：http://nd.muxihuayi.cn

#include <iostream>
来源：http://do.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://bh.jianghongdianzi.cn

[S32] C++：字符串
来源：http://cx.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ui.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ob.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bw.newstarts.cn

[S34] C++：遍历 vector
来源：http://nl.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ep.yuexingan06.cn

[S35] C++：map
来源：http://dq.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://il.shxzskj.cn

[S36] C++：unordered_map
来源：http://xw.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ig.chemitech.net.cn

[S37] C++：set
来源：http://zd.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kk.huixinmuqiang.cn

[S38] C++：排序
来源：http://rm.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://li.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://bj.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hp.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ph.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vs.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://bo.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://af.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://rz.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://dc.muxihuayi.cn

[S43] C++：智能指针
来源：http://yd.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ga.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://qo.nicolike.cn

void inc(int &x) { ++x; }
来源：http://hq.shxzskj.cn

[S45] C++：lambda
来源：http://ga.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ic.szsharing.cn

[S46] C++：函数模板
来源：http://en.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bk.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://lx.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qx.hahajie.cn

[S48] C++：逐行读文件
来源：http://vi.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ob.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://vb.jctech888.com.cn

[S49] C++：写文件
来源：http://ix.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gq.asd995.cn

[S50] C++：格式化数字
来源：http://rr.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://li.nicolike.cn

[S51] C++：显式类型转换
来源：http://fq.bjjhwx.cn

static_cast<double>(a) / b
来源：http://yv.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://ce.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://ve.yuexingan06.cn

[S53] C++：移动语义
来源：http://yd.colortex.cn

std::vector<int> w = std::move(v);
来源：http://zl.9csxet.cn

[S54] C++：异常处理
来源：http://qh.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xh.szxytkj.cn

[S55] C++：结构化绑定
来源：http://lf.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qe.chemitech.net.cn

[S56] C++：optional
来源：http://kk.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dp.hahajie.cn

[S57] C++：编译期常量
来源：http://nh.bookmarksfly.cn

constexpr int N = 10;
来源：http://wo.bookmarksfly.cn

[S58] C++：命名空间
来源：http://ut.521024.cn

namespace ns { int f() { return 1; } }
来源：http://zn.shtwfgs.cn

[S59] C++：静态断言
来源：http://fg.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qx.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://pv.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ip.huanxung.cn

================================================================================
来源：http://ku.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ij.huanxung.cn

================================================================================
来源：http://ef.nszjky.cn

[T01] Kotlin：Hello World
来源：http://fk.asd995.cn

println("Hello")
来源：http://bq.lnxyls.cn

[T02] Kotlin：变量
来源：http://ds.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bf.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://rn.yuntaijiaju.cn

"值: $b"
来源：http://ca.shxzukj.cn

[T04] Kotlin：空安全
来源：http://rp.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://gs.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://vf.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rl.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://dd.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mf.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://ii.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bi.nicolike.cn

[T08] Kotlin：数据类
来源：http://vc.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://rc.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://rr.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://mh.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://wm.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zy.bjjhwx.cn

[T11] Kotlin：协程
来源：http://sn.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uw.hahajie.cn

[T12] Kotlin：解构声明
来源：http://te.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://cy.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://ig.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://jv.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://ym.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://fz.9csxet.cn

[T15] Kotlin：接口
来源：http://bx.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://rr.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://tz.gzmigu.cn

print("Hello")
来源：http://ym.szxytkj.cn

[T17] Swift：变量与常量
来源：http://rc.shxzukj.cn

var a = 1;  let b = 2
来源：http://yb.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://yr.shxzukj.cn

"值: \(b)"
来源：http://lm.szsharing.cn

[T19] Swift：可选绑定
来源：http://wv.9csxet.cn

if let n = opt { print(n) }
来源：http://wq.colortex.cn

[T20] Swift：数组操作
来源：http://fr.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pl.haigaiapp.cn

[T21] Swift：遍历
来源：http://yb.newstarts.cn

for x in a { print(x) }
来源：http://yb.hahajie.cn

[T22] Swift：字典
来源：http://ss.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qs.szxytkj.cn

[T23] Swift：函数
来源：http://vj.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bo.hnjuh.cn

[T24] Swift：闭包
来源：http://md.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ck.shxzukj.cn

[T25] Swift：结构体
来源：http://xu.shxzukj.cn

struct P { var x: Int }
来源：http://kz.nicolike.cn

[T26] Swift：类与重写
来源：http://ib.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://hy.shxzskj.cn

[T27] Swift：错误处理
来源：http://nm.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://yn.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://zk.szsharing.cn

enum Color { case red, green }
来源：http://re.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://ul.shxzukj.cn

guard let x = opt else { return }
来源：http://zx.nicolike.cn

[T30] Swift：协议
来源：http://nx.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://rv.nicolike.cn

[T31] Lua：Hello World
来源：http://ly.shxzskj.cn

print("Hello")
来源：http://uq.colortex.cn

[T32] Lua：局部变量
来源：http://at.hnjuh.cn

local a = 1
来源：http://fm.muxihuayi.cn


<!-- 参考信息 -->