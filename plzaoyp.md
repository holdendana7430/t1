代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ar.chemitech.net.cn

[R24] 大小写转换
来源：http://bk.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mh.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://yk.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nf.shtwfgs.cn

[R26] 命令替换
来源：http://do.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://cy.colortex.cn

[R27] 算术展开
来源：http://ug.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://om.nszjky.cn

[R28] 浮点运算
来源：http://jq.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://vp.nszjky.cn

[R29] 定义函数
来源：http://ds.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bu.nszjky.cn

[R30] 函数返回状态码
来源：http://ew.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://kn.newstarts.cn

[R31] 局部变量
来源：http://lw.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://ul.wgjwhj.cn

[R32] 参数个数校验
来源：http://je.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wt.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://mw.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lh.wgjwhj.cn

[R34] 退出时清理
来源：http://im.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bv.yuexingan06.cn

[R35] 后台执行并等待
来源：http://xv.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hj.9csxet.cn

[R36] 并发执行多个任务
来源：http://vb.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yu.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://kl.haigaiapp.cn

files=$(ls -1)
来源：http://us.nicolike.cn

[R38] 管道串联
来源：http://um.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://pk.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://pw.chemitech.net.cn

cmd > out.log 2>&1
来源：http://uz.lnxyls.cn

[R40] 追加写日志
来源：http://fr.bjjhwx.cn

echo "log" >> out.log
来源：http://sz.bookmarksfly.cn

[R41] 丢弃输出
来源：http://bw.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://eh.gzmigu.cn

[R42] 输入重定向
来源：http://nd.jianghongdianzi.cn

wc -l < a.txt
来源：http://sw.szxytkj.cn

[R43] 按名字查找文件
来源：http://mn.haigaiapp.cn

find . -name "*.log" -type f
来源：http://vp.colortex.cn

[R44] 按修改时间查找
来源：http://br.nicolike.cn

find . -mtime -7 -type f
来源：http://ak.hahajie.cn

[R45] 批量删除
来源：http://iw.colortex.cn

find . -name "*.tmp" -delete
来源：http://se.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://rj.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nm.asd995.cn

[R47] sed 单行替换
来源：http://vm.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rm.huanxung.cn

[R48] awk 取指定列
来源：http://lx.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ol.lnxyls.cn

[R49] awk 带条件
来源：http://kb.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tl.asd995.cn

[R50] awk 求和
来源：http://yy.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yc.9csxet.cn

[R51] 排序去重取前几
来源：http://wx.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ei.jianghongdianzi.cn

[R52] 统计行数
来源：http://no.asd995.cn

wc -l a.txt
来源：http://ig.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://fc.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://es.szxytkj.cn

[R54] 比较两个文件
来源：http://ks.hahajie.cn

diff a.txt b.txt
来源：http://sb.haigaiapp.cn

[R55] 压缩与解压
来源：http://lq.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nl.huixiangedu.cn

[R56] 远程拷贝
来源：http://dn.haigaiapp.cn

scp file user@host:/path/
来源：http://dh.nszjky.cn

[R57] 远程执行命令
来源：http://zs.9csxet.cn

ssh user@host 'uptime'
来源：http://dw.muxihuayi.cn

[R58] 下载文件
来源：http://cx.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pf.wgjwhj.cn

[R59] 发 POST JSON
来源：http://tx.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hl.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://wa.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qd.yuexingan06.cn

[R61] 磁盘占用
来源：http://fw.gzmigu.cn

df -h;  du -sh *
来源：http://xt.hahajie.cn

[R62] 找最占空间的文件
来源：http://pm.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://wt.jctech888.com.cn

[R63] 内存与进程
来源：http://tb.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://sa.lnxyls.cn

[R64] 结束进程
来源：http://zv.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://dq.wgjwhj.cn

[R65] 查看端口占用
来源：http://hv.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://id.szsharing.cn

[R66] 定时任务
来源：http://ip.huanxung.cn

crontab -e;  crontab -l
来源：http://yq.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://ai.521024.cn

openssl rand -hex 16
来源：http://zw.jctech888.com.cn

[R68] 计算文件校验值
来源：http://mo.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fr.nszjky.cn

[R69] 生成随机密码
来源：http://nc.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://nr.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://bg.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://qz.panjiajie.cn

[R71] 日期格式化
来源：http://xw.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yd.521024.cn

[R72] 等待端口就绪
来源：http://yl.lnxyls.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ds.wgjwhj.cn

[R73] 分割大日志
来源：http://do.chemitech.net.cn

split -l 1000 big.log part_
来源：http://jm.yuntaijiaju.cn

[R74] 批量重命名
来源：http://ku.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://se.newstarts.cn

[R75] 导出环境变量
来源：http://ia.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://kn.hahajie.cn

[R76] 使用临时文件
来源：http://eo.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xz.huixiangedu.cn

[R77] 读取用户输入
来源：http://gr.szxytkj.cn

read -rp "请输入: " ans
来源：http://el.shxzskj.cn

[R78] 交互式菜单
来源：http://fh.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cz.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://bc.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ls.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://hg.colortex.cn

time ./run.sh
来源：http://hc.bookmarksfly.cn

================================================================================
来源：http://ru.bookmarksfly.cn

S. C / C++ 专题
来源：http://kl.9csxet.cn

================================================================================
来源：http://gw.chemitech.net.cn

[S01] C：Hello World
来源：http://we.muxihuayi.cn

#include <stdio.h>
来源：http://of.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ms.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://ul.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://fr.yuexingan06.cn

[S03] C：读入整数
来源：http://al.nicolike.cn

int x; scanf("%d", &x);
来源：http://ng.bjjhwx.cn

[S04] C：字符串复制
来源：http://rg.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rv.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://of.jianghongdianzi.cn

strlen(s)
来源：http://yo.nicolike.cn

[S06] C：字符串比较
来源：http://sv.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://ua.newstarts.cn

[S07] C：数组遍历求和
来源：http://pn.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xm.521024.cn

[S08] C：动态内存分配与释放
来源：http://kl.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://em.521024.cn

[S09] C：结构体定义与初始化
来源：http://dp.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jv.gzmigu.cn

[S10] C：指针与解引用
来源：http://wn.nszjky.cn

int *p = &a;  *p = 5;
来源：http://ug.colortex.cn

[S11] C：逐行读文件
来源：http://vz.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://gp.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uy.nicolike.cn

fclose(f);
来源：http://jn.jctech888.com.cn

[S12] C：写文件
来源：http://rj.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rc.lnxyls.cn

[S13] C：宏定义
来源：http://ys.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sq.huanxung.cn

[S14] C：枚举
来源：http://la.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://py.huixinmuqiang.cn

[S15] C：类型转换
来源：http://xj.shtwfgs.cn

(double) a / b
来源：http://gn.haigaiapp.cn

[S16] C：位操作置位
来源：http://qo.shtwfgs.cn

x |= (1 << 3);
来源：http://wb.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://ii.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hr.panjiajie.cn

[S18] C：命令行参数
来源：http://ve.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://jm.jianghongdianzi.cn

[S19] C：快速排序
来源：http://fz.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ol.nicolike.cn

[S20] C：二分查找
来源：http://mu.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zv.bjjhwx.cn

[S21] C：字符类别判断
来源：http://fk.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://na.shxzskj.cn

[S22] C：字符串转数字
来源：http://lu.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pd.lnxyls.cn

[S23] C：随机数
来源：http://al.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://np.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://oe.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vo.haigaiapp.cn

[S25] C：内存拷贝
来源：http://ej.haigaiapp.cn

memcpy(dst, src, n);
来源：http://ws.shxzskj.cn

[S26] C：内存清零
来源：http://an.colortex.cn

memset(a, 0, sizeof a);
来源：http://qt.wgjwhj.cn

[S27] C：定义常量
来源：http://lk.szsharing.cn

const double PI = 3.14159;
来源：http://el.9csxet.cn

[S28] C：静态变量
来源：http://ct.muxihuayi.cn

static int counter = 0;
来源：http://ms.nicolike.cn

[S29] C：变参函数
来源：http://jz.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oe.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://eh.wgjwhj.cn

#ifndef X_H
来源：http://ks.panjiajie.cn

#define X_H
来源：http://tg.colortex.cn

#endif
来源：http://wj.nicolike.cn

[S31] C++：Hello World
来源：http://mk.muxihuayi.cn

#include <iostream>
来源：http://uk.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://uu.panjiajie.cn

[S32] C++：字符串
来源：http://oi.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://xt.521024.cn

[S33] C++：vector 增删
来源：http://si.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://we.shxzukj.cn

[S34] C++：遍历 vector
来源：http://fp.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://mn.shxzskj.cn

[S35] C++：map
来源：http://bb.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zz.haigaiapp.cn

[S36] C++：unordered_map
来源：http://jh.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ge.yuexingan06.cn

[S37] C++：set
来源：http://de.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dt.chemitech.net.cn

[S38] C++：排序
来源：http://qz.colortex.cn

std::sort(v.begin(), v.end());
来源：http://mw.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://th.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xo.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://he.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kp.szxytkj.cn

[S41] C++：类与构造函数
来源：http://ar.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ru.asd995.cn

[S42] C++：继承与虚函数
来源：http://ti.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://ag.chemitech.net.cn

[S43] C++：智能指针
来源：http://bg.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://ql.haigaiapp.cn

[S44] C++：引用传参
来源：http://kv.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://dh.shxzskj.cn

[S45] C++：lambda
来源：http://pu.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://af.chemitech.net.cn

[S46] C++：函数模板
来源：http://py.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rk.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://hl.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iq.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://lj.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hl.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://gz.shxzskj.cn

[S49] C++：写文件
来源：http://og.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ti.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://rr.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uk.shxzukj.cn

[S51] C++：显式类型转换
来源：http://nu.szsharing.cn

static_cast<double>(a) / b
来源：http://ap.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://xl.szsharing.cn

int size() const noexcept { return n_; }
来源：http://cn.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://pb.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://au.hahajie.cn

[S54] C++：异常处理
来源：http://cu.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mx.gzmigu.cn

[S55] C++：结构化绑定
来源：http://fr.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ck.nszjky.cn

[S56] C++：optional
来源：http://ub.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ne.asd995.cn

[S57] C++：编译期常量
来源：http://id.yuntaijiaju.cn

constexpr int N = 10;
来源：http://hk.lnxyls.cn

[S58] C++：命名空间
来源：http://as.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://vq.haigaiapp.cn

[S59] C++：静态断言
来源：http://ir.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sv.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://ub.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xy.yuexingan06.cn

================================================================================
来源：http://tv.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ao.asd995.cn

================================================================================
来源：http://dc.nicolike.cn

[T01] Kotlin：Hello World
来源：http://dz.bookmarksfly.cn

println("Hello")
来源：http://bm.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://zc.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iz.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://gp.hnjuh.cn

"值: $b"
来源：http://cu.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://vn.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://xa.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://ix.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hj.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://vv.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yt.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://mv.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jm.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://lc.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ty.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://xb.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://gc.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://nc.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rg.shxzskj.cn

[T11] Kotlin：协程
来源：http://ph.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://of.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://jc.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ej.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://ao.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://co.nicolike.cn

[T14] Kotlin：循环
来源：http://fw.szsharing.cn

for (i in 1..10) println(i)
来源：http://lz.9csxet.cn

[T15] Kotlin：接口
来源：http://hv.nicolike.cn

interface Shape { fun area(): Double }
来源：http://gd.bjjhwx.cn

[T16] Swift：Hello World
来源：http://yu.yuexingan06.cn

print("Hello")
来源：http://vw.newstarts.cn

[T17] Swift：变量与常量
来源：http://cb.huixiangedu.cn

var a = 1;  let b = 2
来源：http://cj.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://vp.haigaiapp.cn

"值: \(b)"
来源：http://ch.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://hd.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://lt.bjjhwx.cn

[T20] Swift：数组操作
来源：http://op.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mn.newstarts.cn

[T21] Swift：遍历
来源：http://re.haigaiapp.cn

for x in a { print(x) }
来源：http://uf.nszjky.cn

[T22] Swift：字典
来源：http://mu.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cl.hahajie.cn

[T23] Swift：函数
来源：http://co.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vl.hahajie.cn

[T24] Swift：闭包
来源：http://dl.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hf.wgjwhj.cn

[T25] Swift：结构体
来源：http://hh.9csxet.cn

struct P { var x: Int }
来源：http://xs.9csxet.cn

[T26] Swift：类与重写
来源：http://cw.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://wh.nszjky.cn


<!-- 参考信息 -->