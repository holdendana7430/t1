代发 wailian999

echo "${#arr[@]}"
来源：http://vr.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://bi.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fo.chemitech.net.cn

[R21] 字符串长度
来源：http://hw.nicolike.cn

echo "${#s}"
来源：http://la.haigaiapp.cn

[R22] 截取子串
来源：http://ls.bjjhwx.cn

echo "${s:0:5}"
来源：http://zu.newstarts.cn

[R23] 字符串替换
来源：http://lr.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yx.muxihuayi.cn

[R24] 大小写转换
来源：http://hy.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ky.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://bs.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ft.nicolike.cn

[R26] 命令替换
来源：http://md.asd995.cn

now=$(date +%F); echo "$now"
来源：http://yi.nszjky.cn

[R27] 算术展开
来源：http://ql.asd995.cn

echo $((1 + 2 * 3))
来源：http://vi.nszjky.cn

[R28] 浮点运算
来源：http://mw.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://ep.bookmarksfly.cn

[R29] 定义函数
来源：http://my.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ds.asd995.cn

[R30] 函数返回状态码
来源：http://tr.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://ty.chemitech.net.cn

[R31] 局部变量
来源：http://cb.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://ah.yuexingan06.cn

[R32] 参数个数校验
来源：http://ov.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uy.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://lj.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zv.9csxet.cn

[R34] 退出时清理
来源：http://hm.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fo.hahajie.cn

[R35] 后台执行并等待
来源：http://nb.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://na.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://fc.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cf.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://at.shtwfgs.cn

files=$(ls -1)
来源：http://tr.haigaiapp.cn

[R38] 管道串联
来源：http://lv.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://pa.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://va.muxihuayi.cn

cmd > out.log 2>&1
来源：http://rj.nicolike.cn

[R40] 追加写日志
来源：http://pz.szsharing.cn

echo "log" >> out.log
来源：http://sx.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ig.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://fy.wgjwhj.cn

[R42] 输入重定向
来源：http://nf.colortex.cn

wc -l < a.txt
来源：http://wc.chemitech.net.cn

[R43] 按名字查找文件
来源：http://ye.lnxyls.cn

find . -name "*.log" -type f
来源：http://pj.gzmigu.cn

[R44] 按修改时间查找
来源：http://zi.gzmigu.cn

find . -mtime -7 -type f
来源：http://za.bookmarksfly.cn

[R45] 批量删除
来源：http://zr.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://am.szsharing.cn

[R46] 递归替换文件内容
来源：http://fa.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yn.hahajie.cn

[R47] sed 单行替换
来源：http://vo.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hc.shtwfgs.cn

[R48] awk 取指定列
来源：http://ub.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://wn.yuntaijiaju.cn

[R49] awk 带条件
来源：http://xp.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xp.bjjhwx.cn

[R50] awk 求和
来源：http://mr.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zq.szxytkj.cn

[R51] 排序去重取前几
来源：http://kk.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kd.hnjuh.cn

[R52] 统计行数
来源：http://fp.bookmarksfly.cn

wc -l a.txt
来源：http://ig.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://tg.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zi.asd995.cn

[R54] 比较两个文件
来源：http://yo.jianghongdianzi.cn

diff a.txt b.txt
来源：http://wg.bjjhwx.cn

[R55] 压缩与解压
来源：http://jw.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tk.nicolike.cn

[R56] 远程拷贝
来源：http://mw.muxihuayi.cn

scp file user@host:/path/
来源：http://rs.szsharing.cn

[R57] 远程执行命令
来源：http://nc.lnxyls.cn

ssh user@host 'uptime'
来源：http://dt.jctech888.com.cn

[R58] 下载文件
来源：http://mz.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fz.chemitech.net.cn

[R59] 发 POST JSON
来源：http://up.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ua.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://zn.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nd.jctech888.com.cn

[R61] 磁盘占用
来源：http://sw.colortex.cn

df -h;  du -sh *
来源：http://yu.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://qp.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://du.colortex.cn

[R63] 内存与进程
来源：http://wj.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://oa.chemitech.net.cn

[R64] 结束进程
来源：http://qd.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://vn.gzmigu.cn

[R65] 查看端口占用
来源：http://dt.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cj.haigaiapp.cn

[R66] 定时任务
来源：http://jl.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://ub.nicolike.cn

[R67] 生成随机十六进制串
来源：http://ll.hnjuh.cn

openssl rand -hex 16
来源：http://im.gzmigu.cn

[R68] 计算文件校验值
来源：http://br.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pb.shxzukj.cn

[R69] 生成随机密码
来源：http://nm.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ar.hahajie.cn

[R70] 时间戳与互转
来源：http://ra.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://kg.jctech888.com.cn

[R71] 日期格式化
来源：http://jl.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fu.panjiajie.cn

[R72] 等待端口就绪
来源：http://zc.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://se.shxzukj.cn

[R73] 分割大日志
来源：http://ap.nszjky.cn

split -l 1000 big.log part_
来源：http://dt.shxzukj.cn

[R74] 批量重命名
来源：http://gm.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://td.521024.cn

[R75] 导出环境变量
来源：http://oj.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ah.hahajie.cn

[R76] 使用临时文件
来源：http://hk.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jz.asd995.cn

[R77] 读取用户输入
来源：http://vg.shtwfgs.cn

read -rp "请输入: " ans
来源：http://mk.gzmigu.cn

[R78] 交互式菜单
来源：http://wf.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xh.shxzskj.cn

[R79] 解析命令行选项
来源：http://pi.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://at.asd995.cn

[R80] 查看脚本执行耗时
来源：http://yw.hahajie.cn

time ./run.sh
来源：http://nr.bjjhwx.cn

================================================================================
来源：http://uq.jctech888.com.cn

S. C / C++ 专题
来源：http://vk.muxihuayi.cn

================================================================================
来源：http://yz.shxzskj.cn

[S01] C：Hello World
来源：http://fi.hnjuh.cn

#include <stdio.h>
来源：http://le.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yn.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://gf.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://wl.9csxet.cn

[S03] C：读入整数
来源：http://ia.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://kg.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://cx.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lj.colortex.cn

[S05] C：字符串长度
来源：http://mk.haigaiapp.cn

strlen(s)
来源：http://ha.shxzukj.cn

[S06] C：字符串比较
来源：http://ct.521024.cn

strcmp(a, b) == 0
来源：http://sx.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://bj.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tf.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://mh.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bt.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://ju.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fs.hnjuh.cn

[S10] C：指针与解引用
来源：http://uw.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://yh.haigaiapp.cn

[S11] C：逐行读文件
来源：http://bi.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://lr.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gg.jctech888.com.cn

fclose(f);
来源：http://gc.panjiajie.cn

[S12] C：写文件
来源：http://om.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xd.hnjuh.cn

[S13] C：宏定义
来源：http://md.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qy.gzmigu.cn

[S14] C：枚举
来源：http://gt.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://hh.muxihuayi.cn

[S15] C：类型转换
来源：http://cz.521024.cn

(double) a / b
来源：http://gm.9csxet.cn

[S16] C：位操作置位
来源：http://di.yuexingan06.cn

x |= (1 << 3);
来源：http://zo.newstarts.cn

[S17] C：安全拼接字符串
来源：http://gt.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vg.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://ac.asd995.cn

int main(int argc, char **argv)
来源：http://lc.colortex.cn

[S19] C：快速排序
来源：http://zc.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eo.9csxet.cn

[S20] C：二分查找
来源：http://aw.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xk.lnxyls.cn

[S21] C：字符类别判断
来源：http://jz.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ff.chemitech.net.cn

[S22] C：字符串转数字
来源：http://cn.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pu.shtwfgs.cn

[S23] C：随机数
来源：http://al.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cj.hahajie.cn

[S24] C：获取本地时间
来源：http://cu.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qm.szsharing.cn

[S25] C：内存拷贝
来源：http://mj.shxzukj.cn

memcpy(dst, src, n);
来源：http://vx.newstarts.cn

[S26] C：内存清零
来源：http://do.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://qn.colortex.cn

[S27] C：定义常量
来源：http://cf.haigaiapp.cn

const double PI = 3.14159;
来源：http://fy.jctech888.com.cn

[S28] C：静态变量
来源：http://jd.hahajie.cn

static int counter = 0;
来源：http://if.haigaiapp.cn

[S29] C：变参函数
来源：http://os.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uz.bjjhwx.cn

[S30] C：头文件保护
来源：http://mu.shxzskj.cn

#ifndef X_H
来源：http://qr.shtwfgs.cn

#define X_H
来源：http://tt.521024.cn

#endif
来源：http://jp.newstarts.cn

[S31] C++：Hello World
来源：http://zh.haigaiapp.cn

#include <iostream>
来源：http://yn.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://hy.521024.cn

[S32] C++：字符串
来源：http://gp.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://al.newstarts.cn

[S33] C++：vector 增删
来源：http://op.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ai.hahajie.cn

[S34] C++：遍历 vector
来源：http://ei.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://ms.shxzskj.cn

[S35] C++：map
来源：http://on.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yq.nicolike.cn

[S36] C++：unordered_map
来源：http://bf.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ai.jctech888.com.cn

[S37] C++：set
来源：http://hj.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hv.hnjuh.cn

[S38] C++：排序
来源：http://ne.521024.cn

std::sort(v.begin(), v.end());
来源：http://ic.asd995.cn

[S39] C++：自定义比较器排序
来源：http://qy.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pv.newstarts.cn

[S40] C++：查找元素
来源：http://um.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ud.nszjky.cn

[S41] C++：类与构造函数
来源：http://fa.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mu.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://qa.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://bk.chemitech.net.cn

[S43] C++：智能指针
来源：http://so.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://zd.huixiangedu.cn

[S44] C++：引用传参
来源：http://rh.521024.cn

void inc(int &x) { ++x; }
来源：http://ij.haigaiapp.cn

[S45] C++：lambda
来源：http://dr.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ml.colortex.cn

[S46] C++：函数模板
来源：http://bj.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ft.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://ux.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qr.newstarts.cn

[S48] C++：逐行读文件
来源：http://fm.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wm.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://zc.gzmigu.cn

[S49] C++：写文件
来源：http://eo.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wj.szxytkj.cn

[S50] C++：格式化数字
来源：http://ib.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mw.newstarts.cn

[S51] C++：显式类型转换
来源：http://cp.haigaiapp.cn

static_cast<double>(a) / b
来源：http://up.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://pm.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://nz.huixiangedu.cn

[S53] C++：移动语义
来源：http://jv.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://tl.jctech888.com.cn

[S54] C++：异常处理
来源：http://mx.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cj.shxzukj.cn

[S55] C++：结构化绑定
来源：http://ck.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rc.lnxyls.cn

[S56] C++：optional
来源：http://kj.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://or.asd995.cn

[S57] C++：编译期常量
来源：http://zo.bjjhwx.cn

constexpr int N = 10;
来源：http://ts.521024.cn

[S58] C++：命名空间
来源：http://cj.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://uy.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://pg.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ip.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://pe.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jk.lnxyls.cn

================================================================================
来源：http://lt.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qd.yuexingan06.cn

================================================================================
来源：http://ma.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://sd.bjjhwx.cn

println("Hello")
来源：http://zb.panjiajie.cn

[T02] Kotlin：变量
来源：http://bm.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sc.521024.cn

[T03] Kotlin：字符串模板
来源：http://ve.muxihuayi.cn

"值: $b"
来源：http://tb.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://fc.szsharing.cn

val n: String? = null;  n?.length
来源：http://ue.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://bs.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qm.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://rd.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ym.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://hl.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zo.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://dn.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://di.colortex.cn

[T09] Kotlin：扩展函数
来源：http://hb.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://ie.huanxung.cn

[T10] Kotlin：默认参数
来源：http://dg.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ue.colortex.cn

[T11] Kotlin：协程
来源：http://qc.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fb.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://xn.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://rx.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://fk.szsharing.cn

val m = mapOf("a" to 1)
来源：http://rb.asd995.cn

[T14] Kotlin：循环
来源：http://nq.colortex.cn

for (i in 1..10) println(i)
来源：http://bj.szxytkj.cn

[T15] Kotlin：接口
来源：http://pq.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://hs.chemitech.net.cn

[T16] Swift：Hello World
来源：http://jq.szxytkj.cn

print("Hello")
来源：http://ek.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://ju.jctech888.com.cn

var a = 1;  let b = 2
来源：http://rr.szsharing.cn

[T18] Swift：字符串插值
来源：http://kl.newstarts.cn

"值: \(b)"
来源：http://ha.521024.cn

[T19] Swift：可选绑定
来源：http://oy.asd995.cn

if let n = opt { print(n) }
来源：http://oa.hnjuh.cn

[T20] Swift：数组操作
来源：http://uz.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vo.colortex.cn

[T21] Swift：遍历
来源：http://li.521024.cn

for x in a { print(x) }
来源：http://es.nicolike.cn

[T22] Swift：字典
来源：http://cn.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ox.jctech888.com.cn


<!-- 参考信息 -->