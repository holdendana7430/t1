代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://dq.521024.cn

[R14] C 风格 for
来源：http://rb.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jh.jctech888.com.cn

[R15] while 逐行读文件
来源：http://td.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lt.muxihuayi.cn

[R16] until 等待条件
来源：http://od.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vd.shxzskj.cn

[R17] 数组定义与取值
来源：http://fx.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jv.colortex.cn

[R18] 遍历数组
来源：http://cj.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fg.nszjky.cn

[R19] 数组长度
来源：http://yg.shxzskj.cn

echo "${#arr[@]}"
来源：http://hz.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://ne.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wh.shxzukj.cn

[R21] 字符串长度
来源：http://oz.shxzskj.cn

echo "${#s}"
来源：http://ru.yuexingan06.cn

[R22] 截取子串
来源：http://hr.nszjky.cn

echo "${s:0:5}"
来源：http://rz.shxzukj.cn

[R23] 字符串替换
来源：http://cr.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xk.asd995.cn

[R24] 大小写转换
来源：http://pa.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fp.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://cf.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kw.nicolike.cn

[R26] 命令替换
来源：http://js.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://zj.shtwfgs.cn

[R27] 算术展开
来源：http://ee.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://rp.bjjhwx.cn

[R28] 浮点运算
来源：http://dk.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://fh.shtwfgs.cn

[R29] 定义函数
来源：http://qm.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ac.colortex.cn

[R30] 函数返回状态码
来源：http://ds.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://se.jianghongdianzi.cn

[R31] 局部变量
来源：http://lx.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://jc.colortex.cn

[R32] 参数个数校验
来源：http://yo.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://on.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://wj.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bq.huanxung.cn

[R34] 退出时清理
来源：http://ot.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sm.szsharing.cn

[R35] 后台执行并等待
来源：http://rd.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://em.asd995.cn

[R36] 并发执行多个任务
来源：http://mn.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ql.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://ip.colortex.cn

files=$(ls -1)
来源：http://uh.huanxung.cn

[R38] 管道串联
来源：http://nl.hnjuh.cn

cat a.txt | grep -i error | wc -l
来源：http://pr.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://gz.hnjuh.cn

cmd > out.log 2>&1
来源：http://qz.yuntaijiaju.cn

[R40] 追加写日志
来源：http://hy.shxzskj.cn

echo "log" >> out.log
来源：http://la.szxytkj.cn

[R41] 丢弃输出
来源：http://dc.hahajie.cn

cmd >/dev/null 2>&1
来源：http://hq.wgjwhj.cn

[R42] 输入重定向
来源：http://mn.yuntaijiaju.cn

wc -l < a.txt
来源：http://xi.shxzukj.cn

[R43] 按名字查找文件
来源：http://hn.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://fn.shtwfgs.cn

[R44] 按修改时间查找
来源：http://fa.shtwfgs.cn

find . -mtime -7 -type f
来源：http://bo.chemitech.net.cn

[R45] 批量删除
来源：http://ao.9csxet.cn

find . -name "*.tmp" -delete
来源：http://vo.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://dz.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tq.colortex.cn

[R47] sed 单行替换
来源：http://nj.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sz.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://fc.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://ew.muxihuayi.cn

[R49] awk 带条件
来源：http://mk.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tj.gzmigu.cn

[R50] awk 求和
来源：http://yv.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mp.szsharing.cn

[R51] 排序去重取前几
来源：http://ax.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jr.lnxyls.cn

[R52] 统计行数
来源：http://da.chemitech.net.cn

wc -l a.txt
来源：http://aa.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://uc.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kf.shxzukj.cn

[R54] 比较两个文件
来源：http://io.nszjky.cn

diff a.txt b.txt
来源：http://wo.szxytkj.cn

[R55] 压缩与解压
来源：http://yz.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tc.hahajie.cn

[R56] 远程拷贝
来源：http://wl.yuexingan06.cn

scp file user@host:/path/
来源：http://zg.hahajie.cn

[R57] 远程执行命令
来源：http://ku.haigaiapp.cn

ssh user@host 'uptime'
来源：http://qz.jianghongdianzi.cn

[R58] 下载文件
来源：http://zr.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xn.shtwfgs.cn

[R59] 发 POST JSON
来源：http://aq.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://it.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ji.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ot.muxihuayi.cn

[R61] 磁盘占用
来源：http://zt.haigaiapp.cn

df -h;  du -sh *
来源：http://hg.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://vv.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://gp.hnjuh.cn

[R63] 内存与进程
来源：http://pi.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://uq.hnjuh.cn

[R64] 结束进程
来源：http://hn.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://pi.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://bk.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iw.huixiangedu.cn

[R66] 定时任务
来源：http://jj.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://mn.colortex.cn

[R67] 生成随机十六进制串
来源：http://ou.9csxet.cn

openssl rand -hex 16
来源：http://nq.nicolike.cn

[R68] 计算文件校验值
来源：http://fl.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dy.9csxet.cn

[R69] 生成随机密码
来源：http://wc.yuexingan06.cn

head -c 16 /dev/urandom | base64
来源：http://hb.huixiangedu.cn

[R70] 时间戳与互转
来源：http://fq.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://ev.hnjuh.cn

[R71] 日期格式化
来源：http://gp.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rf.shxzukj.cn

[R72] 等待端口就绪
来源：http://yn.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ve.newstarts.cn

[R73] 分割大日志
来源：http://gb.hahajie.cn

split -l 1000 big.log part_
来源：http://mt.yuexingan06.cn

[R74] 批量重命名
来源：http://yh.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mv.colortex.cn

[R75] 导出环境变量
来源：http://rp.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://yg.wgjwhj.cn

[R76] 使用临时文件
来源：http://lt.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fc.shtwfgs.cn

[R77] 读取用户输入
来源：http://wm.bjjhwx.cn

read -rp "请输入: " ans
来源：http://kc.chemitech.net.cn

[R78] 交互式菜单
来源：http://tu.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mi.jctech888.com.cn

[R79] 解析命令行选项
来源：http://jc.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tc.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://rx.panjiajie.cn

time ./run.sh
来源：http://pq.szxytkj.cn

================================================================================
来源：http://ia.shtwfgs.cn

S. C / C++ 专题
来源：http://mx.huixinmuqiang.cn

================================================================================
来源：http://hf.jianghongdianzi.cn

[S01] C：Hello World
来源：http://yv.bookmarksfly.cn

#include <stdio.h>
来源：http://yp.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ei.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://gq.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://kf.chemitech.net.cn

[S03] C：读入整数
来源：http://zg.szxytkj.cn

int x; scanf("%d", &x);
来源：http://ls.huanxung.cn

[S04] C：字符串复制
来源：http://ds.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gj.yuexingan06.cn

[S05] C：字符串长度
来源：http://fc.bjjhwx.cn

strlen(s)
来源：http://sv.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://wt.newstarts.cn

strcmp(a, b) == 0
来源：http://ew.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://qj.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jd.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://cy.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qt.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://ku.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hn.panjiajie.cn

[S10] C：指针与解引用
来源：http://pp.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://nw.jctech888.com.cn

[S11] C：逐行读文件
来源：http://ka.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://zo.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oc.nszjky.cn

fclose(f);
来源：http://ql.jctech888.com.cn

[S12] C：写文件
来源：http://yi.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lu.newstarts.cn

[S13] C：宏定义
来源：http://dg.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://we.bookmarksfly.cn

[S14] C：枚举
来源：http://qn.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://df.9csxet.cn

[S15] C：类型转换
来源：http://kp.muxihuayi.cn

(double) a / b
来源：http://nj.wgjwhj.cn

[S16] C：位操作置位
来源：http://lp.muxihuayi.cn

x |= (1 << 3);
来源：http://vp.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://lk.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sh.bjjhwx.cn

[S18] C：命令行参数
来源：http://gg.shtwfgs.cn

int main(int argc, char **argv)
来源：http://ks.huanxung.cn

[S19] C：快速排序
来源：http://ij.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tl.wgjwhj.cn

[S20] C：二分查找
来源：http://zo.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ou.chemitech.net.cn

[S21] C：字符类别判断
来源：http://gv.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xk.huanxung.cn

[S22] C：字符串转数字
来源：http://zw.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hahajie.cn

[S23] C：随机数
来源：http://sd.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://in.hahajie.cn

[S24] C：获取本地时间
来源：http://yx.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://me.huanxung.cn

[S25] C：内存拷贝
来源：http://zp.shxzskj.cn

memcpy(dst, src, n);
来源：http://hs.huixinmuqiang.cn

[S26] C：内存清零
来源：http://gv.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://st.nicolike.cn

[S27] C：定义常量
来源：http://se.9csxet.cn

const double PI = 3.14159;
来源：http://pe.9csxet.cn

[S28] C：静态变量
来源：http://wv.huixinmuqiang.cn

static int counter = 0;
来源：http://df.jctech888.com.cn

[S29] C：变参函数
来源：http://dw.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hk.nicolike.cn

[S30] C：头文件保护
来源：http://oo.chemitech.net.cn

#ifndef X_H
来源：http://rx.panjiajie.cn

#define X_H
来源：http://dx.hahajie.cn

#endif
来源：http://hs.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://eh.521024.cn

#include <iostream>
来源：http://ns.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://nv.nicolike.cn

[S32] C++：字符串
来源：http://io.panjiajie.cn

std::string s = "hi";  s += "!";
来源：http://fq.szsharing.cn

[S33] C++：vector 增删
来源：http://gq.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://js.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://zr.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://we.szsharing.cn

[S35] C++：map
来源：http://sf.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pu.jctech888.com.cn

[S36] C++：unordered_map
来源：http://la.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bz.bookmarksfly.cn

[S37] C++：set
来源：http://fc.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nv.panjiajie.cn

[S38] C++：排序
来源：http://ef.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://zx.colortex.cn

[S39] C++：自定义比较器排序
来源：http://ak.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oa.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://hg.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wn.9csxet.cn

[S41] C++：类与构造函数
来源：http://ps.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://el.9csxet.cn

[S42] C++：继承与虚函数
来源：http://vo.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://hm.newstarts.cn

[S43] C++：智能指针
来源：http://ox.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://pm.colortex.cn

[S44] C++：引用传参
来源：http://xq.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://kx.chemitech.net.cn

[S45] C++：lambda
来源：http://tu.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qn.wgjwhj.cn

[S46] C++：函数模板
来源：http://rt.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://md.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://wb.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qp.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://su.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pn.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://oy.wgjwhj.cn

[S49] C++：写文件
来源：http://zh.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://su.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://dt.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dq.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://og.bjjhwx.cn

static_cast<double>(a) / b
来源：http://io.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://oj.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://dd.bookmarksfly.cn

[S53] C++：移动语义
来源：http://wq.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://yq.szxytkj.cn

[S54] C++：异常处理
来源：http://xy.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wk.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://pn.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vt.521024.cn

[S56] C++：optional
来源：http://ql.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://og.9csxet.cn

[S57] C++：编译期常量
来源：http://yc.huixinmuqiang.cn

constexpr int N = 10;
来源：http://ew.hahajie.cn

[S58] C++：命名空间
来源：http://dy.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://bd.szxytkj.cn

[S59] C++：静态断言
来源：http://bm.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ud.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://eh.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rb.haigaiapp.cn

================================================================================
来源：http://oz.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lq.521024.cn

================================================================================
来源：http://pz.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://st.gzmigu.cn

println("Hello")
来源：http://cp.shtwfgs.cn

[T02] Kotlin：变量
来源：http://jl.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://um.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://mj.bookmarksfly.cn

"值: $b"
来源：http://xv.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://va.colortex.cn

val n: String? = null;  n?.length
来源：http://je.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://ep.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hv.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://wn.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ip.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://tv.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ra.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://xo.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://is.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://ut.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://cm.colortex.cn

[T10] Kotlin：默认参数
来源：http://sp.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yz.521024.cn

[T11] Kotlin：协程
来源：http://zt.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xy.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://vj.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://lf.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://zj.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://vl.521024.cn

[T14] Kotlin：循环
来源：http://tn.521024.cn

for (i in 1..10) println(i)
来源：http://ol.shtwfgs.cn

[T15] Kotlin：接口
来源：http://qo.newstarts.cn

interface Shape { fun area(): Double }
来源：http://uv.hahajie.cn

[T16] Swift：Hello World
来源：http://vp.9csxet.cn

print("Hello")
来源：http://ka.nicolike.cn


<!-- 参考信息 -->