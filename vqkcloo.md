代发 wailian999

echo $((1 + 2 * 3))
来源：http://uq.521024.cn

[R28] 浮点运算
来源：http://rt.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://nm.bjjhwx.cn

[R29] 定义函数
来源：http://th.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nd.lnxyls.cn

[R30] 函数返回状态码
来源：http://hr.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://re.lnxyls.cn

[R31] 局部变量
来源：http://dc.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://zi.muxihuayi.cn

[R32] 参数个数校验
来源：http://nd.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gh.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://xm.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jt.wgjwhj.cn

[R34] 退出时清理
来源：http://pe.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jw.nszjky.cn

[R35] 后台执行并等待
来源：http://lv.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://im.521024.cn

[R36] 并发执行多个任务
来源：http://mn.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gg.shxzukj.cn

[R37] 把输出赋给变量
来源：http://me.wgjwhj.cn

files=$(ls -1)
来源：http://ex.muxihuayi.cn

[R38] 管道串联
来源：http://ll.shxzukj.cn

cat a.txt | grep -i error | wc -l
来源：http://cf.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://nb.nszjky.cn

cmd > out.log 2>&1
来源：http://em.jianghongdianzi.cn

[R40] 追加写日志
来源：http://wh.huixinmuqiang.cn

echo "log" >> out.log
来源：http://rr.gzmigu.cn

[R41] 丢弃输出
来源：http://mo.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://lh.newstarts.cn

[R42] 输入重定向
来源：http://kx.shtwfgs.cn

wc -l < a.txt
来源：http://gw.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://rz.hahajie.cn

find . -name "*.log" -type f
来源：http://vx.szxytkj.cn

[R44] 按修改时间查找
来源：http://oy.lnxyls.cn

find . -mtime -7 -type f
来源：http://pe.bjjhwx.cn

[R45] 批量删除
来源：http://oe.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://ra.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://uq.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pz.nicolike.cn

[R47] sed 单行替换
来源：http://aw.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gk.jctech888.com.cn

[R48] awk 取指定列
来源：http://gv.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://ef.gzmigu.cn

[R49] awk 带条件
来源：http://jd.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wa.huanxung.cn

[R50] awk 求和
来源：http://ad.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://em.newstarts.cn

[R51] 排序去重取前几
来源：http://io.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sf.nszjky.cn

[R52] 统计行数
来源：http://os.wgjwhj.cn

wc -l a.txt
来源：http://qz.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://ol.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xw.yuexingan06.cn

[R54] 比较两个文件
来源：http://uu.szxytkj.cn

diff a.txt b.txt
来源：http://wd.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://wk.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ca.9csxet.cn

[R56] 远程拷贝
来源：http://dt.lnxyls.cn

scp file user@host:/path/
来源：http://rs.bookmarksfly.cn

[R57] 远程执行命令
来源：http://ei.panjiajie.cn

ssh user@host 'uptime'
来源：http://mj.bookmarksfly.cn

[R58] 下载文件
来源：http://cq.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ym.szxytkj.cn

[R59] 发 POST JSON
来源：http://fj.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tx.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://qv.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sg.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://nm.szxytkj.cn

df -h;  du -sh *
来源：http://lz.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://ys.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://wh.colortex.cn

[R63] 内存与进程
来源：http://gx.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://bp.haigaiapp.cn

[R64] 结束进程
来源：http://kw.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://si.gzmigu.cn

[R65] 查看端口占用
来源：http://zm.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sl.szsharing.cn

[R66] 定时任务
来源：http://jz.9csxet.cn

crontab -e;  crontab -l
来源：http://iz.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://mx.wgjwhj.cn

openssl rand -hex 16
来源：http://ql.haigaiapp.cn

[R68] 计算文件校验值
来源：http://ya.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cw.haigaiapp.cn

[R69] 生成随机密码
来源：http://cn.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://zv.panjiajie.cn

[R70] 时间戳与互转
来源：http://mf.huanxung.cn

date +%s;  date -d @1700000000
来源：http://mk.szsharing.cn

[R71] 日期格式化
来源：http://fv.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bk.muxihuayi.cn

[R72] 等待端口就绪
来源：http://dw.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kb.chemitech.net.cn

[R73] 分割大日志
来源：http://ir.jctech888.com.cn

split -l 1000 big.log part_
来源：http://ma.gzmigu.cn

[R74] 批量重命名
来源：http://zh.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yi.wgjwhj.cn

[R75] 导出环境变量
来源：http://pg.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://um.bookmarksfly.cn

[R76] 使用临时文件
来源：http://dj.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://od.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://ia.9csxet.cn

read -rp "请输入: " ans
来源：http://rc.bookmarksfly.cn

[R78] 交互式菜单
来源：http://rp.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gw.9csxet.cn

[R79] 解析命令行选项
来源：http://uw.huixinmuqiang.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yz.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://bs.shxzskj.cn

time ./run.sh
来源：http://st.newstarts.cn

================================================================================
来源：http://fr.huixinmuqiang.cn

S. C / C++ 专题
来源：http://ea.haigaiapp.cn

================================================================================
来源：http://ha.shxzskj.cn

[S01] C：Hello World
来源：http://yp.muxihuayi.cn

#include <stdio.h>
来源：http://bv.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wp.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://rb.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://ku.asd995.cn

[S03] C：读入整数
来源：http://wx.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://ij.haigaiapp.cn

[S04] C：字符串复制
来源：http://bu.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fh.jctech888.com.cn

[S05] C：字符串长度
来源：http://mf.521024.cn

strlen(s)
来源：http://ht.muxihuayi.cn

[S06] C：字符串比较
来源：http://si.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://ye.colortex.cn

[S07] C：数组遍历求和
来源：http://qt.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ch.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://vj.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fc.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://dy.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wx.szsharing.cn

[S10] C：指针与解引用
来源：http://tp.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://hh.huanxung.cn

[S11] C：逐行读文件
来源：http://fu.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ba.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hp.yuexingan06.cn

fclose(f);
来源：http://ao.521024.cn

[S12] C：写文件
来源：http://do.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hj.wgjwhj.cn

[S13] C：宏定义
来源：http://sy.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jw.jctech888.com.cn

[S14] C：枚举
来源：http://bj.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://hs.yuntaijiaju.cn

[S15] C：类型转换
来源：http://so.bjjhwx.cn

(double) a / b
来源：http://dx.huanxung.cn

[S16] C：位操作置位
来源：http://iy.nszjky.cn

x |= (1 << 3);
来源：http://lf.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://an.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gb.wgjwhj.cn

[S18] C：命令行参数
来源：http://dn.newstarts.cn

int main(int argc, char **argv)
来源：http://qb.wgjwhj.cn

[S19] C：快速排序
来源：http://dh.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xj.yuexingan06.cn

[S20] C：二分查找
来源：http://dj.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://za.hnjuh.cn

[S21] C：字符类别判断
来源：http://je.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pw.hnjuh.cn

[S22] C：字符串转数字
来源：http://nn.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sd.shtwfgs.cn

[S23] C：随机数
来源：http://rm.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ce.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://wm.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aj.hahajie.cn

[S25] C：内存拷贝
来源：http://nc.jctech888.com.cn

memcpy(dst, src, n);
来源：http://nm.jianghongdianzi.cn

[S26] C：内存清零
来源：http://ht.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://vu.bjjhwx.cn

[S27] C：定义常量
来源：http://er.newstarts.cn

const double PI = 3.14159;
来源：http://mk.colortex.cn

[S28] C：静态变量
来源：http://yz.yuntaijiaju.cn

static int counter = 0;
来源：http://qb.hnjuh.cn

[S29] C：变参函数
来源：http://hx.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qn.asd995.cn

[S30] C：头文件保护
来源：http://oa.szxytkj.cn

#ifndef X_H
来源：http://ut.521024.cn

#define X_H
来源：http://us.haigaiapp.cn

#endif
来源：http://wr.szxytkj.cn

[S31] C++：Hello World
来源：http://hi.jianghongdianzi.cn

#include <iostream>
来源：http://fw.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://dk.shtwfgs.cn

[S32] C++：字符串
来源：http://op.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://px.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://aa.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fr.hahajie.cn

[S34] C++：遍历 vector
来源：http://sm.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://th.huanxung.cn

[S35] C++：map
来源：http://gn.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wc.lnxyls.cn

[S36] C++：unordered_map
来源：http://ib.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://og.shtwfgs.cn

[S37] C++：set
来源：http://ql.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gc.panjiajie.cn

[S38] C++：排序
来源：http://cn.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://ng.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://xp.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cy.bookmarksfly.cn

[S40] C++：查找元素
来源：http://jm.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qp.newstarts.cn

[S41] C++：类与构造函数
来源：http://ku.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iu.colortex.cn

[S42] C++：继承与虚函数
来源：http://xl.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://db.yuexingan06.cn

[S43] C++：智能指针
来源：http://jr.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://zo.szxytkj.cn

[S44] C++：引用传参
来源：http://bq.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://dg.huixinmuqiang.cn

[S45] C++：lambda
来源：http://eq.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rj.shtwfgs.cn

[S46] C++：函数模板
来源：http://ma.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jj.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://dw.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jr.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://st.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tf.newstarts.cn

while (std::getline(in, line)) { }
来源：http://xj.shxzskj.cn

[S49] C++：写文件
来源：http://lx.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pf.colortex.cn

[S50] C++：格式化数字
来源：http://lq.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ly.asd995.cn

[S51] C++：显式类型转换
来源：http://ye.newstarts.cn

static_cast<double>(a) / b
来源：http://vl.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://ym.szsharing.cn

int size() const noexcept { return n_; }
来源：http://ef.haigaiapp.cn

[S53] C++：移动语义
来源：http://lr.asd995.cn

std::vector<int> w = std::move(v);
来源：http://ze.hahajie.cn

[S54] C++：异常处理
来源：http://ti.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gt.huanxung.cn

[S55] C++：结构化绑定
来源：http://iq.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xe.shtwfgs.cn

[S56] C++：optional
来源：http://dh.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mv.haigaiapp.cn

[S57] C++：编译期常量
来源：http://st.colortex.cn

constexpr int N = 10;
来源：http://tt.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://sk.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://by.gzmigu.cn

[S59] C++：静态断言
来源：http://ve.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qc.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://jy.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gd.huanxung.cn

================================================================================
来源：http://zw.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hv.panjiajie.cn

================================================================================
来源：http://eu.hahajie.cn

[T01] Kotlin：Hello World
来源：http://dt.nicolike.cn

println("Hello")
来源：http://gc.haigaiapp.cn

[T02] Kotlin：变量
来源：http://qt.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qd.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://dp.asd995.cn

"值: $b"
来源：http://xq.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://tf.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://xh.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://gi.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ko.521024.cn

[T06] Kotlin：集合映射
来源：http://od.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://am.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://yl.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zw.panjiajie.cn

[T08] Kotlin：数据类
来源：http://fo.colortex.cn

data class User(val name: String, val age: Int)
来源：http://wz.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://jw.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://se.nicolike.cn

[T10] Kotlin：默认参数
来源：http://fg.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sf.newstarts.cn

[T11] Kotlin：协程
来源：http://qz.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ew.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://fz.521024.cn

val (a, b) = Pair(1, 2)
来源：http://vw.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://vv.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://as.gzmigu.cn

[T14] Kotlin：循环
来源：http://po.szsharing.cn

for (i in 1..10) println(i)
来源：http://bm.nicolike.cn

[T15] Kotlin：接口
来源：http://dh.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://mr.hnjuh.cn

[T16] Swift：Hello World
来源：http://ae.chemitech.net.cn

print("Hello")
来源：http://zd.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://ef.hahajie.cn

var a = 1;  let b = 2
来源：http://st.shxzukj.cn

[T18] Swift：字符串插值
来源：http://eg.yuexingan06.cn

"值: \(b)"
来源：http://su.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://dp.9csxet.cn

if let n = opt { print(n) }
来源：http://nl.panjiajie.cn

[T20] Swift：数组操作
来源：http://rq.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://he.shxzukj.cn

[T21] Swift：遍历
来源：http://tb.yuntaijiaju.cn

for x in a { print(x) }
来源：http://um.colortex.cn

[T22] Swift：字典
来源：http://wr.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nc.huixinmuqiang.cn

[T23] Swift：函数
来源：http://xy.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yu.muxihuayi.cn

[T24] Swift：闭包
来源：http://to.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pu.haigaiapp.cn

[T25] Swift：结构体
来源：http://ut.panjiajie.cn

struct P { var x: Int }
来源：http://sw.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://kd.colortex.cn

class A: Base { override func f() {} }
来源：http://gz.newstarts.cn

[T27] Swift：错误处理
来源：http://pe.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://kx.huixiangedu.cn

[T28] Swift：枚举
来源：http://va.yuexingan06.cn

enum Color { case red, green }
来源：http://ss.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://re.bookmarksfly.cn

guard let x = opt else { return }
来源：http://qf.521024.cn

[T30] Swift：协议
来源：http://hi.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://hh.huanxung.cn


<!-- 参考信息 -->