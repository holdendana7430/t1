代发 wailian999

R. Bash 专题
来源：http://fv.yuntaijiaju.cn

================================================================================
来源：http://so.panjiajie.cn

[R01] shebang 与严格模式
来源：http://vr.shxzskj.cn

#!/usr/bin/env bash
来源：http://dr.nszjky.cn

set -euo pipefail
来源：http://qk.asd995.cn

[R02] 变量赋值与使用
来源：http://fj.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://ac.jianghongdianzi.cn

[R03] 只读变量
来源：http://xz.lnxyls.cn

readonly PI=3.14
来源：http://wj.colortex.cn

[R04] 位置参数
来源：http://eq.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zd.nszjky.cn

[R05] 参数默认值
来源：http://ex.huanxung.cn

name="${1:-default}"
来源：http://au.huanxung.cn

[R06] 判断命令是否存在
来源：http://pb.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nq.muxihuayi.cn

[R07] if 判断文件
来源：http://ya.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ey.yuexingan06.cn

[R08] 数值比较
来源：http://sw.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sn.chemitech.net.cn

[R09] 字符串比较
来源：http://ch.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cz.newstarts.cn

[R10] 正则匹配
来源：http://ab.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lx.yuntaijiaju.cn

[R11] case 多分支
来源：http://ie.hnjuh.cn

case "$1" in
来源：http://sc.szxytkj.cn

start) echo "启动" ;;
来源：http://hr.colortex.cn

stop)  echo "停止" ;;
来源：http://eu.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://fc.shtwfgs.cn

esac
来源：http://ea.hahajie.cn

[R12] for 遍历文件
来源：http://xf.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://yx.szsharing.cn

[R13] for 计数循环
来源：http://ou.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://km.huanxung.cn

[R14] C 风格 for
来源：http://tj.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://px.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://ax.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ra.521024.cn

[R16] until 等待条件
来源：http://tf.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ys.nicolike.cn

[R17] 数组定义与取值
来源：http://ym.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dx.shtwfgs.cn

[R18] 遍历数组
来源：http://mp.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sw.wgjwhj.cn

[R19] 数组长度
来源：http://dh.wgjwhj.cn

echo "${#arr[@]}"
来源：http://jt.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://ch.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fq.chemitech.net.cn

[R21] 字符串长度
来源：http://kt.wgjwhj.cn

echo "${#s}"
来源：http://va.jctech888.com.cn

[R22] 截取子串
来源：http://ed.nszjky.cn

echo "${s:0:5}"
来源：http://ky.huanxung.cn

[R23] 字符串替换
来源：http://fm.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pk.huixiangedu.cn

[R24] 大小写转换
来源：http://zh.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xs.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://ht.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yj.szsharing.cn

[R26] 命令替换
来源：http://dj.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://sk.hnjuh.cn

[R27] 算术展开
来源：http://wi.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://rl.lnxyls.cn

[R28] 浮点运算
来源：http://fc.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://kj.asd995.cn

[R29] 定义函数
来源：http://zz.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ui.huanxung.cn

[R30] 函数返回状态码
来源：http://wj.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://fr.521024.cn

[R31] 局部变量
来源：http://jg.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://dc.jctech888.com.cn

[R32] 参数个数校验
来源：http://jo.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hg.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://qu.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tv.panjiajie.cn

[R34] 退出时清理
来源：http://vw.szsharing.cn

trap 'rm -f "$tmp"' EXIT
来源：http://er.shxzskj.cn

[R35] 后台执行并等待
来源：http://cd.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hw.nszjky.cn

[R36] 并发执行多个任务
来源：http://le.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fs.lnxyls.cn

[R37] 把输出赋给变量
来源：http://om.chemitech.net.cn

files=$(ls -1)
来源：http://yv.shxzukj.cn

[R38] 管道串联
来源：http://zd.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://qy.nszjky.cn

[R39] 重定向标准输出与错误
来源：http://ix.newstarts.cn

cmd > out.log 2>&1
来源：http://fd.haigaiapp.cn

[R40] 追加写日志
来源：http://es.wgjwhj.cn

echo "log" >> out.log
来源：http://sy.nicolike.cn

[R41] 丢弃输出
来源：http://vl.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://hx.huanxung.cn

[R42] 输入重定向
来源：http://th.huixinmuqiang.cn

wc -l < a.txt
来源：http://ua.nszjky.cn

[R43] 按名字查找文件
来源：http://jt.newstarts.cn

find . -name "*.log" -type f
来源：http://kr.huixiangedu.cn

[R44] 按修改时间查找
来源：http://qn.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://ps.panjiajie.cn

[R45] 批量删除
来源：http://gu.bookmarksfly.cn

find . -name "*.tmp" -delete
来源：http://sd.huanxung.cn

[R46] 递归替换文件内容
来源：http://uq.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xj.huixiangedu.cn

[R47] sed 单行替换
来源：http://ab.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ef.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ba.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://ko.newstarts.cn

[R49] awk 带条件
来源：http://zh.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qx.newstarts.cn

[R50] awk 求和
来源：http://dn.newstarts.cn

awk '{s += $2} END {print s}' a.txt
来源：http://we.lnxyls.cn

[R51] 排序去重取前几
来源：http://cv.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://id.shtwfgs.cn

[R52] 统计行数
来源：http://ka.huixiangedu.cn

wc -l a.txt
来源：http://qu.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://rm.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mf.asd995.cn

[R54] 比较两个文件
来源：http://tu.9csxet.cn

diff a.txt b.txt
来源：http://dx.hahajie.cn

[R55] 压缩与解压
来源：http://fx.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sc.huixiangedu.cn

[R56] 远程拷贝
来源：http://gl.lnxyls.cn

scp file user@host:/path/
来源：http://uo.nszjky.cn

[R57] 远程执行命令
来源：http://fg.hahajie.cn

ssh user@host 'uptime'
来源：http://fl.chemitech.net.cn

[R58] 下载文件
来源：http://dp.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wz.jctech888.com.cn

[R59] 发 POST JSON
来源：http://vk.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xx.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://oy.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oz.nicolike.cn

[R61] 磁盘占用
来源：http://ev.shxzskj.cn

df -h;  du -sh *
来源：http://rq.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://ta.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://kd.jianghongdianzi.cn

[R63] 内存与进程
来源：http://wm.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://qv.nszjky.cn

[R64] 结束进程
来源：http://jj.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://im.bookmarksfly.cn

[R65] 查看端口占用
来源：http://zc.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rw.bjjhwx.cn

[R66] 定时任务
来源：http://bi.hahajie.cn

crontab -e;  crontab -l
来源：http://en.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://rb.nszjky.cn

openssl rand -hex 16
来源：http://dk.wgjwhj.cn

[R68] 计算文件校验值
来源：http://mh.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jn.huanxung.cn

[R69] 生成随机密码
来源：http://rc.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://vq.chemitech.net.cn

[R70] 时间戳与互转
来源：http://ts.szsharing.cn

date +%s;  date -d @1700000000
来源：http://uh.szsharing.cn

[R71] 日期格式化
来源：http://zm.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dm.jctech888.com.cn

[R72] 等待端口就绪
来源：http://yp.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yo.szxytkj.cn

[R73] 分割大日志
来源：http://tl.9csxet.cn

split -l 1000 big.log part_
来源：http://me.bjjhwx.cn

[R74] 批量重命名
来源：http://br.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vq.nicolike.cn

[R75] 导出环境变量
来源：http://pf.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://mo.jctech888.com.cn

[R76] 使用临时文件
来源：http://tv.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://td.asd995.cn

[R77] 读取用户输入
来源：http://rh.colortex.cn

read -rp "请输入: " ans
来源：http://sg.haigaiapp.cn

[R78] 交互式菜单
来源：http://vu.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uq.asd995.cn

[R79] 解析命令行选项
来源：http://fe.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cr.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://zc.gzmigu.cn

time ./run.sh
来源：http://rh.colortex.cn

================================================================================
来源：http://yn.shxzskj.cn

S. C / C++ 专题
来源：http://dc.szsharing.cn

================================================================================
来源：http://yl.shxzukj.cn

[S01] C：Hello World
来源：http://dn.huixinmuqiang.cn

#include <stdio.h>
来源：http://qg.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wj.asd995.cn

[S02] C：变量与格式化输出
来源：http://rn.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://vt.lnxyls.cn

[S03] C：读入整数
来源：http://qg.gzmigu.cn

int x; scanf("%d", &x);
来源：http://hv.shxzskj.cn

[S04] C：字符串复制
来源：http://jl.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://it.nszjky.cn

[S05] C：字符串长度
来源：http://ae.shtwfgs.cn

strlen(s)
来源：http://du.shxzskj.cn

[S06] C：字符串比较
来源：http://yu.bjjhwx.cn

strcmp(a, b) == 0
来源：http://iu.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://xp.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wm.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://zm.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fu.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://dj.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kr.521024.cn

[S10] C：指针与解引用
来源：http://ou.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://rl.jctech888.com.cn

[S11] C：逐行读文件
来源：http://kv.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://rx.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://me.jianghongdianzi.cn

fclose(f);
来源：http://nm.bjjhwx.cn

[S12] C：写文件
来源：http://pc.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xs.nszjky.cn

[S13] C：宏定义
来源：http://hq.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bn.9csxet.cn

[S14] C：枚举
来源：http://yl.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://sa.muxihuayi.cn

[S15] C：类型转换
来源：http://le.hnjuh.cn

(double) a / b
来源：http://lx.chemitech.net.cn

[S16] C：位操作置位
来源：http://or.shxzskj.cn

x |= (1 << 3);
来源：http://mp.huanxung.cn

[S17] C：安全拼接字符串
来源：http://um.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bi.muxihuayi.cn

[S18] C：命令行参数
来源：http://kl.newstarts.cn

int main(int argc, char **argv)
来源：http://nq.hnjuh.cn

[S19] C：快速排序
来源：http://ej.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sd.jctech888.com.cn

[S20] C：二分查找
来源：http://vd.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ua.shxzukj.cn

[S21] C：字符类别判断
来源：http://tb.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cf.nszjky.cn

[S22] C：字符串转数字
来源：http://ar.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://da.huanxung.cn

[S23] C：随机数
来源：http://vb.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://my.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://kt.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wt.bjjhwx.cn

[S25] C：内存拷贝
来源：http://zw.shtwfgs.cn

memcpy(dst, src, n);
来源：http://ys.bjjhwx.cn

[S26] C：内存清零
来源：http://zo.asd995.cn

memset(a, 0, sizeof a);
来源：http://lu.muxihuayi.cn

[S27] C：定义常量
来源：http://cm.colortex.cn

const double PI = 3.14159;
来源：http://da.szxytkj.cn

[S28] C：静态变量
来源：http://wp.newstarts.cn

static int counter = 0;
来源：http://pp.9csxet.cn

[S29] C：变参函数
来源：http://bk.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bj.nicolike.cn

[S30] C：头文件保护
来源：http://lz.nicolike.cn

#ifndef X_H
来源：http://md.huixiangedu.cn

#define X_H
来源：http://eb.asd995.cn

#endif
来源：http://xl.hahajie.cn

[S31] C++：Hello World
来源：http://ck.521024.cn

#include <iostream>
来源：http://ox.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://ms.bjjhwx.cn

[S32] C++：字符串
来源：http://hg.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://vg.hnjuh.cn

[S33] C++：vector 增删
来源：http://pj.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uk.shxzskj.cn

[S34] C++：遍历 vector
来源：http://tt.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://xs.shxzskj.cn

[S35] C++：map
来源：http://ih.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lq.shtwfgs.cn

[S36] C++：unordered_map
来源：http://ow.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://te.panjiajie.cn

[S37] C++：set
来源：http://ok.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vp.521024.cn

[S38] C++：排序
来源：http://ge.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://lb.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://ot.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qn.shxzskj.cn

[S40] C++：查找元素
来源：http://ng.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sp.panjiajie.cn

[S41] C++：类与构造函数
来源：http://hn.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gk.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://gs.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://fj.521024.cn

[S43] C++：智能指针
来源：http://iw.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://uj.bookmarksfly.cn

[S44] C++：引用传参
来源：http://qb.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://qe.521024.cn

[S45] C++：lambda
来源：http://hz.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rs.muxihuayi.cn

[S46] C++：函数模板
来源：http://wk.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pz.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://re.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hh.asd995.cn

[S48] C++：逐行读文件
来源：http://ws.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gp.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://ga.muxihuayi.cn

[S49] C++：写文件
来源：http://dz.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mk.szxytkj.cn

[S50] C++：格式化数字
来源：http://qv.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lr.nicolike.cn

[S51] C++：显式类型转换
来源：http://fz.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://kg.asd995.cn

[S52] C++：const 与 noexcept
来源：http://cu.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://tv.yuexingan06.cn

[S53] C++：移动语义
来源：http://eu.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ye.szsharing.cn

[S54] C++：异常处理
来源：http://lr.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ot.gzmigu.cn

[S55] C++：结构化绑定
来源：http://zr.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sv.asd995.cn

[S56] C++：optional
来源：http://vh.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ve.shtwfgs.cn

[S57] C++：编译期常量
来源：http://nk.szsharing.cn

constexpr int N = 10;
来源：http://qg.shtwfgs.cn

[S58] C++：命名空间
来源：http://ky.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://fl.nszjky.cn

[S59] C++：静态断言
来源：http://uj.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sr.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://og.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yw.newstarts.cn

================================================================================
来源：http://og.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qb.asd995.cn

================================================================================
来源：http://ic.gzmigu.cn


<!-- 参考信息 -->