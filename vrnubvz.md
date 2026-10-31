代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qh.huixiangedu.cn

[R10] 正则匹配
来源：http://me.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ji.yuntaijiaju.cn

[R11] case 多分支
来源：http://hx.shxzukj.cn

case "$1" in
来源：http://jo.huanxung.cn

start) echo "启动" ;;
来源：http://qc.szsharing.cn

stop)  echo "停止" ;;
来源：http://dd.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://fb.asd995.cn

esac
来源：http://ps.jctech888.com.cn

[R12] for 遍历文件
来源：http://xv.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://gz.yuexingan06.cn

[R13] for 计数循环
来源：http://ok.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://jw.yuntaijiaju.cn

[R14] C 风格 for
来源：http://og.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ch.wgjwhj.cn

[R15] while 逐行读文件
来源：http://he.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pq.shxzskj.cn

[R16] until 等待条件
来源：http://um.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://re.muxihuayi.cn

[R17] 数组定义与取值
来源：http://jf.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jp.chemitech.net.cn

[R18] 遍历数组
来源：http://wa.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cj.lnxyls.cn

[R19] 数组长度
来源：http://fl.gzmigu.cn

echo "${#arr[@]}"
来源：http://ad.huanxung.cn

[R20] 关联数组（字典）
来源：http://lg.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sg.panjiajie.cn

[R21] 字符串长度
来源：http://sb.huanxung.cn

echo "${#s}"
来源：http://rf.lnxyls.cn

[R22] 截取子串
来源：http://ha.panjiajie.cn

echo "${s:0:5}"
来源：http://tf.huixinmuqiang.cn

[R23] 字符串替换
来源：http://ks.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hv.521024.cn

[R24] 大小写转换
来源：http://hk.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mk.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://pa.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sg.newstarts.cn

[R26] 命令替换
来源：http://rf.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://po.nicolike.cn

[R27] 算术展开
来源：http://sh.nicolike.cn

echo $((1 + 2 * 3))
来源：http://nj.521024.cn

[R28] 浮点运算
来源：http://jb.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://is.asd995.cn

[R29] 定义函数
来源：http://rf.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ar.gzmigu.cn

[R30] 函数返回状态码
来源：http://ga.wgjwhj.cn

f() { return 0; }; f || echo "失败了"
来源：http://tt.huanxung.cn

[R31] 局部变量
来源：http://vg.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://jr.shxzskj.cn

[R32] 参数个数校验
来源：http://mz.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mn.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://qg.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lh.521024.cn

[R34] 退出时清理
来源：http://ju.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xa.muxihuayi.cn

[R35] 后台执行并等待
来源：http://wq.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jb.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://zz.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tx.newstarts.cn

[R37] 把输出赋给变量
来源：http://mm.9csxet.cn

files=$(ls -1)
来源：http://ze.muxihuayi.cn

[R38] 管道串联
来源：http://cu.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://mz.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://ri.colortex.cn

cmd > out.log 2>&1
来源：http://rl.newstarts.cn

[R40] 追加写日志
来源：http://hq.colortex.cn

echo "log" >> out.log
来源：http://mv.shxzukj.cn

[R41] 丢弃输出
来源：http://ws.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://ln.shxzukj.cn

[R42] 输入重定向
来源：http://dy.nszjky.cn

wc -l < a.txt
来源：http://bi.szxytkj.cn

[R43] 按名字查找文件
来源：http://mi.yuexingan06.cn

find . -name "*.log" -type f
来源：http://mz.wgjwhj.cn

[R44] 按修改时间查找
来源：http://vo.hahajie.cn

find . -mtime -7 -type f
来源：http://fo.521024.cn

[R45] 批量删除
来源：http://uv.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://uf.521024.cn

[R46] 递归替换文件内容
来源：http://ga.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sq.shxzskj.cn

[R47] sed 单行替换
来源：http://bz.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ke.nszjky.cn

[R48] awk 取指定列
来源：http://tt.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://iz.521024.cn

[R49] awk 带条件
来源：http://wy.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qt.colortex.cn

[R50] awk 求和
来源：http://dc.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sn.wgjwhj.cn

[R51] 排序去重取前几
来源：http://pk.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oy.huixinmuqiang.cn

[R52] 统计行数
来源：http://ud.newstarts.cn

wc -l a.txt
来源：http://ad.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://xl.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dd.gzmigu.cn

[R54] 比较两个文件
来源：http://zy.newstarts.cn

diff a.txt b.txt
来源：http://fl.bjjhwx.cn

[R55] 压缩与解压
来源：http://pf.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bx.9csxet.cn

[R56] 远程拷贝
来源：http://lm.huixiangedu.cn

scp file user@host:/path/
来源：http://ac.newstarts.cn

[R57] 远程执行命令
来源：http://bz.jctech888.com.cn

ssh user@host 'uptime'
来源：http://cr.huanxung.cn

[R58] 下载文件
来源：http://xm.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kc.gzmigu.cn

[R59] 发 POST JSON
来源：http://nm.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uy.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://cn.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ld.nicolike.cn

[R61] 磁盘占用
来源：http://qn.9csxet.cn

df -h;  du -sh *
来源：http://zt.hahajie.cn

[R62] 找最占空间的文件
来源：http://ju.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://mj.newstarts.cn

[R63] 内存与进程
来源：http://ex.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://ev.shxzukj.cn

[R64] 结束进程
来源：http://iv.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://se.9csxet.cn

[R65] 查看端口占用
来源：http://nf.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kp.huixiangedu.cn

[R66] 定时任务
来源：http://cp.jctech888.com.cn

crontab -e;  crontab -l
来源：http://mm.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://wo.bookmarksfly.cn

openssl rand -hex 16
来源：http://js.hahajie.cn

[R68] 计算文件校验值
来源：http://xo.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ku.panjiajie.cn

[R69] 生成随机密码
来源：http://mo.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://st.nicolike.cn

[R70] 时间戳与互转
来源：http://nb.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://sm.bjjhwx.cn

[R71] 日期格式化
来源：http://zc.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://im.huanxung.cn

[R72] 等待端口就绪
来源：http://zn.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://po.gzmigu.cn

[R73] 分割大日志
来源：http://op.huixiangedu.cn

split -l 1000 big.log part_
来源：http://re.szsharing.cn

[R74] 批量重命名
来源：http://zh.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ba.shtwfgs.cn

[R75] 导出环境变量
来源：http://rk.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://pl.szsharing.cn

[R76] 使用临时文件
来源：http://qg.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rw.nicolike.cn

[R77] 读取用户输入
来源：http://bi.hahajie.cn

read -rp "请输入: " ans
来源：http://zv.9csxet.cn

[R78] 交互式菜单
来源：http://fy.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ol.hahajie.cn

[R79] 解析命令行选项
来源：http://aj.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vc.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://sb.huanxung.cn

time ./run.sh
来源：http://ps.hnjuh.cn

================================================================================
来源：http://fa.bookmarksfly.cn

S. C / C++ 专题
来源：http://na.panjiajie.cn

================================================================================
来源：http://in.lnxyls.cn

[S01] C：Hello World
来源：http://yw.shxzukj.cn

#include <stdio.h>
来源：http://bq.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qg.colortex.cn

[S02] C：变量与格式化输出
来源：http://an.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://wl.521024.cn

[S03] C：读入整数
来源：http://th.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://zk.huixiangedu.cn

[S04] C：字符串复制
来源：http://cr.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zz.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://gw.lnxyls.cn

strlen(s)
来源：http://cu.bookmarksfly.cn

[S06] C：字符串比较
来源：http://kk.chemitech.net.cn

strcmp(a, b) == 0
来源：http://qr.nszjky.cn

[S07] C：数组遍历求和
来源：http://ve.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ae.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://zv.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jj.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://qr.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kl.colortex.cn

[S10] C：指针与解引用
来源：http://zv.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://ex.shxzukj.cn

[S11] C：逐行读文件
来源：http://gz.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://sm.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ca.szsharing.cn

fclose(f);
来源：http://js.gzmigu.cn

[S12] C：写文件
来源：http://oz.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ai.jianghongdianzi.cn

[S13] C：宏定义
来源：http://qt.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lb.shtwfgs.cn

[S14] C：枚举
来源：http://dg.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://xv.shxzukj.cn

[S15] C：类型转换
来源：http://dh.bookmarksfly.cn

(double) a / b
来源：http://ih.nicolike.cn

[S16] C：位操作置位
来源：http://an.yuntaijiaju.cn

x |= (1 << 3);
来源：http://ib.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://kr.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tz.huixiangedu.cn

[S18] C：命令行参数
来源：http://iy.shtwfgs.cn

int main(int argc, char **argv)
来源：http://au.yuntaijiaju.cn

[S19] C：快速排序
来源：http://ci.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kc.hahajie.cn

[S20] C：二分查找
来源：http://sw.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xy.nicolike.cn

[S21] C：字符类别判断
来源：http://ll.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kj.wgjwhj.cn

[S22] C：字符串转数字
来源：http://mr.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://co.nszjky.cn

[S23] C：随机数
来源：http://ub.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ci.yuexingan06.cn

[S24] C：获取本地时间
来源：http://no.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ry.nicolike.cn

[S25] C：内存拷贝
来源：http://nt.521024.cn

memcpy(dst, src, n);
来源：http://lf.yuntaijiaju.cn

[S26] C：内存清零
来源：http://bt.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://br.shtwfgs.cn

[S27] C：定义常量
来源：http://so.asd995.cn

const double PI = 3.14159;
来源：http://ml.jianghongdianzi.cn

[S28] C：静态变量
来源：http://hx.shxzukj.cn

static int counter = 0;
来源：http://hh.szxytkj.cn

[S29] C：变参函数
来源：http://si.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tw.521024.cn

[S30] C：头文件保护
来源：http://jr.9csxet.cn

#ifndef X_H
来源：http://hr.gzmigu.cn

#define X_H
来源：http://ll.jianghongdianzi.cn

#endif
来源：http://rb.asd995.cn

[S31] C++：Hello World
来源：http://bl.hnjuh.cn

#include <iostream>
来源：http://qc.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://pn.huixiangedu.cn

[S32] C++：字符串
来源：http://dt.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://kb.muxihuayi.cn

[S33] C++：vector 增删
来源：http://os.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wn.newstarts.cn

[S34] C++：遍历 vector
来源：http://hl.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://xk.hahajie.cn

[S35] C++：map
来源：http://qz.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eh.muxihuayi.cn

[S36] C++：unordered_map
来源：http://ma.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dl.nicolike.cn

[S37] C++：set
来源：http://yt.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vr.szxytkj.cn

[S38] C++：排序
来源：http://ki.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://gt.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://he.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rr.haigaiapp.cn

[S40] C++：查找元素
来源：http://fi.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xq.hnjuh.cn

[S41] C++：类与构造函数
来源：http://by.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wa.9csxet.cn

[S42] C++：继承与虚函数
来源：http://bz.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://yp.asd995.cn

[S43] C++：智能指针
来源：http://at.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://oh.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ts.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ib.nicolike.cn

[S45] C++：lambda
来源：http://ht.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ac.9csxet.cn

[S46] C++：函数模板
来源：http://fv.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xi.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://xd.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://og.nszjky.cn

[S48] C++：逐行读文件
来源：http://jg.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nh.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://dn.hnjuh.cn

[S49] C++：写文件
来源：http://gc.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://az.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://nl.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://id.nszjky.cn

[S51] C++：显式类型转换
来源：http://ip.yuexingan06.cn

static_cast<double>(a) / b
来源：http://yv.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://dc.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://hd.muxihuayi.cn

[S53] C++：移动语义
来源：http://bl.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://hg.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://mg.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zr.shxzskj.cn

[S55] C++：结构化绑定
来源：http://ql.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lt.521024.cn

[S56] C++：optional
来源：http://xm.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://te.bjjhwx.cn

[S57] C++：编译期常量
来源：http://mf.gzmigu.cn

constexpr int N = 10;
来源：http://qc.shxzskj.cn

[S58] C++：命名空间
来源：http://of.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://dx.huanxung.cn

[S59] C++：静态断言
来源：http://mm.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lf.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://na.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://si.lnxyls.cn

================================================================================
来源：http://gw.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://co.szxytkj.cn

================================================================================
来源：http://me.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://un.bjjhwx.cn

println("Hello")
来源：http://wk.panjiajie.cn

[T02] Kotlin：变量
来源：http://wv.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wt.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://xi.hahajie.cn

"值: $b"
来源：http://xe.shxzskj.cn

[T04] Kotlin：空安全
来源：http://lz.9csxet.cn

val n: String? = null;  n?.length
来源：http://zz.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://ku.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ng.colortex.cn

[T06] Kotlin：集合映射
来源：http://qm.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mb.asd995.cn

[T07] Kotlin：集合过滤
来源：http://gh.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rv.hnjuh.cn

[T08] Kotlin：数据类
来源：http://kf.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://ui.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://sr.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://uc.nszjky.cn

[T10] Kotlin：默认参数
来源：http://it.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ct.shtwfgs.cn


<!-- 参考信息 -->