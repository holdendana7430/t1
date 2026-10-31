代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pg.bjjhwx.cn

[R08] 数值比较
来源：http://eo.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uv.nszjky.cn

[R09] 字符串比较
来源：http://qc.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bs.asd995.cn

[R10] 正则匹配
来源：http://xu.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pq.hahajie.cn

[R11] case 多分支
来源：http://zg.shtwfgs.cn

case "$1" in
来源：http://iu.szsharing.cn

start) echo "启动" ;;
来源：http://ba.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://nn.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://df.huixiangedu.cn

esac
来源：http://sf.nicolike.cn

[R12] for 遍历文件
来源：http://cm.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://rp.panjiajie.cn

[R13] for 计数循环
来源：http://ly.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://as.szxytkj.cn

[R14] C 风格 for
来源：http://pe.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vz.shxzskj.cn

[R15] while 逐行读文件
来源：http://lm.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ki.bookmarksfly.cn

[R16] until 等待条件
来源：http://xd.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qj.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://oa.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mv.huanxung.cn

[R18] 遍历数组
来源：http://jl.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xw.gzmigu.cn

[R19] 数组长度
来源：http://qy.lnxyls.cn

echo "${#arr[@]}"
来源：http://jn.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://jk.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kl.szsharing.cn

[R21] 字符串长度
来源：http://iu.nicolike.cn

echo "${#s}"
来源：http://ui.colortex.cn

[R22] 截取子串
来源：http://kv.521024.cn

echo "${s:0:5}"
来源：http://py.shxzskj.cn

[R23] 字符串替换
来源：http://xu.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rb.jianghongdianzi.cn

[R24] 大小写转换
来源：http://lk.9csxet.cn

echo "${s^^}"; echo "${s,,}"
来源：http://le.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://lp.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ec.nszjky.cn

[R26] 命令替换
来源：http://ye.521024.cn

now=$(date +%F); echo "$now"
来源：http://zc.panjiajie.cn

[R27] 算术展开
来源：http://wt.huanxung.cn

echo $((1 + 2 * 3))
来源：http://ty.nicolike.cn

[R28] 浮点运算
来源：http://ox.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://wg.haigaiapp.cn

[R29] 定义函数
来源：http://ix.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bl.gzmigu.cn

[R30] 函数返回状态码
来源：http://zc.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://bw.nszjky.cn

[R31] 局部变量
来源：http://xv.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://eg.newstarts.cn

[R32] 参数个数校验
来源：http://bl.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gy.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://qm.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xa.shxzskj.cn

[R34] 退出时清理
来源：http://na.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nn.huixiangedu.cn

[R35] 后台执行并等待
来源：http://ul.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ao.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://iz.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://in.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://jt.yuexingan06.cn

files=$(ls -1)
来源：http://ub.9csxet.cn

[R38] 管道串联
来源：http://cy.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://gg.521024.cn

[R39] 重定向标准输出与错误
来源：http://oq.shtwfgs.cn

cmd > out.log 2>&1
来源：http://lt.colortex.cn

[R40] 追加写日志
来源：http://ke.panjiajie.cn

echo "log" >> out.log
来源：http://yj.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://sp.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://la.haigaiapp.cn

[R42] 输入重定向
来源：http://fl.9csxet.cn

wc -l < a.txt
来源：http://by.hnjuh.cn

[R43] 按名字查找文件
来源：http://gf.521024.cn

find . -name "*.log" -type f
来源：http://pl.jianghongdianzi.cn

[R44] 按修改时间查找
来源：http://dp.shtwfgs.cn

find . -mtime -7 -type f
来源：http://ov.chemitech.net.cn

[R45] 批量删除
来源：http://ex.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://ir.szxytkj.cn

[R46] 递归替换文件内容
来源：http://jj.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://st.muxihuayi.cn

[R47] sed 单行替换
来源：http://lb.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gk.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://hp.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://at.yuntaijiaju.cn

[R49] awk 带条件
来源：http://sy.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gf.gzmigu.cn

[R50] awk 求和
来源：http://ki.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wu.huanxung.cn

[R51] 排序去重取前几
来源：http://tm.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xa.hahajie.cn

[R52] 统计行数
来源：http://fg.yuntaijiaju.cn

wc -l a.txt
来源：http://td.huixiangedu.cn

[R53] 查看文件头与实时尾
来源：http://cw.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yr.hahajie.cn

[R54] 比较两个文件
来源：http://ha.panjiajie.cn

diff a.txt b.txt
来源：http://tm.shxzukj.cn

[R55] 压缩与解压
来源：http://ji.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kt.haigaiapp.cn

[R56] 远程拷贝
来源：http://pu.yuntaijiaju.cn

scp file user@host:/path/
来源：http://ww.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://fj.szsharing.cn

ssh user@host 'uptime'
来源：http://ag.szsharing.cn

[R58] 下载文件
来源：http://rg.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uf.szxytkj.cn

[R59] 发 POST JSON
来源：http://ay.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uk.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://cx.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wl.nszjky.cn

[R61] 磁盘占用
来源：http://ew.yuntaijiaju.cn

df -h;  du -sh *
来源：http://sp.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://wb.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://ng.muxihuayi.cn

[R63] 内存与进程
来源：http://gw.shtwfgs.cn

free -h;  ps aux | grep nginx
来源：http://mt.colortex.cn

[R64] 结束进程
来源：http://pg.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://ep.huixiangedu.cn

[R65] 查看端口占用
来源：http://pm.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://av.szsharing.cn

[R66] 定时任务
来源：http://yj.9csxet.cn

crontab -e;  crontab -l
来源：http://yp.huixiangedu.cn

[R67] 生成随机十六进制串
来源：http://xc.haigaiapp.cn

openssl rand -hex 16
来源：http://qy.panjiajie.cn

[R68] 计算文件校验值
来源：http://op.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yf.huixiangedu.cn

[R69] 生成随机密码
来源：http://an.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://bf.nicolike.cn

[R70] 时间戳与互转
来源：http://ww.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://yh.hahajie.cn

[R71] 日期格式化
来源：http://ev.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aa.shxzukj.cn

[R72] 等待端口就绪
来源：http://zg.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ts.asd995.cn

[R73] 分割大日志
来源：http://gr.521024.cn

split -l 1000 big.log part_
来源：http://tb.gzmigu.cn

[R74] 批量重命名
来源：http://ds.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tw.chemitech.net.cn

[R75] 导出环境变量
来源：http://gg.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://cf.wgjwhj.cn

[R76] 使用临时文件
来源：http://oo.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ys.gzmigu.cn

[R77] 读取用户输入
来源：http://jk.chemitech.net.cn

read -rp "请输入: " ans
来源：http://ue.lnxyls.cn

[R78] 交互式菜单
来源：http://iq.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://na.panjiajie.cn

[R79] 解析命令行选项
来源：http://pz.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yi.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://jn.colortex.cn

time ./run.sh
来源：http://oe.521024.cn

================================================================================
来源：http://oh.jianghongdianzi.cn

S. C / C++ 专题
来源：http://jn.yuexingan06.cn

================================================================================
来源：http://ld.yuexingan06.cn

[S01] C：Hello World
来源：http://xw.huanxung.cn

#include <stdio.h>
来源：http://ur.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gp.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://zt.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://qx.hahajie.cn

[S03] C：读入整数
来源：http://ff.nicolike.cn

int x; scanf("%d", &x);
来源：http://ry.lnxyls.cn

[S04] C：字符串复制
来源：http://ta.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yt.bookmarksfly.cn

[S05] C：字符串长度
来源：http://fx.huanxung.cn

strlen(s)
来源：http://tk.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://lx.lnxyls.cn

strcmp(a, b) == 0
来源：http://nc.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://bd.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qu.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://hc.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kk.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://qi.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ou.gzmigu.cn

[S10] C：指针与解引用
来源：http://su.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ue.hahajie.cn

[S11] C：逐行读文件
来源：http://yv.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://lw.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vr.bookmarksfly.cn

fclose(f);
来源：http://ju.shtwfgs.cn

[S12] C：写文件
来源：http://nn.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pf.yuntaijiaju.cn

[S13] C：宏定义
来源：http://jx.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ne.shtwfgs.cn

[S14] C：枚举
来源：http://zv.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://vj.lnxyls.cn

[S15] C：类型转换
来源：http://yk.shtwfgs.cn

(double) a / b
来源：http://gk.colortex.cn

[S16] C：位操作置位
来源：http://ex.jctech888.com.cn

x |= (1 << 3);
来源：http://za.nszjky.cn

[S17] C：安全拼接字符串
来源：http://rt.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yd.gzmigu.cn

[S18] C：命令行参数
来源：http://zq.wgjwhj.cn

int main(int argc, char **argv)
来源：http://sr.nszjky.cn

[S19] C：快速排序
来源：http://ye.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ye.shxzskj.cn

[S20] C：二分查找
来源：http://hb.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sz.huixiangedu.cn

[S21] C：字符类别判断
来源：http://ye.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gt.chemitech.net.cn

[S22] C：字符串转数字
来源：http://mb.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gq.bookmarksfly.cn

[S23] C：随机数
来源：http://bo.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tt.nszjky.cn

[S24] C：获取本地时间
来源：http://mj.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bj.newstarts.cn

[S25] C：内存拷贝
来源：http://bh.shtwfgs.cn

memcpy(dst, src, n);
来源：http://oh.jctech888.com.cn

[S26] C：内存清零
来源：http://go.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://xs.szsharing.cn

[S27] C：定义常量
来源：http://zb.colortex.cn

const double PI = 3.14159;
来源：http://vp.huixinmuqiang.cn

[S28] C：静态变量
来源：http://iy.szxytkj.cn

static int counter = 0;
来源：http://oe.jianghongdianzi.cn

[S29] C：变参函数
来源：http://ly.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ql.9csxet.cn

[S30] C：头文件保护
来源：http://sq.nszjky.cn

#ifndef X_H
来源：http://aw.yuexingan06.cn

#define X_H
来源：http://qr.shxzskj.cn

#endif
来源：http://tn.bookmarksfly.cn

[S31] C++：Hello World
来源：http://fb.wgjwhj.cn

#include <iostream>
来源：http://al.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://ew.hnjuh.cn

[S32] C++：字符串
来源：http://xt.colortex.cn

std::string s = "hi";  s += "!";
来源：http://bk.hnjuh.cn

[S33] C++：vector 增删
来源：http://xr.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ca.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://af.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://si.huixiangedu.cn

[S35] C++：map
来源：http://ol.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://be.nicolike.cn

[S36] C++：unordered_map
来源：http://ws.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iu.jianghongdianzi.cn

[S37] C++：set
来源：http://oo.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qy.hahajie.cn

[S38] C++：排序
来源：http://ik.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://qa.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://ip.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://au.asd995.cn

[S40] C++：查找元素
来源：http://id.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ou.lnxyls.cn

[S41] C++：类与构造函数
来源：http://hf.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nl.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://ve.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://ro.shxzukj.cn

[S43] C++：智能指针
来源：http://ek.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://bn.lnxyls.cn

[S44] C++：引用传参
来源：http://vy.newstarts.cn

void inc(int &x) { ++x; }
来源：http://kt.521024.cn

[S45] C++：lambda
来源：http://kp.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zi.shxzskj.cn

[S46] C++：函数模板
来源：http://eb.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nx.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ez.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nb.panjiajie.cn

[S48] C++：逐行读文件
来源：http://ts.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pb.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://ly.szsharing.cn

[S49] C++：写文件
来源：http://sn.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gj.asd995.cn

[S50] C++：格式化数字
来源：http://iu.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yw.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://nh.hahajie.cn

static_cast<double>(a) / b
来源：http://ac.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://cx.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://dg.521024.cn

[S53] C++：移动语义
来源：http://bc.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://pz.shtwfgs.cn

[S54] C++：异常处理
来源：http://hr.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ef.asd995.cn

[S55] C++：结构化绑定
来源：http://kd.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uo.asd995.cn

[S56] C++：optional
来源：http://hd.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yg.newstarts.cn

[S57] C++：编译期常量
来源：http://sn.colortex.cn

constexpr int N = 10;
来源：http://zz.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://hk.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://lz.bjjhwx.cn

[S59] C++：静态断言
来源：http://pr.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://es.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://xz.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ch.jianghongdianzi.cn

================================================================================
来源：http://je.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uy.huanxung.cn

================================================================================
来源：http://hc.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://kt.panjiajie.cn

println("Hello")
来源：http://ib.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ss.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xn.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://df.wgjwhj.cn

"值: $b"
来源：http://zh.bjjhwx.cn

[T04] Kotlin：空安全
来源：http://dq.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://lp.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://cd.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sj.nszjky.cn

[T06] Kotlin：集合映射
来源：http://pb.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uy.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://ww.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://we.521024.cn

[T08] Kotlin：数据类
来源：http://bw.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://xa.szsharing.cn


<!-- 参考信息 -->