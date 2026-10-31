代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ha.lnxyls.cn

[Q90] 生成序号列
来源：http://ua.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zb.yuntaijiaju.cn

================================================================================
来源：http://uk.nicolike.cn

R. Bash 专题
来源：http://lo.shxzskj.cn

================================================================================
来源：http://oa.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://fm.colortex.cn

#!/usr/bin/env bash
来源：http://wk.muxihuayi.cn

set -euo pipefail
来源：http://ka.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://uf.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://xl.shtwfgs.cn

[R03] 只读变量
来源：http://iz.nszjky.cn

readonly PI=3.14
来源：http://qg.wgjwhj.cn

[R04] 位置参数
来源：http://yb.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kp.hahajie.cn

[R05] 参数默认值
来源：http://ce.haigaiapp.cn

name="${1:-default}"
来源：http://jm.panjiajie.cn

[R06] 判断命令是否存在
来源：http://es.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ey.szsharing.cn

[R07] if 判断文件
来源：http://bu.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wh.haigaiapp.cn

[R08] 数值比较
来源：http://jw.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hd.jianghongdianzi.cn

[R09] 字符串比较
来源：http://pa.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cb.muxihuayi.cn

[R10] 正则匹配
来源：http://nb.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fr.panjiajie.cn

[R11] case 多分支
来源：http://lh.hnjuh.cn

case "$1" in
来源：http://yb.shxzskj.cn

start) echo "启动" ;;
来源：http://xb.gzmigu.cn

stop)  echo "停止" ;;
来源：http://yq.colortex.cn

*)     echo "未知命令" ;;
来源：http://nt.huixiangedu.cn

esac
来源：http://fh.muxihuayi.cn

[R12] for 遍历文件
来源：http://cb.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://qv.huixinmuqiang.cn

[R13] for 计数循环
来源：http://oo.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://tw.shxzskj.cn

[R14] C 风格 for
来源：http://nn.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rp.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://fa.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tg.asd995.cn

[R16] until 等待条件
来源：http://yy.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xv.bjjhwx.cn

[R17] 数组定义与取值
来源：http://kg.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://br.nicolike.cn

[R18] 遍历数组
来源：http://af.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fi.521024.cn

[R19] 数组长度
来源：http://bg.521024.cn

echo "${#arr[@]}"
来源：http://yx.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://fd.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tr.hnjuh.cn

[R21] 字符串长度
来源：http://nk.shtwfgs.cn

echo "${#s}"
来源：http://xi.nszjky.cn

[R22] 截取子串
来源：http://pf.bookmarksfly.cn

echo "${s:0:5}"
来源：http://tg.jctech888.com.cn

[R23] 字符串替换
来源：http://qy.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sk.521024.cn

[R24] 大小写转换
来源：http://du.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://si.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://mg.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wt.jctech888.com.cn

[R26] 命令替换
来源：http://on.colortex.cn

now=$(date +%F); echo "$now"
来源：http://gk.asd995.cn

[R27] 算术展开
来源：http://lj.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://fc.gzmigu.cn

[R28] 浮点运算
来源：http://qc.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://zv.shxzskj.cn

[R29] 定义函数
来源：http://la.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nz.nicolike.cn

[R30] 函数返回状态码
来源：http://ad.newstarts.cn

f() { return 0; }; f || echo "失败了"
来源：http://uz.haigaiapp.cn

[R31] 局部变量
来源：http://eu.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://ew.lnxyls.cn

[R32] 参数个数校验
来源：http://no.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ss.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://gd.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ur.yuntaijiaju.cn

[R34] 退出时清理
来源：http://gj.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oe.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://jv.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wl.nszjky.cn

[R36] 并发执行多个任务
来源：http://pr.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://at.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://xf.szxytkj.cn

files=$(ls -1)
来源：http://iq.huixiangedu.cn

[R38] 管道串联
来源：http://rv.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://ur.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://lm.shtwfgs.cn

cmd > out.log 2>&1
来源：http://jm.9csxet.cn

[R40] 追加写日志
来源：http://kh.asd995.cn

echo "log" >> out.log
来源：http://zx.wgjwhj.cn

[R41] 丢弃输出
来源：http://fm.nszjky.cn

cmd >/dev/null 2>&1
来源：http://ic.9csxet.cn

[R42] 输入重定向
来源：http://oa.bjjhwx.cn

wc -l < a.txt
来源：http://xr.chemitech.net.cn

[R43] 按名字查找文件
来源：http://ys.yuexingan06.cn

find . -name "*.log" -type f
来源：http://nu.colortex.cn

[R44] 按修改时间查找
来源：http://we.hahajie.cn

find . -mtime -7 -type f
来源：http://zx.szsharing.cn

[R45] 批量删除
来源：http://pm.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://co.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://xh.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qx.nicolike.cn

[R47] sed 单行替换
来源：http://nr.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nn.nicolike.cn

[R48] awk 取指定列
来源：http://ps.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://jy.bookmarksfly.cn

[R49] awk 带条件
来源：http://bl.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lt.gzmigu.cn

[R50] awk 求和
来源：http://mb.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ya.szsharing.cn

[R51] 排序去重取前几
来源：http://kq.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://we.hahajie.cn

[R52] 统计行数
来源：http://ki.szxytkj.cn

wc -l a.txt
来源：http://nc.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://ap.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dh.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://qw.521024.cn

diff a.txt b.txt
来源：http://nh.chemitech.net.cn

[R55] 压缩与解压
来源：http://us.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oo.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://yl.szsharing.cn

scp file user@host:/path/
来源：http://tc.chemitech.net.cn

[R57] 远程执行命令
来源：http://tz.haigaiapp.cn

ssh user@host 'uptime'
来源：http://lo.huixiangedu.cn

[R58] 下载文件
来源：http://vr.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zx.shxzskj.cn

[R59] 发 POST JSON
来源：http://oy.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mu.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://mt.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ap.bookmarksfly.cn

[R61] 磁盘占用
来源：http://dh.hnjuh.cn

df -h;  du -sh *
来源：http://kb.haigaiapp.cn

[R62] 找最占空间的文件
来源：http://ac.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://ib.huixinmuqiang.cn

[R63] 内存与进程
来源：http://dj.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://dc.huanxung.cn

[R64] 结束进程
来源：http://nd.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://kq.szsharing.cn

[R65] 查看端口占用
来源：http://sv.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gs.szxytkj.cn

[R66] 定时任务
来源：http://md.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://aa.nszjky.cn

[R67] 生成随机十六进制串
来源：http://cb.shxzukj.cn

openssl rand -hex 16
来源：http://sp.muxihuayi.cn

[R68] 计算文件校验值
来源：http://tz.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rd.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://xl.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://ao.haigaiapp.cn

[R70] 时间戳与互转
来源：http://kw.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://zo.panjiajie.cn

[R71] 日期格式化
来源：http://ti.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://te.szxytkj.cn

[R72] 等待端口就绪
来源：http://jg.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mw.jctech888.com.cn

[R73] 分割大日志
来源：http://nm.yuntaijiaju.cn

split -l 1000 big.log part_
来源：http://aw.lnxyls.cn

[R74] 批量重命名
来源：http://aw.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qn.wgjwhj.cn

[R75] 导出环境变量
来源：http://ft.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://mf.nszjky.cn

[R76] 使用临时文件
来源：http://bo.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bd.newstarts.cn

[R77] 读取用户输入
来源：http://gb.newstarts.cn

read -rp "请输入: " ans
来源：http://fk.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://pt.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pv.shxzukj.cn

[R79] 解析命令行选项
来源：http://bt.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tw.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ll.jianghongdianzi.cn

time ./run.sh
来源：http://ej.chemitech.net.cn

================================================================================
来源：http://qc.bookmarksfly.cn

S. C / C++ 专题
来源：http://mx.bookmarksfly.cn

================================================================================
来源：http://gc.bjjhwx.cn

[S01] C：Hello World
来源：http://da.jctech888.com.cn

#include <stdio.h>
来源：http://gf.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://st.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://yc.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://bq.gzmigu.cn

[S03] C：读入整数
来源：http://cw.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://ca.521024.cn

[S04] C：字符串复制
来源：http://vq.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jk.jctech888.com.cn

[S05] C：字符串长度
来源：http://dh.521024.cn

strlen(s)
来源：http://ud.asd995.cn

[S06] C：字符串比较
来源：http://ry.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://rq.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://fz.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fh.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://tr.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yr.asd995.cn

[S09] C：结构体定义与初始化
来源：http://jd.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xo.yuexingan06.cn

[S10] C：指针与解引用
来源：http://gd.asd995.cn

int *p = &a;  *p = 5;
来源：http://uv.521024.cn

[S11] C：逐行读文件
来源：http://tb.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://nz.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nu.shxzukj.cn

fclose(f);
来源：http://sx.lnxyls.cn

[S12] C：写文件
来源：http://mi.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xy.panjiajie.cn

[S13] C：宏定义
来源：http://zk.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eb.huanxung.cn

[S14] C：枚举
来源：http://yr.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ev.huixiangedu.cn

[S15] C：类型转换
来源：http://jx.bjjhwx.cn

(double) a / b
来源：http://ml.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://dn.huixinmuqiang.cn

x |= (1 << 3);
来源：http://er.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://up.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cr.szsharing.cn

[S18] C：命令行参数
来源：http://cs.bjjhwx.cn

int main(int argc, char **argv)
来源：http://dj.521024.cn

[S19] C：快速排序
来源：http://rn.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://th.shxzukj.cn

[S20] C：二分查找
来源：http://sq.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wv.9csxet.cn

[S21] C：字符类别判断
来源：http://cb.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ip.9csxet.cn

[S22] C：字符串转数字
来源：http://ut.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jh.bjjhwx.cn

[S23] C：随机数
来源：http://uv.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tx.szxytkj.cn

[S24] C：获取本地时间
来源：http://ms.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ce.bjjhwx.cn

[S25] C：内存拷贝
来源：http://zf.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://as.lnxyls.cn

[S26] C：内存清零
来源：http://nf.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://mh.szsharing.cn

[S27] C：定义常量
来源：http://lm.yuexingan06.cn

const double PI = 3.14159;
来源：http://wc.huanxung.cn

[S28] C：静态变量
来源：http://wq.huanxung.cn

static int counter = 0;
来源：http://zz.chemitech.net.cn

[S29] C：变参函数
来源：http://lt.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ys.gzmigu.cn

[S30] C：头文件保护
来源：http://mh.hahajie.cn

#ifndef X_H
来源：http://bz.shxzskj.cn

#define X_H
来源：http://ur.shtwfgs.cn

#endif
来源：http://nn.9csxet.cn

[S31] C++：Hello World
来源：http://ub.szsharing.cn

#include <iostream>
来源：http://kc.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://cg.521024.cn

[S32] C++：字符串
来源：http://gm.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://hh.haigaiapp.cn

[S33] C++：vector 增删
来源：http://bm.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gy.nszjky.cn

[S34] C++：遍历 vector
来源：http://ov.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://yc.shxzskj.cn

[S35] C++：map
来源：http://ap.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://du.bjjhwx.cn

[S36] C++：unordered_map
来源：http://ix.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ss.haigaiapp.cn

[S37] C++：set
来源：http://nj.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cx.jctech888.com.cn

[S38] C++：排序
来源：http://xh.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://ly.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://qx.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://se.haigaiapp.cn

[S40] C++：查找元素
来源：http://zf.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gs.newstarts.cn

[S41] C++：类与构造函数
来源：http://ea.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ly.asd995.cn

[S42] C++：继承与虚函数
来源：http://gd.szsharing.cn

class B : public Base { public: void f() override {} };
来源：http://pe.huanxung.cn

[S43] C++：智能指针
来源：http://xn.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://wr.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://so.newstarts.cn

void inc(int &x) { ++x; }
来源：http://nm.jianghongdianzi.cn

[S45] C++：lambda
来源：http://kt.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dk.yuexingan06.cn

[S46] C++：函数模板
来源：http://gu.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hm.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://gk.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hq.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://mh.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hv.9csxet.cn

while (std::getline(in, line)) { }
来源：http://hf.huixinmuqiang.cn

[S49] C++：写文件
来源：http://qd.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://do.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ev.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jy.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://nk.yuexingan06.cn

static_cast<double>(a) / b
来源：http://oc.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://uy.hahajie.cn

int size() const noexcept { return n_; }
来源：http://iy.panjiajie.cn

[S53] C++：移动语义
来源：http://vu.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://gw.hnjuh.cn

[S54] C++：异常处理
来源：http://tw.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zn.lnxyls.cn

[S55] C++：结构化绑定
来源：http://dv.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rf.asd995.cn

[S56] C++：optional
来源：http://th.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://so.yuexingan06.cn

[S57] C++：编译期常量
来源：http://dz.nszjky.cn

constexpr int N = 10;
来源：http://yj.szxytkj.cn

[S58] C++：命名空间
来源：http://wb.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://zo.lnxyls.cn

[S59] C++：静态断言
来源：http://nl.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gm.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://nu.hnjuh.cn


<!-- 参考信息 -->