代发 wailian999

echo $((1 + 2 * 3))
来源：http://ui.nicolike.cn

[R28] 浮点运算
来源：http://ke.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://yj.huixinmuqiang.cn

[R29] 定义函数
来源：http://ei.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zd.asd995.cn

[R30] 函数返回状态码
来源：http://xl.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ed.bjjhwx.cn

[R31] 局部变量
来源：http://wt.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://ll.nicolike.cn

[R32] 参数个数校验
来源：http://xt.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ts.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://ei.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pi.nicolike.cn

[R34] 退出时清理
来源：http://yd.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uq.wgjwhj.cn

[R35] 后台执行并等待
来源：http://aj.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yi.colortex.cn

[R36] 并发执行多个任务
来源：http://nd.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mz.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://vi.jianghongdianzi.cn

files=$(ls -1)
来源：http://sh.chemitech.net.cn

[R38] 管道串联
来源：http://md.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://kv.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://ui.9csxet.cn

cmd > out.log 2>&1
来源：http://fn.chemitech.net.cn

[R40] 追加写日志
来源：http://ri.huanxung.cn

echo "log" >> out.log
来源：http://fq.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://qn.wgjwhj.cn

cmd >/dev/null 2>&1
来源：http://tm.yuexingan06.cn

[R42] 输入重定向
来源：http://wa.chemitech.net.cn

wc -l < a.txt
来源：http://kt.yuntaijiaju.cn

[R43] 按名字查找文件
来源：http://in.huanxung.cn

find . -name "*.log" -type f
来源：http://kj.huixiangedu.cn

[R44] 按修改时间查找
来源：http://us.shxzukj.cn

find . -mtime -7 -type f
来源：http://nl.hnjuh.cn

[R45] 批量删除
来源：http://kj.colortex.cn

find . -name "*.tmp" -delete
来源：http://ph.hnjuh.cn

[R46] 递归替换文件内容
来源：http://hv.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qq.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://mk.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yw.huixiangedu.cn

[R48] awk 取指定列
来源：http://jk.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://wl.huixiangedu.cn

[R49] awk 带条件
来源：http://pu.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ar.haigaiapp.cn

[R50] awk 求和
来源：http://ax.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xr.hahajie.cn

[R51] 排序去重取前几
来源：http://bt.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ly.huixiangedu.cn

[R52] 统计行数
来源：http://pi.shxzukj.cn

wc -l a.txt
来源：http://oq.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://fy.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mh.chemitech.net.cn

[R54] 比较两个文件
来源：http://uf.shxzskj.cn

diff a.txt b.txt
来源：http://tt.9csxet.cn

[R55] 压缩与解压
来源：http://zd.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wf.9csxet.cn

[R56] 远程拷贝
来源：http://ui.shxzukj.cn

scp file user@host:/path/
来源：http://ui.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://lp.nszjky.cn

ssh user@host 'uptime'
来源：http://jz.yuexingan06.cn

[R58] 下载文件
来源：http://qz.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ru.wgjwhj.cn

[R59] 发 POST JSON
来源：http://wi.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://og.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://la.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://in.haigaiapp.cn

[R61] 磁盘占用
来源：http://ef.shxzskj.cn

df -h;  du -sh *
来源：http://wm.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://hk.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://kv.jctech888.com.cn

[R63] 内存与进程
来源：http://dj.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://ew.newstarts.cn

[R64] 结束进程
来源：http://do.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://eo.shtwfgs.cn

[R65] 查看端口占用
来源：http://nz.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cv.shxzskj.cn

[R66] 定时任务
来源：http://tq.yuexingan06.cn

crontab -e;  crontab -l
来源：http://lu.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://us.bookmarksfly.cn

openssl rand -hex 16
来源：http://qp.521024.cn

[R68] 计算文件校验值
来源：http://mm.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://px.newstarts.cn

[R69] 生成随机密码
来源：http://ts.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://io.asd995.cn

[R70] 时间戳与互转
来源：http://rq.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://ww.jctech888.com.cn

[R71] 日期格式化
来源：http://vh.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ly.haigaiapp.cn

[R72] 等待端口就绪
来源：http://rq.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wv.hahajie.cn

[R73] 分割大日志
来源：http://rk.nszjky.cn

split -l 1000 big.log part_
来源：http://dd.asd995.cn

[R74] 批量重命名
来源：http://bp.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lv.hnjuh.cn

[R75] 导出环境变量
来源：http://ep.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://ss.shxzukj.cn

[R76] 使用临时文件
来源：http://kh.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bk.9csxet.cn

[R77] 读取用户输入
来源：http://dc.521024.cn

read -rp "请输入: " ans
来源：http://gi.jctech888.com.cn

[R78] 交互式菜单
来源：http://qu.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ax.szsharing.cn

[R79] 解析命令行选项
来源：http://mm.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hg.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://wk.yuexingan06.cn

time ./run.sh
来源：http://wt.nicolike.cn

================================================================================
来源：http://eu.yuntaijiaju.cn

S. C / C++ 专题
来源：http://yl.hahajie.cn

================================================================================
来源：http://aq.shxzukj.cn

[S01] C：Hello World
来源：http://pz.huanxung.cn

#include <stdio.h>
来源：http://an.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yz.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://nj.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://ua.newstarts.cn

[S03] C：读入整数
来源：http://jt.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://er.szxytkj.cn

[S04] C：字符串复制
来源：http://mf.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zd.shxzskj.cn

[S05] C：字符串长度
来源：http://ii.szxytkj.cn

strlen(s)
来源：http://mz.chemitech.net.cn

[S06] C：字符串比较
来源：http://qi.jctech888.com.cn

strcmp(a, b) == 0
来源：http://ud.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://vu.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bl.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://ck.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qj.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://lr.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rn.huixiangedu.cn

[S10] C：指针与解引用
来源：http://tk.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://vq.haigaiapp.cn

[S11] C：逐行读文件
来源：http://ac.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://yv.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nu.haigaiapp.cn

fclose(f);
来源：http://xc.hahajie.cn

[S12] C：写文件
来源：http://wp.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ik.szxytkj.cn

[S13] C：宏定义
来源：http://sb.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://le.nszjky.cn

[S14] C：枚举
来源：http://qa.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://lu.szsharing.cn

[S15] C：类型转换
来源：http://bt.huixiangedu.cn

(double) a / b
来源：http://st.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://mj.yuntaijiaju.cn

x |= (1 << 3);
来源：http://ek.asd995.cn

[S17] C：安全拼接字符串
来源：http://ec.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nb.shxzskj.cn

[S18] C：命令行参数
来源：http://kh.panjiajie.cn

int main(int argc, char **argv)
来源：http://yf.bjjhwx.cn

[S19] C：快速排序
来源：http://hm.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tt.newstarts.cn

[S20] C：二分查找
来源：http://xd.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yp.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://wy.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hu.asd995.cn

[S22] C：字符串转数字
来源：http://sb.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lr.bookmarksfly.cn

[S23] C：随机数
来源：http://fp.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qh.szsharing.cn

[S24] C：获取本地时间
来源：http://rq.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mw.szxytkj.cn

[S25] C：内存拷贝
来源：http://rk.wgjwhj.cn

memcpy(dst, src, n);
来源：http://yg.szxytkj.cn

[S26] C：内存清零
来源：http://hu.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://zm.jctech888.com.cn

[S27] C：定义常量
来源：http://ly.bookmarksfly.cn

const double PI = 3.14159;
来源：http://fd.bjjhwx.cn

[S28] C：静态变量
来源：http://sg.szsharing.cn

static int counter = 0;
来源：http://tv.hahajie.cn

[S29] C：变参函数
来源：http://hg.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ls.nicolike.cn

[S30] C：头文件保护
来源：http://hm.nicolike.cn

#ifndef X_H
来源：http://sa.hnjuh.cn

#define X_H
来源：http://qa.lnxyls.cn

#endif
来源：http://vf.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ht.521024.cn

#include <iostream>
来源：http://dw.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://iu.newstarts.cn

[S32] C++：字符串
来源：http://mc.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://gz.colortex.cn

[S33] C++：vector 增删
来源：http://pm.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mm.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://jc.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://it.lnxyls.cn

[S35] C++：map
来源：http://lx.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uo.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://ha.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ai.9csxet.cn

[S37] C++：set
来源：http://du.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qv.yuntaijiaju.cn

[S38] C++：排序
来源：http://sx.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://rj.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ha.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wh.shtwfgs.cn

[S40] C++：查找元素
来源：http://fp.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rj.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ht.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yz.colortex.cn

[S42] C++：继承与虚函数
来源：http://ss.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://rk.bookmarksfly.cn

[S43] C++：智能指针
来源：http://wo.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://ew.huixiangedu.cn

[S44] C++：引用传参
来源：http://tl.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://dl.wgjwhj.cn

[S45] C++：lambda
来源：http://hg.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jj.szxytkj.cn

[S46] C++：函数模板
来源：http://ef.shxzukj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yf.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://oo.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bk.panjiajie.cn

[S48] C++：逐行读文件
来源：http://hu.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ng.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://nd.huixiangedu.cn

[S49] C++：写文件
来源：http://qz.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sq.huixiangedu.cn

[S50] C++：格式化数字
来源：http://zl.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oy.hahajie.cn

[S51] C++：显式类型转换
来源：http://av.muxihuayi.cn

static_cast<double>(a) / b
来源：http://ka.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://ng.9csxet.cn

int size() const noexcept { return n_; }
来源：http://dj.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://kz.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://mi.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://jz.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://il.szsharing.cn

[S55] C++：结构化绑定
来源：http://li.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pf.521024.cn

[S56] C++：optional
来源：http://fb.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zx.lnxyls.cn

[S57] C++：编译期常量
来源：http://jp.lnxyls.cn

constexpr int N = 10;
来源：http://hv.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://cg.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://xt.nszjky.cn

[S59] C++：静态断言
来源：http://vw.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ux.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://nm.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lx.bookmarksfly.cn

================================================================================
来源：http://qf.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iz.9csxet.cn

================================================================================
来源：http://bb.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://ol.colortex.cn

println("Hello")
来源：http://gu.hnjuh.cn

[T02] Kotlin：变量
来源：http://yf.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cr.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://tp.szxytkj.cn

"值: $b"
来源：http://oc.lnxyls.cn

[T04] Kotlin：空安全
来源：http://st.521024.cn

val n: String? = null;  n?.length
来源：http://cj.colortex.cn

[T05] Kotlin：when 表达式
来源：http://ks.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ju.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://ys.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tf.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://bc.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://op.shxzskj.cn

[T08] Kotlin：数据类
来源：http://zi.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://gl.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://hc.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://fu.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://xk.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qt.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://gu.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rt.asd995.cn

[T12] Kotlin：解构声明
来源：http://fd.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://rx.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://zo.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://hp.huixiangedu.cn

[T14] Kotlin：循环
来源：http://kv.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://nr.szsharing.cn

[T15] Kotlin：接口
来源：http://xo.colortex.cn

interface Shape { fun area(): Double }
来源：http://on.haigaiapp.cn

[T16] Swift：Hello World
来源：http://we.muxihuayi.cn

print("Hello")
来源：http://pd.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://mw.yuexingan06.cn

var a = 1;  let b = 2
来源：http://bq.colortex.cn

[T18] Swift：字符串插值
来源：http://xc.gzmigu.cn

"值: \(b)"
来源：http://cg.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://jr.hnjuh.cn

if let n = opt { print(n) }
来源：http://yk.colortex.cn

[T20] Swift：数组操作
来源：http://rz.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yn.yuexingan06.cn

[T21] Swift：遍历
来源：http://rt.9csxet.cn

for x in a { print(x) }
来源：http://ih.yuexingan06.cn

[T22] Swift：字典
来源：http://if.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nl.huixiangedu.cn

[T23] Swift：函数
来源：http://gy.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zs.shxzukj.cn

[T24] Swift：闭包
来源：http://ge.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tn.asd995.cn

[T25] Swift：结构体
来源：http://sl.haigaiapp.cn

struct P { var x: Int }
来源：http://ui.huanxung.cn

[T26] Swift：类与重写
来源：http://le.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://jw.shxzukj.cn

[T27] Swift：错误处理
来源：http://up.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://iv.panjiajie.cn

[T28] Swift：枚举
来源：http://qq.szsharing.cn

enum Color { case red, green }
来源：http://rw.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://mv.colortex.cn

guard let x = opt else { return }
来源：http://bd.shxzukj.cn

[T30] Swift：协议
来源：http://ff.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://dl.nicolike.cn


<!-- 参考信息 -->