代发 wailian999

echo "${#s}"
来源：http://zq.nszjky.cn

[R22] 截取子串
来源：http://pi.yuexingan06.cn

echo "${s:0:5}"
来源：http://aj.yuexingan06.cn

[R23] 字符串替换
来源：http://ru.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zt.shtwfgs.cn

[R24] 大小写转换
来源：http://ba.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gt.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://wk.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://my.colortex.cn

[R26] 命令替换
来源：http://nj.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://eo.jianghongdianzi.cn

[R27] 算术展开
来源：http://kl.gzmigu.cn

echo $((1 + 2 * 3))
来源：http://bs.hahajie.cn

[R28] 浮点运算
来源：http://ru.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ky.panjiajie.cn

[R29] 定义函数
来源：http://kh.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iv.asd995.cn

[R30] 函数返回状态码
来源：http://lx.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://xt.nszjky.cn

[R31] 局部变量
来源：http://qn.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://io.jctech888.com.cn

[R32] 参数个数校验
来源：http://yg.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sc.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://hm.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ua.huanxung.cn

[R34] 退出时清理
来源：http://gg.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mh.jctech888.com.cn

[R35] 后台执行并等待
来源：http://ch.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wb.colortex.cn

[R36] 并发执行多个任务
来源：http://pc.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eh.lnxyls.cn

[R37] 把输出赋给变量
来源：http://cz.jianghongdianzi.cn

files=$(ls -1)
来源：http://ll.hnjuh.cn

[R38] 管道串联
来源：http://pi.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://bj.yuexingan06.cn

[R39] 重定向标准输出与错误
来源：http://vs.lnxyls.cn

cmd > out.log 2>&1
来源：http://hi.shtwfgs.cn

[R40] 追加写日志
来源：http://nx.colortex.cn

echo "log" >> out.log
来源：http://fj.newstarts.cn

[R41] 丢弃输出
来源：http://mp.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://lx.hnjuh.cn

[R42] 输入重定向
来源：http://cg.521024.cn

wc -l < a.txt
来源：http://xr.chemitech.net.cn

[R43] 按名字查找文件
来源：http://tz.bookmarksfly.cn

find . -name "*.log" -type f
来源：http://xx.huanxung.cn

[R44] 按修改时间查找
来源：http://hp.haigaiapp.cn

find . -mtime -7 -type f
来源：http://ob.hnjuh.cn

[R45] 批量删除
来源：http://ma.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://sg.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://mi.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dr.newstarts.cn

[R47] sed 单行替换
来源：http://ha.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cu.colortex.cn

[R48] awk 取指定列
来源：http://vh.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://to.hnjuh.cn

[R49] awk 带条件
来源：http://yr.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zb.huixiangedu.cn

[R50] awk 求和
来源：http://tq.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pd.panjiajie.cn

[R51] 排序去重取前几
来源：http://xl.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ak.szxytkj.cn

[R52] 统计行数
来源：http://cu.shtwfgs.cn

wc -l a.txt
来源：http://na.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://hm.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ut.9csxet.cn

[R54] 比较两个文件
来源：http://sp.9csxet.cn

diff a.txt b.txt
来源：http://hc.jctech888.com.cn

[R55] 压缩与解压
来源：http://qt.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tr.hahajie.cn

[R56] 远程拷贝
来源：http://oc.521024.cn

scp file user@host:/path/
来源：http://iv.wgjwhj.cn

[R57] 远程执行命令
来源：http://wm.newstarts.cn

ssh user@host 'uptime'
来源：http://ac.hnjuh.cn

[R58] 下载文件
来源：http://va.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bm.wgjwhj.cn

[R59] 发 POST JSON
来源：http://tu.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oi.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://qy.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mw.wgjwhj.cn

[R61] 磁盘占用
来源：http://ws.huixinmuqiang.cn

df -h;  du -sh *
来源：http://xz.shxzukj.cn

[R62] 找最占空间的文件
来源：http://pb.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://fk.hnjuh.cn

[R63] 内存与进程
来源：http://gw.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://nz.bjjhwx.cn

[R64] 结束进程
来源：http://fo.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://mz.szxytkj.cn

[R65] 查看端口占用
来源：http://hs.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://io.haigaiapp.cn

[R66] 定时任务
来源：http://iu.haigaiapp.cn

crontab -e;  crontab -l
来源：http://xw.nszjky.cn

[R67] 生成随机十六进制串
来源：http://qs.bjjhwx.cn

openssl rand -hex 16
来源：http://wi.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://lu.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ee.huanxung.cn

[R69] 生成随机密码
来源：http://bj.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://zw.shtwfgs.cn

[R70] 时间戳与互转
来源：http://cx.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://je.panjiajie.cn

[R71] 日期格式化
来源：http://uf.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kw.colortex.cn

[R72] 等待端口就绪
来源：http://ad.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ho.chemitech.net.cn

[R73] 分割大日志
来源：http://fm.panjiajie.cn

split -l 1000 big.log part_
来源：http://jf.jctech888.com.cn

[R74] 批量重命名
来源：http://mj.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oc.lnxyls.cn

[R75] 导出环境变量
来源：http://od.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://oa.chemitech.net.cn

[R76] 使用临时文件
来源：http://jp.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ax.huixiangedu.cn

[R77] 读取用户输入
来源：http://zp.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://cn.asd995.cn

[R78] 交互式菜单
来源：http://fe.panjiajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vy.szsharing.cn

[R79] 解析命令行选项
来源：http://rc.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mw.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://ok.hahajie.cn

time ./run.sh
来源：http://vd.yuntaijiaju.cn

================================================================================
来源：http://fe.lnxyls.cn

S. C / C++ 专题
来源：http://uv.huanxung.cn

================================================================================
来源：http://vj.huixiangedu.cn

[S01] C：Hello World
来源：http://ow.hnjuh.cn

#include <stdio.h>
来源：http://rq.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qc.colortex.cn

[S02] C：变量与格式化输出
来源：http://hf.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://dj.huanxung.cn

[S03] C：读入整数
来源：http://ss.hahajie.cn

int x; scanf("%d", &x);
来源：http://xn.newstarts.cn

[S04] C：字符串复制
来源：http://yr.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://es.hahajie.cn

[S05] C：字符串长度
来源：http://yg.gzmigu.cn

strlen(s)
来源：http://fb.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://dy.haigaiapp.cn

strcmp(a, b) == 0
来源：http://ui.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://ow.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://br.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://hc.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://va.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://nu.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lp.yuexingan06.cn

[S10] C：指针与解引用
来源：http://py.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://us.haigaiapp.cn

[S11] C：逐行读文件
来源：http://ug.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://er.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gc.lnxyls.cn

fclose(f);
来源：http://rr.muxihuayi.cn

[S12] C：写文件
来源：http://lz.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bu.huixinmuqiang.cn

[S13] C：宏定义
来源：http://wt.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dl.lnxyls.cn

[S14] C：枚举
来源：http://ep.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://je.wgjwhj.cn

[S15] C：类型转换
来源：http://mm.huixinmuqiang.cn

(double) a / b
来源：http://an.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://hf.bjjhwx.cn

x |= (1 << 3);
来源：http://eo.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://jv.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bt.9csxet.cn

[S18] C：命令行参数
来源：http://he.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://xl.huanxung.cn

[S19] C：快速排序
来源：http://am.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://va.nicolike.cn

[S20] C：二分查找
来源：http://vh.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yt.hahajie.cn

[S21] C：字符类别判断
来源：http://fl.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zv.szsharing.cn

[S22] C：字符串转数字
来源：http://sa.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fr.shtwfgs.cn

[S23] C：随机数
来源：http://zg.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pw.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ki.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ho.nicolike.cn

[S25] C：内存拷贝
来源：http://bf.yuexingan06.cn

memcpy(dst, src, n);
来源：http://vd.gzmigu.cn

[S26] C：内存清零
来源：http://me.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://di.hahajie.cn

[S27] C：定义常量
来源：http://us.newstarts.cn

const double PI = 3.14159;
来源：http://jl.9csxet.cn

[S28] C：静态变量
来源：http://lg.szxytkj.cn

static int counter = 0;
来源：http://dh.521024.cn

[S29] C：变参函数
来源：http://gt.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xa.szxytkj.cn

[S30] C：头文件保护
来源：http://fn.yuntaijiaju.cn

#ifndef X_H
来源：http://ki.9csxet.cn

#define X_H
来源：http://em.huixinmuqiang.cn

#endif
来源：http://qd.szsharing.cn

[S31] C++：Hello World
来源：http://da.bookmarksfly.cn

#include <iostream>
来源：http://yq.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://er.chemitech.net.cn

[S32] C++：字符串
来源：http://qn.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://bt.shxzukj.cn

[S33] C++：vector 增删
来源：http://jh.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bl.hahajie.cn

[S34] C++：遍历 vector
来源：http://ai.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ro.9csxet.cn

[S35] C++：map
来源：http://ec.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ap.9csxet.cn

[S36] C++：unordered_map
来源：http://cv.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vi.jctech888.com.cn

[S37] C++：set
来源：http://fx.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ss.asd995.cn

[S38] C++：排序
来源：http://hw.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://ke.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://mf.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xh.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://vf.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ic.colortex.cn

[S41] C++：类与构造函数
来源：http://iy.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hr.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://qj.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://qu.yuexingan06.cn

[S43] C++：智能指针
来源：http://ep.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://tc.colortex.cn

[S44] C++：引用传参
来源：http://gi.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://hb.shxzukj.cn

[S45] C++：lambda
来源：http://cw.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ui.colortex.cn

[S46] C++：函数模板
来源：http://gy.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ht.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://gg.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ub.shxzukj.cn

[S48] C++：逐行读文件
来源：http://op.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mq.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://bf.lnxyls.cn

[S49] C++：写文件
来源：http://wf.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pk.521024.cn

[S50] C++：格式化数字
来源：http://bv.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dd.9csxet.cn

[S51] C++：显式类型转换
来源：http://zt.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://of.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://so.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://cr.huanxung.cn

[S53] C++：移动语义
来源：http://mf.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://av.wgjwhj.cn

[S54] C++：异常处理
来源：http://cj.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://et.hahajie.cn

[S55] C++：结构化绑定
来源：http://kl.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kt.colortex.cn

[S56] C++：optional
来源：http://hf.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sj.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://ey.colortex.cn

constexpr int N = 10;
来源：http://ot.gzmigu.cn

[S58] C++：命名空间
来源：http://if.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://oi.wgjwhj.cn

[S59] C++：静态断言
来源：http://hl.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nf.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://jj.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dw.nicolike.cn

================================================================================
来源：http://xy.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zn.shxzskj.cn

================================================================================
来源：http://xz.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://iz.jianghongdianzi.cn

println("Hello")
来源：http://gx.haigaiapp.cn

[T02] Kotlin：变量
来源：http://qe.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ge.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://sx.521024.cn

"值: $b"
来源：http://vz.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://sv.lnxyls.cn

val n: String? = null;  n?.length
来源：http://qw.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://lq.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://au.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://yu.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rn.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://xi.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rc.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://bm.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://kf.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://az.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://fa.521024.cn

[T10] Kotlin：默认参数
来源：http://al.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ql.shxzukj.cn

[T11] Kotlin：协程
来源：http://gs.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vm.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://gq.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://yd.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://mh.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://ky.szxytkj.cn

[T14] Kotlin：循环
来源：http://yr.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://ed.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://qq.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://mz.lnxyls.cn

[T16] Swift：Hello World
来源：http://wk.nicolike.cn

print("Hello")
来源：http://ko.lnxyls.cn

[T17] Swift：变量与常量
来源：http://yo.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ny.9csxet.cn

[T18] Swift：字符串插值
来源：http://ws.huanxung.cn

"值: \(b)"
来源：http://ak.newstarts.cn

[T19] Swift：可选绑定
来源：http://iq.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://xs.gzmigu.cn

[T20] Swift：数组操作
来源：http://vk.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rd.panjiajie.cn

[T21] Swift：遍历
来源：http://nx.lnxyls.cn

for x in a { print(x) }
来源：http://vg.bookmarksfly.cn

[T22] Swift：字典
来源：http://lq.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ly.9csxet.cn

[T23] Swift：函数
来源：http://xz.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oy.jctech888.com.cn

[T24] Swift：闭包
来源：http://zb.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ru.9csxet.cn


<!-- 参考信息 -->