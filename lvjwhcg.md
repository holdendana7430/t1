代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://io.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qq.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jm.hahajie.cn

[Q89] 判断表是否存在
来源：http://wr.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xl.bookmarksfly.cn

[Q90] 生成序号列
来源：http://iu.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lc.huanxung.cn

================================================================================
来源：http://zc.shxzukj.cn

R. Bash 专题
来源：http://rl.newstarts.cn

================================================================================
来源：http://ia.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://xf.chemitech.net.cn

#!/usr/bin/env bash
来源：http://ab.haigaiapp.cn

set -euo pipefail
来源：http://nd.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://jj.shxzskj.cn

name="Tom"; echo "$name"
来源：http://rb.szxytkj.cn

[R03] 只读变量
来源：http://md.gzmigu.cn

readonly PI=3.14
来源：http://fk.haigaiapp.cn

[R04] 位置参数
来源：http://cb.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mc.shxzskj.cn

[R05] 参数默认值
来源：http://np.bjjhwx.cn

name="${1:-default}"
来源：http://gm.nicolike.cn

[R06] 判断命令是否存在
来源：http://tb.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qe.521024.cn

[R07] if 判断文件
来源：http://hn.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wq.shtwfgs.cn

[R08] 数值比较
来源：http://gj.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hx.asd995.cn

[R09] 字符串比较
来源：http://mc.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bm.yuexingan06.cn

[R10] 正则匹配
来源：http://nu.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ex.jctech888.com.cn

[R11] case 多分支
来源：http://ch.nszjky.cn

case "$1" in
来源：http://bz.newstarts.cn

start) echo "启动" ;;
来源：http://mm.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://ik.nszjky.cn

*)     echo "未知命令" ;;
来源：http://cz.wgjwhj.cn

esac
来源：http://bz.szxytkj.cn

[R12] for 遍历文件
来源：http://ny.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://qx.jianghongdianzi.cn

[R13] for 计数循环
来源：http://bz.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://re.szxytkj.cn

[R14] C 风格 for
来源：http://cj.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ca.gzmigu.cn

[R15] while 逐行读文件
来源：http://ib.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://om.newstarts.cn

[R16] until 等待条件
来源：http://ey.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gk.newstarts.cn

[R17] 数组定义与取值
来源：http://dh.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yc.bjjhwx.cn

[R18] 遍历数组
来源：http://vy.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wp.jianghongdianzi.cn

[R19] 数组长度
来源：http://fk.asd995.cn

echo "${#arr[@]}"
来源：http://rg.shxzskj.cn

[R20] 关联数组（字典）
来源：http://sy.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rr.521024.cn

[R21] 字符串长度
来源：http://ft.shxzskj.cn

echo "${#s}"
来源：http://pj.haigaiapp.cn

[R22] 截取子串
来源：http://ps.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://jc.yuexingan06.cn

[R23] 字符串替换
来源：http://pl.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uq.newstarts.cn

[R24] 大小写转换
来源：http://li.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vc.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://nw.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rt.bjjhwx.cn

[R26] 命令替换
来源：http://fz.asd995.cn

now=$(date +%F); echo "$now"
来源：http://lr.huanxung.cn

[R27] 算术展开
来源：http://gq.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://sm.nszjky.cn

[R28] 浮点运算
来源：http://kp.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://dm.9csxet.cn

[R29] 定义函数
来源：http://hx.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ys.hahajie.cn

[R30] 函数返回状态码
来源：http://yg.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://zt.bjjhwx.cn

[R31] 局部变量
来源：http://pb.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://te.szsharing.cn

[R32] 参数个数校验
来源：http://vu.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lm.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://oh.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vx.yuntaijiaju.cn

[R34] 退出时清理
来源：http://yn.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mi.bjjhwx.cn

[R35] 后台执行并等待
来源：http://zj.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://po.panjiajie.cn

[R36] 并发执行多个任务
来源：http://yg.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fv.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://yz.chemitech.net.cn

files=$(ls -1)
来源：http://za.chemitech.net.cn

[R38] 管道串联
来源：http://ws.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://ty.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://aa.gzmigu.cn

cmd > out.log 2>&1
来源：http://tq.huanxung.cn

[R40] 追加写日志
来源：http://fd.jianghongdianzi.cn

echo "log" >> out.log
来源：http://cd.521024.cn

[R41] 丢弃输出
来源：http://gm.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://dv.colortex.cn

[R42] 输入重定向
来源：http://ue.colortex.cn

wc -l < a.txt
来源：http://vq.newstarts.cn

[R43] 按名字查找文件
来源：http://sr.newstarts.cn

find . -name "*.log" -type f
来源：http://ms.nszjky.cn

[R44] 按修改时间查找
来源：http://ml.colortex.cn

find . -mtime -7 -type f
来源：http://vc.huanxung.cn

[R45] 批量删除
来源：http://vo.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://hw.nicolike.cn

[R46] 递归替换文件内容
来源：http://qy.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ot.nicolike.cn

[R47] sed 单行替换
来源：http://ft.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xk.szxytkj.cn

[R48] awk 取指定列
来源：http://ir.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://ff.hahajie.cn

[R49] awk 带条件
来源：http://gc.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ng.muxihuayi.cn

[R50] awk 求和
来源：http://yp.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ly.haigaiapp.cn

[R51] 排序去重取前几
来源：http://rr.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ga.lnxyls.cn

[R52] 统计行数
来源：http://rv.9csxet.cn

wc -l a.txt
来源：http://rr.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://zg.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wr.9csxet.cn

[R54] 比较两个文件
来源：http://kl.szsharing.cn

diff a.txt b.txt
来源：http://pf.hahajie.cn

[R55] 压缩与解压
来源：http://hk.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://du.bookmarksfly.cn

[R56] 远程拷贝
来源：http://ez.jctech888.com.cn

scp file user@host:/path/
来源：http://ch.521024.cn

[R57] 远程执行命令
来源：http://xm.521024.cn

ssh user@host 'uptime'
来源：http://wm.shxzukj.cn

[R58] 下载文件
来源：http://rx.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ou.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://jb.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ij.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ae.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bj.asd995.cn

[R61] 磁盘占用
来源：http://ib.panjiajie.cn

df -h;  du -sh *
来源：http://yv.asd995.cn

[R62] 找最占空间的文件
来源：http://ip.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://gd.hnjuh.cn

[R63] 内存与进程
来源：http://oc.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://yy.shxzskj.cn

[R64] 结束进程
来源：http://nh.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://yn.newstarts.cn

[R65] 查看端口占用
来源：http://bl.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jc.9csxet.cn

[R66] 定时任务
来源：http://bd.muxihuayi.cn

crontab -e;  crontab -l
来源：http://hn.9csxet.cn

[R67] 生成随机十六进制串
来源：http://tz.wgjwhj.cn

openssl rand -hex 16
来源：http://kn.szsharing.cn

[R68] 计算文件校验值
来源：http://sb.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fx.521024.cn

[R69] 生成随机密码
来源：http://lc.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://fe.hahajie.cn

[R70] 时间戳与互转
来源：http://qt.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://ha.nszjky.cn

[R71] 日期格式化
来源：http://xb.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ku.colortex.cn

[R72] 等待端口就绪
来源：http://vh.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ly.shxzskj.cn

[R73] 分割大日志
来源：http://st.jctech888.com.cn

split -l 1000 big.log part_
来源：http://rv.huixiangedu.cn

[R74] 批量重命名
来源：http://lx.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rx.bjjhwx.cn

[R75] 导出环境变量
来源：http://ww.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://ea.szxytkj.cn

[R76] 使用临时文件
来源：http://ro.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://um.shxzukj.cn

[R77] 读取用户输入
来源：http://zp.shxzskj.cn

read -rp "请输入: " ans
来源：http://lr.wgjwhj.cn

[R78] 交互式菜单
来源：http://xd.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fd.521024.cn

[R79] 解析命令行选项
来源：http://ow.szxytkj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fs.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://cy.521024.cn

time ./run.sh
来源：http://nd.szsharing.cn

================================================================================
来源：http://cp.jianghongdianzi.cn

S. C / C++ 专题
来源：http://dx.huixiangedu.cn

================================================================================
来源：http://zj.panjiajie.cn

[S01] C：Hello World
来源：http://fy.9csxet.cn

#include <stdio.h>
来源：http://gl.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fm.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://hp.wgjwhj.cn

int a = 10; printf("%d\n", a);
来源：http://py.panjiajie.cn

[S03] C：读入整数
来源：http://or.gzmigu.cn

int x; scanf("%d", &x);
来源：http://bl.gzmigu.cn

[S04] C：字符串复制
来源：http://jc.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cc.huanxung.cn

[S05] C：字符串长度
来源：http://aw.bjjhwx.cn

strlen(s)
来源：http://oh.huanxung.cn

[S06] C：字符串比较
来源：http://nt.szxytkj.cn

strcmp(a, b) == 0
来源：http://ji.lnxyls.cn

[S07] C：数组遍历求和
来源：http://ea.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://at.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://xz.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sy.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://ci.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qf.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://yf.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://pm.wgjwhj.cn

[S11] C：逐行读文件
来源：http://cu.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://co.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rn.hahajie.cn

fclose(f);
来源：http://pc.shxzukj.cn

[S12] C：写文件
来源：http://ps.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pq.huixinmuqiang.cn

[S13] C：宏定义
来源：http://jo.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tk.huixiangedu.cn

[S14] C：枚举
来源：http://sk.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://lz.jctech888.com.cn

[S15] C：类型转换
来源：http://tu.bookmarksfly.cn

(double) a / b
来源：http://js.gzmigu.cn

[S16] C：位操作置位
来源：http://ar.9csxet.cn

x |= (1 << 3);
来源：http://va.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://xi.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uw.panjiajie.cn

[S18] C：命令行参数
来源：http://gc.9csxet.cn

int main(int argc, char **argv)
来源：http://th.yuexingan06.cn

[S19] C：快速排序
来源：http://zj.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ep.huixiangedu.cn

[S20] C：二分查找
来源：http://nk.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fr.gzmigu.cn

[S21] C：字符类别判断
来源：http://wf.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ds.shxzskj.cn

[S22] C：字符串转数字
来源：http://eo.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ht.haigaiapp.cn

[S23] C：随机数
来源：http://vp.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://id.huixiangedu.cn

[S24] C：获取本地时间
来源：http://wb.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ii.yuexingan06.cn

[S25] C：内存拷贝
来源：http://qm.szxytkj.cn

memcpy(dst, src, n);
来源：http://du.newstarts.cn

[S26] C：内存清零
来源：http://hm.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://df.hnjuh.cn

[S27] C：定义常量
来源：http://zf.hahajie.cn

const double PI = 3.14159;
来源：http://lh.wgjwhj.cn

[S28] C：静态变量
来源：http://iu.bjjhwx.cn

static int counter = 0;
来源：http://vt.haigaiapp.cn

[S29] C：变参函数
来源：http://ky.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cz.bookmarksfly.cn

[S30] C：头文件保护
来源：http://mb.asd995.cn

#ifndef X_H
来源：http://cw.jctech888.com.cn

#define X_H
来源：http://bj.wgjwhj.cn

#endif
来源：http://hk.asd995.cn

[S31] C++：Hello World
来源：http://iu.muxihuayi.cn

#include <iostream>
来源：http://op.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ft.hnjuh.cn

[S32] C++：字符串
来源：http://zc.colortex.cn

std::string s = "hi";  s += "!";
来源：http://qp.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://qk.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pr.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://ib.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://ro.yuexingan06.cn

[S35] C++：map
来源：http://fs.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ra.nicolike.cn

[S36] C++：unordered_map
来源：http://lv.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sb.szsharing.cn

[S37] C++：set
来源：http://xc.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ei.newstarts.cn

[S38] C++：排序
来源：http://nw.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://fn.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://id.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xp.muxihuayi.cn

[S40] C++：查找元素
来源：http://so.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ax.newstarts.cn

[S41] C++：类与构造函数
来源：http://dz.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ly.huanxung.cn

[S42] C++：继承与虚函数
来源：http://hh.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://vz.9csxet.cn

[S43] C++：智能指针
来源：http://bf.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://ea.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://fa.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://du.hnjuh.cn

[S45] C++：lambda
来源：http://ig.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dl.lnxyls.cn

[S46] C++：函数模板
来源：http://xm.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sb.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://sd.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ee.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://eo.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ba.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://hk.szxytkj.cn

[S49] C++：写文件
来源：http://ds.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wo.muxihuayi.cn

[S50] C++：格式化数字
来源：http://de.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mj.asd995.cn

[S51] C++：显式类型转换
来源：http://oe.hnjuh.cn

static_cast<double>(a) / b
来源：http://cz.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://mz.szsharing.cn

int size() const noexcept { return n_; }
来源：http://to.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://rp.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://he.haigaiapp.cn

[S54] C++：异常处理
来源：http://an.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rm.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ul.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ot.huanxung.cn

[S56] C++：optional
来源：http://yh.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zw.huixiangedu.cn

[S57] C++：编译期常量
来源：http://kj.yuntaijiaju.cn

constexpr int N = 10;
来源：http://cj.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://no.colortex.cn


<!-- 参考信息 -->