代发 wailian999

case "$1" in
来源：http://bf.9csxet.cn

start) echo "启动" ;;
来源：http://by.hahajie.cn

stop)  echo "停止" ;;
来源：http://bv.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://ti.bjjhwx.cn

esac
来源：http://oe.szsharing.cn

[R12] for 遍历文件
来源：http://tx.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://be.bookmarksfly.cn

[R13] for 计数循环
来源：http://ty.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://pp.shxzukj.cn

[R14] C 风格 for
来源：http://fy.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ak.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://ni.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qk.muxihuayi.cn

[R16] until 等待条件
来源：http://iq.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ju.9csxet.cn

[R17] 数组定义与取值
来源：http://ha.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jd.shxzukj.cn

[R18] 遍历数组
来源：http://as.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sq.gzmigu.cn

[R19] 数组长度
来源：http://rp.nicolike.cn

echo "${#arr[@]}"
来源：http://pp.hahajie.cn

[R20] 关联数组（字典）
来源：http://dh.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ed.jctech888.com.cn

[R21] 字符串长度
来源：http://gs.szxytkj.cn

echo "${#s}"
来源：http://lp.colortex.cn

[R22] 截取子串
来源：http://pu.shxzukj.cn

echo "${s:0:5}"
来源：http://au.colortex.cn

[R23] 字符串替换
来源：http://dc.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dh.panjiajie.cn

[R24] 大小写转换
来源：http://pg.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iw.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://lq.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rw.shxzskj.cn

[R26] 命令替换
来源：http://gm.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://fe.hahajie.cn

[R27] 算术展开
来源：http://rq.521024.cn

echo $((1 + 2 * 3))
来源：http://cd.shxzukj.cn

[R28] 浮点运算
来源：http://jz.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://uw.yuexingan06.cn

[R29] 定义函数
来源：http://vi.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xm.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://ls.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://oz.hahajie.cn

[R31] 局部变量
来源：http://da.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://bs.hahajie.cn

[R32] 参数个数校验
来源：http://ka.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zc.colortex.cn

[R33] 捕获错误并提示行号
来源：http://ss.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ak.gzmigu.cn

[R34] 退出时清理
来源：http://vy.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cz.jctech888.com.cn

[R35] 后台执行并等待
来源：http://mb.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rc.521024.cn

[R36] 并发执行多个任务
来源：http://sx.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kp.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://km.asd995.cn

files=$(ls -1)
来源：http://lh.nicolike.cn

[R38] 管道串联
来源：http://gl.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://sh.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://sk.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://mi.hahajie.cn

[R40] 追加写日志
来源：http://qs.huanxung.cn

echo "log" >> out.log
来源：http://ea.chemitech.net.cn

[R41] 丢弃输出
来源：http://iv.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://nu.huixiangedu.cn

[R42] 输入重定向
来源：http://hf.huixiangedu.cn

wc -l < a.txt
来源：http://od.shxzukj.cn

[R43] 按名字查找文件
来源：http://xk.yuexingan06.cn

find . -name "*.log" -type f
来源：http://sj.shxzukj.cn

[R44] 按修改时间查找
来源：http://pi.nicolike.cn

find . -mtime -7 -type f
来源：http://ud.huixiangedu.cn

[R45] 批量删除
来源：http://ug.nicolike.cn

find . -name "*.tmp" -delete
来源：http://rl.nicolike.cn

[R46] 递归替换文件内容
来源：http://qe.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ix.jctech888.com.cn

[R47] sed 单行替换
来源：http://ff.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tr.nicolike.cn

[R48] awk 取指定列
来源：http://md.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://nz.hnjuh.cn

[R49] awk 带条件
来源：http://os.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ja.muxihuayi.cn

[R50] awk 求和
来源：http://cx.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kl.bjjhwx.cn

[R51] 排序去重取前几
来源：http://mq.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dw.szsharing.cn

[R52] 统计行数
来源：http://sd.bjjhwx.cn

wc -l a.txt
来源：http://lp.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://bi.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vr.hnjuh.cn

[R54] 比较两个文件
来源：http://cr.yuntaijiaju.cn

diff a.txt b.txt
来源：http://yv.9csxet.cn

[R55] 压缩与解压
来源：http://zz.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kh.shxzskj.cn

[R56] 远程拷贝
来源：http://dt.gzmigu.cn

scp file user@host:/path/
来源：http://yj.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://dg.shxzukj.cn

ssh user@host 'uptime'
来源：http://ly.hahajie.cn

[R58] 下载文件
来源：http://mq.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mw.shtwfgs.cn

[R59] 发 POST JSON
来源：http://hg.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://le.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://ea.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ph.jctech888.com.cn

[R61] 磁盘占用
来源：http://go.wgjwhj.cn

df -h;  du -sh *
来源：http://fa.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://jb.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ib.yuexingan06.cn

[R63] 内存与进程
来源：http://mw.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://wp.shtwfgs.cn

[R64] 结束进程
来源：http://kl.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://lu.jctech888.com.cn

[R65] 查看端口占用
来源：http://xv.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ku.jianghongdianzi.cn

[R66] 定时任务
来源：http://qg.nicolike.cn

crontab -e;  crontab -l
来源：http://tf.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://tq.newstarts.cn

openssl rand -hex 16
来源：http://sl.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://cp.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jh.shtwfgs.cn

[R69] 生成随机密码
来源：http://sw.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://if.haigaiapp.cn

[R70] 时间戳与互转
来源：http://il.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://pa.colortex.cn

[R71] 日期格式化
来源：http://vh.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xk.gzmigu.cn

[R72] 等待端口就绪
来源：http://ku.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xs.shxzskj.cn

[R73] 分割大日志
来源：http://ft.9csxet.cn

split -l 1000 big.log part_
来源：http://jp.lnxyls.cn

[R74] 批量重命名
来源：http://et.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fz.bjjhwx.cn

[R75] 导出环境变量
来源：http://fz.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://ss.bookmarksfly.cn

[R76] 使用临时文件
来源：http://aq.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zf.huixiangedu.cn

[R77] 读取用户输入
来源：http://wa.521024.cn

read -rp "请输入: " ans
来源：http://ij.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://ay.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uc.huixiangedu.cn

[R79] 解析命令行选项
来源：http://is.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jz.asd995.cn

[R80] 查看脚本执行耗时
来源：http://jy.panjiajie.cn

time ./run.sh
来源：http://yx.shxzskj.cn

================================================================================
来源：http://uf.jianghongdianzi.cn

S. C / C++ 专题
来源：http://di.hnjuh.cn

================================================================================
来源：http://rh.muxihuayi.cn

[S01] C：Hello World
来源：http://zc.huanxung.cn

#include <stdio.h>
来源：http://lf.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://op.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://kh.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://bm.gzmigu.cn

[S03] C：读入整数
来源：http://di.colortex.cn

int x; scanf("%d", &x);
来源：http://mt.bjjhwx.cn

[S04] C：字符串复制
来源：http://oc.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://py.nicolike.cn

[S05] C：字符串长度
来源：http://hl.shxzskj.cn

strlen(s)
来源：http://ri.bjjhwx.cn

[S06] C：字符串比较
来源：http://kw.gzmigu.cn

strcmp(a, b) == 0
来源：http://jk.colortex.cn

[S07] C：数组遍历求和
来源：http://dy.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ds.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://tu.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ws.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://yd.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://al.huanxung.cn

[S10] C：指针与解引用
来源：http://qq.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://ng.yuexingan06.cn

[S11] C：逐行读文件
来源：http://au.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://rs.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nq.yuexingan06.cn

fclose(f);
来源：http://dt.shxzukj.cn

[S12] C：写文件
来源：http://lv.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gm.jianghongdianzi.cn

[S13] C：宏定义
来源：http://db.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rl.shxzskj.cn

[S14] C：枚举
来源：http://ie.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://of.hnjuh.cn

[S15] C：类型转换
来源：http://pf.yuntaijiaju.cn

(double) a / b
来源：http://oy.521024.cn

[S16] C：位操作置位
来源：http://nw.hnjuh.cn

x |= (1 << 3);
来源：http://xr.hahajie.cn

[S17] C：安全拼接字符串
来源：http://le.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xm.gzmigu.cn

[S18] C：命令行参数
来源：http://oz.lnxyls.cn

int main(int argc, char **argv)
来源：http://ld.nicolike.cn

[S19] C：快速排序
来源：http://yr.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xh.asd995.cn

[S20] C：二分查找
来源：http://dm.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ty.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://tr.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rw.nicolike.cn

[S22] C：字符串转数字
来源：http://vt.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gw.panjiajie.cn

[S23] C：随机数
来源：http://bv.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pm.lnxyls.cn

[S24] C：获取本地时间
来源：http://nk.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kk.nszjky.cn

[S25] C：内存拷贝
来源：http://pq.huixiangedu.cn

memcpy(dst, src, n);
来源：http://lc.lnxyls.cn

[S26] C：内存清零
来源：http://cn.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://wa.521024.cn

[S27] C：定义常量
来源：http://go.nicolike.cn

const double PI = 3.14159;
来源：http://jb.szxytkj.cn

[S28] C：静态变量
来源：http://jd.huixinmuqiang.cn

static int counter = 0;
来源：http://rk.bjjhwx.cn

[S29] C：变参函数
来源：http://ox.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tc.jctech888.com.cn

[S30] C：头文件保护
来源：http://du.colortex.cn

#ifndef X_H
来源：http://zf.shtwfgs.cn

#define X_H
来源：http://mh.shxzukj.cn

#endif
来源：http://sr.shxzskj.cn

[S31] C++：Hello World
来源：http://xi.yuntaijiaju.cn

#include <iostream>
来源：http://wi.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://hs.shxzukj.cn

[S32] C++：字符串
来源：http://le.521024.cn

std::string s = "hi";  s += "!";
来源：http://fk.hnjuh.cn

[S33] C++：vector 增删
来源：http://iw.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hq.gzmigu.cn

[S34] C++：遍历 vector
来源：http://tf.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://lk.panjiajie.cn

[S35] C++：map
来源：http://jr.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rf.bjjhwx.cn

[S36] C++：unordered_map
来源：http://sz.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vd.nicolike.cn

[S37] C++：set
来源：http://as.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vn.hahajie.cn

[S38] C++：排序
来源：http://sz.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://mg.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://ty.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jq.muxihuayi.cn

[S40] C++：查找元素
来源：http://uj.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vg.hahajie.cn

[S41] C++：类与构造函数
来源：http://zz.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zb.9csxet.cn

[S42] C++：继承与虚函数
来源：http://vi.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://ae.bookmarksfly.cn

[S43] C++：智能指针
来源：http://tq.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://ye.nszjky.cn

[S44] C++：引用传参
来源：http://mb.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://bb.bjjhwx.cn

[S45] C++：lambda
来源：http://gg.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wb.bookmarksfly.cn

[S46] C++：函数模板
来源：http://no.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://li.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://vx.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tx.nicolike.cn

[S48] C++：逐行读文件
来源：http://le.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gu.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ad.huixiangedu.cn

[S49] C++：写文件
来源：http://mf.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bg.shxzukj.cn

[S50] C++：格式化数字
来源：http://jf.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jd.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://fw.panjiajie.cn

static_cast<double>(a) / b
来源：http://ao.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://ck.521024.cn

int size() const noexcept { return n_; }
来源：http://vn.huanxung.cn

[S53] C++：移动语义
来源：http://pt.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://hz.nszjky.cn

[S54] C++：异常处理
来源：http://bf.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yx.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://tv.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qo.szsharing.cn

[S56] C++：optional
来源：http://bl.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qa.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://sh.yuntaijiaju.cn

constexpr int N = 10;
来源：http://ep.gzmigu.cn

[S58] C++：命名空间
来源：http://ok.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://vy.huanxung.cn

[S59] C++：静态断言
来源：http://aq.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hd.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://yn.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qo.bjjhwx.cn

================================================================================
来源：http://al.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ty.asd995.cn

================================================================================
来源：http://sg.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://wv.haigaiapp.cn

println("Hello")
来源：http://ip.wgjwhj.cn

[T02] Kotlin：变量
来源：http://og.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wo.521024.cn

[T03] Kotlin：字符串模板
来源：http://tx.521024.cn

"值: $b"
来源：http://ve.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://sc.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://ri.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://ac.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nk.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ox.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lp.colortex.cn

[T07] Kotlin：集合过滤
来源：http://jj.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tx.newstarts.cn

[T08] Kotlin：数据类
来源：http://ec.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://xu.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://du.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://jl.huanxung.cn

[T10] Kotlin：默认参数
来源：http://lc.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zd.colortex.cn

[T11] Kotlin：协程
来源：http://xg.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ml.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://nd.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://ed.szsharing.cn


<!-- 参考信息 -->