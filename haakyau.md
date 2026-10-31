代发 wailian999

echo "${#arr[@]}"
来源：http://dj.colortex.cn

[R20] 关联数组（字典）
来源：http://uc.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fp.hnjuh.cn

[R21] 字符串长度
来源：http://mb.wgjwhj.cn

echo "${#s}"
来源：http://qs.chemitech.net.cn

[R22] 截取子串
来源：http://sr.hnjuh.cn

echo "${s:0:5}"
来源：http://rb.bjjhwx.cn

[R23] 字符串替换
来源：http://an.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://on.bookmarksfly.cn

[R24] 大小写转换
来源：http://rj.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pz.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://au.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uw.chemitech.net.cn

[R26] 命令替换
来源：http://lq.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://gk.shtwfgs.cn

[R27] 算术展开
来源：http://vu.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://rt.szxytkj.cn

[R28] 浮点运算
来源：http://cz.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://sm.9csxet.cn

[R29] 定义函数
来源：http://ts.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nc.nszjky.cn

[R30] 函数返回状态码
来源：http://ey.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://gk.yuntaijiaju.cn

[R31] 局部变量
来源：http://ym.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://hy.panjiajie.cn

[R32] 参数个数校验
来源：http://yx.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hr.asd995.cn

[R33] 捕获错误并提示行号
来源：http://zs.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ov.521024.cn

[R34] 退出时清理
来源：http://pi.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kj.colortex.cn

[R35] 后台执行并等待
来源：http://fb.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bh.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://wg.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rw.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://iy.chemitech.net.cn

files=$(ls -1)
来源：http://gg.shxzskj.cn

[R38] 管道串联
来源：http://gl.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://kl.521024.cn

[R39] 重定向标准输出与错误
来源：http://vl.jctech888.com.cn

cmd > out.log 2>&1
来源：http://tu.colortex.cn

[R40] 追加写日志
来源：http://ms.nszjky.cn

echo "log" >> out.log
来源：http://lx.panjiajie.cn

[R41] 丢弃输出
来源：http://wv.9csxet.cn

cmd >/dev/null 2>&1
来源：http://dt.shxzukj.cn

[R42] 输入重定向
来源：http://tv.yuntaijiaju.cn

wc -l < a.txt
来源：http://yo.jctech888.com.cn

[R43] 按名字查找文件
来源：http://ks.newstarts.cn

find . -name "*.log" -type f
来源：http://ta.lnxyls.cn

[R44] 按修改时间查找
来源：http://iz.shtwfgs.cn

find . -mtime -7 -type f
来源：http://lq.colortex.cn

[R45] 批量删除
来源：http://xk.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://pu.szxytkj.cn

[R46] 递归替换文件内容
来源：http://eo.nszjky.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ro.nszjky.cn

[R47] sed 单行替换
来源：http://xb.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fx.hahajie.cn

[R48] awk 取指定列
来源：http://zi.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://bf.hahajie.cn

[R49] awk 带条件
来源：http://ab.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oh.bjjhwx.cn

[R50] awk 求和
来源：http://mi.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sm.szsharing.cn

[R51] 排序去重取前几
来源：http://ti.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://op.yuntaijiaju.cn

[R52] 统计行数
来源：http://gq.szxytkj.cn

wc -l a.txt
来源：http://hl.shxzukj.cn

[R53] 查看文件头与实时尾
来源：http://ls.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ox.shxzskj.cn

[R54] 比较两个文件
来源：http://if.9csxet.cn

diff a.txt b.txt
来源：http://cc.9csxet.cn

[R55] 压缩与解压
来源：http://en.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://si.jctech888.com.cn

[R56] 远程拷贝
来源：http://fc.9csxet.cn

scp file user@host:/path/
来源：http://kx.chemitech.net.cn

[R57] 远程执行命令
来源：http://oe.huanxung.cn

ssh user@host 'uptime'
来源：http://vf.huanxung.cn

[R58] 下载文件
来源：http://th.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fz.haigaiapp.cn

[R59] 发 POST JSON
来源：http://nd.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://to.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://ds.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lk.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://mk.bjjhwx.cn

df -h;  du -sh *
来源：http://hs.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://jf.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://py.gzmigu.cn

[R63] 内存与进程
来源：http://lr.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://ys.yuexingan06.cn

[R64] 结束进程
来源：http://yy.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://kr.lnxyls.cn

[R65] 查看端口占用
来源：http://uo.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ot.shxzskj.cn

[R66] 定时任务
来源：http://ad.hahajie.cn

crontab -e;  crontab -l
来源：http://or.9csxet.cn

[R67] 生成随机十六进制串
来源：http://wa.muxihuayi.cn

openssl rand -hex 16
来源：http://cq.chemitech.net.cn

[R68] 计算文件校验值
来源：http://gh.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bf.hahajie.cn

[R69] 生成随机密码
来源：http://dv.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://fn.gzmigu.cn

[R70] 时间戳与互转
来源：http://yq.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://ap.huanxung.cn

[R71] 日期格式化
来源：http://mq.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kz.szxytkj.cn

[R72] 等待端口就绪
来源：http://zj.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mi.hnjuh.cn

[R73] 分割大日志
来源：http://gl.huanxung.cn

split -l 1000 big.log part_
来源：http://uu.shxzukj.cn

[R74] 批量重命名
来源：http://dx.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://io.9csxet.cn

[R75] 导出环境变量
来源：http://cn.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://au.muxihuayi.cn

[R76] 使用临时文件
来源：http://ju.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ig.nicolike.cn

[R77] 读取用户输入
来源：http://el.panjiajie.cn

read -rp "请输入: " ans
来源：http://xj.huixiangedu.cn

[R78] 交互式菜单
来源：http://pv.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fk.shxzskj.cn

[R79] 解析命令行选项
来源：http://jf.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vm.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://qy.huixiangedu.cn

time ./run.sh
来源：http://ny.nicolike.cn

================================================================================
来源：http://lc.hahajie.cn

S. C / C++ 专题
来源：http://wi.bjjhwx.cn

================================================================================
来源：http://vq.chemitech.net.cn

[S01] C：Hello World
来源：http://zv.yuntaijiaju.cn

#include <stdio.h>
来源：http://pt.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ty.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://dt.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://fa.nszjky.cn

[S03] C：读入整数
来源：http://gy.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://oy.nszjky.cn

[S04] C：字符串复制
来源：http://rx.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lq.szxytkj.cn

[S05] C：字符串长度
来源：http://ru.yuexingan06.cn

strlen(s)
来源：http://ss.szxytkj.cn

[S06] C：字符串比较
来源：http://df.gzmigu.cn

strcmp(a, b) == 0
来源：http://zc.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://ko.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gi.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://ag.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jx.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://ay.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ks.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://uy.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://nx.nicolike.cn

[S11] C：逐行读文件
来源：http://ua.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://tv.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qn.huanxung.cn

fclose(f);
来源：http://yd.hahajie.cn

[S12] C：写文件
来源：http://at.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lq.yuexingan06.cn

[S13] C：宏定义
来源：http://gd.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lf.shxzskj.cn

[S14] C：枚举
来源：http://px.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://ob.hahajie.cn

[S15] C：类型转换
来源：http://ky.huanxung.cn

(double) a / b
来源：http://wg.bjjhwx.cn

[S16] C：位操作置位
来源：http://jl.muxihuayi.cn

x |= (1 << 3);
来源：http://ov.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://pm.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dr.gzmigu.cn

[S18] C：命令行参数
来源：http://jj.521024.cn

int main(int argc, char **argv)
来源：http://vp.lnxyls.cn

[S19] C：快速排序
来源：http://al.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ff.shtwfgs.cn

[S20] C：二分查找
来源：http://ag.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lx.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://xt.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ys.shxzukj.cn

[S22] C：字符串转数字
来源：http://xq.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aj.9csxet.cn

[S23] C：随机数
来源：http://uy.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lr.newstarts.cn

[S24] C：获取本地时间
来源：http://qd.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rf.shxzskj.cn

[S25] C：内存拷贝
来源：http://ix.bjjhwx.cn

memcpy(dst, src, n);
来源：http://vm.colortex.cn

[S26] C：内存清零
来源：http://rq.nicolike.cn

memset(a, 0, sizeof a);
来源：http://qz.huixiangedu.cn

[S27] C：定义常量
来源：http://kk.shxzukj.cn

const double PI = 3.14159;
来源：http://jc.jctech888.com.cn

[S28] C：静态变量
来源：http://vn.jianghongdianzi.cn

static int counter = 0;
来源：http://qo.szsharing.cn

[S29] C：变参函数
来源：http://om.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ai.shxzskj.cn

[S30] C：头文件保护
来源：http://yx.shtwfgs.cn

#ifndef X_H
来源：http://iu.jctech888.com.cn

#define X_H
来源：http://rb.colortex.cn

#endif
来源：http://sh.chemitech.net.cn

[S31] C++：Hello World
来源：http://al.huixinmuqiang.cn

#include <iostream>
来源：http://wl.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://zo.huixinmuqiang.cn

[S32] C++：字符串
来源：http://eq.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://hn.nszjky.cn

[S33] C++：vector 增删
来源：http://od.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nd.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://eq.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://fr.jianghongdianzi.cn

[S35] C++：map
来源：http://eg.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vf.hahajie.cn

[S36] C++：unordered_map
来源：http://kj.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aw.wgjwhj.cn

[S37] C++：set
来源：http://yq.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rs.shtwfgs.cn

[S38] C++：排序
来源：http://hr.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://uf.shxzskj.cn

[S39] C++：自定义比较器排序
来源：http://fz.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pc.9csxet.cn

[S40] C++：查找元素
来源：http://ps.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fk.szsharing.cn

[S41] C++：类与构造函数
来源：http://qv.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eu.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://zp.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://of.lnxyls.cn

[S43] C++：智能指针
来源：http://sl.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://vp.hahajie.cn

[S44] C++：引用传参
来源：http://oi.colortex.cn

void inc(int &x) { ++x; }
来源：http://av.szsharing.cn

[S45] C++：lambda
来源：http://ya.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://po.asd995.cn

[S46] C++：函数模板
来源：http://mb.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yi.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://lx.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://se.9csxet.cn

[S48] C++：逐行读文件
来源：http://qg.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mm.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://lq.szxytkj.cn

[S49] C++：写文件
来源：http://nz.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ha.shxzskj.cn

[S50] C++：格式化数字
来源：http://mu.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ev.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://ul.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://co.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://zr.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://kf.lnxyls.cn

[S53] C++：移动语义
来源：http://tl.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://do.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://nc.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnjuh.cn

[S55] C++：结构化绑定
来源：http://ps.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dq.bookmarksfly.cn

[S56] C++：optional
来源：http://yz.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zo.jctech888.com.cn

[S57] C++：编译期常量
来源：http://zp.panjiajie.cn

constexpr int N = 10;
来源：http://ge.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://ft.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://km.lnxyls.cn

[S59] C++：静态断言
来源：http://mo.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://it.colortex.cn

[S60] C++：遍历并删除元素
来源：http://sw.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vd.huixiangedu.cn

================================================================================
来源：http://ii.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zi.huanxung.cn

================================================================================
来源：http://lg.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://jq.asd995.cn

println("Hello")
来源：http://lu.szxytkj.cn

[T02] Kotlin：变量
来源：http://bs.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oc.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://bi.bjjhwx.cn

"值: $b"
来源：http://zt.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://do.nszjky.cn

val n: String? = null;  n?.length
来源：http://od.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://mb.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vm.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://lz.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xm.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://mu.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jz.newstarts.cn

[T08] Kotlin：数据类
来源：http://gs.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://mw.521024.cn

[T09] Kotlin：扩展函数
来源：http://mp.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://yl.9csxet.cn

[T10] Kotlin：默认参数
来源：http://go.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gs.haigaiapp.cn

[T11] Kotlin：协程
来源：http://qq.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ir.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://lf.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://rz.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://md.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://hb.huanxung.cn

[T14] Kotlin：循环
来源：http://gk.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://wa.nszjky.cn

[T15] Kotlin：接口
来源：http://gz.huanxung.cn

interface Shape { fun area(): Double }
来源：http://gc.huanxung.cn

[T16] Swift：Hello World
来源：http://of.nicolike.cn

print("Hello")
来源：http://ui.shxzskj.cn

[T17] Swift：变量与常量
来源：http://sl.gzmigu.cn

var a = 1;  let b = 2
来源：http://zq.bookmarksfly.cn

[T18] Swift：字符串插值
来源：http://zh.colortex.cn

"值: \(b)"
来源：http://st.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://tm.wgjwhj.cn

if let n = opt { print(n) }
来源：http://tw.nszjky.cn

[T20] Swift：数组操作
来源：http://be.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gr.nszjky.cn

[T21] Swift：遍历
来源：http://rh.huanxung.cn

for x in a { print(x) }
来源：http://yp.huanxung.cn

[T22] Swift：字典
来源：http://ri.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://eh.yuexingan06.cn


<!-- 参考信息 -->