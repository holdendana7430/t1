代发 wailian999

echo "${#arr[@]}"
来源：http://vl.shxzukj.cn

[R20] 关联数组（字典）
来源：http://pu.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cc.huixiangedu.cn

[R21] 字符串长度
来源：http://ou.bookmarksfly.cn

echo "${#s}"
来源：http://ry.bookmarksfly.cn

[R22] 截取子串
来源：http://dy.newstarts.cn

echo "${s:0:5}"
来源：http://cn.huixinmuqiang.cn

[R23] 字符串替换
来源：http://kp.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jk.wgjwhj.cn

[R24] 大小写转换
来源：http://ul.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gx.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://da.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://oa.bjjhwx.cn

[R26] 命令替换
来源：http://ls.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://rf.chemitech.net.cn

[R27] 算术展开
来源：http://dd.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://ox.huixinmuqiang.cn

[R28] 浮点运算
来源：http://wp.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://ta.hahajie.cn

[R29] 定义函数
来源：http://ur.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ui.521024.cn

[R30] 函数返回状态码
来源：http://hw.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://nd.nicolike.cn

[R31] 局部变量
来源：http://pm.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://fv.panjiajie.cn

[R32] 参数个数校验
来源：http://rx.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kj.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://kf.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ou.nszjky.cn

[R34] 退出时清理
来源：http://ad.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cx.colortex.cn

[R35] 后台执行并等待
来源：http://by.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ny.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://ec.wgjwhj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qd.panjiajie.cn

[R37] 把输出赋给变量
来源：http://qy.szxytkj.cn

files=$(ls -1)
来源：http://nk.huanxung.cn

[R38] 管道串联
来源：http://vu.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://cq.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://te.jctech888.com.cn

cmd > out.log 2>&1
来源：http://au.panjiajie.cn

[R40] 追加写日志
来源：http://vt.hahajie.cn

echo "log" >> out.log
来源：http://bc.colortex.cn

[R41] 丢弃输出
来源：http://dj.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://oa.lnxyls.cn

[R42] 输入重定向
来源：http://ys.chemitech.net.cn

wc -l < a.txt
来源：http://ib.huanxung.cn

[R43] 按名字查找文件
来源：http://ku.chemitech.net.cn

find . -name "*.log" -type f
来源：http://hx.hahajie.cn

[R44] 按修改时间查找
来源：http://zl.szsharing.cn

find . -mtime -7 -type f
来源：http://ak.panjiajie.cn

[R45] 批量删除
来源：http://pc.9csxet.cn

find . -name "*.tmp" -delete
来源：http://fb.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://xq.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eo.haigaiapp.cn

[R47] sed 单行替换
来源：http://ip.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gr.shxzukj.cn

[R48] awk 取指定列
来源：http://ku.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://gv.jianghongdianzi.cn

[R49] awk 带条件
来源：http://qv.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xo.bookmarksfly.cn

[R50] awk 求和
来源：http://dy.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ay.nszjky.cn

[R51] 排序去重取前几
来源：http://zz.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sp.asd995.cn

[R52] 统计行数
来源：http://pf.szsharing.cn

wc -l a.txt
来源：http://yi.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://lg.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dj.colortex.cn

[R54] 比较两个文件
来源：http://ms.jianghongdianzi.cn

diff a.txt b.txt
来源：http://ei.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://ft.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ir.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://sm.shxzskj.cn

scp file user@host:/path/
来源：http://zk.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://xk.newstarts.cn

ssh user@host 'uptime'
来源：http://dr.9csxet.cn

[R58] 下载文件
来源：http://or.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ra.9csxet.cn

[R59] 发 POST JSON
来源：http://fh.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ah.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://lj.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jw.chemitech.net.cn

[R61] 磁盘占用
来源：http://ti.panjiajie.cn

df -h;  du -sh *
来源：http://hq.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://bg.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://le.haigaiapp.cn

[R63] 内存与进程
来源：http://ol.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://ui.yuexingan06.cn

[R64] 结束进程
来源：http://es.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://oj.jctech888.com.cn

[R65] 查看端口占用
来源：http://du.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sf.lnxyls.cn

[R66] 定时任务
来源：http://wj.huanxung.cn

crontab -e;  crontab -l
来源：http://uq.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://cs.huixinmuqiang.cn

openssl rand -hex 16
来源：http://hf.haigaiapp.cn

[R68] 计算文件校验值
来源：http://kw.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iz.shxzukj.cn

[R69] 生成随机密码
来源：http://it.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://cm.shxzukj.cn

[R70] 时间戳与互转
来源：http://ot.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://ug.gzmigu.cn

[R71] 日期格式化
来源：http://ar.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ai.panjiajie.cn

[R72] 等待端口就绪
来源：http://mo.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fc.szxytkj.cn

[R73] 分割大日志
来源：http://fe.9csxet.cn

split -l 1000 big.log part_
来源：http://pu.newstarts.cn

[R74] 批量重命名
来源：http://ul.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kc.nszjky.cn

[R75] 导出环境变量
来源：http://wt.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://qf.hahajie.cn

[R76] 使用临时文件
来源：http://in.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aw.haigaiapp.cn

[R77] 读取用户输入
来源：http://wc.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://nm.haigaiapp.cn

[R78] 交互式菜单
来源：http://nz.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://if.nicolike.cn

[R79] 解析命令行选项
来源：http://hd.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ij.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://wh.hnjuh.cn

time ./run.sh
来源：http://uu.gzmigu.cn

================================================================================
来源：http://yw.shxzskj.cn

S. C / C++ 专题
来源：http://dm.panjiajie.cn

================================================================================
来源：http://ap.szsharing.cn

[S01] C：Hello World
来源：http://oj.szsharing.cn

#include <stdio.h>
来源：http://pl.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cl.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://cn.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://om.szxytkj.cn

[S03] C：读入整数
来源：http://kn.lnxyls.cn

int x; scanf("%d", &x);
来源：http://lx.jctech888.com.cn

[S04] C：字符串复制
来源：http://co.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bu.shtwfgs.cn

[S05] C：字符串长度
来源：http://uq.asd995.cn

strlen(s)
来源：http://uo.asd995.cn

[S06] C：字符串比较
来源：http://xa.haigaiapp.cn

strcmp(a, b) == 0
来源：http://ic.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://eh.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://og.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ta.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gx.colortex.cn

[S09] C：结构体定义与初始化
来源：http://hl.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eo.chemitech.net.cn

[S10] C：指针与解引用
来源：http://ck.nszjky.cn

int *p = &a;  *p = 5;
来源：http://uc.9csxet.cn

[S11] C：逐行读文件
来源：http://sl.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://ew.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mb.bjjhwx.cn

fclose(f);
来源：http://lq.wgjwhj.cn

[S12] C：写文件
来源：http://fo.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dj.muxihuayi.cn

[S13] C：宏定义
来源：http://mh.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ca.chemitech.net.cn

[S14] C：枚举
来源：http://yw.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://yp.bjjhwx.cn

[S15] C：类型转换
来源：http://tv.muxihuayi.cn

(double) a / b
来源：http://mt.521024.cn

[S16] C：位操作置位
来源：http://sz.newstarts.cn

x |= (1 << 3);
来源：http://vv.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://qn.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bk.szsharing.cn

[S18] C：命令行参数
来源：http://oc.gzmigu.cn

int main(int argc, char **argv)
来源：http://tt.9csxet.cn

[S19] C：快速排序
来源：http://xi.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cd.jctech888.com.cn

[S20] C：二分查找
来源：http://dj.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rg.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://zp.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gg.bjjhwx.cn

[S22] C：字符串转数字
来源：http://qc.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://no.shtwfgs.cn

[S23] C：随机数
来源：http://jm.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lz.panjiajie.cn

[S24] C：获取本地时间
来源：http://eq.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mo.shxzskj.cn

[S25] C：内存拷贝
来源：http://jp.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://fj.bjjhwx.cn

[S26] C：内存清零
来源：http://ve.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://ci.muxihuayi.cn

[S27] C：定义常量
来源：http://kc.wgjwhj.cn

const double PI = 3.14159;
来源：http://ce.nszjky.cn

[S28] C：静态变量
来源：http://rf.bookmarksfly.cn

static int counter = 0;
来源：http://xb.lnxyls.cn

[S29] C：变参函数
来源：http://iv.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mj.shxzskj.cn

[S30] C：头文件保护
来源：http://bt.chemitech.net.cn

#ifndef X_H
来源：http://qm.yuexingan06.cn

#define X_H
来源：http://uz.hnjuh.cn

#endif
来源：http://me.bjjhwx.cn

[S31] C++：Hello World
来源：http://uj.chemitech.net.cn

#include <iostream>
来源：http://vo.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://rn.wgjwhj.cn

[S32] C++：字符串
来源：http://ip.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://zt.bjjhwx.cn

[S33] C++：vector 增删
来源：http://xz.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cc.lnxyls.cn

[S34] C++：遍历 vector
来源：http://sq.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://qw.colortex.cn

[S35] C++：map
来源：http://dk.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lv.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://zs.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lf.shxzukj.cn

[S37] C++：set
来源：http://iq.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fb.newstarts.cn

[S38] C++：排序
来源：http://sy.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://zl.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://dd.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://su.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://sf.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ld.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://qe.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://in.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://ct.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://jy.lnxyls.cn

[S43] C++：智能指针
来源：http://cu.521024.cn

auto p = std::make_unique<int>(5);
来源：http://xc.wgjwhj.cn

[S44] C++：引用传参
来源：http://vr.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://sn.bookmarksfly.cn

[S45] C++：lambda
来源：http://gb.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eo.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://ju.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fp.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://ij.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yg.asd995.cn

[S48] C++：逐行读文件
来源：http://aa.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yf.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ub.jctech888.com.cn

[S49] C++：写文件
来源：http://uo.chemitech.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qk.wgjwhj.cn

[S50] C++：格式化数字
来源：http://oq.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xq.huanxung.cn

[S51] C++：显式类型转换
来源：http://mv.colortex.cn

static_cast<double>(a) / b
来源：http://wb.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://gk.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://uq.shxzukj.cn

[S53] C++：移动语义
来源：http://ow.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://bg.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://up.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rg.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://bp.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uh.asd995.cn

[S56] C++：optional
来源：http://ic.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ou.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://fg.shxzskj.cn

constexpr int N = 10;
来源：http://mr.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://rv.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://yp.chemitech.net.cn

[S59] C++：静态断言
来源：http://kt.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cl.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://wk.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vf.muxihuayi.cn

================================================================================
来源：http://gz.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vg.nszjky.cn

================================================================================
来源：http://ld.hahajie.cn

[T01] Kotlin：Hello World
来源：http://jg.huixiangedu.cn

println("Hello")
来源：http://wc.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://wq.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qp.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://ih.9csxet.cn

"值: $b"
来源：http://zx.hahajie.cn

[T04] Kotlin：空安全
来源：http://lk.szsharing.cn

val n: String? = null;  n?.length
来源：http://wi.asd995.cn

[T05] Kotlin：when 表达式
来源：http://bt.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cb.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://nd.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yb.asd995.cn

[T07] Kotlin：集合过滤
来源：http://wf.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wf.hnjuh.cn

[T08] Kotlin：数据类
来源：http://ha.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://yz.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://qi.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://dj.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://ry.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fr.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ap.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ax.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://qd.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://kx.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://jl.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://mb.gzmigu.cn

[T14] Kotlin：循环
来源：http://ov.colortex.cn

for (i in 1..10) println(i)
来源：http://rv.asd995.cn

[T15] Kotlin：接口
来源：http://rf.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://qj.huanxung.cn

[T16] Swift：Hello World
来源：http://wo.muxihuayi.cn

print("Hello")
来源：http://cl.521024.cn

[T17] Swift：变量与常量
来源：http://oh.hnjuh.cn

var a = 1;  let b = 2
来源：http://mz.gzmigu.cn

[T18] Swift：字符串插值
来源：http://op.521024.cn

"值: \(b)"
来源：http://ka.hnjuh.cn

[T19] Swift：可选绑定
来源：http://jl.chemitech.net.cn

if let n = opt { print(n) }
来源：http://nu.huixiangedu.cn

[T20] Swift：数组操作
来源：http://my.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oy.panjiajie.cn

[T21] Swift：遍历
来源：http://qr.bookmarksfly.cn

for x in a { print(x) }
来源：http://so.colortex.cn

[T22] Swift：字典
来源：http://fp.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tx.gzmigu.cn


<!-- 参考信息 -->