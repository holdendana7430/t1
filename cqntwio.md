代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://me.gzmigu.cn

[R18] 遍历数组
来源：http://ta.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jt.hnjuh.cn

[R19] 数组长度
来源：http://pl.bjjhwx.cn

echo "${#arr[@]}"
来源：http://bp.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://wp.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jx.huixinmuqiang.cn

[R21] 字符串长度
来源：http://cn.haigaiapp.cn

echo "${#s}"
来源：http://ov.asd995.cn

[R22] 截取子串
来源：http://fd.muxihuayi.cn

echo "${s:0:5}"
来源：http://vg.newstarts.cn

[R23] 字符串替换
来源：http://vq.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aw.newstarts.cn

[R24] 大小写转换
来源：http://zw.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pk.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://ku.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vr.yuexingan06.cn

[R26] 命令替换
来源：http://ad.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://xm.szsharing.cn

[R27] 算术展开
来源：http://bo.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://kb.yuexingan06.cn

[R28] 浮点运算
来源：http://mq.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://da.panjiajie.cn

[R29] 定义函数
来源：http://fe.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ul.jctech888.com.cn

[R30] 函数返回状态码
来源：http://ru.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://rr.shxzukj.cn

[R31] 局部变量
来源：http://ni.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://fv.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://rr.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lw.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://ga.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://px.bjjhwx.cn

[R34] 退出时清理
来源：http://zs.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xw.szsharing.cn

[R35] 后台执行并等待
来源：http://tt.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wc.shxzukj.cn

[R36] 并发执行多个任务
来源：http://dw.chemitech.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mg.hnjuh.cn

[R37] 把输出赋给变量
来源：http://tn.9csxet.cn

files=$(ls -1)
来源：http://pj.nszjky.cn

[R38] 管道串联
来源：http://by.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://ex.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://oy.huixiangedu.cn

cmd > out.log 2>&1
来源：http://su.yuntaijiaju.cn

[R40] 追加写日志
来源：http://cg.chemitech.net.cn

echo "log" >> out.log
来源：http://mr.shxzskj.cn

[R41] 丢弃输出
来源：http://td.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://pk.9csxet.cn

[R42] 输入重定向
来源：http://xo.bookmarksfly.cn

wc -l < a.txt
来源：http://ua.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://vb.haigaiapp.cn

find . -name "*.log" -type f
来源：http://yl.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://pg.wgjwhj.cn

find . -mtime -7 -type f
来源：http://ux.szsharing.cn

[R45] 批量删除
来源：http://kz.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://ag.shxzukj.cn

[R46] 递归替换文件内容
来源：http://un.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ev.panjiajie.cn

[R47] sed 单行替换
来源：http://uw.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hc.nicolike.cn

[R48] awk 取指定列
来源：http://ap.521024.cn

awk '{print $1, $3}' a.txt
来源：http://ks.nicolike.cn

[R49] awk 带条件
来源：http://ik.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cc.gzmigu.cn

[R50] awk 求和
来源：http://hf.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gs.yuexingan06.cn

[R51] 排序去重取前几
来源：http://sk.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sm.yuntaijiaju.cn

[R52] 统计行数
来源：http://ys.huixiangedu.cn

wc -l a.txt
来源：http://ki.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://vm.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jl.nicolike.cn

[R54] 比较两个文件
来源：http://la.newstarts.cn

diff a.txt b.txt
来源：http://so.bookmarksfly.cn

[R55] 压缩与解压
来源：http://vh.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mr.shxzskj.cn

[R56] 远程拷贝
来源：http://ws.gzmigu.cn

scp file user@host:/path/
来源：http://hs.huixiangedu.cn

[R57] 远程执行命令
来源：http://kv.gzmigu.cn

ssh user@host 'uptime'
来源：http://fi.shtwfgs.cn

[R58] 下载文件
来源：http://yd.haigaiapp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://va.szxytkj.cn

[R59] 发 POST JSON
来源：http://jk.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ji.521024.cn

[R60] 只看 HTTP 状态码
来源：http://hk.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tn.huixiangedu.cn

[R61] 磁盘占用
来源：http://iw.521024.cn

df -h;  du -sh *
来源：http://oj.shxzukj.cn

[R62] 找最占空间的文件
来源：http://px.521024.cn

du -ah . | sort -rh | head -10
来源：http://cd.jianghongdianzi.cn

[R63] 内存与进程
来源：http://gz.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://bh.gzmigu.cn

[R64] 结束进程
来源：http://bi.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://uu.panjiajie.cn

[R65] 查看端口占用
来源：http://iq.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vn.521024.cn

[R66] 定时任务
来源：http://px.shxzskj.cn

crontab -e;  crontab -l
来源：http://ll.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://wm.bjjhwx.cn

openssl rand -hex 16
来源：http://gg.bjjhwx.cn

[R68] 计算文件校验值
来源：http://mf.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yf.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://dn.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://wg.521024.cn

[R70] 时间戳与互转
来源：http://ig.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://po.wgjwhj.cn

[R71] 日期格式化
来源：http://en.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mc.shxzskj.cn

[R72] 等待端口就绪
来源：http://xj.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sz.bjjhwx.cn

[R73] 分割大日志
来源：http://ll.hahajie.cn

split -l 1000 big.log part_
来源：http://ro.jctech888.com.cn

[R74] 批量重命名
来源：http://wh.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kf.bookmarksfly.cn

[R75] 导出环境变量
来源：http://bo.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://am.bjjhwx.cn

[R76] 使用临时文件
来源：http://kx.szxytkj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gj.521024.cn

[R77] 读取用户输入
来源：http://ux.muxihuayi.cn

read -rp "请输入: " ans
来源：http://vs.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://lr.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mo.muxihuayi.cn

[R79] 解析命令行选项
来源：http://rw.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yv.wgjwhj.cn

[R80] 查看脚本执行耗时
来源：http://oe.yuexingan06.cn

time ./run.sh
来源：http://jg.hnjuh.cn

================================================================================
来源：http://qm.shxzukj.cn

S. C / C++ 专题
来源：http://we.asd995.cn

================================================================================
来源：http://io.szxytkj.cn

[S01] C：Hello World
来源：http://gs.colortex.cn

#include <stdio.h>
来源：http://uf.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kz.newstarts.cn

[S02] C：变量与格式化输出
来源：http://bj.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://xx.bookmarksfly.cn

[S03] C：读入整数
来源：http://yj.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://ox.9csxet.cn

[S04] C：字符串复制
来源：http://kn.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://me.jctech888.com.cn

[S05] C：字符串长度
来源：http://fo.panjiajie.cn

strlen(s)
来源：http://mg.asd995.cn

[S06] C：字符串比较
来源：http://ab.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://pj.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://zw.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ut.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://eq.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tp.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://ax.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://na.colortex.cn

[S10] C：指针与解引用
来源：http://kt.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://oo.gzmigu.cn

[S11] C：逐行读文件
来源：http://di.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ky.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pe.muxihuayi.cn

fclose(f);
来源：http://gu.wgjwhj.cn

[S12] C：写文件
来源：http://dk.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hg.huixiangedu.cn

[S13] C：宏定义
来源：http://qa.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zw.shtwfgs.cn

[S14] C：枚举
来源：http://dk.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://it.huixiangedu.cn

[S15] C：类型转换
来源：http://rj.newstarts.cn

(double) a / b
来源：http://ar.nicolike.cn

[S16] C：位操作置位
来源：http://ut.bookmarksfly.cn

x |= (1 << 3);
来源：http://kl.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://gf.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gr.huanxung.cn

[S18] C：命令行参数
来源：http://tx.yuexingan06.cn

int main(int argc, char **argv)
来源：http://sr.muxihuayi.cn

[S19] C：快速排序
来源：http://vr.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ub.yuntaijiaju.cn

[S20] C：二分查找
来源：http://nk.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rk.wgjwhj.cn

[S21] C：字符类别判断
来源：http://au.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ka.shxzukj.cn

[S22] C：字符串转数字
来源：http://bm.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kq.huanxung.cn

[S23] C：随机数
来源：http://mq.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://os.521024.cn

[S24] C：获取本地时间
来源：http://jk.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fa.muxihuayi.cn

[S25] C：内存拷贝
来源：http://gq.newstarts.cn

memcpy(dst, src, n);
来源：http://he.muxihuayi.cn

[S26] C：内存清零
来源：http://vg.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://zp.hnjuh.cn

[S27] C：定义常量
来源：http://ho.shxzukj.cn

const double PI = 3.14159;
来源：http://oh.colortex.cn

[S28] C：静态变量
来源：http://ds.gzmigu.cn

static int counter = 0;
来源：http://je.muxihuayi.cn

[S29] C：变参函数
来源：http://sx.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ai.hnjuh.cn

[S30] C：头文件保护
来源：http://yf.newstarts.cn

#ifndef X_H
来源：http://oq.hnjuh.cn

#define X_H
来源：http://ec.panjiajie.cn

#endif
来源：http://ty.wgjwhj.cn

[S31] C++：Hello World
来源：http://kq.szxytkj.cn

#include <iostream>
来源：http://ld.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://oe.hahajie.cn

[S32] C++：字符串
来源：http://uu.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://ni.panjiajie.cn

[S33] C++：vector 增删
来源：http://pq.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vx.panjiajie.cn

[S34] C++：遍历 vector
来源：http://yx.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://yr.yuexingan06.cn

[S35] C++：map
来源：http://wy.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cw.hnjuh.cn

[S36] C++：unordered_map
来源：http://fe.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://os.shxzukj.cn

[S37] C++：set
来源：http://qz.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qo.colortex.cn

[S38] C++：排序
来源：http://uf.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://qm.shtwfgs.cn

[S39] C++：自定义比较器排序
来源：http://ih.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://we.shtwfgs.cn

[S40] C++：查找元素
来源：http://xs.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://no.nszjky.cn

[S41] C++：类与构造函数
来源：http://sq.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://js.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://ju.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://rg.muxihuayi.cn

[S43] C++：智能指针
来源：http://ns.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://jg.szsharing.cn

[S44] C++：引用传参
来源：http://bd.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://ny.colortex.cn

[S45] C++：lambda
来源：http://er.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vb.521024.cn

[S46] C++：函数模板
来源：http://in.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eu.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://cj.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kn.panjiajie.cn

[S48] C++：逐行读文件
来源：http://wl.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ad.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ju.jianghongdianzi.cn

[S49] C++：写文件
来源：http://vj.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bo.hnjuh.cn

[S50] C++：格式化数字
来源：http://vl.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vz.szsharing.cn

[S51] C++：显式类型转换
来源：http://pc.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://cz.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://we.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://dd.nszjky.cn

[S53] C++：移动语义
来源：http://fa.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://mt.szxytkj.cn

[S54] C++：异常处理
来源：http://hu.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fu.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://cq.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yy.szsharing.cn

[S56] C++：optional
来源：http://og.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ju.panjiajie.cn

[S57] C++：编译期常量
来源：http://hy.9csxet.cn

constexpr int N = 10;
来源：http://ce.gzmigu.cn

[S58] C++：命名空间
来源：http://wk.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://dw.nicolike.cn

[S59] C++：静态断言
来源：http://qd.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://um.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://ts.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gt.9csxet.cn

================================================================================
来源：http://pc.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bn.nicolike.cn

================================================================================
来源：http://vq.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ly.asd995.cn

println("Hello")
来源：http://zj.521024.cn

[T02] Kotlin：变量
来源：http://aj.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fj.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://kl.hnjuh.cn

"值: $b"
来源：http://tu.panjiajie.cn

[T04] Kotlin：空安全
来源：http://ba.hahajie.cn

val n: String? = null;  n?.length
来源：http://sk.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://ov.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zd.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://ci.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ql.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://jm.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nd.szsharing.cn

[T08] Kotlin：数据类
来源：http://sl.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://tm.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://gm.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://is.nicolike.cn

[T10] Kotlin：默认参数
来源：http://df.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tt.shtwfgs.cn

[T11] Kotlin：协程
来源：http://dc.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tf.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://bz.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://rx.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://bt.hahajie.cn

val m = mapOf("a" to 1)
来源：http://xp.huanxung.cn

[T14] Kotlin：循环
来源：http://no.521024.cn

for (i in 1..10) println(i)
来源：http://ds.nszjky.cn

[T15] Kotlin：接口
来源：http://kr.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://np.szsharing.cn

[T16] Swift：Hello World
来源：http://lv.bookmarksfly.cn

print("Hello")
来源：http://xp.shxzskj.cn

[T17] Swift：变量与常量
来源：http://gg.nszjky.cn

var a = 1;  let b = 2
来源：http://oe.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://ob.shtwfgs.cn

"值: \(b)"
来源：http://rx.hahajie.cn

[T19] Swift：可选绑定
来源：http://gw.yuexingan06.cn

if let n = opt { print(n) }
来源：http://lb.haigaiapp.cn

[T20] Swift：数组操作
来源：http://ul.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hw.huanxung.cn


<!-- 参考信息 -->