代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ci.newstarts.cn

[R10] 正则匹配
来源：http://iy.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sh.yuntaijiaju.cn

[R11] case 多分支
来源：http://gw.gzmigu.cn

case "$1" in
来源：http://sr.hnjuh.cn

start) echo "启动" ;;
来源：http://lu.9csxet.cn

stop)  echo "停止" ;;
来源：http://gx.hahajie.cn

*)     echo "未知命令" ;;
来源：http://xn.panjiajie.cn

esac
来源：http://zz.bookmarksfly.cn

[R12] for 遍历文件
来源：http://by.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://em.szsharing.cn

[R13] for 计数循环
来源：http://he.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://gs.wgjwhj.cn

[R14] C 风格 for
来源：http://mj.yuntaijiaju.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eh.521024.cn

[R15] while 逐行读文件
来源：http://hb.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pr.huixiangedu.cn

[R16] until 等待条件
来源：http://nm.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aw.9csxet.cn

[R17] 数组定义与取值
来源：http://cf.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ig.colortex.cn

[R18] 遍历数组
来源：http://ns.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kk.chemitech.net.cn

[R19] 数组长度
来源：http://qe.nszjky.cn

echo "${#arr[@]}"
来源：http://hc.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://fh.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qp.asd995.cn

[R21] 字符串长度
来源：http://ic.hnjuh.cn

echo "${#s}"
来源：http://td.asd995.cn

[R22] 截取子串
来源：http://aj.chemitech.net.cn

echo "${s:0:5}"
来源：http://ip.nszjky.cn

[R23] 字符串替换
来源：http://eb.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://er.gzmigu.cn

[R24] 大小写转换
来源：http://em.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ni.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://ji.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qq.521024.cn

[R26] 命令替换
来源：http://wq.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://wl.wgjwhj.cn

[R27] 算术展开
来源：http://bl.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://gp.muxihuayi.cn

[R28] 浮点运算
来源：http://na.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://ao.shxzukj.cn

[R29] 定义函数
来源：http://ke.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ko.panjiajie.cn

[R30] 函数返回状态码
来源：http://mh.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://ut.bjjhwx.cn

[R31] 局部变量
来源：http://kk.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://fr.gzmigu.cn

[R32] 参数个数校验
来源：http://qy.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nk.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://jx.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bi.shxzukj.cn

[R34] 退出时清理
来源：http://we.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nj.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://sz.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yf.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://af.nszjky.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uq.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ka.newstarts.cn

files=$(ls -1)
来源：http://dg.hahajie.cn

[R38] 管道串联
来源：http://sj.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://yf.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://ux.yuexingan06.cn

cmd > out.log 2>&1
来源：http://jt.muxihuayi.cn

[R40] 追加写日志
来源：http://wa.hahajie.cn

echo "log" >> out.log
来源：http://cr.newstarts.cn

[R41] 丢弃输出
来源：http://al.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://qb.haigaiapp.cn

[R42] 输入重定向
来源：http://sz.chemitech.net.cn

wc -l < a.txt
来源：http://ac.shtwfgs.cn

[R43] 按名字查找文件
来源：http://gy.nicolike.cn

find . -name "*.log" -type f
来源：http://wq.yuexingan06.cn

[R44] 按修改时间查找
来源：http://pr.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://qp.shxzukj.cn

[R45] 批量删除
来源：http://ec.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://vy.shxzukj.cn

[R46] 递归替换文件内容
来源：http://eh.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kd.hnjuh.cn

[R47] sed 单行替换
来源：http://te.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sa.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://au.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://mr.haigaiapp.cn

[R49] awk 带条件
来源：http://tv.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bw.shxzukj.cn

[R50] awk 求和
来源：http://si.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pf.panjiajie.cn

[R51] 排序去重取前几
来源：http://ed.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yr.huixiangedu.cn

[R52] 统计行数
来源：http://io.jctech888.com.cn

wc -l a.txt
来源：http://xo.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://fd.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mv.lnxyls.cn

[R54] 比较两个文件
来源：http://tm.shxzukj.cn

diff a.txt b.txt
来源：http://to.muxihuayi.cn

[R55] 压缩与解压
来源：http://xh.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pj.panjiajie.cn

[R56] 远程拷贝
来源：http://fj.bjjhwx.cn

scp file user@host:/path/
来源：http://rw.nszjky.cn

[R57] 远程执行命令
来源：http://gv.huixiangedu.cn

ssh user@host 'uptime'
来源：http://ul.colortex.cn

[R58] 下载文件
来源：http://pf.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hi.jctech888.com.cn

[R59] 发 POST JSON
来源：http://oa.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://no.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://qg.bookmarksfly.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tl.huanxung.cn

[R61] 磁盘占用
来源：http://vw.shtwfgs.cn

df -h;  du -sh *
来源：http://ef.gzmigu.cn

[R62] 找最占空间的文件
来源：http://dd.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://xo.panjiajie.cn

[R63] 内存与进程
来源：http://to.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://oz.huixinmuqiang.cn

[R64] 结束进程
来源：http://ti.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://kl.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://sr.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ga.yuexingan06.cn

[R66] 定时任务
来源：http://dx.jctech888.com.cn

crontab -e;  crontab -l
来源：http://yz.asd995.cn

[R67] 生成随机十六进制串
来源：http://ll.bjjhwx.cn

openssl rand -hex 16
来源：http://va.yuexingan06.cn

[R68] 计算文件校验值
来源：http://kk.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://il.chemitech.net.cn

[R69] 生成随机密码
来源：http://ys.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://hd.muxihuayi.cn

[R70] 时间戳与互转
来源：http://mq.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ob.szsharing.cn

[R71] 日期格式化
来源：http://kk.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dt.huixiangedu.cn

[R72] 等待端口就绪
来源：http://xz.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pf.yuntaijiaju.cn

[R73] 分割大日志
来源：http://kk.jctech888.com.cn

split -l 1000 big.log part_
来源：http://xp.bjjhwx.cn

[R74] 批量重命名
来源：http://ps.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pw.huixiangedu.cn

[R75] 导出环境变量
来源：http://dm.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://kt.hnjuh.cn

[R76] 使用临时文件
来源：http://xy.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xk.chemitech.net.cn

[R77] 读取用户输入
来源：http://id.shxzskj.cn

read -rp "请输入: " ans
来源：http://xw.asd995.cn

[R78] 交互式菜单
来源：http://tf.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tc.nicolike.cn

[R79] 解析命令行选项
来源：http://rh.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bi.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://zg.huanxung.cn

time ./run.sh
来源：http://bj.nicolike.cn

================================================================================
来源：http://tf.wgjwhj.cn

S. C / C++ 专题
来源：http://yh.muxihuayi.cn

================================================================================
来源：http://ld.huanxung.cn

[S01] C：Hello World
来源：http://am.huanxung.cn

#include <stdio.h>
来源：http://gu.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fj.newstarts.cn

[S02] C：变量与格式化输出
来源：http://yu.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://gp.yuexingan06.cn

[S03] C：读入整数
来源：http://pd.nszjky.cn

int x; scanf("%d", &x);
来源：http://sa.hnjuh.cn

[S04] C：字符串复制
来源：http://ag.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wd.panjiajie.cn

[S05] C：字符串长度
来源：http://it.haigaiapp.cn

strlen(s)
来源：http://ht.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://hr.wgjwhj.cn

strcmp(a, b) == 0
来源：http://hb.hahajie.cn

[S07] C：数组遍历求和
来源：http://eu.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gq.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://tt.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nm.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://ri.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qo.panjiajie.cn

[S10] C：指针与解引用
来源：http://pz.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://gs.shxzukj.cn

[S11] C：逐行读文件
来源：http://vr.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ng.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ze.9csxet.cn

fclose(f);
来源：http://bn.nicolike.cn

[S12] C：写文件
来源：http://uk.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://np.colortex.cn

[S13] C：宏定义
来源：http://th.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ap.gzmigu.cn

[S14] C：枚举
来源：http://xh.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://bt.jianghongdianzi.cn

[S15] C：类型转换
来源：http://qd.9csxet.cn

(double) a / b
来源：http://er.nszjky.cn

[S16] C：位操作置位
来源：http://os.huixiangedu.cn

x |= (1 << 3);
来源：http://rj.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://sb.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sn.chemitech.net.cn

[S18] C：命令行参数
来源：http://cv.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://iq.huanxung.cn

[S19] C：快速排序
来源：http://mb.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sw.nszjky.cn

[S20] C：二分查找
来源：http://pc.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kd.9csxet.cn

[S21] C：字符类别判断
来源：http://xa.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qz.hnjuh.cn

[S22] C：字符串转数字
来源：http://dt.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://im.huixinmuqiang.cn

[S23] C：随机数
来源：http://wv.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zf.bjjhwx.cn

[S24] C：获取本地时间
来源：http://su.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://de.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ir.hnjuh.cn

memcpy(dst, src, n);
来源：http://us.yuntaijiaju.cn

[S26] C：内存清零
来源：http://gq.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://ly.nicolike.cn

[S27] C：定义常量
来源：http://sj.huanxung.cn

const double PI = 3.14159;
来源：http://zb.huanxung.cn

[S28] C：静态变量
来源：http://ro.haigaiapp.cn

static int counter = 0;
来源：http://yh.szxytkj.cn

[S29] C：变参函数
来源：http://fw.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yn.muxihuayi.cn

[S30] C：头文件保护
来源：http://ji.shxzskj.cn

#ifndef X_H
来源：http://nh.hahajie.cn

#define X_H
来源：http://mc.szxytkj.cn

#endif
来源：http://ws.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://ra.szxytkj.cn

#include <iostream>
来源：http://oj.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://wl.muxihuayi.cn

[S32] C++：字符串
来源：http://yu.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://nj.huanxung.cn

[S33] C++：vector 增删
来源：http://zz.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tw.nszjky.cn

[S34] C++：遍历 vector
来源：http://og.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://sg.hnjuh.cn

[S35] C++：map
来源：http://xr.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cg.wgjwhj.cn

[S36] C++：unordered_map
来源：http://hu.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jv.chemitech.net.cn

[S37] C++：set
来源：http://sf.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vs.jctech888.com.cn

[S38] C++：排序
来源：http://rm.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://cj.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://lz.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bc.bjjhwx.cn

[S40] C++：查找元素
来源：http://wl.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://og.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://ih.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://al.szsharing.cn

[S42] C++：继承与虚函数
来源：http://st.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://wk.asd995.cn

[S43] C++：智能指针
来源：http://xm.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://kl.huixiangedu.cn

[S44] C++：引用传参
来源：http://bs.szsharing.cn

void inc(int &x) { ++x; }
来源：http://zk.wgjwhj.cn

[S45] C++：lambda
来源：http://mh.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aa.jctech888.com.cn

[S46] C++：函数模板
来源：http://dt.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sf.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://ae.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gl.panjiajie.cn

[S48] C++：逐行读文件
来源：http://xj.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dp.newstarts.cn

while (std::getline(in, line)) { }
来源：http://kn.lnxyls.cn

[S49] C++：写文件
来源：http://to.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zs.jctech888.com.cn

[S50] C++：格式化数字
来源：http://rg.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yn.szsharing.cn

[S51] C++：显式类型转换
来源：http://ud.huanxung.cn

static_cast<double>(a) / b
来源：http://ld.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://zv.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://lq.haigaiapp.cn

[S53] C++：移动语义
来源：http://pp.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://zm.jctech888.com.cn

[S54] C++：异常处理
来源：http://yr.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fx.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://jx.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fg.lnxyls.cn

[S56] C++：optional
来源：http://lr.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ug.yuexingan06.cn

[S57] C++：编译期常量
来源：http://xk.jianghongdianzi.cn

constexpr int N = 10;
来源：http://jt.szxytkj.cn

[S58] C++：命名空间
来源：http://dx.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://od.newstarts.cn

[S59] C++：静态断言
来源：http://md.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vu.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://ql.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ge.szsharing.cn

================================================================================
来源：http://fx.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yo.huixinmuqiang.cn

================================================================================
来源：http://oe.9csxet.cn

[T01] Kotlin：Hello World
来源：http://oh.wgjwhj.cn

println("Hello")
来源：http://in.hahajie.cn

[T02] Kotlin：变量
来源：http://ny.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yn.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://qv.gzmigu.cn

"值: $b"
来源：http://in.nszjky.cn

[T04] Kotlin：空安全
来源：http://hj.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://ho.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://zn.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uc.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://pt.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bd.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://jb.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ho.9csxet.cn

[T08] Kotlin：数据类
来源：http://vg.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://je.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://mw.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://vj.colortex.cn

[T10] Kotlin：默认参数
来源：http://nk.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://op.nszjky.cn


<!-- 参考信息 -->