代发 wailian999

echo "${#arr[@]}"
来源：http://ls.asd995.cn

[R20] 关联数组（字典）
来源：http://fy.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oa.hahajie.cn

[R21] 字符串长度
来源：http://tk.colortex.cn

echo "${#s}"
来源：http://js.yuexingan06.cn

[R22] 截取子串
来源：http://an.nicolike.cn

echo "${s:0:5}"
来源：http://ah.gzmigu.cn

[R23] 字符串替换
来源：http://sq.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tg.asd995.cn

[R24] 大小写转换
来源：http://pg.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xi.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://vb.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ph.shxzukj.cn

[R26] 命令替换
来源：http://dn.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://cb.huixiangedu.cn

[R27] 算术展开
来源：http://yt.521024.cn

echo $((1 + 2 * 3))
来源：http://op.yuexingan06.cn

[R28] 浮点运算
来源：http://kz.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://ij.wgjwhj.cn

[R29] 定义函数
来源：http://ms.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ai.521024.cn

[R30] 函数返回状态码
来源：http://jh.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://ge.wgjwhj.cn

[R31] 局部变量
来源：http://cb.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://nm.nicolike.cn

[R32] 参数个数校验
来源：http://nf.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mh.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://pa.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://os.jianghongdianzi.cn

[R34] 退出时清理
来源：http://le.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ke.muxihuayi.cn

[R35] 后台执行并等待
来源：http://qh.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qh.521024.cn

[R36] 并发执行多个任务
来源：http://vw.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fo.asd995.cn

[R37] 把输出赋给变量
来源：http://zi.hnjuh.cn

files=$(ls -1)
来源：http://cv.huixinmuqiang.cn

[R38] 管道串联
来源：http://tf.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://gh.panjiajie.cn

[R39] 重定向标准输出与错误
来源：http://he.panjiajie.cn

cmd > out.log 2>&1
来源：http://il.shtwfgs.cn

[R40] 追加写日志
来源：http://fi.szxytkj.cn

echo "log" >> out.log
来源：http://ou.panjiajie.cn

[R41] 丢弃输出
来源：http://mx.9csxet.cn

cmd >/dev/null 2>&1
来源：http://yp.haigaiapp.cn

[R42] 输入重定向
来源：http://kz.yuexingan06.cn

wc -l < a.txt
来源：http://ga.jctech888.com.cn

[R43] 按名字查找文件
来源：http://ld.lnxyls.cn

find . -name "*.log" -type f
来源：http://jh.nszjky.cn

[R44] 按修改时间查找
来源：http://ym.newstarts.cn

find . -mtime -7 -type f
来源：http://pf.haigaiapp.cn

[R45] 批量删除
来源：http://mm.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://aq.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://iv.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qm.nszjky.cn

[R47] sed 单行替换
来源：http://rx.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cx.panjiajie.cn

[R48] awk 取指定列
来源：http://av.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://db.colortex.cn

[R49] awk 带条件
来源：http://uk.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xz.shxzukj.cn

[R50] awk 求和
来源：http://ns.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cx.haigaiapp.cn

[R51] 排序去重取前几
来源：http://ia.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fn.huanxung.cn

[R52] 统计行数
来源：http://zc.nszjky.cn

wc -l a.txt
来源：http://qr.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://aq.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ap.chemitech.net.cn

[R54] 比较两个文件
来源：http://jj.chemitech.net.cn

diff a.txt b.txt
来源：http://ih.yuexingan06.cn

[R55] 压缩与解压
来源：http://ay.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qw.bookmarksfly.cn

[R56] 远程拷贝
来源：http://ir.nicolike.cn

scp file user@host:/path/
来源：http://yk.panjiajie.cn

[R57] 远程执行命令
来源：http://ra.shxzskj.cn

ssh user@host 'uptime'
来源：http://bz.asd995.cn

[R58] 下载文件
来源：http://sl.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://la.gzmigu.cn

[R59] 发 POST JSON
来源：http://dc.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sp.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://nq.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vl.lnxyls.cn

[R61] 磁盘占用
来源：http://zr.chemitech.net.cn

df -h;  du -sh *
来源：http://if.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://gc.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://hr.colortex.cn

[R63] 内存与进程
来源：http://zg.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://yz.9csxet.cn

[R64] 结束进程
来源：http://pz.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://bj.hnjuh.cn

[R65] 查看端口占用
来源：http://pw.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dc.haigaiapp.cn

[R66] 定时任务
来源：http://bc.hahajie.cn

crontab -e;  crontab -l
来源：http://kv.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://yk.9csxet.cn

openssl rand -hex 16
来源：http://fu.9csxet.cn

[R68] 计算文件校验值
来源：http://cn.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jf.hahajie.cn

[R69] 生成随机密码
来源：http://ey.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://lz.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://xr.nszjky.cn

date +%s;  date -d @1700000000
来源：http://zr.yuexingan06.cn

[R71] 日期格式化
来源：http://bm.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qc.shxzskj.cn

[R72] 等待端口就绪
来源：http://ih.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://su.haigaiapp.cn

[R73] 分割大日志
来源：http://no.lnxyls.cn

split -l 1000 big.log part_
来源：http://io.chemitech.net.cn

[R74] 批量重命名
来源：http://kd.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ja.gzmigu.cn

[R75] 导出环境变量
来源：http://km.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://gu.chemitech.net.cn

[R76] 使用临时文件
来源：http://lx.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qo.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ud.shxzskj.cn

read -rp "请输入: " ans
来源：http://lg.jianghongdianzi.cn

[R78] 交互式菜单
来源：http://qm.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dl.muxihuayi.cn

[R79] 解析命令行选项
来源：http://yl.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dh.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://hi.haigaiapp.cn

time ./run.sh
来源：http://wd.nicolike.cn

================================================================================
来源：http://mp.asd995.cn

S. C / C++ 专题
来源：http://ob.hahajie.cn

================================================================================
来源：http://lp.haigaiapp.cn

[S01] C：Hello World
来源：http://te.lnxyls.cn

#include <stdio.h>
来源：http://jc.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ii.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://ev.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://ud.szxytkj.cn

[S03] C：读入整数
来源：http://tl.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://ol.szxytkj.cn

[S04] C：字符串复制
来源：http://mh.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xr.colortex.cn

[S05] C：字符串长度
来源：http://xm.yuexingan06.cn

strlen(s)
来源：http://hb.hahajie.cn

[S06] C：字符串比较
来源：http://io.hahajie.cn

strcmp(a, b) == 0
来源：http://qx.szxytkj.cn

[S07] C：数组遍历求和
来源：http://dz.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rd.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://ej.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wb.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://oi.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yd.chemitech.net.cn

[S10] C：指针与解引用
来源：http://pv.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ur.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://kf.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://mb.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mt.hahajie.cn

fclose(f);
来源：http://ag.asd995.cn

[S12] C：写文件
来源：http://wx.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sg.huixiangedu.cn

[S13] C：宏定义
来源：http://kp.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oc.521024.cn

[S14] C：枚举
来源：http://gp.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://dh.bookmarksfly.cn

[S15] C：类型转换
来源：http://ke.asd995.cn

(double) a / b
来源：http://rw.newstarts.cn

[S16] C：位操作置位
来源：http://ow.bookmarksfly.cn

x |= (1 << 3);
来源：http://ti.hahajie.cn

[S17] C：安全拼接字符串
来源：http://xg.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nt.wgjwhj.cn

[S18] C：命令行参数
来源：http://fw.yuexingan06.cn

int main(int argc, char **argv)
来源：http://ge.panjiajie.cn

[S19] C：快速排序
来源：http://mf.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ov.panjiajie.cn

[S20] C：二分查找
来源：http://dk.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ha.shxzskj.cn

[S21] C：字符类别判断
来源：http://dg.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ol.9csxet.cn

[S22] C：字符串转数字
来源：http://or.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yf.shxzskj.cn

[S23] C：随机数
来源：http://xb.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tt.wgjwhj.cn

[S24] C：获取本地时间
来源：http://bt.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tg.nicolike.cn

[S25] C：内存拷贝
来源：http://lp.shxzukj.cn

memcpy(dst, src, n);
来源：http://fh.shtwfgs.cn

[S26] C：内存清零
来源：http://jq.521024.cn

memset(a, 0, sizeof a);
来源：http://lr.nicolike.cn

[S27] C：定义常量
来源：http://ix.shxzskj.cn

const double PI = 3.14159;
来源：http://yv.haigaiapp.cn

[S28] C：静态变量
来源：http://vr.nicolike.cn

static int counter = 0;
来源：http://sz.hahajie.cn

[S29] C：变参函数
来源：http://lz.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zy.shtwfgs.cn

[S30] C：头文件保护
来源：http://do.muxihuayi.cn

#ifndef X_H
来源：http://hv.bjjhwx.cn

#define X_H
来源：http://ke.colortex.cn

#endif
来源：http://uj.hahajie.cn

[S31] C++：Hello World
来源：http://jv.jianghongdianzi.cn

#include <iostream>
来源：http://di.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://xb.yuexingan06.cn

[S32] C++：字符串
来源：http://xo.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://gv.chemitech.net.cn

[S33] C++：vector 增删
来源：http://ad.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ap.nszjky.cn

[S34] C++：遍历 vector
来源：http://jc.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://bl.bookmarksfly.cn

[S35] C++：map
来源：http://bn.newstarts.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://us.huixiangedu.cn

[S36] C++：unordered_map
来源：http://pv.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://su.shxzskj.cn

[S37] C++：set
来源：http://st.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bd.yuntaijiaju.cn

[S38] C++：排序
来源：http://dg.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://rp.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://jy.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uc.szxytkj.cn

[S40] C++：查找元素
来源：http://rm.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uv.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://in.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://up.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://us.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://qx.yuexingan06.cn

[S43] C++：智能指针
来源：http://wv.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://mq.huixiangedu.cn

[S44] C++：引用传参
来源：http://cd.hahajie.cn

void inc(int &x) { ++x; }
来源：http://vr.huixinmuqiang.cn

[S45] C++：lambda
来源：http://ju.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nf.bjjhwx.cn

[S46] C++：函数模板
来源：http://zr.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fw.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://ry.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hp.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://fu.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qt.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://wp.nszjky.cn

[S49] C++：写文件
来源：http://kz.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://if.9csxet.cn

[S50] C++：格式化数字
来源：http://sy.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zw.521024.cn

[S51] C++：显式类型转换
来源：http://kl.9csxet.cn

static_cast<double>(a) / b
来源：http://hf.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://ur.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://uv.shxzskj.cn

[S53] C++：移动语义
来源：http://rx.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://mj.muxihuayi.cn

[S54] C++：异常处理
来源：http://vm.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bt.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://sp.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bu.lnxyls.cn

[S56] C++：optional
来源：http://xs.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://db.nicolike.cn

[S57] C++：编译期常量
来源：http://xz.colortex.cn

constexpr int N = 10;
来源：http://ks.huixiangedu.cn

[S58] C++：命名空间
来源：http://bs.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://gq.szsharing.cn

[S59] C++：静态断言
来源：http://cz.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://np.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://ks.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pi.huixinmuqiang.cn

================================================================================
来源：http://cy.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kc.asd995.cn

================================================================================
来源：http://aq.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://mf.nicolike.cn

println("Hello")
来源：http://nf.9csxet.cn

[T02] Kotlin：变量
来源：http://ds.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://da.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://fl.gzmigu.cn

"值: $b"
来源：http://za.newstarts.cn

[T04] Kotlin：空安全
来源：http://xh.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://rs.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://nn.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gr.nszjky.cn

[T06] Kotlin：集合映射
来源：http://ol.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xq.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://vn.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://li.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://at.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://bz.lnxyls.cn

[T09] Kotlin：扩展函数
来源：http://tm.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://qc.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://rq.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xl.hahajie.cn

[T11] Kotlin：协程
来源：http://ah.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ku.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://zt.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://go.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://it.521024.cn

val m = mapOf("a" to 1)
来源：http://hj.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://kh.newstarts.cn

for (i in 1..10) println(i)
来源：http://ov.521024.cn

[T15] Kotlin：接口
来源：http://ry.huanxung.cn

interface Shape { fun area(): Double }
来源：http://ro.nszjky.cn

[T16] Swift：Hello World
来源：http://dz.gzmigu.cn

print("Hello")
来源：http://cd.szsharing.cn

[T17] Swift：变量与常量
来源：http://yo.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://tu.lnxyls.cn

[T18] Swift：字符串插值
来源：http://pb.shtwfgs.cn

"值: \(b)"
来源：http://ll.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://wi.chemitech.net.cn

if let n = opt { print(n) }
来源：http://jt.asd995.cn

[T20] Swift：数组操作
来源：http://qq.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hv.huanxung.cn

[T21] Swift：遍历
来源：http://wn.bjjhwx.cn

for x in a { print(x) }
来源：http://qe.bjjhwx.cn

[T22] Swift：字典
来源：http://wq.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mz.gzmigu.cn


<!-- 参考信息 -->