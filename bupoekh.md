代发 wailian999

esac
来源：http://pv.521024.cn

[R12] for 遍历文件
来源：http://pi.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://it.shtwfgs.cn

[R13] for 计数循环
来源：http://tq.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://yf.shxzskj.cn

[R14] C 风格 for
来源：http://pk.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ib.hahajie.cn

[R15] while 逐行读文件
来源：http://qu.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xb.haigaiapp.cn

[R16] until 等待条件
来源：http://pf.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lm.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://xc.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zg.hahajie.cn

[R18] 遍历数组
来源：http://ge.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xq.jianghongdianzi.cn

[R19] 数组长度
来源：http://yq.gzmigu.cn

echo "${#arr[@]}"
来源：http://lx.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://cm.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hv.haigaiapp.cn

[R21] 字符串长度
来源：http://tc.shxzskj.cn

echo "${#s}"
来源：http://po.hnjuh.cn

[R22] 截取子串
来源：http://gq.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://ax.shtwfgs.cn

[R23] 字符串替换
来源：http://yy.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mq.colortex.cn

[R24] 大小写转换
来源：http://vk.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://om.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://hm.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lo.yuexingan06.cn

[R26] 命令替换
来源：http://ds.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://cc.haigaiapp.cn

[R27] 算术展开
来源：http://zn.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://uw.shxzukj.cn

[R28] 浮点运算
来源：http://tb.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://se.shxzukj.cn

[R29] 定义函数
来源：http://zk.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wt.chemitech.net.cn

[R30] 函数返回状态码
来源：http://fo.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://fw.panjiajie.cn

[R31] 局部变量
来源：http://xq.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://be.shxzskj.cn

[R32] 参数个数校验
来源：http://dl.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ka.asd995.cn

[R33] 捕获错误并提示行号
来源：http://ka.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xm.nszjky.cn

[R34] 退出时清理
来源：http://aa.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fy.huixiangedu.cn

[R35] 后台执行并等待
来源：http://dt.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yt.hnjuh.cn

[R36] 并发执行多个任务
来源：http://lw.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ec.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://gl.szsharing.cn

files=$(ls -1)
来源：http://uv.panjiajie.cn

[R38] 管道串联
来源：http://wc.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://xm.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://il.lnxyls.cn

cmd > out.log 2>&1
来源：http://qm.newstarts.cn

[R40] 追加写日志
来源：http://tu.newstarts.cn

echo "log" >> out.log
来源：http://dy.huixiangedu.cn

[R41] 丢弃输出
来源：http://is.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://wy.lnxyls.cn

[R42] 输入重定向
来源：http://jo.gzmigu.cn

wc -l < a.txt
来源：http://ue.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://aa.bjjhwx.cn

find . -name "*.log" -type f
来源：http://fs.huanxung.cn

[R44] 按修改时间查找
来源：http://uu.jctech888.com.cn

find . -mtime -7 -type f
来源：http://yk.shxzskj.cn

[R45] 批量删除
来源：http://dw.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://in.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://eg.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vy.nicolike.cn

[R47] sed 单行替换
来源：http://ee.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qj.gzmigu.cn

[R48] awk 取指定列
来源：http://tz.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://ft.muxihuayi.cn

[R49] awk 带条件
来源：http://yl.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fr.gzmigu.cn

[R50] awk 求和
来源：http://ot.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zo.521024.cn

[R51] 排序去重取前几
来源：http://ql.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bp.gzmigu.cn

[R52] 统计行数
来源：http://qi.jianghongdianzi.cn

wc -l a.txt
来源：http://ds.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://wk.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fi.newstarts.cn

[R54] 比较两个文件
来源：http://xf.jianghongdianzi.cn

diff a.txt b.txt
来源：http://pi.nszjky.cn

[R55] 压缩与解压
来源：http://kt.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wa.shxzukj.cn

[R56] 远程拷贝
来源：http://cn.bookmarksfly.cn

scp file user@host:/path/
来源：http://ep.shtwfgs.cn

[R57] 远程执行命令
来源：http://kt.shxzukj.cn

ssh user@host 'uptime'
来源：http://fz.muxihuayi.cn

[R58] 下载文件
来源：http://mo.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://id.muxihuayi.cn

[R59] 发 POST JSON
来源：http://bs.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://am.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://sa.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gd.colortex.cn

[R61] 磁盘占用
来源：http://gj.muxihuayi.cn

df -h;  du -sh *
来源：http://jj.asd995.cn

[R62] 找最占空间的文件
来源：http://gq.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://kt.9csxet.cn

[R63] 内存与进程
来源：http://yb.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://gc.bjjhwx.cn

[R64] 结束进程
来源：http://hm.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://rn.lnxyls.cn

[R65] 查看端口占用
来源：http://wl.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jb.chemitech.net.cn

[R66] 定时任务
来源：http://lq.wgjwhj.cn

crontab -e;  crontab -l
来源：http://nf.colortex.cn

[R67] 生成随机十六进制串
来源：http://qi.bookmarksfly.cn

openssl rand -hex 16
来源：http://po.jctech888.com.cn

[R68] 计算文件校验值
来源：http://uf.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gw.shxzskj.cn

[R69] 生成随机密码
来源：http://yw.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://ln.9csxet.cn

[R70] 时间戳与互转
来源：http://db.hahajie.cn

date +%s;  date -d @1700000000
来源：http://mj.chemitech.net.cn

[R71] 日期格式化
来源：http://nw.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dw.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://ad.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ng.jctech888.com.cn

[R73] 分割大日志
来源：http://hu.wgjwhj.cn

split -l 1000 big.log part_
来源：http://rw.szxytkj.cn

[R74] 批量重命名
来源：http://qy.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cg.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://py.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gc.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://nz.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://du.lnxyls.cn

[R77] 读取用户输入
来源：http://de.gzmigu.cn

read -rp "请输入: " ans
来源：http://cp.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://lb.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gt.szsharing.cn

[R79] 解析命令行选项
来源：http://lo.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xd.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://jy.colortex.cn

time ./run.sh
来源：http://eq.yuexingan06.cn

================================================================================
来源：http://dn.newstarts.cn

S. C / C++ 专题
来源：http://pq.muxihuayi.cn

================================================================================
来源：http://yk.wgjwhj.cn

[S01] C：Hello World
来源：http://pw.newstarts.cn

#include <stdio.h>
来源：http://cq.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uq.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://ah.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://hc.szsharing.cn

[S03] C：读入整数
来源：http://oc.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://yq.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://ia.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gz.nszjky.cn

[S05] C：字符串长度
来源：http://lg.bjjhwx.cn

strlen(s)
来源：http://cp.hahajie.cn

[S06] C：字符串比较
来源：http://oh.haigaiapp.cn

strcmp(a, b) == 0
来源：http://dj.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://ad.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zl.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://qo.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mg.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://te.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yl.gzmigu.cn

[S10] C：指针与解引用
来源：http://eu.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://vb.shxzskj.cn

[S11] C：逐行读文件
来源：http://zy.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://sg.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sw.yuntaijiaju.cn

fclose(f);
来源：http://ok.yuntaijiaju.cn

[S12] C：写文件
来源：http://yq.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ga.nszjky.cn

[S13] C：宏定义
来源：http://qz.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ru.colortex.cn

[S14] C：枚举
来源：http://dr.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://qz.hahajie.cn

[S15] C：类型转换
来源：http://hh.chemitech.net.cn

(double) a / b
来源：http://ov.huanxung.cn

[S16] C：位操作置位
来源：http://lm.bjjhwx.cn

x |= (1 << 3);
来源：http://ks.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://rb.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nr.hahajie.cn

[S18] C：命令行参数
来源：http://qa.9csxet.cn

int main(int argc, char **argv)
来源：http://mc.yuntaijiaju.cn

[S19] C：快速排序
来源：http://pr.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lw.muxihuayi.cn

[S20] C：二分查找
来源：http://qm.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jx.haigaiapp.cn

[S21] C：字符类别判断
来源：http://hw.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dk.shtwfgs.cn

[S22] C：字符串转数字
来源：http://nx.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eo.newstarts.cn

[S23] C：随机数
来源：http://wf.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://av.colortex.cn

[S24] C：获取本地时间
来源：http://lx.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xf.hahajie.cn

[S25] C：内存拷贝
来源：http://fb.gzmigu.cn

memcpy(dst, src, n);
来源：http://ie.haigaiapp.cn

[S26] C：内存清零
来源：http://ea.colortex.cn

memset(a, 0, sizeof a);
来源：http://ox.shtwfgs.cn

[S27] C：定义常量
来源：http://sz.jctech888.com.cn

const double PI = 3.14159;
来源：http://di.huixinmuqiang.cn

[S28] C：静态变量
来源：http://cj.bookmarksfly.cn

static int counter = 0;
来源：http://ql.yuntaijiaju.cn

[S29] C：变参函数
来源：http://jy.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pp.hnjuh.cn

[S30] C：头文件保护
来源：http://aa.9csxet.cn

#ifndef X_H
来源：http://si.panjiajie.cn

#define X_H
来源：http://ev.huixinmuqiang.cn

#endif
来源：http://df.wgjwhj.cn

[S31] C++：Hello World
来源：http://wm.lnxyls.cn

#include <iostream>
来源：http://is.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://ej.shxzskj.cn

[S32] C++：字符串
来源：http://gn.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://sp.521024.cn

[S33] C++：vector 增删
来源：http://mh.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://db.szsharing.cn

[S34] C++：遍历 vector
来源：http://yg.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://yp.shtwfgs.cn

[S35] C++：map
来源：http://dg.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wx.shxzskj.cn

[S36] C++：unordered_map
来源：http://ks.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wi.newstarts.cn

[S37] C++：set
来源：http://lo.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eb.521024.cn

[S38] C++：排序
来源：http://vt.colortex.cn

std::sort(v.begin(), v.end());
来源：http://pe.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://kn.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gd.shxzukj.cn

[S40] C++：查找元素
来源：http://rm.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jf.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://zh.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lr.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://xx.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://lf.9csxet.cn

[S43] C++：智能指针
来源：http://ik.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://dh.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://lz.nicolike.cn

void inc(int &x) { ++x; }
来源：http://ro.colortex.cn

[S45] C++：lambda
来源：http://zw.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://za.shxzukj.cn

[S46] C++：函数模板
来源：http://fn.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xd.521024.cn

[S47] C++：结构化绑定遍历
来源：http://de.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nv.huanxung.cn

[S48] C++：逐行读文件
来源：http://si.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ik.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://yk.huixiangedu.cn

[S49] C++：写文件
来源：http://bw.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nw.nicolike.cn

[S50] C++：格式化数字
来源：http://lv.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ec.panjiajie.cn

[S51] C++：显式类型转换
来源：http://yy.hahajie.cn

static_cast<double>(a) / b
来源：http://sz.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://je.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://mb.9csxet.cn

[S53] C++：移动语义
来源：http://av.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://uc.nicolike.cn

[S54] C++：异常处理
来源：http://st.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dx.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://th.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yo.yuexingan06.cn

[S56] C++：optional
来源：http://vs.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cn.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ey.hahajie.cn

constexpr int N = 10;
来源：http://wm.shtwfgs.cn

[S58] C++：命名空间
来源：http://lw.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://ag.lnxyls.cn

[S59] C++：静态断言
来源：http://zr.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ax.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://vm.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ae.huixinmuqiang.cn

================================================================================
来源：http://wf.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pg.muxihuayi.cn

================================================================================
来源：http://uw.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://ll.newstarts.cn

println("Hello")
来源：http://ya.wgjwhj.cn

[T02] Kotlin：变量
来源：http://dz.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ew.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://ct.nicolike.cn

"值: $b"
来源：http://vl.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://ha.gzmigu.cn

val n: String? = null;  n?.length
来源：http://vo.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://rk.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://df.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://rl.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pr.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://yy.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rv.nszjky.cn

[T08] Kotlin：数据类
来源：http://rz.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://hf.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://vc.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://pl.nszjky.cn

[T10] Kotlin：默认参数
来源：http://bh.521024.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ah.szsharing.cn

[T11] Kotlin：协程
来源：http://tz.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sx.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://en.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://tv.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://bb.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://ju.newstarts.cn

[T14] Kotlin：循环
来源：http://ny.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://lw.jctech888.com.cn


<!-- 参考信息 -->