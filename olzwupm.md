代发 wailian999

R. Bash 专题
来源：http://hf.lnxyls.cn

================================================================================
来源：http://gp.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://hc.szxytkj.cn

#!/usr/bin/env bash
来源：http://yb.yuntaijiaju.cn

set -euo pipefail
来源：http://ro.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://hx.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://nu.hnjuh.cn

[R03] 只读变量
来源：http://kl.chemitech.net.cn

readonly PI=3.14
来源：http://ye.szxytkj.cn

[R04] 位置参数
来源：http://ih.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pd.muxihuayi.cn

[R05] 参数默认值
来源：http://aa.asd995.cn

name="${1:-default}"
来源：http://el.hahajie.cn

[R06] 判断命令是否存在
来源：http://uy.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lg.jctech888.com.cn

[R07] if 判断文件
来源：http://hp.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ij.hahajie.cn

[R08] 数值比较
来源：http://we.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ft.szxytkj.cn

[R09] 字符串比较
来源：http://yg.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oh.9csxet.cn

[R10] 正则匹配
来源：http://pk.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qd.panjiajie.cn

[R11] case 多分支
来源：http://uv.chemitech.net.cn

case "$1" in
来源：http://tx.hahajie.cn

start) echo "启动" ;;
来源：http://gk.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://xa.szsharing.cn

*)     echo "未知命令" ;;
来源：http://bf.9csxet.cn

esac
来源：http://ku.panjiajie.cn

[R12] for 遍历文件
来源：http://mk.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://yo.panjiajie.cn

[R13] for 计数循环
来源：http://vb.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://pa.shxzskj.cn

[R14] C 风格 for
来源：http://lu.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ts.wgjwhj.cn

[R15] while 逐行读文件
来源：http://cy.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dm.huixiangedu.cn

[R16] until 等待条件
来源：http://jp.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ip.szxytkj.cn

[R17] 数组定义与取值
来源：http://qj.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dg.jctech888.com.cn

[R18] 遍历数组
来源：http://zc.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cz.colortex.cn

[R19] 数组长度
来源：http://zx.yuexingan06.cn

echo "${#arr[@]}"
来源：http://mx.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://gy.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sj.521024.cn

[R21] 字符串长度
来源：http://jk.shxzukj.cn

echo "${#s}"
来源：http://ak.newstarts.cn

[R22] 截取子串
来源：http://bf.huixiangedu.cn

echo "${s:0:5}"
来源：http://yj.nicolike.cn

[R23] 字符串替换
来源：http://vm.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ke.panjiajie.cn

[R24] 大小写转换
来源：http://uh.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ik.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://xz.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://np.521024.cn

[R26] 命令替换
来源：http://xy.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://ho.lnxyls.cn

[R27] 算术展开
来源：http://qb.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://fb.muxihuayi.cn

[R28] 浮点运算
来源：http://ha.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://bz.shxzukj.cn

[R29] 定义函数
来源：http://tc.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fg.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://px.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://rj.lnxyls.cn

[R31] 局部变量
来源：http://cr.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://tz.chemitech.net.cn

[R32] 参数个数校验
来源：http://qn.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fa.jctech888.com.cn

[R33] 捕获错误并提示行号
来源：http://ol.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bj.shtwfgs.cn

[R34] 退出时清理
来源：http://sh.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://em.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://ax.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ax.szsharing.cn

[R36] 并发执行多个任务
来源：http://gn.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ei.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://pc.shtwfgs.cn

files=$(ls -1)
来源：http://bn.lnxyls.cn

[R38] 管道串联
来源：http://wm.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://dm.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://wb.nicolike.cn

cmd > out.log 2>&1
来源：http://dc.nszjky.cn

[R40] 追加写日志
来源：http://lf.jctech888.com.cn

echo "log" >> out.log
来源：http://tz.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://iy.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://ji.colortex.cn

[R42] 输入重定向
来源：http://zi.bookmarksfly.cn

wc -l < a.txt
来源：http://jr.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://re.shxzskj.cn

find . -name "*.log" -type f
来源：http://iw.shtwfgs.cn

[R44] 按修改时间查找
来源：http://gz.huanxung.cn

find . -mtime -7 -type f
来源：http://ux.huixinmuqiang.cn

[R45] 批量删除
来源：http://wo.nszjky.cn

find . -name "*.tmp" -delete
来源：http://gg.521024.cn

[R46] 递归替换文件内容
来源：http://ys.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oy.521024.cn

[R47] sed 单行替换
来源：http://ce.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ic.huixinmuqiang.cn

[R48] awk 取指定列
来源：http://yb.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://mw.521024.cn

[R49] awk 带条件
来源：http://go.bookmarksfly.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://le.shxzskj.cn

[R50] awk 求和
来源：http://qd.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sc.yuexingan06.cn

[R51] 排序去重取前几
来源：http://qb.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yt.jctech888.com.cn

[R52] 统计行数
来源：http://td.521024.cn

wc -l a.txt
来源：http://qb.521024.cn

[R53] 查看文件头与实时尾
来源：http://rs.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qz.szxytkj.cn

[R54] 比较两个文件
来源：http://nb.huixinmuqiang.cn

diff a.txt b.txt
来源：http://kd.lnxyls.cn

[R55] 压缩与解压
来源：http://jf.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gs.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://jz.yuntaijiaju.cn

scp file user@host:/path/
来源：http://ay.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://qw.shxzskj.cn

ssh user@host 'uptime'
来源：http://ei.jianghongdianzi.cn

[R58] 下载文件
来源：http://up.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sa.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://lx.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zj.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://wd.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fx.jctech888.com.cn

[R61] 磁盘占用
来源：http://pt.chemitech.net.cn

df -h;  du -sh *
来源：http://ov.shxzukj.cn

[R62] 找最占空间的文件
来源：http://rx.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://pb.521024.cn

[R63] 内存与进程
来源：http://sx.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://pr.huixiangedu.cn

[R64] 结束进程
来源：http://gn.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://za.nicolike.cn

[R65] 查看端口占用
来源：http://an.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oy.521024.cn

[R66] 定时任务
来源：http://ai.panjiajie.cn

crontab -e;  crontab -l
来源：http://ii.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://gt.asd995.cn

openssl rand -hex 16
来源：http://fb.szxytkj.cn

[R68] 计算文件校验值
来源：http://sy.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ib.hnjuh.cn

[R69] 生成随机密码
来源：http://pz.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ik.szsharing.cn

[R70] 时间戳与互转
来源：http://nr.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://ec.jctech888.com.cn

[R71] 日期格式化
来源：http://sv.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://th.huanxung.cn

[R72] 等待端口就绪
来源：http://ok.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jn.hahajie.cn

[R73] 分割大日志
来源：http://kw.jctech888.com.cn

split -l 1000 big.log part_
来源：http://ix.bookmarksfly.cn

[R74] 批量重命名
来源：http://qc.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jb.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://hg.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://kd.hahajie.cn

[R76] 使用临时文件
来源：http://ll.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bf.shtwfgs.cn

[R77] 读取用户输入
来源：http://co.hnjuh.cn

read -rp "请输入: " ans
来源：http://ym.jctech888.com.cn

[R78] 交互式菜单
来源：http://qx.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vl.shtwfgs.cn

[R79] 解析命令行选项
来源：http://ei.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eh.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://ft.haigaiapp.cn

time ./run.sh
来源：http://wu.9csxet.cn

================================================================================
来源：http://zi.chemitech.net.cn

S. C / C++ 专题
来源：http://ap.gzmigu.cn

================================================================================
来源：http://ov.muxihuayi.cn

[S01] C：Hello World
来源：http://ot.bookmarksfly.cn

#include <stdio.h>
来源：http://rs.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bc.huixiangedu.cn

[S02] C：变量与格式化输出
来源：http://ob.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://zj.chemitech.net.cn

[S03] C：读入整数
来源：http://gm.9csxet.cn

int x; scanf("%d", &x);
来源：http://bl.panjiajie.cn

[S04] C：字符串复制
来源：http://de.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ce.nszjky.cn

[S05] C：字符串长度
来源：http://nj.wgjwhj.cn

strlen(s)
来源：http://xz.nicolike.cn

[S06] C：字符串比较
来源：http://fr.panjiajie.cn

strcmp(a, b) == 0
来源：http://xh.shxzskj.cn

[S07] C：数组遍历求和
来源：http://vp.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sq.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://ir.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pc.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://dp.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rk.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://px.nszjky.cn

int *p = &a;  *p = 5;
来源：http://hb.chemitech.net.cn

[S11] C：逐行读文件
来源：http://qn.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://df.szxytkj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ja.hahajie.cn

fclose(f);
来源：http://au.colortex.cn

[S12] C：写文件
来源：http://as.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ts.yuexingan06.cn

[S13] C：宏定义
来源：http://kp.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lr.szsharing.cn

[S14] C：枚举
来源：http://ib.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://bc.shxzskj.cn

[S15] C：类型转换
来源：http://bx.nicolike.cn

(double) a / b
来源：http://yw.huixiangedu.cn

[S16] C：位操作置位
来源：http://mh.szxytkj.cn

x |= (1 << 3);
来源：http://xx.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://yq.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dl.521024.cn

[S18] C：命令行参数
来源：http://jg.chemitech.net.cn

int main(int argc, char **argv)
来源：http://ju.521024.cn

[S19] C：快速排序
来源：http://gg.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cm.yuntaijiaju.cn

[S20] C：二分查找
来源：http://ar.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tl.bjjhwx.cn

[S21] C：字符类别判断
来源：http://wl.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dq.521024.cn

[S22] C：字符串转数字
来源：http://qg.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hq.nszjky.cn

[S23] C：随机数
来源：http://ra.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://te.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://qu.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sg.huanxung.cn

[S25] C：内存拷贝
来源：http://kk.haigaiapp.cn

memcpy(dst, src, n);
来源：http://re.newstarts.cn

[S26] C：内存清零
来源：http://sp.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://sj.huixiangedu.cn

[S27] C：定义常量
来源：http://aw.shxzukj.cn

const double PI = 3.14159;
来源：http://gg.huixinmuqiang.cn

[S28] C：静态变量
来源：http://io.asd995.cn

static int counter = 0;
来源：http://xu.bookmarksfly.cn

[S29] C：变参函数
来源：http://se.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hf.muxihuayi.cn

[S30] C：头文件保护
来源：http://yp.yuntaijiaju.cn

#ifndef X_H
来源：http://yp.hahajie.cn

#define X_H
来源：http://cf.bjjhwx.cn

#endif
来源：http://wo.shxzskj.cn

[S31] C++：Hello World
来源：http://lu.hahajie.cn

#include <iostream>
来源：http://vr.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://wc.jctech888.com.cn

[S32] C++：字符串
来源：http://uu.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://mf.haigaiapp.cn

[S33] C++：vector 增删
来源：http://xq.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zq.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://dg.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://jg.shtwfgs.cn

[S35] C++：map
来源：http://qw.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://el.chemitech.net.cn

[S36] C++：unordered_map
来源：http://rm.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tp.newstarts.cn

[S37] C++：set
来源：http://ky.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zs.bjjhwx.cn

[S38] C++：排序
来源：http://yt.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://cs.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://fs.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yt.shxzukj.cn

[S40] C++：查找元素
来源：http://nq.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://di.shxzukj.cn

[S41] C++：类与构造函数
来源：http://sl.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rw.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://xm.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://xo.hnjuh.cn

[S43] C++：智能指针
来源：http://ls.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://oe.bookmarksfly.cn

[S44] C++：引用传参
来源：http://uz.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://nj.szxytkj.cn

[S45] C++：lambda
来源：http://vl.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cw.jctech888.com.cn

[S46] C++：函数模板
来源：http://lh.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fm.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://lq.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vp.huanxung.cn

[S48] C++：逐行读文件
来源：http://ni.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zj.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://re.jctech888.com.cn

[S49] C++：写文件
来源：http://qi.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xv.panjiajie.cn

[S50] C++：格式化数字
来源：http://op.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iw.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://uc.muxihuayi.cn

static_cast<double>(a) / b
来源：http://hs.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://yi.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://wn.hahajie.cn

[S53] C++：移动语义
来源：http://zg.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://aq.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://wt.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nw.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://qw.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iy.shxzskj.cn

[S56] C++：optional
来源：http://zy.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://va.asd995.cn

[S57] C++：编译期常量
来源：http://nv.haigaiapp.cn

constexpr int N = 10;
来源：http://mv.haigaiapp.cn

[S58] C++：命名空间
来源：http://xn.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://nc.asd995.cn

[S59] C++：静态断言
来源：http://eu.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://en.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ag.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fo.huanxung.cn

================================================================================
来源：http://sr.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://md.lnxyls.cn

================================================================================
来源：http://mp.huixinmuqiang.cn


<!-- 参考信息 -->