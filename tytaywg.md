代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nw.lnxyls.cn

[Q90] 生成序号列
来源：http://vn.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mr.huixiangedu.cn

================================================================================
来源：http://ts.colortex.cn

R. Bash 专题
来源：http://qo.huixiangedu.cn

================================================================================
来源：http://kp.shxzukj.cn

[R01] shebang 与严格模式
来源：http://rl.521024.cn

#!/usr/bin/env bash
来源：http://eh.bookmarksfly.cn

set -euo pipefail
来源：http://hz.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://wn.newstarts.cn

name="Tom"; echo "$name"
来源：http://kq.jianghongdianzi.cn

[R03] 只读变量
来源：http://uc.huixinmuqiang.cn

readonly PI=3.14
来源：http://dx.nicolike.cn

[R04] 位置参数
来源：http://zt.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.521024.cn

[R05] 参数默认值
来源：http://sc.9csxet.cn

name="${1:-default}"
来源：http://yu.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://se.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lm.nszjky.cn

[R07] if 判断文件
来源：http://xf.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uo.newstarts.cn

[R08] 数值比较
来源：http://of.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://af.nicolike.cn

[R09] 字符串比较
来源：http://em.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jr.hahajie.cn

[R10] 正则匹配
来源：http://jw.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ns.shxzskj.cn

[R11] case 多分支
来源：http://sf.asd995.cn

case "$1" in
来源：http://wi.huixiangedu.cn

start) echo "启动" ;;
来源：http://md.nicolike.cn

stop)  echo "停止" ;;
来源：http://wz.huanxung.cn

*)     echo "未知命令" ;;
来源：http://dv.huixiangedu.cn

esac
来源：http://qk.muxihuayi.cn

[R12] for 遍历文件
来源：http://uc.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://vy.szsharing.cn

[R13] for 计数循环
来源：http://mg.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://rz.gzmigu.cn

[R14] C 风格 for
来源：http://pr.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mm.nszjky.cn

[R15] while 逐行读文件
来源：http://uh.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nl.bookmarksfly.cn

[R16] until 等待条件
来源：http://pg.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ra.huixiangedu.cn

[R17] 数组定义与取值
来源：http://py.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mp.yuntaijiaju.cn

[R18] 遍历数组
来源：http://qw.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uy.shtwfgs.cn

[R19] 数组长度
来源：http://om.szsharing.cn

echo "${#arr[@]}"
来源：http://oe.hnjuh.cn

[R20] 关联数组（字典）
来源：http://et.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ct.szxytkj.cn

[R21] 字符串长度
来源：http://xv.yuntaijiaju.cn

echo "${#s}"
来源：http://zt.szxytkj.cn

[R22] 截取子串
来源：http://gx.asd995.cn

echo "${s:0:5}"
来源：http://ni.shtwfgs.cn

[R23] 字符串替换
来源：http://cz.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mh.nszjky.cn

[R24] 大小写转换
来源：http://bo.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tk.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://lc.huixinmuqiang.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hy.muxihuayi.cn

[R26] 命令替换
来源：http://og.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://ze.colortex.cn

[R27] 算术展开
来源：http://is.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://td.colortex.cn

[R28] 浮点运算
来源：http://zs.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://ll.bjjhwx.cn

[R29] 定义函数
来源：http://xd.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://do.huixiangedu.cn

[R30] 函数返回状态码
来源：http://yd.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://kk.szxytkj.cn

[R31] 局部变量
来源：http://it.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://kw.lnxyls.cn

[R32] 参数个数校验
来源：http://mc.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tr.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://ep.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nk.nicolike.cn

[R34] 退出时清理
来源：http://oj.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fa.shxzskj.cn

[R35] 后台执行并等待
来源：http://lb.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sd.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://wo.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ib.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://gc.szsharing.cn

files=$(ls -1)
来源：http://mk.colortex.cn

[R38] 管道串联
来源：http://ta.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://er.asd995.cn

[R39] 重定向标准输出与错误
来源：http://ku.chemitech.net.cn

cmd > out.log 2>&1
来源：http://vy.nicolike.cn

[R40] 追加写日志
来源：http://dv.9csxet.cn

echo "log" >> out.log
来源：http://uv.yuexingan06.cn

[R41] 丢弃输出
来源：http://az.hahajie.cn

cmd >/dev/null 2>&1
来源：http://pf.hahajie.cn

[R42] 输入重定向
来源：http://rx.nicolike.cn

wc -l < a.txt
来源：http://lq.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://ld.yuexingan06.cn

find . -name "*.log" -type f
来源：http://vp.jctech888.com.cn

[R44] 按修改时间查找
来源：http://xt.nicolike.cn

find . -mtime -7 -type f
来源：http://gc.521024.cn

[R45] 批量删除
来源：http://ns.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://dk.colortex.cn

[R46] 递归替换文件内容
来源：http://ql.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lq.muxihuayi.cn

[R47] sed 单行替换
来源：http://we.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gq.szxytkj.cn

[R48] awk 取指定列
来源：http://rj.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://go.nicolike.cn

[R49] awk 带条件
来源：http://cw.nszjky.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uw.newstarts.cn

[R50] awk 求和
来源：http://ah.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tb.nszjky.cn

[R51] 排序去重取前几
来源：http://xr.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://si.chemitech.net.cn

[R52] 统计行数
来源：http://iv.jctech888.com.cn

wc -l a.txt
来源：http://zp.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://eh.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jr.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://rw.colortex.cn

diff a.txt b.txt
来源：http://ft.yuexingan06.cn

[R55] 压缩与解压
来源：http://rq.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pt.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://bb.colortex.cn

scp file user@host:/path/
来源：http://cg.huixiangedu.cn

[R57] 远程执行命令
来源：http://tj.colortex.cn

ssh user@host 'uptime'
来源：http://uy.wgjwhj.cn

[R58] 下载文件
来源：http://zl.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gv.nicolike.cn

[R59] 发 POST JSON
来源：http://ip.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://le.521024.cn

[R60] 只看 HTTP 状态码
来源：http://lt.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yh.hnjuh.cn

[R61] 磁盘占用
来源：http://ry.521024.cn

df -h;  du -sh *
来源：http://mc.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://cj.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://eu.chemitech.net.cn

[R63] 内存与进程
来源：http://ik.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://kq.huixiangedu.cn

[R64] 结束进程
来源：http://cp.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://kc.szxytkj.cn

[R65] 查看端口占用
来源：http://ro.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uf.hnjuh.cn

[R66] 定时任务
来源：http://qs.chemitech.net.cn

crontab -e;  crontab -l
来源：http://eg.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://ld.newstarts.cn

openssl rand -hex 16
来源：http://ao.lnxyls.cn

[R68] 计算文件校验值
来源：http://vy.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qn.hahajie.cn

[R69] 生成随机密码
来源：http://ao.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://mf.panjiajie.cn

[R70] 时间戳与互转
来源：http://kt.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://cw.yuexingan06.cn

[R71] 日期格式化
来源：http://bf.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bw.lnxyls.cn

[R72] 等待端口就绪
来源：http://jk.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fa.huixinmuqiang.cn

[R73] 分割大日志
来源：http://ov.panjiajie.cn

split -l 1000 big.log part_
来源：http://tl.haigaiapp.cn

[R74] 批量重命名
来源：http://wm.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pu.gzmigu.cn

[R75] 导出环境变量
来源：http://zv.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://hi.9csxet.cn

[R76] 使用临时文件
来源：http://tr.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tn.nicolike.cn

[R77] 读取用户输入
来源：http://sw.huixiangedu.cn

read -rp "请输入: " ans
来源：http://qw.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://jt.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nz.colortex.cn

[R79] 解析命令行选项
来源：http://eh.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ap.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://tp.haigaiapp.cn

time ./run.sh
来源：http://ng.panjiajie.cn

================================================================================
来源：http://yk.bookmarksfly.cn

S. C / C++ 专题
来源：http://uw.newstarts.cn

================================================================================
来源：http://yr.bookmarksfly.cn

[S01] C：Hello World
来源：http://vg.521024.cn

#include <stdio.h>
来源：http://qz.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vx.nicolike.cn

[S02] C：变量与格式化输出
来源：http://hu.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://nh.chemitech.net.cn

[S03] C：读入整数
来源：http://cb.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://lv.asd995.cn

[S04] C：字符串复制
来源：http://et.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oz.521024.cn

[S05] C：字符串长度
来源：http://gs.lnxyls.cn

strlen(s)
来源：http://fj.muxihuayi.cn

[S06] C：字符串比较
来源：http://wk.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://fw.521024.cn

[S07] C：数组遍历求和
来源：http://jy.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kl.asd995.cn

[S08] C：动态内存分配与释放
来源：http://rb.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ku.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://ct.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ra.bjjhwx.cn

[S10] C：指针与解引用
来源：http://qw.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://iu.shxzskj.cn

[S11] C：逐行读文件
来源：http://vs.huixiangedu.cn

FILE *f = fopen("a.txt", "r");
来源：http://vu.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wz.hahajie.cn

fclose(f);
来源：http://rl.newstarts.cn

[S12] C：写文件
来源：http://ko.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mt.shxzukj.cn

[S13] C：宏定义
来源：http://on.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hn.shxzukj.cn

[S14] C：枚举
来源：http://al.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://dy.bookmarksfly.cn

[S15] C：类型转换
来源：http://hi.nicolike.cn

(double) a / b
来源：http://rz.shxzukj.cn

[S16] C：位操作置位
来源：http://zh.shxzskj.cn

x |= (1 << 3);
来源：http://de.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://vv.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bl.szxytkj.cn

[S18] C：命令行参数
来源：http://wp.haigaiapp.cn

int main(int argc, char **argv)
来源：http://qc.yuntaijiaju.cn

[S19] C：快速排序
来源：http://op.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://du.hnjuh.cn

[S20] C：二分查找
来源：http://zy.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ro.shxzskj.cn

[S21] C：字符类别判断
来源：http://oo.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ei.asd995.cn

[S22] C：字符串转数字
来源：http://fs.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dd.newstarts.cn

[S23] C：随机数
来源：http://le.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wo.szsharing.cn

[S24] C：获取本地时间
来源：http://ra.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bq.asd995.cn

[S25] C：内存拷贝
来源：http://eo.shtwfgs.cn

memcpy(dst, src, n);
来源：http://yo.yuntaijiaju.cn

[S26] C：内存清零
来源：http://nu.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://yg.chemitech.net.cn

[S27] C：定义常量
来源：http://sd.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://uy.huixinmuqiang.cn

[S28] C：静态变量
来源：http://db.muxihuayi.cn

static int counter = 0;
来源：http://bb.nicolike.cn

[S29] C：变参函数
来源：http://qh.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ka.haigaiapp.cn

[S30] C：头文件保护
来源：http://bd.nszjky.cn

#ifndef X_H
来源：http://st.shxzukj.cn

#define X_H
来源：http://aw.jctech888.com.cn

#endif
来源：http://gl.huixiangedu.cn

[S31] C++：Hello World
来源：http://ih.lnxyls.cn

#include <iostream>
来源：http://pl.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://nu.521024.cn

[S32] C++：字符串
来源：http://mz.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://et.gzmigu.cn

[S33] C++：vector 增删
来源：http://pj.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jp.hahajie.cn

[S34] C++：遍历 vector
来源：http://sq.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ag.muxihuayi.cn

[S35] C++：map
来源：http://hl.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ku.asd995.cn

[S36] C++：unordered_map
来源：http://om.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rh.bjjhwx.cn

[S37] C++：set
来源：http://xm.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zb.bjjhwx.cn

[S38] C++：排序
来源：http://te.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://ww.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://cb.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://od.nszjky.cn

[S40] C++：查找元素
来源：http://xt.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xh.szxytkj.cn

[S41] C++：类与构造函数
来源：http://tl.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ai.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://kd.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://xr.panjiajie.cn

[S43] C++：智能指针
来源：http://zx.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://rm.bookmarksfly.cn

[S44] C++：引用传参
来源：http://wu.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://so.gzmigu.cn

[S45] C++：lambda
来源：http://rj.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fq.colortex.cn

[S46] C++：函数模板
来源：http://zn.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fq.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://oe.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pn.shxzskj.cn

[S48] C++：逐行读文件
来源：http://cf.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://id.521024.cn

while (std::getline(in, line)) { }
来源：http://ay.yuexingan06.cn

[S49] C++：写文件
来源：http://xt.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ap.szxytkj.cn

[S50] C++：格式化数字
来源：http://oi.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jl.shxzskj.cn

[S51] C++：显式类型转换
来源：http://az.bjjhwx.cn

static_cast<double>(a) / b
来源：http://sl.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://vs.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://wt.shxzukj.cn

[S53] C++：移动语义
来源：http://ac.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://jc.shxzskj.cn

[S54] C++：异常处理
来源：http://vy.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eq.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://zg.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zc.asd995.cn

[S56] C++：optional
来源：http://sv.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zg.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://wm.newstarts.cn

constexpr int N = 10;
来源：http://kv.521024.cn

[S58] C++：命名空间
来源：http://gh.yuexingan06.cn

namespace ns { int f() { return 1; } }
来源：http://hi.jctech888.com.cn

[S59] C++：静态断言
来源：http://rm.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gt.colortex.cn

[S60] C++：遍历并删除元素
来源：http://ke.nszjky.cn


<!-- 参考信息 -->