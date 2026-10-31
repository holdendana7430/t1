代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://ns.bjjhwx.cn

[R18] 遍历数组
来源：http://oj.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sz.panjiajie.cn

[R19] 数组长度
来源：http://sa.nszjky.cn

echo "${#arr[@]}"
来源：http://rx.gzmigu.cn

[R20] 关联数组（字典）
来源：http://yg.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gp.gzmigu.cn

[R21] 字符串长度
来源：http://vh.nszjky.cn

echo "${#s}"
来源：http://se.colortex.cn

[R22] 截取子串
来源：http://vy.gzmigu.cn

echo "${s:0:5}"
来源：http://wy.jianghongdianzi.cn

[R23] 字符串替换
来源：http://qx.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pr.newstarts.cn

[R24] 大小写转换
来源：http://kv.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ce.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://ia.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://od.haigaiapp.cn

[R26] 命令替换
来源：http://ht.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://pf.huixiangedu.cn

[R27] 算术展开
来源：http://go.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://cu.nicolike.cn

[R28] 浮点运算
来源：http://my.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://oz.nszjky.cn

[R29] 定义函数
来源：http://pg.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mr.chemitech.net.cn

[R30] 函数返回状态码
来源：http://xi.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://mz.wgjwhj.cn

[R31] 局部变量
来源：http://om.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://pq.hnjuh.cn

[R32] 参数个数校验
来源：http://gd.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jq.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://tz.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://au.shxzukj.cn

[R34] 退出时清理
来源：http://oc.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://si.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://mv.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hk.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://jh.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mt.panjiajie.cn

[R37] 把输出赋给变量
来源：http://hh.bookmarksfly.cn

files=$(ls -1)
来源：http://nb.521024.cn

[R38] 管道串联
来源：http://gh.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://gk.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://zi.bookmarksfly.cn

cmd > out.log 2>&1
来源：http://yl.huixinmuqiang.cn

[R40] 追加写日志
来源：http://jk.huixiangedu.cn

echo "log" >> out.log
来源：http://vq.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://iy.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://vz.nszjky.cn

[R42] 输入重定向
来源：http://ns.hnjuh.cn

wc -l < a.txt
来源：http://ik.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://pe.bjjhwx.cn

find . -name "*.log" -type f
来源：http://ro.shxzukj.cn

[R44] 按修改时间查找
来源：http://rx.huanxung.cn

find . -mtime -7 -type f
来源：http://zl.haigaiapp.cn

[R45] 批量删除
来源：http://nu.521024.cn

find . -name "*.tmp" -delete
来源：http://lj.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://ra.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mc.haigaiapp.cn

[R47] sed 单行替换
来源：http://uk.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ql.huixiangedu.cn

[R48] awk 取指定列
来源：http://wp.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://jg.muxihuayi.cn

[R49] awk 带条件
来源：http://vw.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wo.szxytkj.cn

[R50] awk 求和
来源：http://ku.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xr.wgjwhj.cn

[R51] 排序去重取前几
来源：http://xg.yuexingan06.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dh.hnjuh.cn

[R52] 统计行数
来源：http://xn.521024.cn

wc -l a.txt
来源：http://rh.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ur.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wp.bookmarksfly.cn

[R54] 比较两个文件
来源：http://cj.hahajie.cn

diff a.txt b.txt
来源：http://pw.shxzukj.cn

[R55] 压缩与解压
来源：http://wb.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qd.lnxyls.cn

[R56] 远程拷贝
来源：http://rh.shxzukj.cn

scp file user@host:/path/
来源：http://ph.szxytkj.cn

[R57] 远程执行命令
来源：http://fy.hnjuh.cn

ssh user@host 'uptime'
来源：http://fs.gzmigu.cn

[R58] 下载文件
来源：http://zr.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mn.bjjhwx.cn

[R59] 发 POST JSON
来源：http://hp.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cs.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://xf.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hv.wgjwhj.cn

[R61] 磁盘占用
来源：http://bh.nicolike.cn

df -h;  du -sh *
来源：http://lm.shxzskj.cn

[R62] 找最占空间的文件
来源：http://mk.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://ve.wgjwhj.cn

[R63] 内存与进程
来源：http://hc.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://an.szxytkj.cn

[R64] 结束进程
来源：http://wj.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://vm.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://jw.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vn.gzmigu.cn

[R66] 定时任务
来源：http://iy.gzmigu.cn

crontab -e;  crontab -l
来源：http://zc.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://wu.nicolike.cn

openssl rand -hex 16
来源：http://sd.hahajie.cn

[R68] 计算文件校验值
来源：http://em.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ie.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://gz.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://ev.chemitech.net.cn

[R70] 时间戳与互转
来源：http://wa.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://et.jctech888.com.cn

[R71] 日期格式化
来源：http://pk.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eb.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://hd.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gv.chemitech.net.cn

[R73] 分割大日志
来源：http://zw.huixiangedu.cn

split -l 1000 big.log part_
来源：http://qz.szxytkj.cn

[R74] 批量重命名
来源：http://qr.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qw.huixiangedu.cn

[R75] 导出环境变量
来源：http://ua.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://ad.yuexingan06.cn

[R76] 使用临时文件
来源：http://hu.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kw.lnxyls.cn

[R77] 读取用户输入
来源：http://ep.bjjhwx.cn

read -rp "请输入: " ans
来源：http://ao.haigaiapp.cn

[R78] 交互式菜单
来源：http://is.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gq.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://na.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tw.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://jh.chemitech.net.cn

time ./run.sh
来源：http://ez.huixiangedu.cn

================================================================================
来源：http://qh.shtwfgs.cn

S. C / C++ 专题
来源：http://tg.lnxyls.cn

================================================================================
来源：http://dj.yuexingan06.cn

[S01] C：Hello World
来源：http://rx.muxihuayi.cn

#include <stdio.h>
来源：http://uw.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sc.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://ur.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://nx.nicolike.cn

[S03] C：读入整数
来源：http://vc.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://rn.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://mi.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dg.bjjhwx.cn

[S05] C：字符串长度
来源：http://hx.haigaiapp.cn

strlen(s)
来源：http://jq.nszjky.cn

[S06] C：字符串比较
来源：http://wz.chemitech.net.cn

strcmp(a, b) == 0
来源：http://ij.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://sl.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ps.colortex.cn

[S08] C：动态内存分配与释放
来源：http://fu.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://it.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://an.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cf.bjjhwx.cn

[S10] C：指针与解引用
来源：http://ka.shtwfgs.cn

int *p = &a;  *p = 5;
来源：http://tf.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://gb.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://ah.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yw.chemitech.net.cn

fclose(f);
来源：http://hp.chemitech.net.cn

[S12] C：写文件
来源：http://ce.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cl.colortex.cn

[S13] C：宏定义
来源：http://at.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bp.jianghongdianzi.cn

[S14] C：枚举
来源：http://zu.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://qz.jctech888.com.cn

[S15] C：类型转换
来源：http://cs.huixinmuqiang.cn

(double) a / b
来源：http://rx.szsharing.cn

[S16] C：位操作置位
来源：http://pp.huanxung.cn

x |= (1 << 3);
来源：http://jt.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://it.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ex.lnxyls.cn

[S18] C：命令行参数
来源：http://ms.nszjky.cn

int main(int argc, char **argv)
来源：http://zl.huixiangedu.cn

[S19] C：快速排序
来源：http://ac.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pq.gzmigu.cn

[S20] C：二分查找
来源：http://bs.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vs.szxytkj.cn

[S21] C：字符类别判断
来源：http://wt.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nc.yuexingan06.cn

[S22] C：字符串转数字
来源：http://uv.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hx.gzmigu.cn

[S23] C：随机数
来源：http://yk.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yn.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://nl.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ot.haigaiapp.cn

[S25] C：内存拷贝
来源：http://wc.haigaiapp.cn

memcpy(dst, src, n);
来源：http://iy.gzmigu.cn

[S26] C：内存清零
来源：http://hy.9csxet.cn

memset(a, 0, sizeof a);
来源：http://yk.szsharing.cn

[S27] C：定义常量
来源：http://nx.shxzukj.cn

const double PI = 3.14159;
来源：http://bw.huixinmuqiang.cn

[S28] C：静态变量
来源：http://re.colortex.cn

static int counter = 0;
来源：http://rq.bookmarksfly.cn

[S29] C：变参函数
来源：http://kz.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tv.huixiangedu.cn

[S30] C：头文件保护
来源：http://tj.szsharing.cn

#ifndef X_H
来源：http://ql.newstarts.cn

#define X_H
来源：http://mm.shxzukj.cn

#endif
来源：http://je.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://cv.chemitech.net.cn

#include <iostream>
来源：http://lb.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://tb.muxihuayi.cn

[S32] C++：字符串
来源：http://oz.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://rr.yuexingan06.cn

[S33] C++：vector 增删
来源：http://sz.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dq.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://jd.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://jd.chemitech.net.cn

[S35] C++：map
来源：http://zl.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hq.colortex.cn

[S36] C++：unordered_map
来源：http://on.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uj.shxzukj.cn

[S37] C++：set
来源：http://ag.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kq.newstarts.cn

[S38] C++：排序
来源：http://sn.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://bh.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://ux.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vo.newstarts.cn

[S40] C++：查找元素
来源：http://zc.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tr.panjiajie.cn

[S41] C++：类与构造函数
来源：http://br.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tx.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://ta.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://jr.muxihuayi.cn

[S43] C++：智能指针
来源：http://xq.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://su.asd995.cn

[S44] C++：引用传参
来源：http://yr.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://hr.hnjuh.cn

[S45] C++：lambda
来源：http://hw.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ds.yuexingan06.cn

[S46] C++：函数模板
来源：http://vx.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kh.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://sl.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rz.lnxyls.cn

[S48] C++：逐行读文件
来源：http://jy.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nm.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://md.shtwfgs.cn

[S49] C++：写文件
来源：http://qt.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jm.shxzukj.cn

[S50] C++：格式化数字
来源：http://wb.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eu.szsharing.cn

[S51] C++：显式类型转换
来源：http://am.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://wg.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://jc.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ow.szsharing.cn

[S53] C++：移动语义
来源：http://rk.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://zy.chemitech.net.cn

[S54] C++：异常处理
来源：http://wv.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mv.newstarts.cn

[S55] C++：结构化绑定
来源：http://al.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uo.521024.cn

[S56] C++：optional
来源：http://em.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://em.colortex.cn

[S57] C++：编译期常量
来源：http://rr.shxzukj.cn

constexpr int N = 10;
来源：http://fn.huixiangedu.cn

[S58] C++：命名空间
来源：http://cb.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://ij.szxytkj.cn

[S59] C++：静态断言
来源：http://mo.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rn.asd995.cn

[S60] C++：遍历并删除元素
来源：http://ux.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qd.9csxet.cn

================================================================================
来源：http://dw.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zo.nicolike.cn

================================================================================
来源：http://xx.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://rd.wgjwhj.cn

println("Hello")
来源：http://wc.gzmigu.cn

[T02] Kotlin：变量
来源：http://bz.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ss.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://ug.jctech888.com.cn

"值: $b"
来源：http://vi.newstarts.cn

[T04] Kotlin：空安全
来源：http://de.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://iz.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://of.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cq.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ri.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hh.521024.cn

[T07] Kotlin：集合过滤
来源：http://ng.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ly.lnxyls.cn

[T08] Kotlin：数据类
来源：http://st.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://th.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://xi.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://ub.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://cc.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tw.shxzukj.cn

[T11] Kotlin：协程
来源：http://qk.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yv.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://dk.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://xv.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://du.szsharing.cn

val m = mapOf("a" to 1)
来源：http://lv.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://og.szsharing.cn

for (i in 1..10) println(i)
来源：http://cv.hnjuh.cn

[T15] Kotlin：接口
来源：http://lr.hahajie.cn

interface Shape { fun area(): Double }
来源：http://zj.nszjky.cn

[T16] Swift：Hello World
来源：http://yw.nicolike.cn

print("Hello")
来源：http://aa.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://rc.haigaiapp.cn

var a = 1;  let b = 2
来源：http://sx.lnxyls.cn

[T18] Swift：字符串插值
来源：http://lq.huanxung.cn

"值: \(b)"
来源：http://cd.colortex.cn

[T19] Swift：可选绑定
来源：http://ss.lnxyls.cn

if let n = opt { print(n) }
来源：http://jy.panjiajie.cn

[T20] Swift：数组操作
来源：http://vk.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rb.yuexingan06.cn


<!-- 参考信息 -->