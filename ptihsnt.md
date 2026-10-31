代发 wailian999

echo "${#s}"
来源：http://qr.szsharing.cn

[R22] 截取子串
来源：http://dp.szxytkj.cn

echo "${s:0:5}"
来源：http://pm.hnjuh.cn

[R23] 字符串替换
来源：http://gf.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jt.szsharing.cn

[R24] 大小写转换
来源：http://sj.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gu.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://wg.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ur.bjjhwx.cn

[R26] 命令替换
来源：http://sk.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://dx.lnxyls.cn

[R27] 算术展开
来源：http://yi.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://gh.huanxung.cn

[R28] 浮点运算
来源：http://no.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://yk.jianghongdianzi.cn

[R29] 定义函数
来源：http://ho.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nc.hahajie.cn

[R30] 函数返回状态码
来源：http://op.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://pq.hahajie.cn

[R31] 局部变量
来源：http://hk.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://hh.newstarts.cn

[R32] 参数个数校验
来源：http://ea.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ac.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://ru.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wx.nszjky.cn

[R34] 退出时清理
来源：http://oq.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qw.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://ix.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oh.panjiajie.cn

[R36] 并发执行多个任务
来源：http://bw.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lj.panjiajie.cn

[R37] 把输出赋给变量
来源：http://py.nszjky.cn

files=$(ls -1)
来源：http://zu.huanxung.cn

[R38] 管道串联
来源：http://cv.colortex.cn

cat a.txt | grep -i error | wc -l
来源：http://sj.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://af.jctech888.com.cn

cmd > out.log 2>&1
来源：http://tm.huixiangedu.cn

[R40] 追加写日志
来源：http://bb.nszjky.cn

echo "log" >> out.log
来源：http://kn.shtwfgs.cn

[R41] 丢弃输出
来源：http://dv.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://si.wgjwhj.cn

[R42] 输入重定向
来源：http://li.huixinmuqiang.cn

wc -l < a.txt
来源：http://vb.panjiajie.cn

[R43] 按名字查找文件
来源：http://qj.hnjuh.cn

find . -name "*.log" -type f
来源：http://ei.huixiangedu.cn

[R44] 按修改时间查找
来源：http://ih.asd995.cn

find . -mtime -7 -type f
来源：http://ll.hnjuh.cn

[R45] 批量删除
来源：http://cq.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://tx.asd995.cn

[R46] 递归替换文件内容
来源：http://cw.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hh.muxihuayi.cn

[R47] sed 单行替换
来源：http://mz.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ny.colortex.cn

[R48] awk 取指定列
来源：http://vf.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://pb.shxzskj.cn

[R49] awk 带条件
来源：http://qg.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kt.muxihuayi.cn

[R50] awk 求和
来源：http://ho.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ni.szxytkj.cn

[R51] 排序去重取前几
来源：http://zz.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hc.hahajie.cn

[R52] 统计行数
来源：http://qi.szxytkj.cn

wc -l a.txt
来源：http://nn.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://zo.newstarts.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yj.bjjhwx.cn

[R54] 比较两个文件
来源：http://iy.521024.cn

diff a.txt b.txt
来源：http://iu.nszjky.cn

[R55] 压缩与解压
来源：http://at.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mp.bookmarksfly.cn

[R56] 远程拷贝
来源：http://jj.panjiajie.cn

scp file user@host:/path/
来源：http://mm.hahajie.cn

[R57] 远程执行命令
来源：http://ab.asd995.cn

ssh user@host 'uptime'
来源：http://gg.hahajie.cn

[R58] 下载文件
来源：http://wf.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cu.shtwfgs.cn

[R59] 发 POST JSON
来源：http://xt.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bl.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://qi.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zs.colortex.cn

[R61] 磁盘占用
来源：http://sb.chemitech.net.cn

df -h;  du -sh *
来源：http://zc.nszjky.cn

[R62] 找最占空间的文件
来源：http://lr.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://ob.yuntaijiaju.cn

[R63] 内存与进程
来源：http://ek.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://dk.nszjky.cn

[R64] 结束进程
来源：http://cp.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://ba.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://tp.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pw.szxytkj.cn

[R66] 定时任务
来源：http://ma.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://gz.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://ap.lnxyls.cn

openssl rand -hex 16
来源：http://ea.haigaiapp.cn

[R68] 计算文件校验值
来源：http://db.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tc.wgjwhj.cn

[R69] 生成随机密码
来源：http://cw.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://ja.nicolike.cn

[R70] 时间戳与互转
来源：http://nq.newstarts.cn

date +%s;  date -d @1700000000
来源：http://gz.chemitech.net.cn

[R71] 日期格式化
来源：http://ag.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zw.wgjwhj.cn

[R72] 等待端口就绪
来源：http://uy.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://du.shxzukj.cn

[R73] 分割大日志
来源：http://ok.shxzukj.cn

split -l 1000 big.log part_
来源：http://pd.haigaiapp.cn

[R74] 批量重命名
来源：http://gc.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cg.colortex.cn

[R75] 导出环境变量
来源：http://bf.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://fp.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://ab.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://el.bookmarksfly.cn

[R77] 读取用户输入
来源：http://lz.lnxyls.cn

read -rp "请输入: " ans
来源：http://hb.colortex.cn

[R78] 交互式菜单
来源：http://nz.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rn.colortex.cn

[R79] 解析命令行选项
来源：http://uw.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sd.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://pi.huanxung.cn

time ./run.sh
来源：http://he.huanxung.cn

================================================================================
来源：http://gw.newstarts.cn

S. C / C++ 专题
来源：http://ft.nicolike.cn

================================================================================
来源：http://zj.yuexingan06.cn

[S01] C：Hello World
来源：http://sb.nicolike.cn

#include <stdio.h>
来源：http://jo.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ew.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://vx.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://tn.hahajie.cn

[S03] C：读入整数
来源：http://gm.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://dm.haigaiapp.cn

[S04] C：字符串复制
来源：http://lq.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://le.shtwfgs.cn

[S05] C：字符串长度
来源：http://xm.nicolike.cn

strlen(s)
来源：http://rj.szxytkj.cn

[S06] C：字符串比较
来源：http://sp.newstarts.cn

strcmp(a, b) == 0
来源：http://bo.panjiajie.cn

[S07] C：数组遍历求和
来源：http://uf.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zl.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://il.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ko.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://fw.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://to.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://ov.521024.cn

int *p = &a;  *p = 5;
来源：http://ho.huixiangedu.cn

[S11] C：逐行读文件
来源：http://tq.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://wo.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hi.bookmarksfly.cn

fclose(f);
来源：http://vh.asd995.cn

[S12] C：写文件
来源：http://yp.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ve.gzmigu.cn

[S13] C：宏定义
来源：http://gu.newstarts.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dd.huanxung.cn

[S14] C：枚举
来源：http://yt.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://tc.hnjuh.cn

[S15] C：类型转换
来源：http://wm.jianghongdianzi.cn

(double) a / b
来源：http://uj.hnjuh.cn

[S16] C：位操作置位
来源：http://ix.haigaiapp.cn

x |= (1 << 3);
来源：http://ga.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://cp.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://im.521024.cn

[S18] C：命令行参数
来源：http://jv.asd995.cn

int main(int argc, char **argv)
来源：http://qi.szsharing.cn

[S19] C：快速排序
来源：http://xz.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://le.jianghongdianzi.cn

[S20] C：二分查找
来源：http://ye.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wo.lnxyls.cn

[S21] C：字符类别判断
来源：http://fk.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tl.gzmigu.cn

[S22] C：字符串转数字
来源：http://kc.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qh.newstarts.cn

[S23] C：随机数
来源：http://mk.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wt.szsharing.cn

[S24] C：获取本地时间
来源：http://dh.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uu.wgjwhj.cn

[S25] C：内存拷贝
来源：http://xt.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://qi.bjjhwx.cn

[S26] C：内存清零
来源：http://bv.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://rf.huixinmuqiang.cn

[S27] C：定义常量
来源：http://cs.521024.cn

const double PI = 3.14159;
来源：http://al.szxytkj.cn

[S28] C：静态变量
来源：http://et.panjiajie.cn

static int counter = 0;
来源：http://yl.yuntaijiaju.cn

[S29] C：变参函数
来源：http://dl.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zr.bjjhwx.cn

[S30] C：头文件保护
来源：http://ub.lnxyls.cn

#ifndef X_H
来源：http://qd.szxytkj.cn

#define X_H
来源：http://rj.jctech888.com.cn

#endif
来源：http://nc.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://br.panjiajie.cn

#include <iostream>
来源：http://mc.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://as.jianghongdianzi.cn

[S32] C++：字符串
来源：http://ki.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://zh.nszjky.cn

[S33] C++：vector 增删
来源：http://ol.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kj.asd995.cn

[S34] C++：遍历 vector
来源：http://hn.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ll.huixiangedu.cn

[S35] C++：map
来源：http://rj.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://am.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://xm.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jl.asd995.cn

[S37] C++：set
来源：http://qw.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jy.huixinmuqiang.cn

[S38] C++：排序
来源：http://hz.colortex.cn

std::sort(v.begin(), v.end());
来源：http://un.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://gr.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sf.panjiajie.cn

[S40] C++：查找元素
来源：http://yw.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vs.colortex.cn

[S41] C++：类与构造函数
来源：http://cg.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sc.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://rh.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://fl.hnjuh.cn

[S43] C++：智能指针
来源：http://pa.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://xj.huixiangedu.cn

[S44] C++：引用传参
来源：http://ai.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://bi.szxytkj.cn

[S45] C++：lambda
来源：http://nu.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mr.521024.cn

[S46] C++：函数模板
来源：http://lm.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://up.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://ms.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wm.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://nk.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ad.nszjky.cn

while (std::getline(in, line)) { }
来源：http://zr.colortex.cn

[S49] C++：写文件
来源：http://ys.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uw.newstarts.cn

[S50] C++：格式化数字
来源：http://ti.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oe.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://wl.nicolike.cn

static_cast<double>(a) / b
来源：http://wq.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://mf.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://rj.asd995.cn

[S53] C++：移动语义
来源：http://ga.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://bg.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://ic.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lw.asd995.cn

[S55] C++：结构化绑定
来源：http://fn.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zo.yuntaijiaju.cn

[S56] C++：optional
来源：http://go.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ne.jctech888.com.cn

[S57] C++：编译期常量
来源：http://eq.hahajie.cn

constexpr int N = 10;
来源：http://mg.muxihuayi.cn

[S58] C++：命名空间
来源：http://oq.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://yz.shtwfgs.cn

[S59] C++：静态断言
来源：http://sh.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kz.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://wx.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sh.shxzskj.cn

================================================================================
来源：http://pt.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jv.chemitech.net.cn

================================================================================
来源：http://lp.asd995.cn

[T01] Kotlin：Hello World
来源：http://bu.hahajie.cn

println("Hello")
来源：http://dp.yuexingan06.cn

[T02] Kotlin：变量
来源：http://yl.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bq.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://fk.nszjky.cn

"值: $b"
来源：http://kv.9csxet.cn

[T04] Kotlin：空安全
来源：http://eh.nicolike.cn

val n: String? = null;  n?.length
来源：http://il.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://vu.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ks.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://si.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mm.521024.cn

[T07] Kotlin：集合过滤
来源：http://oi.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ge.shxzukj.cn

[T08] Kotlin：数据类
来源：http://bn.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://kv.colortex.cn

[T09] Kotlin：扩展函数
来源：http://hc.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://ky.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://ie.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vd.haigaiapp.cn

[T11] Kotlin：协程
来源：http://jv.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qa.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://vb.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://td.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://sn.huanxung.cn

val m = mapOf("a" to 1)
来源：http://sy.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://bq.shxzskj.cn

for (i in 1..10) println(i)
来源：http://wz.panjiajie.cn

[T15] Kotlin：接口
来源：http://hk.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://br.asd995.cn

[T16] Swift：Hello World
来源：http://ob.szxytkj.cn

print("Hello")
来源：http://xr.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://ym.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://tm.nicolike.cn

[T18] Swift：字符串插值
来源：http://mi.9csxet.cn

"值: \(b)"
来源：http://or.hahajie.cn

[T19] Swift：可选绑定
来源：http://ln.huanxung.cn

if let n = opt { print(n) }
来源：http://vh.chemitech.net.cn

[T20] Swift：数组操作
来源：http://gb.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://na.huixiangedu.cn

[T21] Swift：遍历
来源：http://jn.shxzskj.cn

for x in a { print(x) }
来源：http://fo.shtwfgs.cn

[T22] Swift：字典
来源：http://sy.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wa.jctech888.com.cn

[T23] Swift：函数
来源：http://qx.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ux.shtwfgs.cn

[T24] Swift：闭包
来源：http://wy.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zy.bjjhwx.cn


<!-- 参考信息 -->