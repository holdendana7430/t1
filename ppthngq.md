代发 wailian999

set -euo pipefail
来源：http://sh.shxzskj.cn

[R02] 变量赋值与使用
来源：http://ij.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://sa.haigaiapp.cn

[R03] 只读变量
来源：http://cy.wgjwhj.cn

readonly PI=3.14
来源：http://fk.asd995.cn

[R04] 位置参数
来源：http://vp.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nh.bookmarksfly.cn

[R05] 参数默认值
来源：http://wk.shxzukj.cn

name="${1:-default}"
来源：http://tw.hahajie.cn

[R06] 判断命令是否存在
来源：http://kl.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aj.shtwfgs.cn

[R07] if 判断文件
来源：http://rt.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dk.yuntaijiaju.cn

[R08] 数值比较
来源：http://dh.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wm.haigaiapp.cn

[R09] 字符串比较
来源：http://tv.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mw.szsharing.cn

[R10] 正则匹配
来源：http://xx.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gd.bjjhwx.cn

[R11] case 多分支
来源：http://uy.9csxet.cn

case "$1" in
来源：http://vm.shxzukj.cn

start) echo "启动" ;;
来源：http://tr.shxzskj.cn

stop)  echo "停止" ;;
来源：http://jk.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://qm.gzmigu.cn

esac
来源：http://tq.hnjuh.cn

[R12] for 遍历文件
来源：http://vq.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://lb.szsharing.cn

[R13] for 计数循环
来源：http://ha.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://zh.huixiangedu.cn

[R14] C 风格 for
来源：http://qk.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kg.szxytkj.cn

[R15] while 逐行读文件
来源：http://ts.shxzukj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gx.yuexingan06.cn

[R16] until 等待条件
来源：http://ak.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://px.hahajie.cn

[R17] 数组定义与取值
来源：http://ge.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://un.haigaiapp.cn

[R18] 遍历数组
来源：http://fc.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fj.hahajie.cn

[R19] 数组长度
来源：http://up.jctech888.com.cn

echo "${#arr[@]}"
来源：http://dt.colortex.cn

[R20] 关联数组（字典）
来源：http://ko.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ye.szsharing.cn

[R21] 字符串长度
来源：http://tn.szxytkj.cn

echo "${#s}"
来源：http://or.bookmarksfly.cn

[R22] 截取子串
来源：http://bf.muxihuayi.cn

echo "${s:0:5}"
来源：http://jw.jctech888.com.cn

[R23] 字符串替换
来源：http://ar.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oc.huixiangedu.cn

[R24] 大小写转换
来源：http://zm.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://di.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://ew.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ks.muxihuayi.cn

[R26] 命令替换
来源：http://yt.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://vb.huixiangedu.cn

[R27] 算术展开
来源：http://pu.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://ql.asd995.cn

[R28] 浮点运算
来源：http://lb.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://kz.asd995.cn

[R29] 定义函数
来源：http://ly.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vz.huanxung.cn

[R30] 函数返回状态码
来源：http://qp.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://mh.gzmigu.cn

[R31] 局部变量
来源：http://za.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://sj.521024.cn

[R32] 参数个数校验
来源：http://ea.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kk.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://gi.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ln.huixiangedu.cn

[R34] 退出时清理
来源：http://nd.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ed.jctech888.com.cn

[R35] 后台执行并等待
来源：http://gb.szxytkj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nn.panjiajie.cn

[R36] 并发执行多个任务
来源：http://fv.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://we.asd995.cn

[R37] 把输出赋给变量
来源：http://gg.huixinmuqiang.cn

files=$(ls -1)
来源：http://lz.panjiajie.cn

[R38] 管道串联
来源：http://ps.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://la.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://ur.wgjwhj.cn

cmd > out.log 2>&1
来源：http://vx.huixinmuqiang.cn

[R40] 追加写日志
来源：http://sb.lnxyls.cn

echo "log" >> out.log
来源：http://fr.newstarts.cn

[R41] 丢弃输出
来源：http://vh.nicolike.cn

cmd >/dev/null 2>&1
来源：http://yb.jctech888.com.cn

[R42] 输入重定向
来源：http://fe.colortex.cn

wc -l < a.txt
来源：http://oj.bjjhwx.cn

[R43] 按名字查找文件
来源：http://rv.shtwfgs.cn

find . -name "*.log" -type f
来源：http://vl.haigaiapp.cn

[R44] 按修改时间查找
来源：http://pf.shxzukj.cn

find . -mtime -7 -type f
来源：http://lu.shxzskj.cn

[R45] 批量删除
来源：http://yh.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://xw.newstarts.cn

[R46] 递归替换文件内容
来源：http://gc.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qs.newstarts.cn

[R47] sed 单行替换
来源：http://vb.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lx.shtwfgs.cn

[R48] awk 取指定列
来源：http://an.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://br.colortex.cn

[R49] awk 带条件
来源：http://jj.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qb.gzmigu.cn

[R50] awk 求和
来源：http://ir.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aj.nicolike.cn

[R51] 排序去重取前几
来源：http://ln.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://re.huixinmuqiang.cn

[R52] 统计行数
来源：http://lc.haigaiapp.cn

wc -l a.txt
来源：http://ok.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://pg.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pv.panjiajie.cn

[R54] 比较两个文件
来源：http://ha.nszjky.cn

diff a.txt b.txt
来源：http://xd.huixiangedu.cn

[R55] 压缩与解压
来源：http://qp.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nv.shxzskj.cn

[R56] 远程拷贝
来源：http://fx.shxzskj.cn

scp file user@host:/path/
来源：http://oc.521024.cn

[R57] 远程执行命令
来源：http://wi.shxzskj.cn

ssh user@host 'uptime'
来源：http://nu.gzmigu.cn

[R58] 下载文件
来源：http://tm.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tc.newstarts.cn

[R59] 发 POST JSON
来源：http://ij.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cj.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://xu.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nl.shtwfgs.cn

[R61] 磁盘占用
来源：http://wh.hnjuh.cn

df -h;  du -sh *
来源：http://ec.nszjky.cn

[R62] 找最占空间的文件
来源：http://ng.asd995.cn

du -ah . | sort -rh | head -10
来源：http://mu.wgjwhj.cn

[R63] 内存与进程
来源：http://oo.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://ww.hnjuh.cn

[R64] 结束进程
来源：http://kp.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://yw.bjjhwx.cn

[R65] 查看端口占用
来源：http://wx.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dw.bjjhwx.cn

[R66] 定时任务
来源：http://kk.bjjhwx.cn

crontab -e;  crontab -l
来源：http://ac.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://jl.wgjwhj.cn

openssl rand -hex 16
来源：http://oy.hahajie.cn

[R68] 计算文件校验值
来源：http://ne.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oo.huanxung.cn

[R69] 生成随机密码
来源：http://jr.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://yd.szxytkj.cn

[R70] 时间戳与互转
来源：http://ok.hahajie.cn

date +%s;  date -d @1700000000
来源：http://of.gzmigu.cn

[R71] 日期格式化
来源：http://ms.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yn.nicolike.cn

[R72] 等待端口就绪
来源：http://ba.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gp.shxzukj.cn

[R73] 分割大日志
来源：http://kj.haigaiapp.cn

split -l 1000 big.log part_
来源：http://yi.521024.cn

[R74] 批量重命名
来源：http://lm.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nf.huanxung.cn

[R75] 导出环境变量
来源：http://lp.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://zp.colortex.cn

[R76] 使用临时文件
来源：http://df.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lk.9csxet.cn

[R77] 读取用户输入
来源：http://mw.muxihuayi.cn

read -rp "请输入: " ans
来源：http://tf.hnjuh.cn

[R78] 交互式菜单
来源：http://je.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yz.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ta.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bm.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://xi.9csxet.cn

time ./run.sh
来源：http://ew.szxytkj.cn

================================================================================
来源：http://yv.521024.cn

S. C / C++ 专题
来源：http://al.szxytkj.cn

================================================================================
来源：http://bo.huixinmuqiang.cn

[S01] C：Hello World
来源：http://px.colortex.cn

#include <stdio.h>
来源：http://tr.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ij.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://ju.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://it.bjjhwx.cn

[S03] C：读入整数
来源：http://aa.huanxung.cn

int x; scanf("%d", &x);
来源：http://to.newstarts.cn

[S04] C：字符串复制
来源：http://hm.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xh.colortex.cn

[S05] C：字符串长度
来源：http://kb.newstarts.cn

strlen(s)
来源：http://ro.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://zu.newstarts.cn

strcmp(a, b) == 0
来源：http://lg.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://dq.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pl.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://sx.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eb.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://ju.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jt.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://gu.huanxung.cn

int *p = &a;  *p = 5;
来源：http://qn.hnjuh.cn

[S11] C：逐行读文件
来源：http://wg.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://id.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uu.newstarts.cn

fclose(f);
来源：http://tj.szxytkj.cn

[S12] C：写文件
来源：http://nb.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ei.asd995.cn

[S13] C：宏定义
来源：http://am.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cp.asd995.cn

[S14] C：枚举
来源：http://cu.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://gk.nicolike.cn

[S15] C：类型转换
来源：http://uv.shxzskj.cn

(double) a / b
来源：http://dl.huixiangedu.cn

[S16] C：位操作置位
来源：http://yf.jctech888.com.cn

x |= (1 << 3);
来源：http://it.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://qs.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aa.szxytkj.cn

[S18] C：命令行参数
来源：http://dy.panjiajie.cn

int main(int argc, char **argv)
来源：http://hr.bookmarksfly.cn

[S19] C：快速排序
来源：http://hx.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qw.shtwfgs.cn

[S20] C：二分查找
来源：http://bn.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jy.lnxyls.cn

[S21] C：字符类别判断
来源：http://wi.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://et.shxzukj.cn

[S22] C：字符串转数字
来源：http://jt.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gc.shxzukj.cn

[S23] C：随机数
来源：http://nx.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aw.chemitech.net.cn

[S24] C：获取本地时间
来源：http://zt.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ug.newstarts.cn

[S25] C：内存拷贝
来源：http://th.lnxyls.cn

memcpy(dst, src, n);
来源：http://gc.haigaiapp.cn

[S26] C：内存清零
来源：http://qk.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://mb.hahajie.cn

[S27] C：定义常量
来源：http://ro.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://wi.9csxet.cn

[S28] C：静态变量
来源：http://pn.szxytkj.cn

static int counter = 0;
来源：http://gj.shxzskj.cn

[S29] C：变参函数
来源：http://sh.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uv.bjjhwx.cn

[S30] C：头文件保护
来源：http://iz.hahajie.cn

#ifndef X_H
来源：http://yi.shtwfgs.cn

#define X_H
来源：http://vc.nicolike.cn

#endif
来源：http://nw.bookmarksfly.cn

[S31] C++：Hello World
来源：http://ue.newstarts.cn

#include <iostream>
来源：http://pi.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://oc.huixinmuqiang.cn

[S32] C++：字符串
来源：http://hw.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://wm.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://dz.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fe.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://xm.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://sc.jctech888.com.cn

[S35] C++：map
来源：http://bh.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://km.hnjuh.cn

[S36] C++：unordered_map
来源：http://ul.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://if.asd995.cn

[S37] C++：set
来源：http://xd.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wj.nszjky.cn

[S38] C++：排序
来源：http://pk.colortex.cn

std::sort(v.begin(), v.end());
来源：http://be.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://oy.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yb.shxzskj.cn

[S40] C++：查找元素
来源：http://xc.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yl.huanxung.cn

[S41] C++：类与构造函数
来源：http://yf.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ly.asd995.cn

[S42] C++：继承与虚函数
来源：http://bc.521024.cn

class B : public Base { public: void f() override {} };
来源：http://na.colortex.cn

[S43] C++：智能指针
来源：http://fk.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://mx.bookmarksfly.cn

[S44] C++：引用传参
来源：http://jm.asd995.cn

void inc(int &x) { ++x; }
来源：http://mt.muxihuayi.cn

[S45] C++：lambda
来源：http://ug.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pk.szsharing.cn

[S46] C++：函数模板
来源：http://un.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://je.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://ke.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qk.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://qk.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vx.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://yv.panjiajie.cn

[S49] C++：写文件
来源：http://tz.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vz.huixiangedu.cn

[S50] C++：格式化数字
来源：http://ie.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bx.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://xo.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://yy.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://hd.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://rl.haigaiapp.cn

[S53] C++：移动语义
来源：http://yh.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://xp.shtwfgs.cn

[S54] C++：异常处理
来源：http://lk.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ph.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://vy.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oj.szsharing.cn

[S56] C++：optional
来源：http://tv.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mc.hnjuh.cn

[S57] C++：编译期常量
来源：http://vq.521024.cn

constexpr int N = 10;
来源：http://eb.shxzskj.cn

[S58] C++：命名空间
来源：http://ab.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://vo.nszjky.cn

[S59] C++：静态断言
来源：http://qe.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cc.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://rn.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rm.huixinmuqiang.cn

================================================================================
来源：http://vk.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xh.asd995.cn

================================================================================
来源：http://tv.newstarts.cn

[T01] Kotlin：Hello World
来源：http://ku.nszjky.cn

println("Hello")
来源：http://np.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ff.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jo.szsharing.cn


<!-- 参考信息 -->