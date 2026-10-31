代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gr.panjiajie.cn

[R10] 正则匹配
来源：http://kn.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ry.huanxung.cn

[R11] case 多分支
来源：http://py.lnxyls.cn

case "$1" in
来源：http://eu.panjiajie.cn

start) echo "启动" ;;
来源：http://tg.nicolike.cn

stop)  echo "停止" ;;
来源：http://er.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://fz.muxihuayi.cn

esac
来源：http://pg.newstarts.cn

[R12] for 遍历文件
来源：http://vr.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://vi.jianghongdianzi.cn

[R13] for 计数循环
来源：http://mo.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://tz.huanxung.cn

[R14] C 风格 for
来源：http://dx.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sr.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://la.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ij.yuntaijiaju.cn

[R16] until 等待条件
来源：http://sw.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ji.lnxyls.cn

[R17] 数组定义与取值
来源：http://jm.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bl.haigaiapp.cn

[R18] 遍历数组
来源：http://ha.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mx.newstarts.cn

[R19] 数组长度
来源：http://un.nszjky.cn

echo "${#arr[@]}"
来源：http://jg.shxzukj.cn

[R20] 关联数组（字典）
来源：http://jg.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oj.muxihuayi.cn

[R21] 字符串长度
来源：http://nb.shxzukj.cn

echo "${#s}"
来源：http://ic.bjjhwx.cn

[R22] 截取子串
来源：http://jl.yuexingan06.cn

echo "${s:0:5}"
来源：http://lp.yuexingan06.cn

[R23] 字符串替换
来源：http://wt.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rj.nszjky.cn

[R24] 大小写转换
来源：http://zm.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bs.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://xt.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mw.shtwfgs.cn

[R26] 命令替换
来源：http://xd.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://bj.nicolike.cn

[R27] 算术展开
来源：http://mu.newstarts.cn

echo $((1 + 2 * 3))
来源：http://ne.hahajie.cn

[R28] 浮点运算
来源：http://ye.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://dm.jctech888.com.cn

[R29] 定义函数
来源：http://bx.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ld.hnjuh.cn

[R30] 函数返回状态码
来源：http://dv.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://kc.yuntaijiaju.cn

[R31] 局部变量
来源：http://br.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://yh.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://pc.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fn.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://kd.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ez.wgjwhj.cn

[R34] 退出时清理
来源：http://ch.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dp.shtwfgs.cn

[R35] 后台执行并等待
来源：http://bw.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yi.asd995.cn

[R36] 并发执行多个任务
来源：http://fg.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rm.nicolike.cn

[R37] 把输出赋给变量
来源：http://zo.shxzskj.cn

files=$(ls -1)
来源：http://zp.haigaiapp.cn

[R38] 管道串联
来源：http://ir.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://er.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://xn.521024.cn

cmd > out.log 2>&1
来源：http://xz.yuexingan06.cn

[R40] 追加写日志
来源：http://mu.hahajie.cn

echo "log" >> out.log
来源：http://wv.chemitech.net.cn

[R41] 丢弃输出
来源：http://gd.9csxet.cn

cmd >/dev/null 2>&1
来源：http://ip.lnxyls.cn

[R42] 输入重定向
来源：http://cw.chemitech.net.cn

wc -l < a.txt
来源：http://ao.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://yx.jctech888.com.cn

find . -name "*.log" -type f
来源：http://sx.bjjhwx.cn

[R44] 按修改时间查找
来源：http://gd.hahajie.cn

find . -mtime -7 -type f
来源：http://kn.shtwfgs.cn

[R45] 批量删除
来源：http://rb.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://ja.shxzukj.cn

[R46] 递归替换文件内容
来源：http://eq.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lt.huixiangedu.cn

[R47] sed 单行替换
来源：http://nj.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jk.wgjwhj.cn

[R48] awk 取指定列
来源：http://io.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://mj.wgjwhj.cn

[R49] awk 带条件
来源：http://mv.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gf.chemitech.net.cn

[R50] awk 求和
来源：http://hv.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ox.newstarts.cn

[R51] 排序去重取前几
来源：http://kx.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ch.hahajie.cn

[R52] 统计行数
来源：http://we.asd995.cn

wc -l a.txt
来源：http://pl.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://sh.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vc.szsharing.cn

[R54] 比较两个文件
来源：http://bs.jianghongdianzi.cn

diff a.txt b.txt
来源：http://qo.chemitech.net.cn

[R55] 压缩与解压
来源：http://jq.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cy.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://vi.chemitech.net.cn

scp file user@host:/path/
来源：http://xz.hahajie.cn

[R57] 远程执行命令
来源：http://qw.nicolike.cn

ssh user@host 'uptime'
来源：http://vg.hnjuh.cn

[R58] 下载文件
来源：http://rv.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fd.hnjuh.cn

[R59] 发 POST JSON
来源：http://eg.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tn.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://xh.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rk.521024.cn

[R61] 磁盘占用
来源：http://jf.gzmigu.cn

df -h;  du -sh *
来源：http://th.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://px.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://lq.yuntaijiaju.cn

[R63] 内存与进程
来源：http://mq.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://jw.asd995.cn

[R64] 结束进程
来源：http://te.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://kr.shtwfgs.cn

[R65] 查看端口占用
来源：http://yd.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ky.colortex.cn

[R66] 定时任务
来源：http://aq.9csxet.cn

crontab -e;  crontab -l
来源：http://oz.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://ez.shtwfgs.cn

openssl rand -hex 16
来源：http://cw.nszjky.cn

[R68] 计算文件校验值
来源：http://gy.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bw.shxzukj.cn

[R69] 生成随机密码
来源：http://np.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ia.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://bi.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://bz.nszjky.cn

[R71] 日期格式化
来源：http://cp.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://so.shxzskj.cn

[R72] 等待端口就绪
来源：http://zs.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ut.haigaiapp.cn

[R73] 分割大日志
来源：http://uz.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://cm.bookmarksfly.cn

[R74] 批量重命名
来源：http://ld.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vb.lnxyls.cn

[R75] 导出环境变量
来源：http://ia.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://rv.haigaiapp.cn

[R76] 使用临时文件
来源：http://kt.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cu.hnjuh.cn

[R77] 读取用户输入
来源：http://ez.shxzukj.cn

read -rp "请输入: " ans
来源：http://lm.shxzskj.cn

[R78] 交互式菜单
来源：http://tf.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jv.yuexingan06.cn

[R79] 解析命令行选项
来源：http://qk.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dz.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://oy.hnjuh.cn

time ./run.sh
来源：http://ps.newstarts.cn

================================================================================
来源：http://uc.shxzukj.cn

S. C / C++ 专题
来源：http://jy.wgjwhj.cn

================================================================================
来源：http://zq.colortex.cn

[S01] C：Hello World
来源：http://au.huixinmuqiang.cn

#include <stdio.h>
来源：http://cv.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yb.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://ap.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://vm.nszjky.cn

[S03] C：读入整数
来源：http://oa.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://xb.521024.cn

[S04] C：字符串复制
来源：http://aw.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lm.huanxung.cn

[S05] C：字符串长度
来源：http://iq.panjiajie.cn

strlen(s)
来源：http://vb.hahajie.cn

[S06] C：字符串比较
来源：http://zj.szsharing.cn

strcmp(a, b) == 0
来源：http://yr.newstarts.cn

[S07] C：数组遍历求和
来源：http://zp.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fq.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://be.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yu.asd995.cn

[S09] C：结构体定义与初始化
来源：http://ry.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ub.9csxet.cn

[S10] C：指针与解引用
来源：http://cx.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://tz.newstarts.cn

[S11] C：逐行读文件
来源：http://om.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://qz.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ns.huixiangedu.cn

fclose(f);
来源：http://en.panjiajie.cn

[S12] C：写文件
来源：http://ih.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gf.nicolike.cn

[S13] C：宏定义
来源：http://hk.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fm.wgjwhj.cn

[S14] C：枚举
来源：http://xb.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://gd.szsharing.cn

[S15] C：类型转换
来源：http://nm.jctech888.com.cn

(double) a / b
来源：http://tc.jctech888.com.cn

[S16] C：位操作置位
来源：http://bu.shxzskj.cn

x |= (1 << 3);
来源：http://om.hahajie.cn

[S17] C：安全拼接字符串
来源：http://qu.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mc.521024.cn

[S18] C：命令行参数
来源：http://je.wgjwhj.cn

int main(int argc, char **argv)
来源：http://fu.wgjwhj.cn

[S19] C：快速排序
来源：http://vk.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gt.asd995.cn

[S20] C：二分查找
来源：http://pj.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uk.haigaiapp.cn

[S21] C：字符类别判断
来源：http://tm.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://du.szxytkj.cn

[S22] C：字符串转数字
来源：http://en.hahajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hw.szsharing.cn

[S23] C：随机数
来源：http://jd.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oj.chemitech.net.cn

[S24] C：获取本地时间
来源：http://bb.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mx.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://uv.yuexingan06.cn

memcpy(dst, src, n);
来源：http://nu.haigaiapp.cn

[S26] C：内存清零
来源：http://xq.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://jj.hahajie.cn

[S27] C：定义常量
来源：http://hc.szxytkj.cn

const double PI = 3.14159;
来源：http://zx.bookmarksfly.cn

[S28] C：静态变量
来源：http://ei.nicolike.cn

static int counter = 0;
来源：http://xm.huanxung.cn

[S29] C：变参函数
来源：http://ri.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hs.bjjhwx.cn

[S30] C：头文件保护
来源：http://tb.colortex.cn

#ifndef X_H
来源：http://ma.shtwfgs.cn

#define X_H
来源：http://cj.9csxet.cn

#endif
来源：http://yk.gzmigu.cn

[S31] C++：Hello World
来源：http://cy.nszjky.cn

#include <iostream>
来源：http://sf.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://te.lnxyls.cn

[S32] C++：字符串
来源：http://su.521024.cn

std::string s = "hi";  s += "!";
来源：http://ib.newstarts.cn

[S33] C++：vector 增删
来源：http://sj.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vq.asd995.cn

[S34] C++：遍历 vector
来源：http://jl.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://yz.hnjuh.cn

[S35] C++：map
来源：http://uj.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vh.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://no.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hi.bjjhwx.cn

[S37] C++：set
来源：http://mv.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://el.gzmigu.cn

[S38] C++：排序
来源：http://dq.asd995.cn

std::sort(v.begin(), v.end());
来源：http://oe.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://jp.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ph.huixiangedu.cn

[S40] C++：查找元素
来源：http://vd.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dj.szsharing.cn

[S41] C++：类与构造函数
来源：http://ic.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ua.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://qz.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://aq.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://cu.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://du.shxzskj.cn

[S44] C++：引用传参
来源：http://ue.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://jv.9csxet.cn

[S45] C++：lambda
来源：http://df.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fn.lnxyls.cn

[S46] C++：函数模板
来源：http://ks.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rb.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://nt.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ey.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://bk.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bx.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://rb.hnjuh.cn

[S49] C++：写文件
来源：http://zk.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cp.shxzskj.cn

[S50] C++：格式化数字
来源：http://tt.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nh.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://af.shxzukj.cn

static_cast<double>(a) / b
来源：http://oe.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://gf.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://ns.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://rn.asd995.cn

std::vector<int> w = std::move(v);
来源：http://ab.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://ws.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://db.nicolike.cn

[S55] C++：结构化绑定
来源：http://tg.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wg.huixiangedu.cn

[S56] C++：optional
来源：http://vk.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wk.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://oa.wgjwhj.cn

constexpr int N = 10;
来源：http://oj.gzmigu.cn

[S58] C++：命名空间
来源：http://ej.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://gb.gzmigu.cn

[S59] C++：静态断言
来源：http://fh.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ni.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://gs.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rm.gzmigu.cn

================================================================================
来源：http://na.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ud.9csxet.cn

================================================================================
来源：http://ib.newstarts.cn

[T01] Kotlin：Hello World
来源：http://hx.shxzskj.cn

println("Hello")
来源：http://ca.bjjhwx.cn

[T02] Kotlin：变量
来源：http://wc.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rs.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://ep.shxzskj.cn

"值: $b"
来源：http://ct.hahajie.cn

[T04] Kotlin：空安全
来源：http://tx.shxzskj.cn

val n: String? = null;  n?.length
来源：http://ew.521024.cn

[T05] Kotlin：when 表达式
来源：http://yd.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://va.newstarts.cn

[T06] Kotlin：集合映射
来源：http://ob.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bp.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://pd.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qp.colortex.cn

[T08] Kotlin：数据类
来源：http://yt.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://ko.asd995.cn

[T09] Kotlin：扩展函数
来源：http://bb.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://yd.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://ri.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://at.huixiangedu.cn


<!-- 参考信息 -->