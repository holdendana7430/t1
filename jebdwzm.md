代发 wailian999

set -euo pipefail
来源：http://bj.shxzukj.cn

[R02] 变量赋值与使用
来源：http://ye.colortex.cn

name="Tom"; echo "$name"
来源：http://qp.wgjwhj.cn

[R03] 只读变量
来源：http://io.shxzukj.cn

readonly PI=3.14
来源：http://uu.szxytkj.cn

[R04] 位置参数
来源：http://ol.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yq.9csxet.cn

[R05] 参数默认值
来源：http://qh.bookmarksfly.cn

name="${1:-default}"
来源：http://pv.lnxyls.cn

[R06] 判断命令是否存在
来源：http://tg.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lq.gzmigu.cn

[R07] if 判断文件
来源：http://ea.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fi.hahajie.cn

[R08] 数值比较
来源：http://eh.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xs.jianghongdianzi.cn

[R09] 字符串比较
来源：http://dx.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qj.bookmarksfly.cn

[R10] 正则匹配
来源：http://zx.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kx.shtwfgs.cn

[R11] case 多分支
来源：http://sk.nicolike.cn

case "$1" in
来源：http://va.lnxyls.cn

start) echo "启动" ;;
来源：http://ek.nicolike.cn

stop)  echo "停止" ;;
来源：http://sm.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://mf.hahajie.cn

esac
来源：http://dc.szsharing.cn

[R12] for 遍历文件
来源：http://ao.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://zh.wgjwhj.cn

[R13] for 计数循环
来源：http://hx.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://ih.jianghongdianzi.cn

[R14] C 风格 for
来源：http://yk.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zm.colortex.cn

[R15] while 逐行读文件
来源：http://dz.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bi.hahajie.cn

[R16] until 等待条件
来源：http://bo.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pi.yuexingan06.cn

[R17] 数组定义与取值
来源：http://xt.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ec.newstarts.cn

[R18] 遍历数组
来源：http://ib.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://il.bjjhwx.cn

[R19] 数组长度
来源：http://df.panjiajie.cn

echo "${#arr[@]}"
来源：http://zv.gzmigu.cn

[R20] 关联数组（字典）
来源：http://ln.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://do.jctech888.com.cn

[R21] 字符串长度
来源：http://yx.szsharing.cn

echo "${#s}"
来源：http://jz.muxihuayi.cn

[R22] 截取子串
来源：http://kj.newstarts.cn

echo "${s:0:5}"
来源：http://rc.huixiangedu.cn

[R23] 字符串替换
来源：http://fy.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vz.newstarts.cn

[R24] 大小写转换
来源：http://gy.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qu.9csxet.cn

[R25] 去后缀 / 去前缀
来源：http://th.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vx.shtwfgs.cn

[R26] 命令替换
来源：http://jh.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://ms.chemitech.net.cn

[R27] 算术展开
来源：http://gz.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://ai.shxzskj.cn

[R28] 浮点运算
来源：http://su.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://sn.huixiangedu.cn

[R29] 定义函数
来源：http://vf.newstarts.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rn.521024.cn

[R30] 函数返回状态码
来源：http://zm.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://cj.muxihuayi.cn

[R31] 局部变量
来源：http://nl.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://nr.lnxyls.cn

[R32] 参数个数校验
来源：http://kc.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://my.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://zt.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ou.shxzskj.cn

[R34] 退出时清理
来源：http://tt.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nb.huixiangedu.cn

[R35] 后台执行并等待
来源：http://en.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yn.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://nm.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qs.shxzskj.cn

[R37] 把输出赋给变量
来源：http://ow.huixiangedu.cn

files=$(ls -1)
来源：http://sg.szsharing.cn

[R38] 管道串联
来源：http://du.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://cb.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://qm.haigaiapp.cn

cmd > out.log 2>&1
来源：http://nz.colortex.cn

[R40] 追加写日志
来源：http://ta.hnjuh.cn

echo "log" >> out.log
来源：http://et.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://yi.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://qj.colortex.cn

[R42] 输入重定向
来源：http://rv.521024.cn

wc -l < a.txt
来源：http://bb.bjjhwx.cn

[R43] 按名字查找文件
来源：http://qb.chemitech.net.cn

find . -name "*.log" -type f
来源：http://wl.9csxet.cn

[R44] 按修改时间查找
来源：http://cf.shtwfgs.cn

find . -mtime -7 -type f
来源：http://rv.hnjuh.cn

[R45] 批量删除
来源：http://ce.521024.cn

find . -name "*.tmp" -delete
来源：http://pk.hnjuh.cn

[R46] 递归替换文件内容
来源：http://jr.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ir.jianghongdianzi.cn

[R47] sed 单行替换
来源：http://vl.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gf.wgjwhj.cn

[R48] awk 取指定列
来源：http://ep.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://zs.colortex.cn

[R49] awk 带条件
来源：http://ff.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lj.jianghongdianzi.cn

[R50] awk 求和
来源：http://ey.szxytkj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hp.shxzskj.cn

[R51] 排序去重取前几
来源：http://zt.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xk.bjjhwx.cn

[R52] 统计行数
来源：http://yy.lnxyls.cn

wc -l a.txt
来源：http://hd.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://bw.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ny.asd995.cn

[R54] 比较两个文件
来源：http://sq.huanxung.cn

diff a.txt b.txt
来源：http://kv.521024.cn

[R55] 压缩与解压
来源：http://wj.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ba.9csxet.cn

[R56] 远程拷贝
来源：http://kk.shtwfgs.cn

scp file user@host:/path/
来源：http://mb.jctech888.com.cn

[R57] 远程执行命令
来源：http://bh.wgjwhj.cn

ssh user@host 'uptime'
来源：http://nd.jianghongdianzi.cn

[R58] 下载文件
来源：http://ya.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ky.jctech888.com.cn

[R59] 发 POST JSON
来源：http://rf.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zp.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://po.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bk.huixiangedu.cn

[R61] 磁盘占用
来源：http://ym.521024.cn

df -h;  du -sh *
来源：http://to.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://fh.jctech888.com.cn

du -ah . | sort -rh | head -10
来源：http://bb.yuexingan06.cn

[R63] 内存与进程
来源：http://fj.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://hf.huixiangedu.cn

[R64] 结束进程
来源：http://qg.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://xa.gzmigu.cn

[R65] 查看端口占用
来源：http://za.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://su.haigaiapp.cn

[R66] 定时任务
来源：http://bj.hnjuh.cn

crontab -e;  crontab -l
来源：http://ch.szsharing.cn

[R67] 生成随机十六进制串
来源：http://iz.lnxyls.cn

openssl rand -hex 16
来源：http://bj.shtwfgs.cn

[R68] 计算文件校验值
来源：http://dz.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sa.shxzukj.cn

[R69] 生成随机密码
来源：http://zf.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://ug.shxzskj.cn

[R70] 时间戳与互转
来源：http://cl.colortex.cn

date +%s;  date -d @1700000000
来源：http://hh.jianghongdianzi.cn

[R71] 日期格式化
来源：http://qh.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nq.huixiangedu.cn

[R72] 等待端口就绪
来源：http://oy.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://er.9csxet.cn

[R73] 分割大日志
来源：http://ai.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ri.muxihuayi.cn

[R74] 批量重命名
来源：http://of.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xk.shxzskj.cn

[R75] 导出环境变量
来源：http://yk.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://dy.hahajie.cn

[R76] 使用临时文件
来源：http://cw.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://se.newstarts.cn

[R77] 读取用户输入
来源：http://zp.huixiangedu.cn

read -rp "请输入: " ans
来源：http://ky.shxzukj.cn

[R78] 交互式菜单
来源：http://zw.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lv.lnxyls.cn

[R79] 解析命令行选项
来源：http://qw.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lt.szsharing.cn

[R80] 查看脚本执行耗时
来源：http://tq.panjiajie.cn

time ./run.sh
来源：http://fb.colortex.cn

================================================================================
来源：http://ea.bookmarksfly.cn

S. C / C++ 专题
来源：http://ek.lnxyls.cn

================================================================================
来源：http://ee.panjiajie.cn

[S01] C：Hello World
来源：http://vx.shxzskj.cn

#include <stdio.h>
来源：http://zu.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wy.asd995.cn

[S02] C：变量与格式化输出
来源：http://sj.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://sb.muxihuayi.cn

[S03] C：读入整数
来源：http://ld.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://ac.huanxung.cn

[S04] C：字符串复制
来源：http://qn.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sc.9csxet.cn

[S05] C：字符串长度
来源：http://qv.hnjuh.cn

strlen(s)
来源：http://pl.shtwfgs.cn

[S06] C：字符串比较
来源：http://vm.chemitech.net.cn

strcmp(a, b) == 0
来源：http://cp.lnxyls.cn

[S07] C：数组遍历求和
来源：http://wm.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ds.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://yd.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pb.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://pk.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ut.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://vq.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://hl.shtwfgs.cn

[S11] C：逐行读文件
来源：http://cd.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://ds.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kt.lnxyls.cn

fclose(f);
来源：http://wv.wgjwhj.cn

[S12] C：写文件
来源：http://sl.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sr.gzmigu.cn

[S13] C：宏定义
来源：http://wl.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vp.huanxung.cn

[S14] C：枚举
来源：http://wn.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://rc.shxzukj.cn

[S15] C：类型转换
来源：http://iw.jctech888.com.cn

(double) a / b
来源：http://zn.yuexingan06.cn

[S16] C：位操作置位
来源：http://la.hnjuh.cn

x |= (1 << 3);
来源：http://qr.nicolike.cn

[S17] C：安全拼接字符串
来源：http://zj.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wl.hnjuh.cn

[S18] C：命令行参数
来源：http://ds.muxihuayi.cn

int main(int argc, char **argv)
来源：http://de.panjiajie.cn

[S19] C：快速排序
来源：http://pv.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ma.muxihuayi.cn

[S20] C：二分查找
来源：http://dc.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ni.chemitech.net.cn

[S21] C：字符类别判断
来源：http://bo.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ze.hahajie.cn

[S22] C：字符串转数字
来源：http://hn.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ax.huixiangedu.cn

[S23] C：随机数
来源：http://va.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uv.huixiangedu.cn

[S24] C：获取本地时间
来源：http://bp.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://no.chemitech.net.cn

[S25] C：内存拷贝
来源：http://au.bjjhwx.cn

memcpy(dst, src, n);
来源：http://qb.nszjky.cn

[S26] C：内存清零
来源：http://zp.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://wk.huanxung.cn

[S27] C：定义常量
来源：http://su.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://qh.bookmarksfly.cn

[S28] C：静态变量
来源：http://qp.shxzskj.cn

static int counter = 0;
来源：http://yq.bjjhwx.cn

[S29] C：变参函数
来源：http://ft.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wx.nszjky.cn

[S30] C：头文件保护
来源：http://qg.hahajie.cn

#ifndef X_H
来源：http://er.shxzukj.cn

#define X_H
来源：http://co.shtwfgs.cn

#endif
来源：http://mp.jctech888.com.cn

[S31] C++：Hello World
来源：http://wl.nszjky.cn

#include <iostream>
来源：http://hb.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://pb.colortex.cn

[S32] C++：字符串
来源：http://mh.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://hd.521024.cn

[S33] C++：vector 增删
来源：http://sz.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pw.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://os.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://wq.bjjhwx.cn

[S35] C++：map
来源：http://ha.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rd.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://nu.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jo.bookmarksfly.cn

[S37] C++：set
来源：http://qp.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://as.huanxung.cn

[S38] C++：排序
来源：http://io.asd995.cn

std::sort(v.begin(), v.end());
来源：http://zq.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://iu.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lm.chemitech.net.cn

[S40] C++：查找元素
来源：http://ow.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ct.9csxet.cn

[S41] C++：类与构造函数
来源：http://fm.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://un.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://vj.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://jg.9csxet.cn

[S43] C++：智能指针
来源：http://xl.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://aj.asd995.cn

[S44] C++：引用传参
来源：http://wk.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://pl.9csxet.cn

[S45] C++：lambda
来源：http://gg.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qh.bjjhwx.cn

[S46] C++：函数模板
来源：http://ig.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xx.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://cy.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gp.hahajie.cn

[S48] C++：逐行读文件
来源：http://vi.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qt.colortex.cn

while (std::getline(in, line)) { }
来源：http://mo.chemitech.net.cn

[S49] C++：写文件
来源：http://yk.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nc.gzmigu.cn

[S50] C++：格式化数字
来源：http://nb.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ji.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://fr.colortex.cn

static_cast<double>(a) / b
来源：http://ua.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://vz.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://qw.yuexingan06.cn

[S53] C++：移动语义
来源：http://kr.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://oc.shtwfgs.cn

[S54] C++：异常处理
来源：http://go.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zv.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://nx.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sb.521024.cn

[S56] C++：optional
来源：http://bz.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://om.huanxung.cn

[S57] C++：编译期常量
来源：http://qi.shxzskj.cn

constexpr int N = 10;
来源：http://yi.gzmigu.cn

[S58] C++：命名空间
来源：http://vp.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://ru.chemitech.net.cn

[S59] C++：静态断言
来源：http://vq.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ts.asd995.cn

[S60] C++：遍历并删除元素
来源：http://bc.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vf.jianghongdianzi.cn

================================================================================
来源：http://tm.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ff.jctech888.com.cn

================================================================================
来源：http://vf.asd995.cn

[T01] Kotlin：Hello World
来源：http://la.colortex.cn

println("Hello")
来源：http://wi.hahajie.cn

[T02] Kotlin：变量
来源：http://be.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mx.panjiajie.cn


<!-- 参考信息 -->