代发 wailian999

echo "${#arr[@]}"
来源：http://ov.newstarts.cn

[R20] 关联数组（字典）
来源：http://zd.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jm.wgjwhj.cn

[R21] 字符串长度
来源：http://cd.lnxyls.cn

echo "${#s}"
来源：http://xt.jianghongdianzi.cn

[R22] 截取子串
来源：http://cb.colortex.cn

echo "${s:0:5}"
来源：http://cw.colortex.cn

[R23] 字符串替换
来源：http://eh.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eb.szxytkj.cn

[R24] 大小写转换
来源：http://nd.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cx.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://va.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ti.huanxung.cn

[R26] 命令替换
来源：http://yz.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://zj.huanxung.cn

[R27] 算术展开
来源：http://eo.nszjky.cn

echo $((1 + 2 * 3))
来源：http://lb.9csxet.cn

[R28] 浮点运算
来源：http://jj.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://mt.newstarts.cn

[R29] 定义函数
来源：http://lk.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hg.yuexingan06.cn

[R30] 函数返回状态码
来源：http://tm.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://qn.huixiangedu.cn

[R31] 局部变量
来源：http://tr.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://rh.szxytkj.cn

[R32] 参数个数校验
来源：http://rc.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sy.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://mj.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hf.haigaiapp.cn

[R34] 退出时清理
来源：http://ww.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kb.panjiajie.cn

[R35] 后台执行并等待
来源：http://za.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://su.gzmigu.cn

[R36] 并发执行多个任务
来源：http://ov.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nd.huanxung.cn

[R37] 把输出赋给变量
来源：http://ih.panjiajie.cn

files=$(ls -1)
来源：http://ba.hnjuh.cn

[R38] 管道串联
来源：http://rs.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://sq.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://ac.muxihuayi.cn

cmd > out.log 2>&1
来源：http://fp.colortex.cn

[R40] 追加写日志
来源：http://ju.bookmarksfly.cn

echo "log" >> out.log
来源：http://yc.haigaiapp.cn

[R41] 丢弃输出
来源：http://dp.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://dv.hnjuh.cn

[R42] 输入重定向
来源：http://jq.hnjuh.cn

wc -l < a.txt
来源：http://gy.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://yx.shxzukj.cn

find . -name "*.log" -type f
来源：http://uz.shxzskj.cn

[R44] 按修改时间查找
来源：http://bd.shxzskj.cn

find . -mtime -7 -type f
来源：http://bs.muxihuayi.cn

[R45] 批量删除
来源：http://gt.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://pa.gzmigu.cn

[R46] 递归替换文件内容
来源：http://ar.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://if.jctech888.com.cn

[R47] sed 单行替换
来源：http://xv.jctech888.com.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tx.chemitech.net.cn

[R48] awk 取指定列
来源：http://rn.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://jj.jianghongdianzi.cn

[R49] awk 带条件
来源：http://ul.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://si.bjjhwx.cn

[R50] awk 求和
来源：http://xw.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sv.wgjwhj.cn

[R51] 排序去重取前几
来源：http://vn.yuntaijiaju.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cj.jianghongdianzi.cn

[R52] 统计行数
来源：http://nj.bookmarksfly.cn

wc -l a.txt
来源：http://cb.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://to.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kr.chemitech.net.cn

[R54] 比较两个文件
来源：http://wo.jctech888.com.cn

diff a.txt b.txt
来源：http://tu.bookmarksfly.cn

[R55] 压缩与解压
来源：http://fj.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uf.nicolike.cn

[R56] 远程拷贝
来源：http://yt.shxzukj.cn

scp file user@host:/path/
来源：http://to.jctech888.com.cn

[R57] 远程执行命令
来源：http://mk.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://uf.bjjhwx.cn

[R58] 下载文件
来源：http://nb.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://th.haigaiapp.cn

[R59] 发 POST JSON
来源：http://pc.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aw.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://pt.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sb.9csxet.cn

[R61] 磁盘占用
来源：http://rq.nicolike.cn

df -h;  du -sh *
来源：http://wj.newstarts.cn

[R62] 找最占空间的文件
来源：http://ho.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://rn.shtwfgs.cn

[R63] 内存与进程
来源：http://bm.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://to.yuexingan06.cn

[R64] 结束进程
来源：http://zu.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://lr.9csxet.cn

[R65] 查看端口占用
来源：http://jd.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ni.huanxung.cn

[R66] 定时任务
来源：http://pq.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://vc.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://iu.szxytkj.cn

openssl rand -hex 16
来源：http://ff.521024.cn

[R68] 计算文件校验值
来源：http://an.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ye.muxihuayi.cn

[R69] 生成随机密码
来源：http://yv.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://gr.muxihuayi.cn

[R70] 时间戳与互转
来源：http://ng.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://qz.hahajie.cn

[R71] 日期格式化
来源：http://on.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lj.szxytkj.cn

[R72] 等待端口就绪
来源：http://jx.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yf.nszjky.cn

[R73] 分割大日志
来源：http://fi.muxihuayi.cn

split -l 1000 big.log part_
来源：http://ca.hnjuh.cn

[R74] 批量重命名
来源：http://wb.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vn.panjiajie.cn

[R75] 导出环境变量
来源：http://fd.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://gu.szsharing.cn

[R76] 使用临时文件
来源：http://mv.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ch.haigaiapp.cn

[R77] 读取用户输入
来源：http://xh.haigaiapp.cn

read -rp "请输入: " ans
来源：http://ph.bjjhwx.cn

[R78] 交互式菜单
来源：http://uy.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cv.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://la.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pu.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://er.shxzskj.cn

time ./run.sh
来源：http://oj.chemitech.net.cn

================================================================================
来源：http://zm.shxzukj.cn

S. C / C++ 专题
来源：http://nm.colortex.cn

================================================================================
来源：http://gv.jctech888.com.cn

[S01] C：Hello World
来源：http://cs.shtwfgs.cn

#include <stdio.h>
来源：http://df.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kc.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://wk.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://tx.bjjhwx.cn

[S03] C：读入整数
来源：http://bn.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://ur.bjjhwx.cn

[S04] C：字符串复制
来源：http://cq.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://id.shxzukj.cn

[S05] C：字符串长度
来源：http://in.bjjhwx.cn

strlen(s)
来源：http://ts.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ww.chemitech.net.cn

strcmp(a, b) == 0
来源：http://un.nicolike.cn

[S07] C：数组遍历求和
来源：http://rg.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nw.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://ax.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ua.shxzukj.cn

[S09] C：结构体定义与初始化
来源：http://wj.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jv.yuexingan06.cn

[S10] C：指针与解引用
来源：http://zv.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://mc.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://mu.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://xo.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eq.muxihuayi.cn

fclose(f);
来源：http://im.panjiajie.cn

[S12] C：写文件
来源：http://zx.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uq.asd995.cn

[S13] C：宏定义
来源：http://gu.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://se.521024.cn

[S14] C：枚举
来源：http://wq.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://cy.gzmigu.cn

[S15] C：类型转换
来源：http://br.9csxet.cn

(double) a / b
来源：http://um.szsharing.cn

[S16] C：位操作置位
来源：http://ee.wgjwhj.cn

x |= (1 << 3);
来源：http://er.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://ns.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yj.huanxung.cn

[S18] C：命令行参数
来源：http://vy.newstarts.cn

int main(int argc, char **argv)
来源：http://ii.muxihuayi.cn

[S19] C：快速排序
来源：http://fc.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hn.yuexingan06.cn

[S20] C：二分查找
来源：http://ci.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lh.521024.cn

[S21] C：字符类别判断
来源：http://fp.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zh.9csxet.cn

[S22] C：字符串转数字
来源：http://ff.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zt.gzmigu.cn

[S23] C：随机数
来源：http://ha.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hy.shtwfgs.cn

[S24] C：获取本地时间
来源：http://wx.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nt.lnxyls.cn

[S25] C：内存拷贝
来源：http://mk.szsharing.cn

memcpy(dst, src, n);
来源：http://lt.muxihuayi.cn

[S26] C：内存清零
来源：http://gr.nszjky.cn

memset(a, 0, sizeof a);
来源：http://lg.colortex.cn

[S27] C：定义常量
来源：http://xy.hahajie.cn

const double PI = 3.14159;
来源：http://zw.hahajie.cn

[S28] C：静态变量
来源：http://mb.huixinmuqiang.cn

static int counter = 0;
来源：http://iq.asd995.cn

[S29] C：变参函数
来源：http://ad.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fw.lnxyls.cn

[S30] C：头文件保护
来源：http://ob.haigaiapp.cn

#ifndef X_H
来源：http://th.jctech888.com.cn

#define X_H
来源：http://ch.shxzukj.cn

#endif
来源：http://kd.asd995.cn

[S31] C++：Hello World
来源：http://ve.shxzskj.cn

#include <iostream>
来源：http://js.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://ou.9csxet.cn

[S32] C++：字符串
来源：http://py.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://af.nszjky.cn

[S33] C++：vector 增删
来源：http://tb.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ii.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://cj.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://ru.szsharing.cn

[S35] C++：map
来源：http://tu.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bt.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://er.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://to.shxzskj.cn

[S37] C++：set
来源：http://mj.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gv.9csxet.cn

[S38] C++：排序
来源：http://lk.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://bk.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://gz.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://on.shxzskj.cn

[S40] C++：查找元素
来源：http://zo.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ub.colortex.cn

[S41] C++：类与构造函数
来源：http://gg.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yr.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://ty.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://nf.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://dn.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://pd.shxzukj.cn

[S44] C++：引用传参
来源：http://mv.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://bg.jctech888.com.cn

[S45] C++：lambda
来源：http://nl.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mg.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://hq.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xp.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://dj.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eo.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://vb.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://re.asd995.cn

while (std::getline(in, line)) { }
来源：http://oo.bjjhwx.cn

[S49] C++：写文件
来源：http://xv.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gk.muxihuayi.cn

[S50] C++：格式化数字
来源：http://rp.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ay.gzmigu.cn

[S51] C++：显式类型转换
来源：http://eh.nicolike.cn

static_cast<double>(a) / b
来源：http://de.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://jp.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://nd.jctech888.com.cn

[S53] C++：移动语义
来源：http://ul.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://bh.lnxyls.cn

[S54] C++：异常处理
来源：http://mh.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fl.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://li.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ys.yuntaijiaju.cn

[S56] C++：optional
来源：http://jh.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eq.asd995.cn

[S57] C++：编译期常量
来源：http://at.nszjky.cn

constexpr int N = 10;
来源：http://rb.521024.cn

[S58] C++：命名空间
来源：http://jz.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://ct.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://xa.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pe.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://ci.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jh.jianghongdianzi.cn

================================================================================
来源：http://lo.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ys.huixinmuqiang.cn

================================================================================
来源：http://jy.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://tt.yuexingan06.cn

println("Hello")
来源：http://qp.muxihuayi.cn

[T02] Kotlin：变量
来源：http://ps.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hy.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://id.9csxet.cn

"值: $b"
来源：http://ex.asd995.cn

[T04] Kotlin：空安全
来源：http://hb.shxzskj.cn

val n: String? = null;  n?.length
来源：http://ae.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://so.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jd.colortex.cn

[T06] Kotlin：集合映射
来源：http://pt.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hw.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://hq.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pr.lnxyls.cn

[T08] Kotlin：数据类
来源：http://nm.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://cb.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://ws.chemitech.net.cn

fun String.exclaim() = this + "!"
来源：http://pl.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://qx.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tn.jctech888.com.cn

[T11] Kotlin：协程
来源：http://vb.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ix.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ei.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://vd.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://nn.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://qk.jctech888.com.cn

[T14] Kotlin：循环
来源：http://xv.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://tp.shxzukj.cn

[T15] Kotlin：接口
来源：http://sq.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://cq.shxzukj.cn

[T16] Swift：Hello World
来源：http://br.asd995.cn

print("Hello")
来源：http://ii.521024.cn

[T17] Swift：变量与常量
来源：http://pj.hahajie.cn

var a = 1;  let b = 2
来源：http://tj.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://or.huanxung.cn

"值: \(b)"
来源：http://bq.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://rv.haigaiapp.cn

if let n = opt { print(n) }
来源：http://df.shxzukj.cn

[T20] Swift：数组操作
来源：http://lh.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ds.shtwfgs.cn

[T21] Swift：遍历
来源：http://ej.colortex.cn

for x in a { print(x) }
来源：http://yw.huixiangedu.cn

[T22] Swift：字典
来源：http://pb.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sr.shxzukj.cn


<!-- 参考信息 -->