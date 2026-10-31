代发 wailian999

echo $((1 + 2 * 3))
来源：http://tw.jianghongdianzi.cn

[R28] 浮点运算
来源：http://nt.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://yi.szsharing.cn

[R29] 定义函数
来源：http://dc.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kt.shxzskj.cn

[R30] 函数返回状态码
来源：http://wn.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://lw.huanxung.cn

[R31] 局部变量
来源：http://dc.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://jn.bookmarksfly.cn

[R32] 参数个数校验
来源：http://nf.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vb.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://aa.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mn.9csxet.cn

[R34] 退出时清理
来源：http://gf.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jr.haigaiapp.cn

[R35] 后台执行并等待
来源：http://px.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ug.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://mw.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hs.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://jj.jianghongdianzi.cn

files=$(ls -1)
来源：http://rq.chemitech.net.cn

[R38] 管道串联
来源：http://wr.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://ps.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://kw.panjiajie.cn

cmd > out.log 2>&1
来源：http://yy.muxihuayi.cn

[R40] 追加写日志
来源：http://gx.521024.cn

echo "log" >> out.log
来源：http://qs.shxzskj.cn

[R41] 丢弃输出
来源：http://ah.521024.cn

cmd >/dev/null 2>&1
来源：http://dh.9csxet.cn

[R42] 输入重定向
来源：http://ya.nszjky.cn

wc -l < a.txt
来源：http://xh.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://fo.colortex.cn

find . -name "*.log" -type f
来源：http://ey.huixiangedu.cn

[R44] 按修改时间查找
来源：http://tl.nszjky.cn

find . -mtime -7 -type f
来源：http://zh.yuntaijiaju.cn

[R45] 批量删除
来源：http://wp.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://jp.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://jl.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wr.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://ic.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jt.bookmarksfly.cn

[R48] awk 取指定列
来源：http://sg.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://zh.chemitech.net.cn

[R49] awk 带条件
来源：http://hr.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hr.muxihuayi.cn

[R50] awk 求和
来源：http://zt.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yh.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://kr.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://us.newstarts.cn

[R52] 统计行数
来源：http://ih.521024.cn

wc -l a.txt
来源：http://jw.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://qi.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cz.hahajie.cn

[R54] 比较两个文件
来源：http://ro.panjiajie.cn

diff a.txt b.txt
来源：http://jx.haigaiapp.cn

[R55] 压缩与解压
来源：http://gs.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zs.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://ai.szsharing.cn

scp file user@host:/path/
来源：http://pq.9csxet.cn

[R57] 远程执行命令
来源：http://uw.huixiangedu.cn

ssh user@host 'uptime'
来源：http://hd.chemitech.net.cn

[R58] 下载文件
来源：http://pj.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dp.521024.cn

[R59] 发 POST JSON
来源：http://wt.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qo.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://iv.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://of.shxzskj.cn

[R61] 磁盘占用
来源：http://qy.yuntaijiaju.cn

df -h;  du -sh *
来源：http://gd.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://xb.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://ud.lnxyls.cn

[R63] 内存与进程
来源：http://ot.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://bw.shtwfgs.cn

[R64] 结束进程
来源：http://xl.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://fg.jctech888.com.cn

[R65] 查看端口占用
来源：http://hm.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pm.colortex.cn

[R66] 定时任务
来源：http://hf.9csxet.cn

crontab -e;  crontab -l
来源：http://iu.9csxet.cn

[R67] 生成随机十六进制串
来源：http://ny.521024.cn

openssl rand -hex 16
来源：http://nn.bjjhwx.cn

[R68] 计算文件校验值
来源：http://nw.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xv.huixiangedu.cn

[R69] 生成随机密码
来源：http://di.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://yc.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://ej.szsharing.cn

date +%s;  date -d @1700000000
来源：http://zy.szxytkj.cn

[R71] 日期格式化
来源：http://tu.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ic.asd995.cn

[R72] 等待端口就绪
来源：http://kr.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hp.bjjhwx.cn

[R73] 分割大日志
来源：http://sv.panjiajie.cn

split -l 1000 big.log part_
来源：http://jg.haigaiapp.cn

[R74] 批量重命名
来源：http://dq.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ja.panjiajie.cn

[R75] 导出环境变量
来源：http://xj.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://uh.yuexingan06.cn

[R76] 使用临时文件
来源：http://gl.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ue.szxytkj.cn

[R77] 读取用户输入
来源：http://ta.asd995.cn

read -rp "请输入: " ans
来源：http://hv.szsharing.cn

[R78] 交互式菜单
来源：http://rk.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://on.lnxyls.cn

[R79] 解析命令行选项
来源：http://ka.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sx.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://kh.asd995.cn

time ./run.sh
来源：http://wk.huixinmuqiang.cn

================================================================================
来源：http://ye.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ta.shxzskj.cn

================================================================================
来源：http://hu.9csxet.cn

[S01] C：Hello World
来源：http://vw.wgjwhj.cn

#include <stdio.h>
来源：http://aw.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dx.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://gi.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://sl.gzmigu.cn

[S03] C：读入整数
来源：http://rk.nszjky.cn

int x; scanf("%d", &x);
来源：http://ox.shxzukj.cn

[S04] C：字符串复制
来源：http://qq.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rk.muxihuayi.cn

[S05] C：字符串长度
来源：http://ab.huixiangedu.cn

strlen(s)
来源：http://mj.asd995.cn

[S06] C：字符串比较
来源：http://cc.hnjuh.cn

strcmp(a, b) == 0
来源：http://kg.colortex.cn

[S07] C：数组遍历求和
来源：http://zu.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ot.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://tb.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ub.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://bc.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mg.lnxyls.cn

[S10] C：指针与解引用
来源：http://xq.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://vb.9csxet.cn

[S11] C：逐行读文件
来源：http://mp.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://uf.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yw.bjjhwx.cn

fclose(f);
来源：http://rk.huanxung.cn

[S12] C：写文件
来源：http://wg.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mg.colortex.cn

[S13] C：宏定义
来源：http://px.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mp.yuexingan06.cn

[S14] C：枚举
来源：http://xx.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://mn.9csxet.cn

[S15] C：类型转换
来源：http://wv.521024.cn

(double) a / b
来源：http://fj.yuexingan06.cn

[S16] C：位操作置位
来源：http://ld.shxzskj.cn

x |= (1 << 3);
来源：http://gr.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://ik.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ck.yuexingan06.cn

[S18] C：命令行参数
来源：http://jx.9csxet.cn

int main(int argc, char **argv)
来源：http://md.9csxet.cn

[S19] C：快速排序
来源：http://lk.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qj.huanxung.cn

[S20] C：二分查找
来源：http://wm.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ro.muxihuayi.cn

[S21] C：字符类别判断
来源：http://fw.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://on.szxytkj.cn

[S22] C：字符串转数字
来源：http://af.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ul.jctech888.com.cn

[S23] C：随机数
来源：http://by.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dg.asd995.cn

[S24] C：获取本地时间
来源：http://of.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://le.asd995.cn

[S25] C：内存拷贝
来源：http://fs.hnjuh.cn

memcpy(dst, src, n);
来源：http://qk.nszjky.cn

[S26] C：内存清零
来源：http://us.521024.cn

memset(a, 0, sizeof a);
来源：http://yj.hnjuh.cn

[S27] C：定义常量
来源：http://bb.bjjhwx.cn

const double PI = 3.14159;
来源：http://qq.panjiajie.cn

[S28] C：静态变量
来源：http://dp.gzmigu.cn

static int counter = 0;
来源：http://rj.huixinmuqiang.cn

[S29] C：变参函数
来源：http://lf.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lm.9csxet.cn

[S30] C：头文件保护
来源：http://wy.hahajie.cn

#ifndef X_H
来源：http://if.newstarts.cn

#define X_H
来源：http://nz.shtwfgs.cn

#endif
来源：http://ol.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ld.hnjuh.cn

#include <iostream>
来源：http://vd.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ad.nszjky.cn

[S32] C++：字符串
来源：http://ro.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://dm.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://zy.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mi.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://sv.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://az.shxzukj.cn

[S35] C++：map
来源：http://io.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ph.asd995.cn

[S36] C++：unordered_map
来源：http://ih.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sb.yuntaijiaju.cn

[S37] C++：set
来源：http://em.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wv.szxytkj.cn

[S38] C++：排序
来源：http://nf.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://bb.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://sl.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zr.szsharing.cn

[S40] C++：查找元素
来源：http://hs.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tx.asd995.cn

[S41] C++：类与构造函数
来源：http://si.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://he.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://jm.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://jw.yuexingan06.cn

[S43] C++：智能指针
来源：http://lz.521024.cn

auto p = std::make_unique<int>(5);
来源：http://cr.9csxet.cn

[S44] C++：引用传参
来源：http://zs.asd995.cn

void inc(int &x) { ++x; }
来源：http://fg.szxytkj.cn

[S45] C++：lambda
来源：http://ui.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tl.gzmigu.cn

[S46] C++：函数模板
来源：http://oz.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fq.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://fd.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eu.nicolike.cn

[S48] C++：逐行读文件
来源：http://uf.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wo.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://mf.hnjuh.cn

[S49] C++：写文件
来源：http://jj.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ri.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://uw.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://av.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://bv.szsharing.cn

static_cast<double>(a) / b
来源：http://bi.colortex.cn

[S52] C++：const 与 noexcept
来源：http://rl.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://bz.shtwfgs.cn

[S53] C++：移动语义
来源：http://so.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://tc.gzmigu.cn

[S54] C++：异常处理
来源：http://dw.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ba.lnxyls.cn

[S55] C++：结构化绑定
来源：http://ox.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eu.huixinmuqiang.cn

[S56] C++：optional
来源：http://ak.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://va.jctech888.com.cn

[S57] C++：编译期常量
来源：http://ee.newstarts.cn

constexpr int N = 10;
来源：http://oa.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://bd.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://wh.shtwfgs.cn

[S59] C++：静态断言
来源：http://hp.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gd.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://dh.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://da.huixiangedu.cn

================================================================================
来源：http://lp.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ho.jctech888.com.cn

================================================================================
来源：http://tf.521024.cn

[T01] Kotlin：Hello World
来源：http://oz.9csxet.cn

println("Hello")
来源：http://xu.muxihuayi.cn

[T02] Kotlin：变量
来源：http://pa.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hq.asd995.cn

[T03] Kotlin：字符串模板
来源：http://vm.gzmigu.cn

"值: $b"
来源：http://zv.hahajie.cn

[T04] Kotlin：空安全
来源：http://ll.shxzukj.cn

val n: String? = null;  n?.length
来源：http://uv.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://us.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iu.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://jx.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ce.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://td.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xh.nicolike.cn

[T08] Kotlin：数据类
来源：http://vr.asd995.cn

data class User(val name: String, val age: Int)
来源：http://by.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://dc.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://rw.9csxet.cn

[T10] Kotlin：默认参数
来源：http://qr.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ux.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://aw.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mp.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://iu.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://rg.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://fw.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://gc.gzmigu.cn

[T14] Kotlin：循环
来源：http://cc.gzmigu.cn

for (i in 1..10) println(i)
来源：http://pw.nszjky.cn

[T15] Kotlin：接口
来源：http://zq.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://ip.colortex.cn

[T16] Swift：Hello World
来源：http://fx.9csxet.cn

print("Hello")
来源：http://dc.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://tm.wgjwhj.cn

var a = 1;  let b = 2
来源：http://uy.shxzskj.cn

[T18] Swift：字符串插值
来源：http://mx.bookmarksfly.cn

"值: \(b)"
来源：http://rg.szsharing.cn

[T19] Swift：可选绑定
来源：http://hh.nicolike.cn

if let n = opt { print(n) }
来源：http://as.nszjky.cn

[T20] Swift：数组操作
来源：http://fu.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iu.haigaiapp.cn

[T21] Swift：遍历
来源：http://eh.huanxung.cn

for x in a { print(x) }
来源：http://wv.nicolike.cn

[T22] Swift：字典
来源：http://fn.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uu.muxihuayi.cn

[T23] Swift：函数
来源：http://tf.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nh.nicolike.cn

[T24] Swift：闭包
来源：http://nv.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xg.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://xf.wgjwhj.cn

struct P { var x: Int }
来源：http://oj.shxzskj.cn

[T26] Swift：类与重写
来源：http://mo.nicolike.cn

class A: Base { override func f() {} }
来源：http://hh.chemitech.net.cn

[T27] Swift：错误处理
来源：http://kh.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://xb.huixiangedu.cn

[T28] Swift：枚举
来源：http://ap.nicolike.cn

enum Color { case red, green }
来源：http://un.asd995.cn

[T29] Swift：guard 提前返回
来源：http://dh.haigaiapp.cn

guard let x = opt else { return }
来源：http://ax.panjiajie.cn

[T30] Swift：协议
来源：http://ck.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://po.yuntaijiaju.cn


<!-- 参考信息 -->