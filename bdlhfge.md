代发 wailian999

echo "${#s}"
来源：http://sc.colortex.cn

[R22] 截取子串
来源：http://id.panjiajie.cn

echo "${s:0:5}"
来源：http://vp.wgjwhj.cn

[R23] 字符串替换
来源：http://dy.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xr.newstarts.cn

[R24] 大小写转换
来源：http://hc.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yp.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://tq.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pq.colortex.cn

[R26] 命令替换
来源：http://nx.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://br.colortex.cn

[R27] 算术展开
来源：http://ra.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://mz.hnjuh.cn

[R28] 浮点运算
来源：http://wa.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://wj.newstarts.cn

[R29] 定义函数
来源：http://oq.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ui.shxzukj.cn

[R30] 函数返回状态码
来源：http://fq.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://hu.yuexingan06.cn

[R31] 局部变量
来源：http://zi.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://vs.521024.cn

[R32] 参数个数校验
来源：http://pv.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jc.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://nq.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wu.nszjky.cn

[R34] 退出时清理
来源：http://vf.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uo.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://wj.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sa.nicolike.cn

[R36] 并发执行多个任务
来源：http://ok.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mj.shxzskj.cn

[R37] 把输出赋给变量
来源：http://ow.szsharing.cn

files=$(ls -1)
来源：http://ft.jctech888.com.cn

[R38] 管道串联
来源：http://wx.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://pm.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://wq.jctech888.com.cn

cmd > out.log 2>&1
来源：http://jn.yuexingan06.cn

[R40] 追加写日志
来源：http://ca.bookmarksfly.cn

echo "log" >> out.log
来源：http://ig.huanxung.cn

[R41] 丢弃输出
来源：http://ll.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://hh.muxihuayi.cn

[R42] 输入重定向
来源：http://kb.lnxyls.cn

wc -l < a.txt
来源：http://kd.szsharing.cn

[R43] 按名字查找文件
来源：http://xw.shtwfgs.cn

find . -name "*.log" -type f
来源：http://zm.hnjuh.cn

[R44] 按修改时间查找
来源：http://hi.huanxung.cn

find . -mtime -7 -type f
来源：http://cu.huixiangedu.cn

[R45] 批量删除
来源：http://rm.nszjky.cn

find . -name "*.tmp" -delete
来源：http://rr.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://ki.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xo.haigaiapp.cn

[R47] sed 单行替换
来源：http://nx.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dt.nicolike.cn

[R48] awk 取指定列
来源：http://et.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://gv.newstarts.cn

[R49] awk 带条件
来源：http://gn.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://px.nszjky.cn

[R50] awk 求和
来源：http://uv.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ws.hnjuh.cn

[R51] 排序去重取前几
来源：http://rk.hnjuh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cd.wgjwhj.cn

[R52] 统计行数
来源：http://dy.wgjwhj.cn

wc -l a.txt
来源：http://bz.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://wm.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hm.yuexingan06.cn

[R54] 比较两个文件
来源：http://uu.wgjwhj.cn

diff a.txt b.txt
来源：http://kr.wgjwhj.cn

[R55] 压缩与解压
来源：http://eb.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xr.hahajie.cn

[R56] 远程拷贝
来源：http://ek.haigaiapp.cn

scp file user@host:/path/
来源：http://ds.bookmarksfly.cn

[R57] 远程执行命令
来源：http://gq.szxytkj.cn

ssh user@host 'uptime'
来源：http://bc.9csxet.cn

[R58] 下载文件
来源：http://ot.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://et.jctech888.com.cn

[R59] 发 POST JSON
来源：http://ai.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ih.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://nr.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zs.newstarts.cn

[R61] 磁盘占用
来源：http://fq.huixinmuqiang.cn

df -h;  du -sh *
来源：http://qa.nszjky.cn

[R62] 找最占空间的文件
来源：http://qq.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://dg.shxzukj.cn

[R63] 内存与进程
来源：http://ct.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://ry.szsharing.cn

[R64] 结束进程
来源：http://dn.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://kz.wgjwhj.cn

[R65] 查看端口占用
来源：http://ic.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://re.chemitech.net.cn

[R66] 定时任务
来源：http://xn.hahajie.cn

crontab -e;  crontab -l
来源：http://lq.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://rj.hnjuh.cn

openssl rand -hex 16
来源：http://bv.chemitech.net.cn

[R68] 计算文件校验值
来源：http://bi.yuexingan06.cn

sha256sum a.txt;  md5sum a.txt
来源：http://be.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://nn.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://op.nszjky.cn

[R70] 时间戳与互转
来源：http://ch.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://qy.huanxung.cn

[R71] 日期格式化
来源：http://ay.shxzukj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cr.hahajie.cn

[R72] 等待端口就绪
来源：http://ut.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://to.wgjwhj.cn

[R73] 分割大日志
来源：http://sl.yuexingan06.cn

split -l 1000 big.log part_
来源：http://us.shxzukj.cn

[R74] 批量重命名
来源：http://ah.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mf.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://pa.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://vg.asd995.cn

[R76] 使用临时文件
来源：http://pb.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ll.szsharing.cn

[R77] 读取用户输入
来源：http://oe.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://uu.szsharing.cn

[R78] 交互式菜单
来源：http://ro.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gb.521024.cn

[R79] 解析命令行选项
来源：http://tb.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ur.521024.cn

[R80] 查看脚本执行耗时
来源：http://fl.huixiangedu.cn

time ./run.sh
来源：http://ds.wgjwhj.cn

================================================================================
来源：http://yj.521024.cn

S. C / C++ 专题
来源：http://vb.gzmigu.cn

================================================================================
来源：http://dd.huanxung.cn

[S01] C：Hello World
来源：http://yb.521024.cn

#include <stdio.h>
来源：http://dg.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://si.newstarts.cn

[S02] C：变量与格式化输出
来源：http://gw.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://wq.huixinmuqiang.cn

[S03] C：读入整数
来源：http://hw.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://yt.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://rk.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gs.muxihuayi.cn

[S05] C：字符串长度
来源：http://hd.yuntaijiaju.cn

strlen(s)
来源：http://ut.nszjky.cn

[S06] C：字符串比较
来源：http://eh.chemitech.net.cn

strcmp(a, b) == 0
来源：http://ha.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://cv.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ft.521024.cn

[S08] C：动态内存分配与释放
来源：http://jw.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qw.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://qe.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ne.huixiangedu.cn

[S10] C：指针与解引用
来源：http://pf.9csxet.cn

int *p = &a;  *p = 5;
来源：http://is.521024.cn

[S11] C：逐行读文件
来源：http://of.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://jj.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dm.yuexingan06.cn

fclose(f);
来源：http://fr.shxzskj.cn

[S12] C：写文件
来源：http://vf.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nu.muxihuayi.cn

[S13] C：宏定义
来源：http://gi.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hv.jianghongdianzi.cn

[S14] C：枚举
来源：http://fx.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://be.chemitech.net.cn

[S15] C：类型转换
来源：http://sy.huanxung.cn

(double) a / b
来源：http://id.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://mf.huixiangedu.cn

x |= (1 << 3);
来源：http://go.hahajie.cn

[S17] C：安全拼接字符串
来源：http://er.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ev.wgjwhj.cn

[S18] C：命令行参数
来源：http://gx.shtwfgs.cn

int main(int argc, char **argv)
来源：http://fo.huixinmuqiang.cn

[S19] C：快速排序
来源：http://fm.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ff.szsharing.cn

[S20] C：二分查找
来源：http://gc.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ze.huixiangedu.cn

[S21] C：字符类别判断
来源：http://wi.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nc.muxihuayi.cn

[S22] C：字符串转数字
来源：http://ke.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pd.szsharing.cn

[S23] C：随机数
来源：http://cy.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ej.szxytkj.cn

[S24] C：获取本地时间
来源：http://jt.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xn.521024.cn

[S25] C：内存拷贝
来源：http://dk.gzmigu.cn

memcpy(dst, src, n);
来源：http://yw.9csxet.cn

[S26] C：内存清零
来源：http://nh.asd995.cn

memset(a, 0, sizeof a);
来源：http://lf.yuexingan06.cn

[S27] C：定义常量
来源：http://uh.hahajie.cn

const double PI = 3.14159;
来源：http://rh.shxzskj.cn

[S28] C：静态变量
来源：http://kj.panjiajie.cn

static int counter = 0;
来源：http://hf.szxytkj.cn

[S29] C：变参函数
来源：http://hf.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rm.asd995.cn

[S30] C：头文件保护
来源：http://vw.lnxyls.cn

#ifndef X_H
来源：http://kj.huanxung.cn

#define X_H
来源：http://uy.colortex.cn

#endif
来源：http://uw.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://xn.wgjwhj.cn

#include <iostream>
来源：http://vn.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://sd.colortex.cn

[S32] C++：字符串
来源：http://va.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://sc.szsharing.cn

[S33] C++：vector 增删
来源：http://fz.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dy.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://pt.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://th.haigaiapp.cn

[S35] C++：map
来源：http://pa.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sg.szxytkj.cn

[S36] C++：unordered_map
来源：http://xp.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kl.huixinmuqiang.cn

[S37] C++：set
来源：http://wh.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wy.huanxung.cn

[S38] C++：排序
来源：http://ae.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://or.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://vv.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pp.muxihuayi.cn

[S40] C++：查找元素
来源：http://vq.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pt.huanxung.cn

[S41] C++：类与构造函数
来源：http://ax.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kx.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://gp.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://oh.yuexingan06.cn

[S43] C++：智能指针
来源：http://yd.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://zg.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://sh.szsharing.cn

void inc(int &x) { ++x; }
来源：http://yn.wgjwhj.cn

[S45] C++：lambda
来源：http://lg.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cq.lnxyls.cn

[S46] C++：函数模板
来源：http://dq.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qc.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://mq.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ve.panjiajie.cn

[S48] C++：逐行读文件
来源：http://wo.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ji.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://qo.jctech888.com.cn

[S49] C++：写文件
来源：http://kn.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cy.muxihuayi.cn

[S50] C++：格式化数字
来源：http://ip.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kc.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://ba.colortex.cn

static_cast<double>(a) / b
来源：http://rt.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://gb.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://on.nszjky.cn

[S53] C++：移动语义
来源：http://ex.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://jf.colortex.cn

[S54] C++：异常处理
来源：http://us.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ky.asd995.cn

[S55] C++：结构化绑定
来源：http://xq.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kg.9csxet.cn

[S56] C++：optional
来源：http://sb.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bm.huixiangedu.cn

[S57] C++：编译期常量
来源：http://zj.huanxung.cn

constexpr int N = 10;
来源：http://mp.colortex.cn

[S58] C++：命名空间
来源：http://ue.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://wt.haigaiapp.cn

[S59] C++：静态断言
来源：http://ia.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bz.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://vv.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xb.jctech888.com.cn

================================================================================
来源：http://xx.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://la.jctech888.com.cn

================================================================================
来源：http://fo.nszjky.cn

[T01] Kotlin：Hello World
来源：http://je.jctech888.com.cn

println("Hello")
来源：http://xt.szxytkj.cn

[T02] Kotlin：变量
来源：http://yn.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zk.asd995.cn

[T03] Kotlin：字符串模板
来源：http://ql.shxzskj.cn

"值: $b"
来源：http://pw.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://bv.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://vm.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://dn.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cv.newstarts.cn

[T06] Kotlin：集合映射
来源：http://nj.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lg.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://xo.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rr.nszjky.cn

[T08] Kotlin：数据类
来源：http://fe.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://dd.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ez.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://ls.szsharing.cn

[T10] Kotlin：默认参数
来源：http://xf.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sb.shxzukj.cn

[T11] Kotlin：协程
来源：http://wg.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uz.nicolike.cn

[T12] Kotlin：解构声明
来源：http://nw.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://np.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://mh.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://om.newstarts.cn

[T14] Kotlin：循环
来源：http://ju.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://cf.huanxung.cn

[T15] Kotlin：接口
来源：http://ii.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://by.colortex.cn

[T16] Swift：Hello World
来源：http://qn.colortex.cn

print("Hello")
来源：http://sl.colortex.cn

[T17] Swift：变量与常量
来源：http://hl.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://uk.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://yc.521024.cn

"值: \(b)"
来源：http://ur.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://dl.9csxet.cn

if let n = opt { print(n) }
来源：http://xb.szxytkj.cn

[T20] Swift：数组操作
来源：http://vb.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ta.colortex.cn

[T21] Swift：遍历
来源：http://jx.yuexingan06.cn

for x in a { print(x) }
来源：http://ne.hnjuh.cn

[T22] Swift：字典
来源：http://as.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xz.muxihuayi.cn

[T23] Swift：函数
来源：http://bh.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://so.chemitech.net.cn

[T24] Swift：闭包
来源：http://fm.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://di.wgjwhj.cn


<!-- 参考信息 -->