代发 wailian999

echo "${#s}"
来源：http://aj.panjiajie.cn

[R22] 截取子串
来源：http://qf.gzmigu.cn

echo "${s:0:5}"
来源：http://nx.nicolike.cn

[R23] 字符串替换
来源：http://rx.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://za.panjiajie.cn

[R24] 大小写转换
来源：http://gt.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ap.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://sg.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vv.shxzskj.cn

[R26] 命令替换
来源：http://vj.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://nc.yuexingan06.cn

[R27] 算术展开
来源：http://td.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://cc.haigaiapp.cn

[R28] 浮点运算
来源：http://hg.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://uy.gzmigu.cn

[R29] 定义函数
来源：http://qn.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ve.521024.cn

[R30] 函数返回状态码
来源：http://nh.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://or.bjjhwx.cn

[R31] 局部变量
来源：http://kh.wgjwhj.cn

f() { local x=1; echo "$x"; }
来源：http://bh.huanxung.cn

[R32] 参数个数校验
来源：http://hx.gzmigu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pe.521024.cn

[R33] 捕获错误并提示行号
来源：http://tv.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nn.asd995.cn

[R34] 退出时清理
来源：http://gu.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cv.newstarts.cn

[R35] 后台执行并等待
来源：http://ve.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://co.hahajie.cn

[R36] 并发执行多个任务
来源：http://gf.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wb.gzmigu.cn

[R37] 把输出赋给变量
来源：http://bh.asd995.cn

files=$(ls -1)
来源：http://as.newstarts.cn

[R38] 管道串联
来源：http://ya.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://ei.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://ea.yuexingan06.cn

cmd > out.log 2>&1
来源：http://dk.hnjuh.cn

[R40] 追加写日志
来源：http://ur.nszjky.cn

echo "log" >> out.log
来源：http://kg.huixiangedu.cn

[R41] 丢弃输出
来源：http://ie.bjjhwx.cn

cmd >/dev/null 2>&1
来源：http://yg.jianghongdianzi.cn

[R42] 输入重定向
来源：http://yh.hnjuh.cn

wc -l < a.txt
来源：http://no.huixiangedu.cn

[R43] 按名字查找文件
来源：http://lx.muxihuayi.cn

find . -name "*.log" -type f
来源：http://az.yuexingan06.cn

[R44] 按修改时间查找
来源：http://ta.shtwfgs.cn

find . -mtime -7 -type f
来源：http://zl.bookmarksfly.cn

[R45] 批量删除
来源：http://nq.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://hl.521024.cn

[R46] 递归替换文件内容
来源：http://bl.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yz.colortex.cn

[R47] sed 单行替换
来源：http://nq.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ky.newstarts.cn

[R48] awk 取指定列
来源：http://jm.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://cj.521024.cn

[R49] awk 带条件
来源：http://nl.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ba.bjjhwx.cn

[R50] awk 求和
来源：http://kw.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ra.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://yh.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://je.nszjky.cn

[R52] 统计行数
来源：http://sz.chemitech.net.cn

wc -l a.txt
来源：http://yi.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://og.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cu.nszjky.cn

[R54] 比较两个文件
来源：http://nm.szsharing.cn

diff a.txt b.txt
来源：http://uq.nicolike.cn

[R55] 压缩与解压
来源：http://al.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nb.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ah.lnxyls.cn

scp file user@host:/path/
来源：http://sb.jctech888.com.cn

[R57] 远程执行命令
来源：http://fl.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://pi.lnxyls.cn

[R58] 下载文件
来源：http://mr.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uk.huixiangedu.cn

[R59] 发 POST JSON
来源：http://ha.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://no.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://vb.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cx.muxihuayi.cn

[R61] 磁盘占用
来源：http://wb.shtwfgs.cn

df -h;  du -sh *
来源：http://dg.shxzukj.cn

[R62] 找最占空间的文件
来源：http://rf.asd995.cn

du -ah . | sort -rh | head -10
来源：http://nl.huixinmuqiang.cn

[R63] 内存与进程
来源：http://bd.asd995.cn

free -h;  ps aux | grep nginx
来源：http://uk.szxytkj.cn

[R64] 结束进程
来源：http://eg.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://ni.szsharing.cn

[R65] 查看端口占用
来源：http://xf.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nx.gzmigu.cn

[R66] 定时任务
来源：http://gv.huanxung.cn

crontab -e;  crontab -l
来源：http://is.nicolike.cn

[R67] 生成随机十六进制串
来源：http://wx.lnxyls.cn

openssl rand -hex 16
来源：http://dy.521024.cn

[R68] 计算文件校验值
来源：http://xt.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iq.asd995.cn

[R69] 生成随机密码
来源：http://ld.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://tg.chemitech.net.cn

[R70] 时间戳与互转
来源：http://tj.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ho.colortex.cn

[R71] 日期格式化
来源：http://rc.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kp.huanxung.cn

[R72] 等待端口就绪
来源：http://ez.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xl.muxihuayi.cn

[R73] 分割大日志
来源：http://jf.shxzukj.cn

split -l 1000 big.log part_
来源：http://nu.bookmarksfly.cn

[R74] 批量重命名
来源：http://ww.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ch.shtwfgs.cn

[R75] 导出环境变量
来源：http://me.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://rr.bookmarksfly.cn

[R76] 使用临时文件
来源：http://ah.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sy.shxzskj.cn

[R77] 读取用户输入
来源：http://jq.shtwfgs.cn

read -rp "请输入: " ans
来源：http://eh.hnjuh.cn

[R78] 交互式菜单
来源：http://ur.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://px.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://mo.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xr.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://xv.gzmigu.cn

time ./run.sh
来源：http://ja.panjiajie.cn

================================================================================
来源：http://oe.yuexingan06.cn

S. C / C++ 专题
来源：http://mv.hahajie.cn

================================================================================
来源：http://sp.521024.cn

[S01] C：Hello World
来源：http://ac.haigaiapp.cn

#include <stdio.h>
来源：http://ge.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hc.hahajie.cn

[S02] C：变量与格式化输出
来源：http://eh.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://tv.szsharing.cn

[S03] C：读入整数
来源：http://wz.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://ht.shtwfgs.cn

[S04] C：字符串复制
来源：http://uu.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pv.shxzskj.cn

[S05] C：字符串长度
来源：http://lk.nszjky.cn

strlen(s)
来源：http://er.nicolike.cn

[S06] C：字符串比较
来源：http://qd.jctech888.com.cn

strcmp(a, b) == 0
来源：http://ey.colortex.cn

[S07] C：数组遍历求和
来源：http://pz.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hg.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://fh.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qo.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://jt.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mj.shxzukj.cn

[S10] C：指针与解引用
来源：http://nx.asd995.cn

int *p = &a;  *p = 5;
来源：http://eb.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://xq.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://hs.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uy.jianghongdianzi.cn

fclose(f);
来源：http://jv.shtwfgs.cn

[S12] C：写文件
来源：http://rd.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bw.yuntaijiaju.cn

[S13] C：宏定义
来源：http://gh.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ox.huixinmuqiang.cn

[S14] C：枚举
来源：http://ka.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://hz.huixinmuqiang.cn

[S15] C：类型转换
来源：http://cv.yuntaijiaju.cn

(double) a / b
来源：http://va.shxzskj.cn

[S16] C：位操作置位
来源：http://na.yuexingan06.cn

x |= (1 << 3);
来源：http://wc.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://jj.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://og.asd995.cn

[S18] C：命令行参数
来源：http://ui.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://vr.panjiajie.cn

[S19] C：快速排序
来源：http://to.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wb.haigaiapp.cn

[S20] C：二分查找
来源：http://km.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kx.hnjuh.cn

[S21] C：字符类别判断
来源：http://gc.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nt.wgjwhj.cn

[S22] C：字符串转数字
来源：http://jf.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lv.newstarts.cn

[S23] C：随机数
来源：http://pb.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vx.colortex.cn

[S24] C：获取本地时间
来源：http://ce.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bs.colortex.cn

[S25] C：内存拷贝
来源：http://xw.shtwfgs.cn

memcpy(dst, src, n);
来源：http://zh.szsharing.cn

[S26] C：内存清零
来源：http://ts.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://qp.gzmigu.cn

[S27] C：定义常量
来源：http://wg.jctech888.com.cn

const double PI = 3.14159;
来源：http://wx.shtwfgs.cn

[S28] C：静态变量
来源：http://wx.shxzukj.cn

static int counter = 0;
来源：http://fe.hahajie.cn

[S29] C：变参函数
来源：http://pm.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gr.gzmigu.cn

[S30] C：头文件保护
来源：http://ma.shxzukj.cn

#ifndef X_H
来源：http://ch.jctech888.com.cn

#define X_H
来源：http://uq.shtwfgs.cn

#endif
来源：http://sl.nszjky.cn

[S31] C++：Hello World
来源：http://ks.chemitech.net.cn

#include <iostream>
来源：http://bk.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://dy.nszjky.cn

[S32] C++：字符串
来源：http://ue.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://az.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ae.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dr.gzmigu.cn

[S34] C++：遍历 vector
来源：http://io.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://hk.jctech888.com.cn

[S35] C++：map
来源：http://wg.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ym.colortex.cn

[S36] C++：unordered_map
来源：http://eh.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://su.huixiangedu.cn

[S37] C++：set
来源：http://fy.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ij.gzmigu.cn

[S38] C++：排序
来源：http://ym.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://ks.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://np.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ya.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://af.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xr.panjiajie.cn

[S41] C++：类与构造函数
来源：http://yi.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vm.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://ps.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://ie.nicolike.cn

[S43] C++：智能指针
来源：http://al.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://mc.lnxyls.cn

[S44] C++：引用传参
来源：http://vp.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://wn.muxihuayi.cn

[S45] C++：lambda
来源：http://zh.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yx.shxzukj.cn

[S46] C++：函数模板
来源：http://vw.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://it.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://rx.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hf.gzmigu.cn

[S48] C++：逐行读文件
来源：http://in.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uf.newstarts.cn

while (std::getline(in, line)) { }
来源：http://wi.hnjuh.cn

[S49] C++：写文件
来源：http://ha.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sv.bjjhwx.cn

[S50] C++：格式化数字
来源：http://ln.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qh.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://lh.9csxet.cn

static_cast<double>(a) / b
来源：http://jv.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://fs.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://jx.szxytkj.cn

[S53] C++：移动语义
来源：http://mg.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://qy.asd995.cn

[S54] C++：异常处理
来源：http://tj.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://my.shxzskj.cn

[S55] C++：结构化绑定
来源：http://nr.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fp.newstarts.cn

[S56] C++：optional
来源：http://kn.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ir.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://wg.szxytkj.cn

constexpr int N = 10;
来源：http://aw.szsharing.cn

[S58] C++：命名空间
来源：http://xs.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://ra.hnjuh.cn

[S59] C++：静态断言
来源：http://wv.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qh.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://qn.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ll.chemitech.net.cn

================================================================================
来源：http://or.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://za.yuexingan06.cn

================================================================================
来源：http://vz.nszjky.cn

[T01] Kotlin：Hello World
来源：http://hg.bookmarksfly.cn

println("Hello")
来源：http://ct.shxzukj.cn

[T02] Kotlin：变量
来源：http://ry.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://df.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://rv.huixiangedu.cn

"值: $b"
来源：http://jm.asd995.cn

[T04] Kotlin：空安全
来源：http://nm.hahajie.cn

val n: String? = null;  n?.length
来源：http://ke.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://qh.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tf.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://rc.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uo.colortex.cn

[T07] Kotlin：集合过滤
来源：http://hq.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://an.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://as.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://rr.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://ae.asd995.cn

fun String.exclaim() = this + "!"
来源：http://md.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://ex.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fm.nicolike.cn

[T11] Kotlin：协程
来源：http://cf.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ai.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://jc.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://ef.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://om.521024.cn

val m = mapOf("a" to 1)
来源：http://vf.gzmigu.cn

[T14] Kotlin：循环
来源：http://qa.szxytkj.cn

for (i in 1..10) println(i)
来源：http://vk.huixiangedu.cn

[T15] Kotlin：接口
来源：http://zj.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://wd.shtwfgs.cn

[T16] Swift：Hello World
来源：http://kq.bookmarksfly.cn

print("Hello")
来源：http://pl.nicolike.cn

[T17] Swift：变量与常量
来源：http://za.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ak.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://oh.hnjuh.cn

"值: \(b)"
来源：http://bh.nicolike.cn

[T19] Swift：可选绑定
来源：http://il.shxzukj.cn

if let n = opt { print(n) }
来源：http://ep.yuexingan06.cn

[T20] Swift：数组操作
来源：http://dp.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gb.hahajie.cn

[T21] Swift：遍历
来源：http://tx.nicolike.cn

for x in a { print(x) }
来源：http://dx.9csxet.cn

[T22] Swift：字典
来源：http://dw.chemitech.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gm.bjjhwx.cn

[T23] Swift：函数
来源：http://ag.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sx.wgjwhj.cn

[T24] Swift：闭包
来源：http://ud.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fo.szsharing.cn


<!-- 参考信息 -->