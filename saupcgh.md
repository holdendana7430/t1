代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://rp.jctech888.com.cn

[R18] 遍历数组
来源：http://zo.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ep.newstarts.cn

[R19] 数组长度
来源：http://vl.huixiangedu.cn

echo "${#arr[@]}"
来源：http://of.colortex.cn

[R20] 关联数组（字典）
来源：http://lj.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ol.huixiangedu.cn

[R21] 字符串长度
来源：http://bz.shxzukj.cn

echo "${#s}"
来源：http://ts.lnxyls.cn

[R22] 截取子串
来源：http://nc.521024.cn

echo "${s:0:5}"
来源：http://by.yuntaijiaju.cn

[R23] 字符串替换
来源：http://rg.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sg.asd995.cn

[R24] 大小写转换
来源：http://ya.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gs.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://hh.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ic.wgjwhj.cn

[R26] 命令替换
来源：http://rw.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://cd.muxihuayi.cn

[R27] 算术展开
来源：http://og.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://dk.asd995.cn

[R28] 浮点运算
来源：http://wl.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://vl.asd995.cn

[R29] 定义函数
来源：http://jo.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kq.nicolike.cn

[R30] 函数返回状态码
来源：http://sb.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://zq.shxzskj.cn

[R31] 局部变量
来源：http://cz.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://pc.nszjky.cn

[R32] 参数个数校验
来源：http://av.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ii.yuexingan06.cn

[R33] 捕获错误并提示行号
来源：http://rs.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uz.jianghongdianzi.cn

[R34] 退出时清理
来源：http://bl.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fv.szxytkj.cn

[R35] 后台执行并等待
来源：http://yz.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ec.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://aw.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ev.gzmigu.cn

[R37] 把输出赋给变量
来源：http://ak.shtwfgs.cn

files=$(ls -1)
来源：http://pm.gzmigu.cn

[R38] 管道串联
来源：http://em.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://oq.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://xv.521024.cn

cmd > out.log 2>&1
来源：http://ee.9csxet.cn

[R40] 追加写日志
来源：http://la.jctech888.com.cn

echo "log" >> out.log
来源：http://gx.bookmarksfly.cn

[R41] 丢弃输出
来源：http://bj.hnjuh.cn

cmd >/dev/null 2>&1
来源：http://gw.gzmigu.cn

[R42] 输入重定向
来源：http://nm.huanxung.cn

wc -l < a.txt
来源：http://uk.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://gg.szxytkj.cn

find . -name "*.log" -type f
来源：http://ld.haigaiapp.cn

[R44] 按修改时间查找
来源：http://zd.szsharing.cn

find . -mtime -7 -type f
来源：http://pq.haigaiapp.cn

[R45] 批量删除
来源：http://ca.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://fn.asd995.cn

[R46] 递归替换文件内容
来源：http://bi.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wd.panjiajie.cn

[R47] sed 单行替换
来源：http://dx.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ju.chemitech.net.cn

[R48] awk 取指定列
来源：http://nr.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://qf.szxytkj.cn

[R49] awk 带条件
来源：http://xk.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jd.bookmarksfly.cn

[R50] awk 求和
来源：http://pg.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gq.hahajie.cn

[R51] 排序去重取前几
来源：http://ed.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gq.panjiajie.cn

[R52] 统计行数
来源：http://wk.jctech888.com.cn

wc -l a.txt
来源：http://to.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://nr.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qs.nicolike.cn

[R54] 比较两个文件
来源：http://ve.bookmarksfly.cn

diff a.txt b.txt
来源：http://al.chemitech.net.cn

[R55] 压缩与解压
来源：http://mo.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jg.521024.cn

[R56] 远程拷贝
来源：http://tl.huanxung.cn

scp file user@host:/path/
来源：http://oc.huixiangedu.cn

[R57] 远程执行命令
来源：http://lt.gzmigu.cn

ssh user@host 'uptime'
来源：http://at.szsharing.cn

[R58] 下载文件
来源：http://aw.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xx.szxytkj.cn

[R59] 发 POST JSON
来源：http://ho.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ro.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://cl.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ah.colortex.cn

[R61] 磁盘占用
来源：http://jr.chemitech.net.cn

df -h;  du -sh *
来源：http://rb.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://tl.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://hk.shtwfgs.cn

[R63] 内存与进程
来源：http://do.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://wi.szxytkj.cn

[R64] 结束进程
来源：http://wq.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://bv.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://lz.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fn.newstarts.cn

[R66] 定时任务
来源：http://gw.huixiangedu.cn

crontab -e;  crontab -l
来源：http://fp.9csxet.cn

[R67] 生成随机十六进制串
来源：http://cm.panjiajie.cn

openssl rand -hex 16
来源：http://tj.hnjuh.cn

[R68] 计算文件校验值
来源：http://gp.521024.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zr.muxihuayi.cn

[R69] 生成随机密码
来源：http://gl.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://qv.lnxyls.cn

[R70] 时间戳与互转
来源：http://xv.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://tc.huanxung.cn

[R71] 日期格式化
来源：http://yf.yuntaijiaju.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ya.wgjwhj.cn

[R72] 等待端口就绪
来源：http://et.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lo.colortex.cn

[R73] 分割大日志
来源：http://nu.shxzskj.cn

split -l 1000 big.log part_
来源：http://ts.yuexingan06.cn

[R74] 批量重命名
来源：http://wd.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ad.shxzskj.cn

[R75] 导出环境变量
来源：http://dr.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://ll.szxytkj.cn

[R76] 使用临时文件
来源：http://hu.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ky.shxzukj.cn

[R77] 读取用户输入
来源：http://vh.panjiajie.cn

read -rp "请输入: " ans
来源：http://yp.hnjuh.cn

[R78] 交互式菜单
来源：http://ij.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uc.hahajie.cn

[R79] 解析命令行选项
来源：http://ev.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nh.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://tw.hahajie.cn

time ./run.sh
来源：http://bd.haigaiapp.cn

================================================================================
来源：http://bb.nszjky.cn

S. C / C++ 专题
来源：http://he.bjjhwx.cn

================================================================================
来源：http://ef.colortex.cn

[S01] C：Hello World
来源：http://gn.muxihuayi.cn

#include <stdio.h>
来源：http://yn.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ia.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://ac.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://ug.shtwfgs.cn

[S03] C：读入整数
来源：http://ho.colortex.cn

int x; scanf("%d", &x);
来源：http://li.nszjky.cn

[S04] C：字符串复制
来源：http://ya.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pa.jctech888.com.cn

[S05] C：字符串长度
来源：http://bc.wgjwhj.cn

strlen(s)
来源：http://me.lnxyls.cn

[S06] C：字符串比较
来源：http://vg.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://eh.nszjky.cn

[S07] C：数组遍历求和
来源：http://iq.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uk.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://qi.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://il.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://ug.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gj.nicolike.cn

[S10] C：指针与解引用
来源：http://ti.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://cb.bjjhwx.cn

[S11] C：逐行读文件
来源：http://oo.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://ja.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://du.bjjhwx.cn

fclose(f);
来源：http://ua.colortex.cn

[S12] C：写文件
来源：http://xw.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rd.wgjwhj.cn

[S13] C：宏定义
来源：http://gp.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pj.hnjuh.cn

[S14] C：枚举
来源：http://ut.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://kr.gzmigu.cn

[S15] C：类型转换
来源：http://zi.newstarts.cn

(double) a / b
来源：http://il.bjjhwx.cn

[S16] C：位操作置位
来源：http://gd.colortex.cn

x |= (1 << 3);
来源：http://bi.szsharing.cn

[S17] C：安全拼接字符串
来源：http://tf.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dk.huanxung.cn

[S18] C：命令行参数
来源：http://lb.asd995.cn

int main(int argc, char **argv)
来源：http://sz.shxzskj.cn

[S19] C：快速排序
来源：http://xf.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xg.hnjuh.cn

[S20] C：二分查找
来源：http://ac.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ae.shxzukj.cn

[S21] C：字符类别判断
来源：http://nu.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://io.shtwfgs.cn

[S22] C：字符串转数字
来源：http://by.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lf.bookmarksfly.cn

[S23] C：随机数
来源：http://zj.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ii.szxytkj.cn

[S24] C：获取本地时间
来源：http://xr.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ls.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://gr.bjjhwx.cn

memcpy(dst, src, n);
来源：http://ot.gzmigu.cn

[S26] C：内存清零
来源：http://zs.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://dt.huixiangedu.cn

[S27] C：定义常量
来源：http://dg.bjjhwx.cn

const double PI = 3.14159;
来源：http://nw.chemitech.net.cn

[S28] C：静态变量
来源：http://ng.asd995.cn

static int counter = 0;
来源：http://wk.lnxyls.cn

[S29] C：变参函数
来源：http://oo.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dx.bookmarksfly.cn

[S30] C：头文件保护
来源：http://fr.nszjky.cn

#ifndef X_H
来源：http://wp.haigaiapp.cn

#define X_H
来源：http://uy.wgjwhj.cn

#endif
来源：http://zw.bookmarksfly.cn

[S31] C++：Hello World
来源：http://en.yuntaijiaju.cn

#include <iostream>
来源：http://lt.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://nl.asd995.cn

[S32] C++：字符串
来源：http://cr.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://ft.asd995.cn

[S33] C++：vector 增删
来源：http://hs.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qa.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ne.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://vd.hahajie.cn

[S35] C++：map
来源：http://sh.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pr.szsharing.cn

[S36] C++：unordered_map
来源：http://wk.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ct.colortex.cn

[S37] C++：set
来源：http://hb.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pz.jianghongdianzi.cn

[S38] C++：排序
来源：http://fg.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://dq.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://gn.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yg.wgjwhj.cn

[S40] C++：查找元素
来源：http://bp.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yp.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://lq.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gi.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://nr.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://yf.nicolike.cn

[S43] C++：智能指针
来源：http://vw.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://bv.hnjuh.cn

[S44] C++：引用传参
来源：http://ji.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://nx.yuexingan06.cn

[S45] C++：lambda
来源：http://jw.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gy.hnjuh.cn

[S46] C++：函数模板
来源：http://xr.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nd.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://va.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uf.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://wl.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ld.asd995.cn

while (std::getline(in, line)) { }
来源：http://oa.newstarts.cn

[S49] C++：写文件
来源：http://aq.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zu.hahajie.cn

[S50] C++：格式化数字
来源：http://av.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nb.szsharing.cn

[S51] C++：显式类型转换
来源：http://eh.chemitech.net.cn

static_cast<double>(a) / b
来源：http://vk.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ut.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://pe.asd995.cn

[S53] C++：移动语义
来源：http://bz.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://jr.jctech888.com.cn

[S54] C++：异常处理
来源：http://fr.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jz.newstarts.cn

[S55] C++：结构化绑定
来源：http://zl.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fi.haigaiapp.cn

[S56] C++：optional
来源：http://to.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://is.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://ga.shxzukj.cn

constexpr int N = 10;
来源：http://py.nszjky.cn

[S58] C++：命名空间
来源：http://it.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://qq.haigaiapp.cn

[S59] C++：静态断言
来源：http://gd.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ui.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://ba.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kb.newstarts.cn

================================================================================
来源：http://qm.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jh.colortex.cn

================================================================================
来源：http://td.huanxung.cn

[T01] Kotlin：Hello World
来源：http://fa.9csxet.cn

println("Hello")
来源：http://qj.9csxet.cn

[T02] Kotlin：变量
来源：http://tf.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://am.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://bv.colortex.cn

"值: $b"
来源：http://zw.newstarts.cn

[T04] Kotlin：空安全
来源：http://mz.shxzukj.cn

val n: String? = null;  n?.length
来源：http://gz.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://dd.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uz.hahajie.cn

[T06] Kotlin：集合映射
来源：http://kp.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fh.asd995.cn

[T07] Kotlin：集合过滤
来源：http://wr.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://la.gzmigu.cn

[T08] Kotlin：数据类
来源：http://af.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://ez.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://hb.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://ed.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://ga.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vl.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ul.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tj.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://hs.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://kt.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://el.newstarts.cn

val m = mapOf("a" to 1)
来源：http://gq.gzmigu.cn

[T14] Kotlin：循环
来源：http://lm.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://dw.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://pb.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://zi.huixiangedu.cn

[T16] Swift：Hello World
来源：http://bv.nicolike.cn

print("Hello")
来源：http://kx.hnjuh.cn

[T17] Swift：变量与常量
来源：http://kj.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://lb.nszjky.cn

[T18] Swift：字符串插值
来源：http://eu.newstarts.cn

"值: \(b)"
来源：http://fk.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://pn.panjiajie.cn

if let n = opt { print(n) }
来源：http://on.gzmigu.cn

[T20] Swift：数组操作
来源：http://ow.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vc.newstarts.cn


<!-- 参考信息 -->