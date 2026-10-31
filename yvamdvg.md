代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cf.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://tm.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gi.521024.cn

================================================================================
来源：http://ni.szsharing.cn

R. Bash 专题
来源：http://nh.muxihuayi.cn

================================================================================
来源：http://qq.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://pf.nicolike.cn

#!/usr/bin/env bash
来源：http://sp.gzmigu.cn

set -euo pipefail
来源：http://oe.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://rb.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://nq.huanxung.cn

[R03] 只读变量
来源：http://kq.gzmigu.cn

readonly PI=3.14
来源：http://or.szxytkj.cn

[R04] 位置参数
来源：http://zf.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ql.jctech888.com.cn

[R05] 参数默认值
来源：http://or.huixinmuqiang.cn

name="${1:-default}"
来源：http://qt.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://jh.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pk.jctech888.com.cn

[R07] if 判断文件
来源：http://fl.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vh.huanxung.cn

[R08] 数值比较
来源：http://ro.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://me.newstarts.cn

[R09] 字符串比较
来源：http://ug.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jh.chemitech.net.cn

[R10] 正则匹配
来源：http://ym.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mz.szxytkj.cn

[R11] case 多分支
来源：http://bk.jctech888.com.cn

case "$1" in
来源：http://ic.lnxyls.cn

start) echo "启动" ;;
来源：http://ze.shxzukj.cn

stop)  echo "停止" ;;
来源：http://re.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://os.hnjuh.cn

esac
来源：http://pt.newstarts.cn

[R12] for 遍历文件
来源：http://nk.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://ry.yuexingan06.cn

[R13] for 计数循环
来源：http://zp.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://dd.yuntaijiaju.cn

[R14] C 风格 for
来源：http://uk.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xv.wgjwhj.cn

[R15] while 逐行读文件
来源：http://hf.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jj.9csxet.cn

[R16] until 等待条件
来源：http://ua.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wx.shtwfgs.cn

[R17] 数组定义与取值
来源：http://qh.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ki.jctech888.com.cn

[R18] 遍历数组
来源：http://ao.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xb.nszjky.cn

[R19] 数组长度
来源：http://pw.panjiajie.cn

echo "${#arr[@]}"
来源：http://zi.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://ev.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ti.szxytkj.cn

[R21] 字符串长度
来源：http://uk.jctech888.com.cn

echo "${#s}"
来源：http://fi.szsharing.cn

[R22] 截取子串
来源：http://nv.gzmigu.cn

echo "${s:0:5}"
来源：http://cp.huanxung.cn

[R23] 字符串替换
来源：http://ri.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tp.hnjuh.cn

[R24] 大小写转换
来源：http://wp.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qq.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://ug.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yz.bookmarksfly.cn

[R26] 命令替换
来源：http://rl.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://cs.panjiajie.cn

[R27] 算术展开
来源：http://tn.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://xi.newstarts.cn

[R28] 浮点运算
来源：http://nl.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://fu.nszjky.cn

[R29] 定义函数
来源：http://tw.huixiangedu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dn.hnjuh.cn

[R30] 函数返回状态码
来源：http://nh.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://ba.muxihuayi.cn

[R31] 局部变量
来源：http://zd.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://pp.9csxet.cn

[R32] 参数个数校验
来源：http://at.huixinmuqiang.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vl.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://em.muxihuayi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ar.colortex.cn

[R34] 退出时清理
来源：http://ab.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fh.shxzukj.cn

[R35] 后台执行并等待
来源：http://ie.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://si.colortex.cn

[R36] 并发执行多个任务
来源：http://yy.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wf.szsharing.cn

[R37] 把输出赋给变量
来源：http://za.chemitech.net.cn

files=$(ls -1)
来源：http://wa.shxzukj.cn

[R38] 管道串联
来源：http://fa.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://gp.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://ez.yuexingan06.cn

cmd > out.log 2>&1
来源：http://wc.asd995.cn

[R40] 追加写日志
来源：http://su.colortex.cn

echo "log" >> out.log
来源：http://dl.haigaiapp.cn

[R41] 丢弃输出
来源：http://it.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://rh.wgjwhj.cn

[R42] 输入重定向
来源：http://cc.huanxung.cn

wc -l < a.txt
来源：http://rz.bookmarksfly.cn

[R43] 按名字查找文件
来源：http://yw.chemitech.net.cn

find . -name "*.log" -type f
来源：http://vi.bookmarksfly.cn

[R44] 按修改时间查找
来源：http://np.haigaiapp.cn

find . -mtime -7 -type f
来源：http://xi.huixinmuqiang.cn

[R45] 批量删除
来源：http://ve.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://gq.521024.cn

[R46] 递归替换文件内容
来源：http://jy.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qy.9csxet.cn

[R47] sed 单行替换
来源：http://bt.szxytkj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lo.chemitech.net.cn

[R48] awk 取指定列
来源：http://vs.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://yx.shxzskj.cn

[R49] awk 带条件
来源：http://xg.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fy.shtwfgs.cn

[R50] awk 求和
来源：http://lf.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vx.nicolike.cn

[R51] 排序去重取前几
来源：http://um.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uv.huanxung.cn

[R52] 统计行数
来源：http://xa.haigaiapp.cn

wc -l a.txt
来源：http://bd.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://tr.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tl.shtwfgs.cn

[R54] 比较两个文件
来源：http://dc.shtwfgs.cn

diff a.txt b.txt
来源：http://fm.hahajie.cn

[R55] 压缩与解压
来源：http://jy.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ij.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://ba.lnxyls.cn

scp file user@host:/path/
来源：http://bv.panjiajie.cn

[R57] 远程执行命令
来源：http://vm.shtwfgs.cn

ssh user@host 'uptime'
来源：http://ca.huixiangedu.cn

[R58] 下载文件
来源：http://vl.newstarts.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://la.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://ot.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lf.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://qv.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lk.asd995.cn

[R61] 磁盘占用
来源：http://ob.shxzskj.cn

df -h;  du -sh *
来源：http://ln.nszjky.cn

[R62] 找最占空间的文件
来源：http://at.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://or.wgjwhj.cn

[R63] 内存与进程
来源：http://hk.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://kk.huanxung.cn

[R64] 结束进程
来源：http://xm.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://ay.szsharing.cn

[R65] 查看端口占用
来源：http://vv.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ef.shxzskj.cn

[R66] 定时任务
来源：http://wf.szsharing.cn

crontab -e;  crontab -l
来源：http://um.huanxung.cn

[R67] 生成随机十六进制串
来源：http://mm.yuntaijiaju.cn

openssl rand -hex 16
来源：http://ej.shxzukj.cn

[R68] 计算文件校验值
来源：http://ka.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ks.haigaiapp.cn

[R69] 生成随机密码
来源：http://ey.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://ib.nszjky.cn

[R70] 时间戳与互转
来源：http://do.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://sj.lnxyls.cn

[R71] 日期格式化
来源：http://sa.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ah.jctech888.com.cn

[R72] 等待端口就绪
来源：http://px.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jc.nicolike.cn

[R73] 分割大日志
来源：http://pk.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://ha.jianghongdianzi.cn

[R74] 批量重命名
来源：http://yn.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vc.muxihuayi.cn

[R75] 导出环境变量
来源：http://hh.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://yl.muxihuayi.cn

[R76] 使用临时文件
来源：http://yl.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nv.yuexingan06.cn

[R77] 读取用户输入
来源：http://tt.haigaiapp.cn

read -rp "请输入: " ans
来源：http://je.gzmigu.cn

[R78] 交互式菜单
来源：http://rw.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yd.yuexingan06.cn

[R79] 解析命令行选项
来源：http://qi.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eh.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://sv.yuexingan06.cn

time ./run.sh
来源：http://aj.huixiangedu.cn

================================================================================
来源：http://op.panjiajie.cn

S. C / C++ 专题
来源：http://yf.huixiangedu.cn

================================================================================
来源：http://dc.bjjhwx.cn

[S01] C：Hello World
来源：http://cj.nszjky.cn

#include <stdio.h>
来源：http://qc.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://of.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://mk.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://gx.szsharing.cn

[S03] C：读入整数
来源：http://rt.shxzskj.cn

int x; scanf("%d", &x);
来源：http://yc.shxzskj.cn

[S04] C：字符串复制
来源：http://fn.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cr.shtwfgs.cn

[S05] C：字符串长度
来源：http://if.shxzskj.cn

strlen(s)
来源：http://sx.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://qa.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://at.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://zd.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wx.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ab.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ho.521024.cn

[S09] C：结构体定义与初始化
来源：http://fj.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rs.hnjuh.cn

[S10] C：指针与解引用
来源：http://ky.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://jb.szsharing.cn

[S11] C：逐行读文件
来源：http://cf.gzmigu.cn

FILE *f = fopen("a.txt", "r");
来源：http://pj.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uq.shxzskj.cn

fclose(f);
来源：http://sk.asd995.cn

[S12] C：写文件
来源：http://lx.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fz.shtwfgs.cn

[S13] C：宏定义
来源：http://ih.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wo.newstarts.cn

[S14] C：枚举
来源：http://aj.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://fx.huanxung.cn

[S15] C：类型转换
来源：http://lj.bjjhwx.cn

(double) a / b
来源：http://ne.521024.cn

[S16] C：位操作置位
来源：http://xq.hahajie.cn

x |= (1 << 3);
来源：http://ia.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://hd.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qy.shtwfgs.cn

[S18] C：命令行参数
来源：http://zq.bjjhwx.cn

int main(int argc, char **argv)
来源：http://mv.shxzukj.cn

[S19] C：快速排序
来源：http://mz.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ee.wgjwhj.cn

[S20] C：二分查找
来源：http://cw.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mo.yuexingan06.cn

[S21] C：字符类别判断
来源：http://fe.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mx.521024.cn

[S22] C：字符串转数字
来源：http://mi.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rh.yuntaijiaju.cn

[S23] C：随机数
来源：http://os.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ce.asd995.cn

[S24] C：获取本地时间
来源：http://sy.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yy.bjjhwx.cn

[S25] C：内存拷贝
来源：http://om.wgjwhj.cn

memcpy(dst, src, n);
来源：http://gr.jianghongdianzi.cn

[S26] C：内存清零
来源：http://dt.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://aq.nicolike.cn

[S27] C：定义常量
来源：http://re.newstarts.cn

const double PI = 3.14159;
来源：http://td.wgjwhj.cn

[S28] C：静态变量
来源：http://gw.huanxung.cn

static int counter = 0;
来源：http://ww.newstarts.cn

[S29] C：变参函数
来源：http://ig.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wk.chemitech.net.cn

[S30] C：头文件保护
来源：http://kq.nicolike.cn

#ifndef X_H
来源：http://nn.szxytkj.cn

#define X_H
来源：http://fo.jianghongdianzi.cn

#endif
来源：http://fc.wgjwhj.cn

[S31] C++：Hello World
来源：http://xw.521024.cn

#include <iostream>
来源：http://nq.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://pr.gzmigu.cn

[S32] C++：字符串
来源：http://bv.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://jr.nszjky.cn

[S33] C++：vector 增删
来源：http://jh.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wt.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://qy.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://pt.bookmarksfly.cn

[S35] C++：map
来源：http://sj.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xt.huixiangedu.cn

[S36] C++：unordered_map
来源：http://wd.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vj.jctech888.com.cn

[S37] C++：set
来源：http://fy.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eh.yuexingan06.cn

[S38] C++：排序
来源：http://gr.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://bf.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://pt.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://up.colortex.cn

[S40] C++：查找元素
来源：http://br.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wm.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://nz.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wh.szsharing.cn

[S42] C++：继承与虚函数
来源：http://tq.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://tc.nicolike.cn

[S43] C++：智能指针
来源：http://zk.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://qj.newstarts.cn

[S44] C++：引用传参
来源：http://la.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://aq.yuexingan06.cn

[S45] C++：lambda
来源：http://tp.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fv.lnxyls.cn

[S46] C++：函数模板
来源：http://iz.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gx.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://gz.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qb.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://rm.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dt.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://as.asd995.cn

[S49] C++：写文件
来源：http://vx.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rj.hnjuh.cn

[S50] C++：格式化数字
来源：http://ab.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hj.shxzskj.cn

[S51] C++：显式类型转换
来源：http://qc.jctech888.com.cn

static_cast<double>(a) / b
来源：http://ep.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://th.521024.cn

int size() const noexcept { return n_; }
来源：http://jk.muxihuayi.cn

[S53] C++：移动语义
来源：http://ap.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://xi.newstarts.cn

[S54] C++：异常处理
来源：http://ir.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ry.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://fw.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kd.huanxung.cn

[S56] C++：optional
来源：http://yr.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tn.9csxet.cn

[S57] C++：编译期常量
来源：http://ql.yuntaijiaju.cn

constexpr int N = 10;
来源：http://tw.asd995.cn

[S58] C++：命名空间
来源：http://si.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://oq.yuntaijiaju.cn

[S59] C++：静态断言
来源：http://ob.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://in.bjjhwx.cn

[S60] C++：遍历并删除元素
来源：http://pu.nicolike.cn


<!-- 参考信息 -->