代发 wailian999

echo "${#s}"
来源：http://sq.shtwfgs.cn

[R22] 截取子串
来源：http://ry.haigaiapp.cn

echo "${s:0:5}"
来源：http://qv.chemitech.net.cn

[R23] 字符串替换
来源：http://ly.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gh.shxzskj.cn

[R24] 大小写转换
来源：http://kf.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hb.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://nk.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ro.muxihuayi.cn

[R26] 命令替换
来源：http://bf.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://mg.szxytkj.cn

[R27] 算术展开
来源：http://fc.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://ex.szsharing.cn

[R28] 浮点运算
来源：http://bm.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://um.shtwfgs.cn

[R29] 定义函数
来源：http://ef.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qd.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://em.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://sx.hnjuh.cn

[R31] 局部变量
来源：http://lf.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://qm.nicolike.cn

[R32] 参数个数校验
来源：http://ii.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yx.521024.cn

[R33] 捕获错误并提示行号
来源：http://mz.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ml.nszjky.cn

[R34] 退出时清理
来源：http://ir.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pj.muxihuayi.cn

[R35] 后台执行并等待
来源：http://ip.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dk.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://tf.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mk.asd995.cn

[R37] 把输出赋给变量
来源：http://ou.szxytkj.cn

files=$(ls -1)
来源：http://of.yuntaijiaju.cn

[R38] 管道串联
来源：http://rk.9csxet.cn

cat a.txt | grep -i error | wc -l
来源：http://aa.521024.cn

[R39] 重定向标准输出与错误
来源：http://qv.huixiangedu.cn

cmd > out.log 2>&1
来源：http://rp.shxzukj.cn

[R40] 追加写日志
来源：http://im.lnxyls.cn

echo "log" >> out.log
来源：http://mb.asd995.cn

[R41] 丢弃输出
来源：http://ri.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://qz.wgjwhj.cn

[R42] 输入重定向
来源：http://jv.shtwfgs.cn

wc -l < a.txt
来源：http://gg.nszjky.cn

[R43] 按名字查找文件
来源：http://hi.nicolike.cn

find . -name "*.log" -type f
来源：http://ff.nszjky.cn

[R44] 按修改时间查找
来源：http://ih.haigaiapp.cn

find . -mtime -7 -type f
来源：http://ad.szxytkj.cn

[R45] 批量删除
来源：http://of.9csxet.cn

find . -name "*.tmp" -delete
来源：http://sg.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://kp.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wr.colortex.cn

[R47] sed 单行替换
来源：http://nt.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xa.hahajie.cn

[R48] awk 取指定列
来源：http://pv.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://nf.bjjhwx.cn

[R49] awk 带条件
来源：http://qk.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ai.huixinmuqiang.cn

[R50] awk 求和
来源：http://bl.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yn.panjiajie.cn

[R51] 排序去重取前几
来源：http://uz.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mm.shxzskj.cn

[R52] 统计行数
来源：http://tq.muxihuayi.cn

wc -l a.txt
来源：http://zn.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://vq.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://op.panjiajie.cn

[R54] 比较两个文件
来源：http://po.yuntaijiaju.cn

diff a.txt b.txt
来源：http://xh.9csxet.cn

[R55] 压缩与解压
来源：http://om.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rr.panjiajie.cn

[R56] 远程拷贝
来源：http://em.muxihuayi.cn

scp file user@host:/path/
来源：http://ib.bookmarksfly.cn

[R57] 远程执行命令
来源：http://gw.colortex.cn

ssh user@host 'uptime'
来源：http://gu.shtwfgs.cn

[R58] 下载文件
来源：http://bh.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vz.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ev.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dn.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://fz.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ae.shxzskj.cn

[R61] 磁盘占用
来源：http://td.hnjuh.cn

df -h;  du -sh *
来源：http://tq.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://rm.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ce.bookmarksfly.cn

[R63] 内存与进程
来源：http://id.521024.cn

free -h;  ps aux | grep nginx
来源：http://bn.hnjuh.cn

[R64] 结束进程
来源：http://uc.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://fc.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://vi.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://km.asd995.cn

[R66] 定时任务
来源：http://fg.colortex.cn

crontab -e;  crontab -l
来源：http://cy.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://mz.lnxyls.cn

openssl rand -hex 16
来源：http://im.gzmigu.cn

[R68] 计算文件校验值
来源：http://ww.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dn.yuexingan06.cn

[R69] 生成随机密码
来源：http://hq.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ql.nszjky.cn

[R70] 时间戳与互转
来源：http://yh.asd995.cn

date +%s;  date -d @1700000000
来源：http://al.hnjuh.cn

[R71] 日期格式化
来源：http://qd.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ac.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ma.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rg.asd995.cn

[R73] 分割大日志
来源：http://za.lnxyls.cn

split -l 1000 big.log part_
来源：http://fp.newstarts.cn

[R74] 批量重命名
来源：http://nl.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yg.hahajie.cn

[R75] 导出环境变量
来源：http://pp.huixinmuqiang.cn

export PATH="$HOME/bin:$PATH"
来源：http://zr.shxzskj.cn

[R76] 使用临时文件
来源：http://zk.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jx.wgjwhj.cn

[R77] 读取用户输入
来源：http://pg.huanxung.cn

read -rp "请输入: " ans
来源：http://eg.bookmarksfly.cn

[R78] 交互式菜单
来源：http://lx.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jr.yuexingan06.cn

[R79] 解析命令行选项
来源：http://qp.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yy.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://bo.chemitech.net.cn

time ./run.sh
来源：http://oa.wgjwhj.cn

================================================================================
来源：http://ut.jctech888.com.cn

S. C / C++ 专题
来源：http://eq.szxytkj.cn

================================================================================
来源：http://cz.huanxung.cn

[S01] C：Hello World
来源：http://mn.lnxyls.cn

#include <stdio.h>
来源：http://ou.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cr.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://vu.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://pb.wgjwhj.cn

[S03] C：读入整数
来源：http://ki.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://co.nicolike.cn

[S04] C：字符串复制
来源：http://sx.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kk.huanxung.cn

[S05] C：字符串长度
来源：http://nu.hahajie.cn

strlen(s)
来源：http://ib.newstarts.cn

[S06] C：字符串比较
来源：http://mq.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://za.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://oq.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dj.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://tt.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zx.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://sa.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aa.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://wh.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://us.colortex.cn

[S11] C：逐行读文件
来源：http://ao.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://tz.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ny.huixiangedu.cn

fclose(f);
来源：http://vx.panjiajie.cn

[S12] C：写文件
来源：http://gz.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ke.bjjhwx.cn

[S13] C：宏定义
来源：http://uy.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gk.panjiajie.cn

[S14] C：枚举
来源：http://ph.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://zf.muxihuayi.cn

[S15] C：类型转换
来源：http://or.9csxet.cn

(double) a / b
来源：http://ns.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://fb.huixiangedu.cn

x |= (1 << 3);
来源：http://nx.szsharing.cn

[S17] C：安全拼接字符串
来源：http://xd.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mw.wgjwhj.cn

[S18] C：命令行参数
来源：http://ma.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ro.nicolike.cn

[S19] C：快速排序
来源：http://xx.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gj.asd995.cn

[S20] C：二分查找
来源：http://az.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lc.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://vu.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dv.chemitech.net.cn

[S22] C：字符串转数字
来源：http://so.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ow.huixinmuqiang.cn

[S23] C：随机数
来源：http://mc.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bj.muxihuayi.cn

[S24] C：获取本地时间
来源：http://fi.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ib.huixiangedu.cn

[S25] C：内存拷贝
来源：http://cw.hnjuh.cn

memcpy(dst, src, n);
来源：http://hf.huixinmuqiang.cn

[S26] C：内存清零
来源：http://si.521024.cn

memset(a, 0, sizeof a);
来源：http://ro.huixinmuqiang.cn

[S27] C：定义常量
来源：http://ui.bookmarksfly.cn

const double PI = 3.14159;
来源：http://eq.9csxet.cn

[S28] C：静态变量
来源：http://wn.haigaiapp.cn

static int counter = 0;
来源：http://tc.jctech888.com.cn

[S29] C：变参函数
来源：http://tk.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cv.shxzukj.cn

[S30] C：头文件保护
来源：http://yw.9csxet.cn

#ifndef X_H
来源：http://sm.bjjhwx.cn

#define X_H
来源：http://fa.nicolike.cn

#endif
来源：http://kn.hahajie.cn

[S31] C++：Hello World
来源：http://lx.shxzskj.cn

#include <iostream>
来源：http://wd.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://zm.9csxet.cn

[S32] C++：字符串
来源：http://cn.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://rm.jctech888.com.cn

[S33] C++：vector 增删
来源：http://lh.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sn.9csxet.cn

[S34] C++：遍历 vector
来源：http://hi.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://tb.asd995.cn

[S35] C++：map
来源：http://zy.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uq.shtwfgs.cn

[S36] C++：unordered_map
来源：http://pz.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ns.bjjhwx.cn

[S37] C++：set
来源：http://wp.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zo.9csxet.cn

[S38] C++：排序
来源：http://wr.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://en.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://yf.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sm.hahajie.cn

[S40] C++：查找元素
来源：http://gp.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nn.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://ve.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mz.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://ww.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://gv.hnjuh.cn

[S43] C++：智能指针
来源：http://ez.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ll.panjiajie.cn

[S44] C++：引用传参
来源：http://hy.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://lx.lnxyls.cn

[S45] C++：lambda
来源：http://gi.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bb.newstarts.cn

[S46] C++：函数模板
来源：http://qi.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nh.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://if.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nr.huanxung.cn

[S48] C++：逐行读文件
来源：http://eh.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://se.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://yz.szsharing.cn

[S49] C++：写文件
来源：http://va.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://te.szxytkj.cn

[S50] C++：格式化数字
来源：http://dq.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vw.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://vq.shtwfgs.cn

static_cast<double>(a) / b
来源：http://en.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://uw.szsharing.cn

int size() const noexcept { return n_; }
来源：http://up.bjjhwx.cn

[S53] C++：移动语义
来源：http://hq.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://lq.9csxet.cn

[S54] C++：异常处理
来源：http://tc.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ht.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://rw.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ha.colortex.cn

[S56] C++：optional
来源：http://rl.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wn.yuexingan06.cn

[S57] C++：编译期常量
来源：http://uh.shxzukj.cn

constexpr int N = 10;
来源：http://vw.lnxyls.cn

[S58] C++：命名空间
来源：http://fz.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://ea.shxzskj.cn

[S59] C++：静态断言
来源：http://sx.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cc.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://uh.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zr.bookmarksfly.cn

================================================================================
来源：http://fl.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vl.9csxet.cn

================================================================================
来源：http://ge.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://gu.bookmarksfly.cn

println("Hello")
来源：http://ir.wgjwhj.cn

[T02] Kotlin：变量
来源：http://uo.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jp.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://kc.hahajie.cn

"值: $b"
来源：http://om.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://ol.panjiajie.cn

val n: String? = null;  n?.length
来源：http://dl.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://yc.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dq.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://og.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bv.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://qi.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ma.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://te.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://gu.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://va.521024.cn

fun String.exclaim() = this + "!"
来源：http://ij.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://wj.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zd.shtwfgs.cn

[T11] Kotlin：协程
来源：http://xf.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gr.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://mf.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://mt.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://vm.521024.cn

val m = mapOf("a" to 1)
来源：http://nl.lnxyls.cn

[T14] Kotlin：循环
来源：http://on.newstarts.cn

for (i in 1..10) println(i)
来源：http://od.colortex.cn

[T15] Kotlin：接口
来源：http://ju.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ia.haigaiapp.cn

[T16] Swift：Hello World
来源：http://or.yuexingan06.cn

print("Hello")
来源：http://gx.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://mf.nicolike.cn

var a = 1;  let b = 2
来源：http://ig.nicolike.cn

[T18] Swift：字符串插值
来源：http://ka.asd995.cn

"值: \(b)"
来源：http://fa.nszjky.cn

[T19] Swift：可选绑定
来源：http://pp.muxihuayi.cn

if let n = opt { print(n) }
来源：http://db.wgjwhj.cn

[T20] Swift：数组操作
来源：http://ka.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oc.chemitech.net.cn

[T21] Swift：遍历
来源：http://wo.wgjwhj.cn

for x in a { print(x) }
来源：http://dm.colortex.cn

[T22] Swift：字典
来源：http://if.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zz.huixinmuqiang.cn

[T23] Swift：函数
来源：http://cu.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ly.gzmigu.cn

[T24] Swift：闭包
来源：http://ok.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kb.panjiajie.cn


<!-- 参考信息 -->