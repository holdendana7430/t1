代发 wailian999

set -euo pipefail
来源：http://yq.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://vs.gzmigu.cn

name="Tom"; echo "$name"
来源：http://qv.huanxung.cn

[R03] 只读变量
来源：http://tb.nicolike.cn

readonly PI=3.14
来源：http://xg.bookmarksfly.cn

[R04] 位置参数
来源：http://sc.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mf.bjjhwx.cn

[R05] 参数默认值
来源：http://xn.jianghongdianzi.cn

name="${1:-default}"
来源：http://iv.hnjuh.cn

[R06] 判断命令是否存在
来源：http://vs.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yo.gzmigu.cn

[R07] if 判断文件
来源：http://cf.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pc.yuntaijiaju.cn

[R08] 数值比较
来源：http://qa.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nt.asd995.cn

[R09] 字符串比较
来源：http://dd.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ul.9csxet.cn

[R10] 正则匹配
来源：http://mx.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ff.lnxyls.cn

[R11] case 多分支
来源：http://hj.newstarts.cn

case "$1" in
来源：http://jp.panjiajie.cn

start) echo "启动" ;;
来源：http://hh.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://kq.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://fg.jctech888.com.cn

esac
来源：http://mk.9csxet.cn

[R12] for 遍历文件
来源：http://kw.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://gu.bookmarksfly.cn

[R13] for 计数循环
来源：http://dx.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://cf.shxzskj.cn

[R14] C 风格 for
来源：http://we.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sh.chemitech.net.cn

[R15] while 逐行读文件
来源：http://pg.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wo.nicolike.cn

[R16] until 等待条件
来源：http://sc.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hv.haigaiapp.cn

[R17] 数组定义与取值
来源：http://nk.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nb.nicolike.cn

[R18] 遍历数组
来源：http://ce.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wy.haigaiapp.cn

[R19] 数组长度
来源：http://xb.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ly.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://jm.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wz.nicolike.cn

[R21] 字符串长度
来源：http://gs.szxytkj.cn

echo "${#s}"
来源：http://yv.hnjuh.cn

[R22] 截取子串
来源：http://rk.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://qp.muxihuayi.cn

[R23] 字符串替换
来源：http://oj.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fd.shxzukj.cn

[R24] 大小写转换
来源：http://ch.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ve.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://zr.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fz.panjiajie.cn

[R26] 命令替换
来源：http://ai.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://bv.bookmarksfly.cn

[R27] 算术展开
来源：http://ae.nszjky.cn

echo $((1 + 2 * 3))
来源：http://dc.muxihuayi.cn

[R28] 浮点运算
来源：http://ak.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://dv.huixiangedu.cn

[R29] 定义函数
来源：http://jd.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tu.jctech888.com.cn

[R30] 函数返回状态码
来源：http://vi.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ew.bookmarksfly.cn

[R31] 局部变量
来源：http://wl.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://qy.huanxung.cn

[R32] 参数个数校验
来源：http://fe.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ux.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://hb.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sl.jctech888.com.cn

[R34] 退出时清理
来源：http://vu.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oe.nicolike.cn

[R35] 后台执行并等待
来源：http://ol.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sk.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://si.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://so.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://zc.huanxung.cn

files=$(ls -1)
来源：http://ro.panjiajie.cn

[R38] 管道串联
来源：http://xx.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://sy.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://ju.panjiajie.cn

cmd > out.log 2>&1
来源：http://dd.wgjwhj.cn

[R40] 追加写日志
来源：http://dg.bookmarksfly.cn

echo "log" >> out.log
来源：http://lr.9csxet.cn

[R41] 丢弃输出
来源：http://xh.colortex.cn

cmd >/dev/null 2>&1
来源：http://ya.huixiangedu.cn

[R42] 输入重定向
来源：http://zl.colortex.cn

wc -l < a.txt
来源：http://dm.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://mw.asd995.cn

find . -name "*.log" -type f
来源：http://bf.shtwfgs.cn

[R44] 按修改时间查找
来源：http://la.szxytkj.cn

find . -mtime -7 -type f
来源：http://yb.chemitech.net.cn

[R45] 批量删除
来源：http://jz.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://pl.lnxyls.cn

[R46] 递归替换文件内容
来源：http://hw.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wh.newstarts.cn

[R47] sed 单行替换
来源：http://cb.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mq.huanxung.cn

[R48] awk 取指定列
来源：http://ru.9csxet.cn

awk '{print $1, $3}' a.txt
来源：http://no.gzmigu.cn

[R49] awk 带条件
来源：http://qn.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tr.shtwfgs.cn

[R50] awk 求和
来源：http://xt.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ce.newstarts.cn

[R51] 排序去重取前几
来源：http://am.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://up.huixiangedu.cn

[R52] 统计行数
来源：http://io.muxihuayi.cn

wc -l a.txt
来源：http://lb.521024.cn

[R53] 查看文件头与实时尾
来源：http://yu.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://to.panjiajie.cn

[R54] 比较两个文件
来源：http://xn.gzmigu.cn

diff a.txt b.txt
来源：http://xs.bjjhwx.cn

[R55] 压缩与解压
来源：http://dy.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wm.shxzukj.cn

[R56] 远程拷贝
来源：http://lu.haigaiapp.cn

scp file user@host:/path/
来源：http://lg.shxzskj.cn

[R57] 远程执行命令
来源：http://xn.hahajie.cn

ssh user@host 'uptime'
来源：http://ma.bookmarksfly.cn

[R58] 下载文件
来源：http://ma.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wz.gzmigu.cn

[R59] 发 POST JSON
来源：http://wv.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oe.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://zw.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xn.huixiangedu.cn

[R61] 磁盘占用
来源：http://sc.haigaiapp.cn

df -h;  du -sh *
来源：http://bm.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://dp.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://wi.jctech888.com.cn

[R63] 内存与进程
来源：http://qh.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://yv.shxzskj.cn

[R64] 结束进程
来源：http://yk.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://er.lnxyls.cn

[R65] 查看端口占用
来源：http://pk.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://si.chemitech.net.cn

[R66] 定时任务
来源：http://kw.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://fk.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://ab.szxytkj.cn

openssl rand -hex 16
来源：http://sr.colortex.cn

[R68] 计算文件校验值
来源：http://ya.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wi.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://av.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://te.nszjky.cn

[R70] 时间戳与互转
来源：http://sl.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://lr.huixinmuqiang.cn

[R71] 日期格式化
来源：http://gl.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ue.lnxyls.cn

[R72] 等待端口就绪
来源：http://af.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sq.szxytkj.cn

[R73] 分割大日志
来源：http://fs.9csxet.cn

split -l 1000 big.log part_
来源：http://yv.hahajie.cn

[R74] 批量重命名
来源：http://ki.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sl.asd995.cn

[R75] 导出环境变量
来源：http://jn.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://md.hnjuh.cn

[R76] 使用临时文件
来源：http://bo.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dc.bjjhwx.cn

[R77] 读取用户输入
来源：http://ma.haigaiapp.cn

read -rp "请输入: " ans
来源：http://nc.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://xl.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zv.bjjhwx.cn

[R79] 解析命令行选项
来源：http://qb.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ua.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://xr.haigaiapp.cn

time ./run.sh
来源：http://qf.shxzskj.cn

================================================================================
来源：http://oi.yuntaijiaju.cn

S. C / C++ 专题
来源：http://if.asd995.cn

================================================================================
来源：http://jg.bjjhwx.cn

[S01] C：Hello World
来源：http://jp.nszjky.cn

#include <stdio.h>
来源：http://fx.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bo.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://zx.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://il.hnjuh.cn

[S03] C：读入整数
来源：http://ps.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://uo.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://dx.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kw.bjjhwx.cn

[S05] C：字符串长度
来源：http://px.jctech888.com.cn

strlen(s)
来源：http://wi.bookmarksfly.cn

[S06] C：字符串比较
来源：http://qe.panjiajie.cn

strcmp(a, b) == 0
来源：http://vy.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://vd.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ij.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://aq.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vt.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://ox.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gf.huixiangedu.cn

[S10] C：指针与解引用
来源：http://sa.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://sv.haigaiapp.cn

[S11] C：逐行读文件
来源：http://og.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://cj.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mf.shxzukj.cn

fclose(f);
来源：http://dg.shtwfgs.cn

[S12] C：写文件
来源：http://ga.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xp.9csxet.cn

[S13] C：宏定义
来源：http://mf.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wq.jianghongdianzi.cn

[S14] C：枚举
来源：http://qh.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://bq.yuexingan06.cn

[S15] C：类型转换
来源：http://ax.bjjhwx.cn

(double) a / b
来源：http://gy.muxihuayi.cn

[S16] C：位操作置位
来源：http://zk.huixinmuqiang.cn

x |= (1 << 3);
来源：http://vn.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://vt.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uu.yuexingan06.cn

[S18] C：命令行参数
来源：http://hh.nicolike.cn

int main(int argc, char **argv)
来源：http://zd.521024.cn

[S19] C：快速排序
来源：http://wl.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bl.jctech888.com.cn

[S20] C：二分查找
来源：http://mi.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hm.hahajie.cn

[S21] C：字符类别判断
来源：http://rc.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gc.nicolike.cn

[S22] C：字符串转数字
来源：http://zk.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oj.asd995.cn

[S23] C：随机数
来源：http://mw.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ni.huanxung.cn

[S24] C：获取本地时间
来源：http://vl.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rs.gzmigu.cn

[S25] C：内存拷贝
来源：http://yh.nszjky.cn

memcpy(dst, src, n);
来源：http://ls.nszjky.cn

[S26] C：内存清零
来源：http://ic.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://pu.szsharing.cn

[S27] C：定义常量
来源：http://cx.panjiajie.cn

const double PI = 3.14159;
来源：http://bb.jianghongdianzi.cn

[S28] C：静态变量
来源：http://ne.9csxet.cn

static int counter = 0;
来源：http://hm.shxzskj.cn

[S29] C：变参函数
来源：http://vy.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dy.521024.cn

[S30] C：头文件保护
来源：http://pf.bookmarksfly.cn

#ifndef X_H
来源：http://iy.521024.cn

#define X_H
来源：http://pt.szxytkj.cn

#endif
来源：http://vv.shxzukj.cn

[S31] C++：Hello World
来源：http://qi.shtwfgs.cn

#include <iostream>
来源：http://go.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://wr.huanxung.cn

[S32] C++：字符串
来源：http://ut.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://ww.nicolike.cn

[S33] C++：vector 增删
来源：http://uy.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mv.panjiajie.cn

[S34] C++：遍历 vector
来源：http://jw.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://ps.bjjhwx.cn

[S35] C++：map
来源：http://tm.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ye.nszjky.cn

[S36] C++：unordered_map
来源：http://bd.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nr.szxytkj.cn

[S37] C++：set
来源：http://zo.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mr.wgjwhj.cn

[S38] C++：排序
来源：http://zp.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://dm.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ad.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vw.chemitech.net.cn

[S40] C++：查找元素
来源：http://to.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://td.hahajie.cn

[S41] C++：类与构造函数
来源：http://lx.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://br.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://hk.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://fe.hnjuh.cn

[S43] C++：智能指针
来源：http://sx.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://ka.szsharing.cn

[S44] C++：引用传参
来源：http://le.nszjky.cn

void inc(int &x) { ++x; }
来源：http://cm.521024.cn

[S45] C++：lambda
来源：http://uq.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lz.hnjuh.cn

[S46] C++：函数模板
来源：http://yn.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pu.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://ir.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eo.newstarts.cn

[S48] C++：逐行读文件
来源：http://iu.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zx.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://ds.shxzukj.cn

[S49] C++：写文件
来源：http://pq.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gs.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ou.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wz.nszjky.cn

[S51] C++：显式类型转换
来源：http://kj.huanxung.cn

static_cast<double>(a) / b
来源：http://gz.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://tp.nszjky.cn

int size() const noexcept { return n_; }
来源：http://km.yuexingan06.cn

[S53] C++：移动语义
来源：http://fr.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://tm.asd995.cn

[S54] C++：异常处理
来源：http://uo.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nq.hahajie.cn

[S55] C++：结构化绑定
来源：http://yg.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ie.hahajie.cn

[S56] C++：optional
来源：http://gh.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tc.huanxung.cn

[S57] C++：编译期常量
来源：http://vy.yuexingan06.cn

constexpr int N = 10;
来源：http://jd.hahajie.cn

[S58] C++：命名空间
来源：http://lb.521024.cn

namespace ns { int f() { return 1; } }
来源：http://rr.haigaiapp.cn

[S59] C++：静态断言
来源：http://zy.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://op.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://ge.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fb.yuexingan06.cn

================================================================================
来源：http://pw.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://co.gzmigu.cn

================================================================================
来源：http://ty.szsharing.cn

[T01] Kotlin：Hello World
来源：http://bw.asd995.cn

println("Hello")
来源：http://ij.nicolike.cn

[T02] Kotlin：变量
来源：http://jy.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nh.shtwfgs.cn


<!-- 参考信息 -->