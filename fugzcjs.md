代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qt.szxytkj.cn

[R08] 数值比较
来源：http://ka.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ij.yuntaijiaju.cn

[R09] 字符串比较
来源：http://sa.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wt.chemitech.net.cn

[R10] 正则匹配
来源：http://wu.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fx.gzmigu.cn

[R11] case 多分支
来源：http://wf.newstarts.cn

case "$1" in
来源：http://ty.chemitech.net.cn

start) echo "启动" ;;
来源：http://xs.hahajie.cn

stop)  echo "停止" ;;
来源：http://kl.hnjuh.cn

*)     echo "未知命令" ;;
来源：http://jg.nicolike.cn

esac
来源：http://ha.huixiangedu.cn

[R12] for 遍历文件
来源：http://hu.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://fo.shxzukj.cn

[R13] for 计数循环
来源：http://gu.chemitech.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://yp.huixiangedu.cn

[R14] C 风格 for
来源：http://yt.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cd.haigaiapp.cn

[R15] while 逐行读文件
来源：http://qd.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jc.shxzskj.cn

[R16] until 等待条件
来源：http://xq.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zv.jctech888.com.cn

[R17] 数组定义与取值
来源：http://yb.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://te.szsharing.cn

[R18] 遍历数组
来源：http://yw.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://al.wgjwhj.cn

[R19] 数组长度
来源：http://rq.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://lm.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://qb.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cs.521024.cn

[R21] 字符串长度
来源：http://of.colortex.cn

echo "${#s}"
来源：http://ax.chemitech.net.cn

[R22] 截取子串
来源：http://lh.hahajie.cn

echo "${s:0:5}"
来源：http://sj.9csxet.cn

[R23] 字符串替换
来源：http://as.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uw.521024.cn

[R24] 大小写转换
来源：http://tj.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kf.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://hm.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jv.hahajie.cn

[R26] 命令替换
来源：http://zf.asd995.cn

now=$(date +%F); echo "$now"
来源：http://uu.newstarts.cn

[R27] 算术展开
来源：http://uz.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://dg.yuexingan06.cn

[R28] 浮点运算
来源：http://zz.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://xp.shxzskj.cn

[R29] 定义函数
来源：http://cl.shtwfgs.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qf.newstarts.cn

[R30] 函数返回状态码
来源：http://je.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://np.jctech888.com.cn

[R31] 局部变量
来源：http://xp.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://no.newstarts.cn

[R32] 参数个数校验
来源：http://qq.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kd.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://hk.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zd.wgjwhj.cn

[R34] 退出时清理
来源：http://mk.colortex.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tt.huanxung.cn

[R35] 后台执行并等待
来源：http://ra.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fy.newstarts.cn

[R36] 并发执行多个任务
来源：http://ne.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eo.szxytkj.cn

[R37] 把输出赋给变量
来源：http://jn.bookmarksfly.cn

files=$(ls -1)
来源：http://xo.nicolike.cn

[R38] 管道串联
来源：http://wk.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://yb.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://qo.asd995.cn

cmd > out.log 2>&1
来源：http://oe.hahajie.cn

[R40] 追加写日志
来源：http://bd.nicolike.cn

echo "log" >> out.log
来源：http://vj.wgjwhj.cn

[R41] 丢弃输出
来源：http://pq.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://ed.haigaiapp.cn

[R42] 输入重定向
来源：http://va.huixiangedu.cn

wc -l < a.txt
来源：http://xi.lnxyls.cn

[R43] 按名字查找文件
来源：http://vh.521024.cn

find . -name "*.log" -type f
来源：http://wr.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://wo.521024.cn

find . -mtime -7 -type f
来源：http://bb.szsharing.cn

[R45] 批量删除
来源：http://ft.szsharing.cn

find . -name "*.tmp" -delete
来源：http://xw.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://oj.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zf.yuexingan06.cn

[R47] sed 单行替换
来源：http://xg.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cg.9csxet.cn

[R48] awk 取指定列
来源：http://ez.521024.cn

awk '{print $1, $3}' a.txt
来源：http://jm.9csxet.cn

[R49] awk 带条件
来源：http://tz.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fa.szxytkj.cn

[R50] awk 求和
来源：http://tv.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ru.chemitech.net.cn

[R51] 排序去重取前几
来源：http://km.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qc.shxzukj.cn

[R52] 统计行数
来源：http://pr.jianghongdianzi.cn

wc -l a.txt
来源：http://dp.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://cg.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://af.lnxyls.cn

[R54] 比较两个文件
来源：http://yv.bookmarksfly.cn

diff a.txt b.txt
来源：http://ul.nicolike.cn

[R55] 压缩与解压
来源：http://ph.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ux.shxzukj.cn

[R56] 远程拷贝
来源：http://et.huanxung.cn

scp file user@host:/path/
来源：http://zb.bookmarksfly.cn

[R57] 远程执行命令
来源：http://fa.shtwfgs.cn

ssh user@host 'uptime'
来源：http://wm.yuexingan06.cn

[R58] 下载文件
来源：http://qs.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mm.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ub.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yu.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ul.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ie.bookmarksfly.cn

[R61] 磁盘占用
来源：http://ys.jctech888.com.cn

df -h;  du -sh *
来源：http://nt.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://as.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://qv.yuntaijiaju.cn

[R63] 内存与进程
来源：http://hc.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://ay.shtwfgs.cn

[R64] 结束进程
来源：http://qi.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://nz.chemitech.net.cn

[R65] 查看端口占用
来源：http://ux.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oa.bjjhwx.cn

[R66] 定时任务
来源：http://an.szxytkj.cn

crontab -e;  crontab -l
来源：http://tv.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://zv.panjiajie.cn

openssl rand -hex 16
来源：http://dq.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://vc.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kp.bookmarksfly.cn

[R69] 生成随机密码
来源：http://rm.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://xj.newstarts.cn

[R70] 时间戳与互转
来源：http://hj.nicolike.cn

date +%s;  date -d @1700000000
来源：http://ls.hahajie.cn

[R71] 日期格式化
来源：http://dv.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://in.szxytkj.cn

[R72] 等待端口就绪
来源：http://hz.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uv.panjiajie.cn

[R73] 分割大日志
来源：http://dk.hahajie.cn

split -l 1000 big.log part_
来源：http://of.521024.cn

[R74] 批量重命名
来源：http://xk.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://an.9csxet.cn

[R75] 导出环境变量
来源：http://qr.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://nd.chemitech.net.cn

[R76] 使用临时文件
来源：http://gp.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kf.panjiajie.cn

[R77] 读取用户输入
来源：http://tn.wgjwhj.cn

read -rp "请输入: " ans
来源：http://pn.shxzukj.cn

[R78] 交互式菜单
来源：http://lz.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uy.szsharing.cn

[R79] 解析命令行选项
来源：http://zb.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vx.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://fa.huixiangedu.cn

time ./run.sh
来源：http://jg.bookmarksfly.cn

================================================================================
来源：http://sh.haigaiapp.cn

S. C / C++ 专题
来源：http://wk.szsharing.cn

================================================================================
来源：http://lc.wgjwhj.cn

[S01] C：Hello World
来源：http://es.huixiangedu.cn

#include <stdio.h>
来源：http://la.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://un.colortex.cn

[S02] C：变量与格式化输出
来源：http://ic.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://ot.huixinmuqiang.cn

[S03] C：读入整数
来源：http://rx.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://di.chemitech.net.cn

[S04] C：字符串复制
来源：http://wf.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xw.huanxung.cn

[S05] C：字符串长度
来源：http://jn.shxzskj.cn

strlen(s)
来源：http://lm.bookmarksfly.cn

[S06] C：字符串比较
来源：http://ds.szsharing.cn

strcmp(a, b) == 0
来源：http://wu.szxytkj.cn

[S07] C：数组遍历求和
来源：http://tc.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kl.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://mu.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rr.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://fh.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gv.wgjwhj.cn

[S10] C：指针与解引用
来源：http://wc.9csxet.cn

int *p = &a;  *p = 5;
来源：http://yi.bjjhwx.cn

[S11] C：逐行读文件
来源：http://hx.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://ov.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ks.szxytkj.cn

fclose(f);
来源：http://qx.jianghongdianzi.cn

[S12] C：写文件
来源：http://ys.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ca.panjiajie.cn

[S13] C：宏定义
来源：http://af.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nw.nicolike.cn

[S14] C：枚举
来源：http://zf.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://fh.nicolike.cn

[S15] C：类型转换
来源：http://lq.521024.cn

(double) a / b
来源：http://nu.shxzukj.cn

[S16] C：位操作置位
来源：http://ag.haigaiapp.cn

x |= (1 << 3);
来源：http://ca.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://le.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vn.newstarts.cn

[S18] C：命令行参数
来源：http://gd.szxytkj.cn

int main(int argc, char **argv)
来源：http://iq.shxzskj.cn

[S19] C：快速排序
来源：http://ir.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://er.szsharing.cn

[S20] C：二分查找
来源：http://bp.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mc.9csxet.cn

[S21] C：字符类别判断
来源：http://pg.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uq.bjjhwx.cn

[S22] C：字符串转数字
来源：http://by.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hf.szxytkj.cn

[S23] C：随机数
来源：http://sb.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gf.shxzskj.cn

[S24] C：获取本地时间
来源：http://ml.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lf.9csxet.cn

[S25] C：内存拷贝
来源：http://ad.panjiajie.cn

memcpy(dst, src, n);
来源：http://gl.wgjwhj.cn

[S26] C：内存清零
来源：http://if.asd995.cn

memset(a, 0, sizeof a);
来源：http://vf.yuntaijiaju.cn

[S27] C：定义常量
来源：http://sl.chemitech.net.cn

const double PI = 3.14159;
来源：http://wx.nicolike.cn

[S28] C：静态变量
来源：http://qp.asd995.cn

static int counter = 0;
来源：http://yo.haigaiapp.cn

[S29] C：变参函数
来源：http://eh.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zp.wgjwhj.cn

[S30] C：头文件保护
来源：http://ls.nszjky.cn

#ifndef X_H
来源：http://sn.yuexingan06.cn

#define X_H
来源：http://ah.asd995.cn

#endif
来源：http://wr.huanxung.cn

[S31] C++：Hello World
来源：http://su.huanxung.cn

#include <iostream>
来源：http://pf.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ei.shxzukj.cn

[S32] C++：字符串
来源：http://wl.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://rb.gzmigu.cn

[S33] C++：vector 增删
来源：http://os.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lw.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://lb.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://bo.shxzukj.cn

[S35] C++：map
来源：http://ir.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kf.szsharing.cn

[S36] C++：unordered_map
来源：http://hj.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://am.yuexingan06.cn

[S37] C++：set
来源：http://wb.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://no.haigaiapp.cn

[S38] C++：排序
来源：http://tc.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://vh.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://zd.colortex.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tw.newstarts.cn

[S40] C++：查找元素
来源：http://yf.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uj.hnjuh.cn

[S41] C++：类与构造函数
来源：http://tv.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sg.asd995.cn

[S42] C++：继承与虚函数
来源：http://pm.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://wn.bjjhwx.cn

[S43] C++：智能指针
来源：http://tm.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://jx.asd995.cn

[S44] C++：引用传参
来源：http://hy.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://ek.jianghongdianzi.cn

[S45] C++：lambda
来源：http://jl.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rx.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://rk.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vn.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://je.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fa.szsharing.cn

[S48] C++：逐行读文件
来源：http://wl.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nl.newstarts.cn

while (std::getline(in, line)) { }
来源：http://gw.chemitech.net.cn

[S49] C++：写文件
来源：http://ny.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kq.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://ml.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cj.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://go.szsharing.cn

static_cast<double>(a) / b
来源：http://jv.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://gm.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://rj.colortex.cn

[S53] C++：移动语义
来源：http://jw.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://cp.szsharing.cn

[S54] C++：异常处理
来源：http://ew.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tk.lnxyls.cn

[S55] C++：结构化绑定
来源：http://gq.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://in.bjjhwx.cn

[S56] C++：optional
来源：http://ls.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oo.szsharing.cn

[S57] C++：编译期常量
来源：http://av.yuexingan06.cn

constexpr int N = 10;
来源：http://df.wgjwhj.cn

[S58] C++：命名空间
来源：http://bw.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://gx.jctech888.com.cn

[S59] C++：静态断言
来源：http://ds.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ai.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://zo.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ds.521024.cn

================================================================================
来源：http://le.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hg.bookmarksfly.cn

================================================================================
来源：http://jp.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://hy.yuexingan06.cn

println("Hello")
来源：http://xl.hnjuh.cn

[T02] Kotlin：变量
来源：http://hp.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://me.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://at.shxzukj.cn

"值: $b"
来源：http://od.panjiajie.cn

[T04] Kotlin：空安全
来源：http://qs.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://ny.colortex.cn

[T05] Kotlin：when 表达式
来源：http://qo.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ho.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://tj.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ps.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://pe.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ny.521024.cn

[T08] Kotlin：数据类
来源：http://ej.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://la.hnjuh.cn


<!-- 参考信息 -->