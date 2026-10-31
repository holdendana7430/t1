代发 wailian999

echo "${#arr[@]}"
来源：http://fk.asd995.cn

[R20] 关联数组（字典）
来源：http://vj.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qe.lnxyls.cn

[R21] 字符串长度
来源：http://hc.szxytkj.cn

echo "${#s}"
来源：http://ju.nicolike.cn

[R22] 截取子串
来源：http://nt.muxihuayi.cn

echo "${s:0:5}"
来源：http://du.lnxyls.cn

[R23] 字符串替换
来源：http://ub.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ra.nszjky.cn

[R24] 大小写转换
来源：http://py.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ey.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://tq.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sp.muxihuayi.cn

[R26] 命令替换
来源：http://lb.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://gw.shxzskj.cn

[R27] 算术展开
来源：http://cu.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://bu.haigaiapp.cn

[R28] 浮点运算
来源：http://nl.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://fa.hahajie.cn

[R29] 定义函数
来源：http://rx.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://td.szsharing.cn

[R30] 函数返回状态码
来源：http://oa.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://jj.shxzskj.cn

[R31] 局部变量
来源：http://yd.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://gv.hahajie.cn

[R32] 参数个数校验
来源：http://zz.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ug.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://vg.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ch.colortex.cn

[R34] 退出时清理
来源：http://et.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gt.panjiajie.cn

[R35] 后台执行并等待
来源：http://fn.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yi.lnxyls.cn

[R36] 并发执行多个任务
来源：http://lk.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hv.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://vt.521024.cn

files=$(ls -1)
来源：http://mq.colortex.cn

[R38] 管道串联
来源：http://sm.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://px.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://qe.nicolike.cn

cmd > out.log 2>&1
来源：http://ey.huanxung.cn

[R40] 追加写日志
来源：http://oy.huixiangedu.cn

echo "log" >> out.log
来源：http://kt.asd995.cn

[R41] 丢弃输出
来源：http://ys.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://fz.gzmigu.cn

[R42] 输入重定向
来源：http://dg.hnjuh.cn

wc -l < a.txt
来源：http://eq.521024.cn

[R43] 按名字查找文件
来源：http://xj.huanxung.cn

find . -name "*.log" -type f
来源：http://vu.haigaiapp.cn

[R44] 按修改时间查找
来源：http://fc.chemitech.net.cn

find . -mtime -7 -type f
来源：http://dd.521024.cn

[R45] 批量删除
来源：http://kg.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://hh.newstarts.cn

[R46] 递归替换文件内容
来源：http://tv.huixiangedu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pj.shxzukj.cn

[R47] sed 单行替换
来源：http://dk.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yg.muxihuayi.cn

[R48] awk 取指定列
来源：http://iz.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://ra.gzmigu.cn

[R49] awk 带条件
来源：http://kf.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cv.huixiangedu.cn

[R50] awk 求和
来源：http://sa.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mu.9csxet.cn

[R51] 排序去重取前几
来源：http://lu.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wt.9csxet.cn

[R52] 统计行数
来源：http://ks.huixinmuqiang.cn

wc -l a.txt
来源：http://yo.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://xi.jctech888.com.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://if.wgjwhj.cn

[R54] 比较两个文件
来源：http://ba.9csxet.cn

diff a.txt b.txt
来源：http://hm.szsharing.cn

[R55] 压缩与解压
来源：http://pr.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://au.bjjhwx.cn

[R56] 远程拷贝
来源：http://el.chemitech.net.cn

scp file user@host:/path/
来源：http://db.gzmigu.cn

[R57] 远程执行命令
来源：http://am.9csxet.cn

ssh user@host 'uptime'
来源：http://fm.jianghongdianzi.cn

[R58] 下载文件
来源：http://dw.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ld.szxytkj.cn

[R59] 发 POST JSON
来源：http://fn.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://at.wgjwhj.cn

[R60] 只看 HTTP 状态码
来源：http://kp.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yf.newstarts.cn

[R61] 磁盘占用
来源：http://er.521024.cn

df -h;  du -sh *
来源：http://of.szxytkj.cn

[R62] 找最占空间的文件
来源：http://hj.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://by.colortex.cn

[R63] 内存与进程
来源：http://ek.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://ak.hahajie.cn

[R64] 结束进程
来源：http://pr.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://ev.hnjuh.cn

[R65] 查看端口占用
来源：http://da.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rg.jianghongdianzi.cn

[R66] 定时任务
来源：http://qg.szsharing.cn

crontab -e;  crontab -l
来源：http://jg.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://xa.bjjhwx.cn

openssl rand -hex 16
来源：http://hk.muxihuayi.cn

[R68] 计算文件校验值
来源：http://ky.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iy.muxihuayi.cn

[R69] 生成随机密码
来源：http://cq.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ez.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://en.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://dl.chemitech.net.cn

[R71] 日期格式化
来源：http://qw.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lb.panjiajie.cn

[R72] 等待端口就绪
来源：http://za.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xf.szsharing.cn

[R73] 分割大日志
来源：http://zo.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://mw.shtwfgs.cn

[R74] 批量重命名
来源：http://yb.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pv.colortex.cn

[R75] 导出环境变量
来源：http://av.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://fn.shxzskj.cn

[R76] 使用临时文件
来源：http://nx.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://of.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://hq.yuexingan06.cn

read -rp "请输入: " ans
来源：http://oc.gzmigu.cn

[R78] 交互式菜单
来源：http://gm.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://de.hnjuh.cn

[R79] 解析命令行选项
来源：http://qh.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kf.colortex.cn

[R80] 查看脚本执行耗时
来源：http://nr.yuntaijiaju.cn

time ./run.sh
来源：http://cr.chemitech.net.cn

================================================================================
来源：http://eu.lnxyls.cn

S. C / C++ 专题
来源：http://ut.nszjky.cn

================================================================================
来源：http://ub.nicolike.cn

[S01] C：Hello World
来源：http://sf.bjjhwx.cn

#include <stdio.h>
来源：http://ty.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fw.521024.cn

[S02] C：变量与格式化输出
来源：http://dc.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://ff.muxihuayi.cn

[S03] C：读入整数
来源：http://wd.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://uj.huixiangedu.cn

[S04] C：字符串复制
来源：http://ey.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vl.yuexingan06.cn

[S05] C：字符串长度
来源：http://ew.huixinmuqiang.cn

strlen(s)
来源：http://bj.colortex.cn

[S06] C：字符串比较
来源：http://kj.szxytkj.cn

strcmp(a, b) == 0
来源：http://bg.gzmigu.cn

[S07] C：数组遍历求和
来源：http://gk.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xa.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://tq.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tu.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://wu.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bs.nicolike.cn

[S10] C：指针与解引用
来源：http://ma.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://di.szsharing.cn

[S11] C：逐行读文件
来源：http://df.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://pr.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zq.hnjuh.cn

fclose(f);
来源：http://zu.panjiajie.cn

[S12] C：写文件
来源：http://ga.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://if.colortex.cn

[S13] C：宏定义
来源：http://ys.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zj.9csxet.cn

[S14] C：枚举
来源：http://yz.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://gr.9csxet.cn

[S15] C：类型转换
来源：http://xd.wgjwhj.cn

(double) a / b
来源：http://gs.haigaiapp.cn

[S16] C：位操作置位
来源：http://ge.jianghongdianzi.cn

x |= (1 << 3);
来源：http://wo.nicolike.cn

[S17] C：安全拼接字符串
来源：http://ry.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lm.szsharing.cn

[S18] C：命令行参数
来源：http://rk.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://xk.shxzskj.cn

[S19] C：快速排序
来源：http://cb.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yo.yuntaijiaju.cn

[S20] C：二分查找
来源：http://dq.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yp.shxzukj.cn

[S21] C：字符类别判断
来源：http://bv.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mj.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://hc.jianghongdianzi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pn.jianghongdianzi.cn

[S23] C：随机数
来源：http://kj.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://if.huanxung.cn

[S24] C：获取本地时间
来源：http://qb.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lt.yuexingan06.cn

[S25] C：内存拷贝
来源：http://ms.huixiangedu.cn

memcpy(dst, src, n);
来源：http://ec.chemitech.net.cn

[S26] C：内存清零
来源：http://os.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://wb.wgjwhj.cn

[S27] C：定义常量
来源：http://uj.gzmigu.cn

const double PI = 3.14159;
来源：http://ej.bookmarksfly.cn

[S28] C：静态变量
来源：http://cf.szxytkj.cn

static int counter = 0;
来源：http://zt.huanxung.cn

[S29] C：变参函数
来源：http://vy.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bn.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://th.szxytkj.cn

#ifndef X_H
来源：http://wa.haigaiapp.cn

#define X_H
来源：http://qf.yuntaijiaju.cn

#endif
来源：http://wq.hahajie.cn

[S31] C++：Hello World
来源：http://jk.bjjhwx.cn

#include <iostream>
来源：http://jk.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://cy.chemitech.net.cn

[S32] C++：字符串
来源：http://pc.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://uk.shxzukj.cn

[S33] C++：vector 增删
来源：http://te.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vi.panjiajie.cn

[S34] C++：遍历 vector
来源：http://nx.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://bl.9csxet.cn

[S35] C++：map
来源：http://eh.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ou.hahajie.cn

[S36] C++：unordered_map
来源：http://mw.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vs.yuntaijiaju.cn

[S37] C++：set
来源：http://uf.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xx.shxzukj.cn

[S38] C++：排序
来源：http://eq.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://jb.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://xg.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ft.521024.cn

[S40] C++：查找元素
来源：http://ok.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://da.szsharing.cn

[S41] C++：类与构造函数
来源：http://ri.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cw.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://pb.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://vq.szxytkj.cn

[S43] C++：智能指针
来源：http://zr.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://op.asd995.cn

[S44] C++：引用传参
来源：http://sb.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://mu.wgjwhj.cn

[S45] C++：lambda
来源：http://sv.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fi.muxihuayi.cn

[S46] C++：函数模板
来源：http://wx.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hl.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://rx.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hb.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://pv.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ot.colortex.cn

while (std::getline(in, line)) { }
来源：http://vk.chemitech.net.cn

[S49] C++：写文件
来源：http://zt.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zh.szsharing.cn

[S50] C++：格式化数字
来源：http://zf.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hb.szxytkj.cn

[S51] C++：显式类型转换
来源：http://ej.haigaiapp.cn

static_cast<double>(a) / b
来源：http://tl.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://yj.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://je.chemitech.net.cn

[S53] C++：移动语义
来源：http://aw.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ei.521024.cn

[S54] C++：异常处理
来源：http://ng.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pm.gzmigu.cn

[S55] C++：结构化绑定
来源：http://pr.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vj.szxytkj.cn

[S56] C++：optional
来源：http://qj.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://df.yuexingan06.cn

[S57] C++：编译期常量
来源：http://xk.shxzskj.cn

constexpr int N = 10;
来源：http://gm.newstarts.cn

[S58] C++：命名空间
来源：http://qk.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://oi.shtwfgs.cn

[S59] C++：静态断言
来源：http://rs.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ta.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://yq.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cr.shxzskj.cn

================================================================================
来源：http://qg.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pk.panjiajie.cn

================================================================================
来源：http://uh.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://ew.hahajie.cn

println("Hello")
来源：http://mr.huanxung.cn

[T02] Kotlin：变量
来源：http://hk.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vd.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://xb.muxihuayi.cn

"值: $b"
来源：http://ve.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://yt.hahajie.cn

val n: String? = null;  n?.length
来源：http://pv.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://ck.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://co.huanxung.cn

[T06] Kotlin：集合映射
来源：http://jp.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bx.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://qn.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nm.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://gt.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://yt.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://ci.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://bp.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://hp.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mc.hnjuh.cn

[T11] Kotlin：协程
来源：http://ee.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ws.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://qo.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://sx.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://st.huanxung.cn

val m = mapOf("a" to 1)
来源：http://dt.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://vq.newstarts.cn

for (i in 1..10) println(i)
来源：http://ca.jctech888.com.cn

[T15] Kotlin：接口
来源：http://vl.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://fx.nicolike.cn

[T16] Swift：Hello World
来源：http://df.huixiangedu.cn

print("Hello")
来源：http://oz.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://yr.jctech888.com.cn

var a = 1;  let b = 2
来源：http://li.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://iw.hahajie.cn

"值: \(b)"
来源：http://qt.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://ye.huanxung.cn

if let n = opt { print(n) }
来源：http://jk.chemitech.net.cn

[T20] Swift：数组操作
来源：http://od.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ad.chemitech.net.cn

[T21] Swift：遍历
来源：http://uw.bookmarksfly.cn

for x in a { print(x) }
来源：http://wc.gzmigu.cn

[T22] Swift：字典
来源：http://yd.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zt.chemitech.net.cn


<!-- 参考信息 -->