代发 wailian999

R. Bash 专题
来源：http://jp.nicolike.cn

================================================================================
来源：http://ng.hahajie.cn

[R01] shebang 与严格模式
来源：http://ft.nicolike.cn

#!/usr/bin/env bash
来源：http://ex.9csxet.cn

set -euo pipefail
来源：http://nx.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://ns.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://wg.shxzukj.cn

[R03] 只读变量
来源：http://mg.hnjuh.cn

readonly PI=3.14
来源：http://kb.hnjuh.cn

[R04] 位置参数
来源：http://zm.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oo.521024.cn

[R05] 参数默认值
来源：http://mz.huixinmuqiang.cn

name="${1:-default}"
来源：http://zj.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://fc.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zj.shxzskj.cn

[R07] if 判断文件
来源：http://le.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ej.yuexingan06.cn

[R08] 数值比较
来源：http://sd.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zq.hahajie.cn

[R09] 字符串比较
来源：http://ze.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gf.chemitech.net.cn

[R10] 正则匹配
来源：http://ic.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kz.nicolike.cn

[R11] case 多分支
来源：http://fs.yuexingan06.cn

case "$1" in
来源：http://wy.colortex.cn

start) echo "启动" ;;
来源：http://me.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://ek.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://bu.521024.cn

esac
来源：http://ar.521024.cn

[R12] for 遍历文件
来源：http://zq.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://la.szsharing.cn

[R13] for 计数循环
来源：http://cn.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://kn.colortex.cn

[R14] C 风格 for
来源：http://hh.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ls.9csxet.cn

[R15] while 逐行读文件
来源：http://yz.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xb.yuexingan06.cn

[R16] until 等待条件
来源：http://jz.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ct.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://ee.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fc.panjiajie.cn

[R18] 遍历数组
来源：http://dj.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://af.yuntaijiaju.cn

[R19] 数组长度
来源：http://ud.colortex.cn

echo "${#arr[@]}"
来源：http://us.panjiajie.cn

[R20] 关联数组（字典）
来源：http://lv.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mh.colortex.cn

[R21] 字符串长度
来源：http://fg.shxzskj.cn

echo "${#s}"
来源：http://ss.szxytkj.cn

[R22] 截取子串
来源：http://xa.huixiangedu.cn

echo "${s:0:5}"
来源：http://tj.jctech888.com.cn

[R23] 字符串替换
来源：http://ui.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nr.shxzskj.cn

[R24] 大小写转换
来源：http://tg.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gi.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://rk.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pt.huanxung.cn

[R26] 命令替换
来源：http://hc.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://er.bookmarksfly.cn

[R27] 算术展开
来源：http://rt.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://kx.panjiajie.cn

[R28] 浮点运算
来源：http://tv.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://de.hahajie.cn

[R29] 定义函数
来源：http://ax.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ok.asd995.cn

[R30] 函数返回状态码
来源：http://sp.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://ty.chemitech.net.cn

[R31] 局部变量
来源：http://cb.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://si.lnxyls.cn

[R32] 参数个数校验
来源：http://ly.bjjhwx.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cd.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://te.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tg.szxytkj.cn

[R34] 退出时清理
来源：http://iy.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xg.shxzukj.cn

[R35] 后台执行并等待
来源：http://yw.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ss.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://pd.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vh.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://ni.shxzukj.cn

files=$(ls -1)
来源：http://fq.lnxyls.cn

[R38] 管道串联
来源：http://eg.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://ns.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://me.yuexingan06.cn

cmd > out.log 2>&1
来源：http://ei.shxzskj.cn

[R40] 追加写日志
来源：http://mo.huixiangedu.cn

echo "log" >> out.log
来源：http://zx.colortex.cn

[R41] 丢弃输出
来源：http://pt.521024.cn

cmd >/dev/null 2>&1
来源：http://gu.panjiajie.cn

[R42] 输入重定向
来源：http://wi.bjjhwx.cn

wc -l < a.txt
来源：http://zx.hahajie.cn

[R43] 按名字查找文件
来源：http://ob.shxzukj.cn

find . -name "*.log" -type f
来源：http://wm.panjiajie.cn

[R44] 按修改时间查找
来源：http://pc.colortex.cn

find . -mtime -7 -type f
来源：http://yp.shtwfgs.cn

[R45] 批量删除
来源：http://hf.huanxung.cn

find . -name "*.tmp" -delete
来源：http://hb.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://ww.shtwfgs.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://du.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://xv.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gd.colortex.cn

[R48] awk 取指定列
来源：http://rt.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://vx.shxzskj.cn

[R49] awk 带条件
来源：http://mc.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bl.lnxyls.cn

[R50] awk 求和
来源：http://gd.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bv.szsharing.cn

[R51] 排序去重取前几
来源：http://ah.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vi.szsharing.cn

[R52] 统计行数
来源：http://yt.bjjhwx.cn

wc -l a.txt
来源：http://hd.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://so.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tg.szxytkj.cn

[R54] 比较两个文件
来源：http://qm.yuexingan06.cn

diff a.txt b.txt
来源：http://kg.chemitech.net.cn

[R55] 压缩与解压
来源：http://rz.shtwfgs.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tu.asd995.cn

[R56] 远程拷贝
来源：http://tr.huixinmuqiang.cn

scp file user@host:/path/
来源：http://ye.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://sw.hahajie.cn

ssh user@host 'uptime'
来源：http://fa.yuexingan06.cn

[R58] 下载文件
来源：http://ke.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oc.bjjhwx.cn

[R59] 发 POST JSON
来源：http://hk.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ht.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://iq.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sm.nszjky.cn

[R61] 磁盘占用
来源：http://ek.nicolike.cn

df -h;  du -sh *
来源：http://wr.colortex.cn

[R62] 找最占空间的文件
来源：http://fg.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://cs.gzmigu.cn

[R63] 内存与进程
来源：http://nx.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://sm.9csxet.cn

[R64] 结束进程
来源：http://qa.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://xm.huixiangedu.cn

[R65] 查看端口占用
来源：http://lr.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ua.huixiangedu.cn

[R66] 定时任务
来源：http://cy.szxytkj.cn

crontab -e;  crontab -l
来源：http://nl.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://pp.colortex.cn

openssl rand -hex 16
来源：http://cl.shxzskj.cn

[R68] 计算文件校验值
来源：http://uz.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://th.huanxung.cn

[R69] 生成随机密码
来源：http://nx.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://cg.yuexingan06.cn

[R70] 时间戳与互转
来源：http://fl.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://lt.jianghongdianzi.cn

[R71] 日期格式化
来源：http://sg.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dy.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://yd.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vh.shxzskj.cn

[R73] 分割大日志
来源：http://us.huanxung.cn

split -l 1000 big.log part_
来源：http://hu.szsharing.cn

[R74] 批量重命名
来源：http://hd.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tt.nicolike.cn

[R75] 导出环境变量
来源：http://in.shtwfgs.cn

export PATH="$HOME/bin:$PATH"
来源：http://va.huanxung.cn

[R76] 使用临时文件
来源：http://on.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hh.9csxet.cn

[R77] 读取用户输入
来源：http://bh.newstarts.cn

read -rp "请输入: " ans
来源：http://gw.jctech888.com.cn

[R78] 交互式菜单
来源：http://nt.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pt.nicolike.cn

[R79] 解析命令行选项
来源：http://uo.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fu.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://rq.nicolike.cn

time ./run.sh
来源：http://bp.szxytkj.cn

================================================================================
来源：http://jp.haigaiapp.cn

S. C / C++ 专题
来源：http://ek.bookmarksfly.cn

================================================================================
来源：http://ve.gzmigu.cn

[S01] C：Hello World
来源：http://gk.shxzukj.cn

#include <stdio.h>
来源：http://qx.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fm.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://of.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://pt.huixinmuqiang.cn

[S03] C：读入整数
来源：http://gk.colortex.cn

int x; scanf("%d", &x);
来源：http://ea.shtwfgs.cn

[S04] C：字符串复制
来源：http://aa.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ys.jctech888.com.cn

[S05] C：字符串长度
来源：http://ff.szsharing.cn

strlen(s)
来源：http://ng.haigaiapp.cn

[S06] C：字符串比较
来源：http://wa.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://rl.shxzukj.cn

[S07] C：数组遍历求和
来源：http://wl.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ey.asd995.cn

[S08] C：动态内存分配与释放
来源：http://dm.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hb.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://tc.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gk.haigaiapp.cn

[S10] C：指针与解引用
来源：http://sj.szsharing.cn

int *p = &a;  *p = 5;
来源：http://jm.shtwfgs.cn

[S11] C：逐行读文件
来源：http://ys.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://we.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gk.wgjwhj.cn

fclose(f);
来源：http://ce.newstarts.cn

[S12] C：写文件
来源：http://jj.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ns.521024.cn

[S13] C：宏定义
来源：http://mh.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gw.wgjwhj.cn

[S14] C：枚举
来源：http://rr.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://mr.shtwfgs.cn

[S15] C：类型转换
来源：http://dr.shxzukj.cn

(double) a / b
来源：http://py.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://rl.lnxyls.cn

x |= (1 << 3);
来源：http://al.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ob.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xu.asd995.cn

[S18] C：命令行参数
来源：http://uy.huanxung.cn

int main(int argc, char **argv)
来源：http://mj.szsharing.cn

[S19] C：快速排序
来源：http://vt.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rv.huanxung.cn

[S20] C：二分查找
来源：http://hz.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uq.hahajie.cn

[S21] C：字符类别判断
来源：http://bk.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vl.colortex.cn

[S22] C：字符串转数字
来源：http://ht.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pk.colortex.cn

[S23] C：随机数
来源：http://ra.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ls.lnxyls.cn

[S24] C：获取本地时间
来源：http://iy.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gu.9csxet.cn

[S25] C：内存拷贝
来源：http://mi.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://ja.hahajie.cn

[S26] C：内存清零
来源：http://tr.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://fj.chemitech.net.cn

[S27] C：定义常量
来源：http://rr.colortex.cn

const double PI = 3.14159;
来源：http://eu.muxihuayi.cn

[S28] C：静态变量
来源：http://am.nszjky.cn

static int counter = 0;
来源：http://wo.panjiajie.cn

[S29] C：变参函数
来源：http://bz.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sr.bjjhwx.cn

[S30] C：头文件保护
来源：http://ra.muxihuayi.cn

#ifndef X_H
来源：http://bt.hahajie.cn

#define X_H
来源：http://qs.hahajie.cn

#endif
来源：http://km.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://vb.bookmarksfly.cn

#include <iostream>
来源：http://uu.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://bi.bjjhwx.cn

[S32] C++：字符串
来源：http://gk.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://cl.yuexingan06.cn

[S33] C++：vector 增删
来源：http://zs.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bm.shxzskj.cn

[S34] C++：遍历 vector
来源：http://ks.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://vz.huanxung.cn

[S35] C++：map
来源：http://sd.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://li.bjjhwx.cn

[S36] C++：unordered_map
来源：http://mx.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kv.521024.cn

[S37] C++：set
来源：http://ab.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ev.yuntaijiaju.cn

[S38] C++：排序
来源：http://jg.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://ui.asd995.cn

[S39] C++：自定义比较器排序
来源：http://ap.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hg.newstarts.cn

[S40] C++：查找元素
来源：http://lj.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hs.szsharing.cn

[S41] C++：类与构造函数
来源：http://iy.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tf.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://sq.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://xa.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://mo.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://bn.colortex.cn

[S44] C++：引用传参
来源：http://mh.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://fz.jctech888.com.cn

[S45] C++：lambda
来源：http://go.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lt.huixiangedu.cn

[S46] C++：函数模板
来源：http://fa.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nf.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://ud.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hf.shxzskj.cn

[S48] C++：逐行读文件
来源：http://qd.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eo.nszjky.cn

while (std::getline(in, line)) { }
来源：http://ti.bjjhwx.cn

[S49] C++：写文件
来源：http://hj.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://he.nszjky.cn

[S50] C++：格式化数字
来源：http://oc.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ih.newstarts.cn

[S51] C++：显式类型转换
来源：http://oe.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ea.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://uf.huanxung.cn

int size() const noexcept { return n_; }
来源：http://ld.bjjhwx.cn

[S53] C++：移动语义
来源：http://eg.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://fj.jctech888.com.cn

[S54] C++：异常处理
来源：http://ma.huanxung.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://so.huanxung.cn

[S55] C++：结构化绑定
来源：http://kx.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uw.hnjuh.cn

[S56] C++：optional
来源：http://qb.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dj.bjjhwx.cn

[S57] C++：编译期常量
来源：http://hb.nicolike.cn

constexpr int N = 10;
来源：http://ic.bjjhwx.cn

[S58] C++：命名空间
来源：http://xv.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://ab.szsharing.cn

[S59] C++：静态断言
来源：http://cy.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sq.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://wq.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dn.shtwfgs.cn

================================================================================
来源：http://rm.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pc.colortex.cn

================================================================================
来源：http://bz.huanxung.cn


<!-- 参考信息 -->