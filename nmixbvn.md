代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://ng.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gp.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mo.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://sa.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ex.bookmarksfly.cn

[Q90] 生成序号列
来源：http://ns.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fl.szsharing.cn

================================================================================
来源：http://er.nicolike.cn

R. Bash 专题
来源：http://zg.nicolike.cn

================================================================================
来源：http://zt.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://xg.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://qk.szsharing.cn

set -euo pipefail
来源：http://qo.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://uk.szxytkj.cn

name="Tom"; echo "$name"
来源：http://xu.szsharing.cn

[R03] 只读变量
来源：http://xs.colortex.cn

readonly PI=3.14
来源：http://xl.huixiangedu.cn

[R04] 位置参数
来源：http://vv.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ra.muxihuayi.cn

[R05] 参数默认值
来源：http://nj.haigaiapp.cn

name="${1:-default}"
来源：http://jk.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://ay.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rg.jianghongdianzi.cn

[R07] if 判断文件
来源：http://tj.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://px.huanxung.cn

[R08] 数值比较
来源：http://py.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jl.shtwfgs.cn

[R09] 字符串比较
来源：http://nt.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tv.gzmigu.cn

[R10] 正则匹配
来源：http://id.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://th.jianghongdianzi.cn

[R11] case 多分支
来源：http://cl.521024.cn

case "$1" in
来源：http://zc.shxzskj.cn

start) echo "启动" ;;
来源：http://mz.9csxet.cn

stop)  echo "停止" ;;
来源：http://js.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://fr.bookmarksfly.cn

esac
来源：http://qo.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://fd.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://na.newstarts.cn

[R13] for 计数循环
来源：http://eb.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://xi.yuexingan06.cn

[R14] C 风格 for
来源：http://pt.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uu.shxzskj.cn

[R15] while 逐行读文件
来源：http://sb.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dg.nszjky.cn

[R16] until 等待条件
来源：http://rb.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ug.haigaiapp.cn

[R17] 数组定义与取值
来源：http://qj.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gg.chemitech.net.cn

[R18] 遍历数组
来源：http://wx.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yt.bookmarksfly.cn

[R19] 数组长度
来源：http://nh.nicolike.cn

echo "${#arr[@]}"
来源：http://xz.szxytkj.cn

[R20] 关联数组（字典）
来源：http://gn.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vu.gzmigu.cn

[R21] 字符串长度
来源：http://zd.muxihuayi.cn

echo "${#s}"
来源：http://uq.shxzskj.cn

[R22] 截取子串
来源：http://kz.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://lv.shxzskj.cn

[R23] 字符串替换
来源：http://kn.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ku.panjiajie.cn

[R24] 大小写转换
来源：http://at.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fb.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://hd.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ta.shtwfgs.cn

[R26] 命令替换
来源：http://lg.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://as.shtwfgs.cn

[R27] 算术展开
来源：http://by.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://jt.nszjky.cn

[R28] 浮点运算
来源：http://mk.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://py.huanxung.cn

[R29] 定义函数
来源：http://ya.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ae.szxytkj.cn

[R30] 函数返回状态码
来源：http://il.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://ig.yuexingan06.cn

[R31] 局部变量
来源：http://dj.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://es.bookmarksfly.cn

[R32] 参数个数校验
来源：http://gq.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xh.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://wc.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qz.chemitech.net.cn

[R34] 退出时清理
来源：http://rk.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rm.gzmigu.cn

[R35] 后台执行并等待
来源：http://rc.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lx.9csxet.cn

[R36] 并发执行多个任务
来源：http://go.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xm.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://lu.bookmarksfly.cn

files=$(ls -1)
来源：http://mw.huixiangedu.cn

[R38] 管道串联
来源：http://dd.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://ko.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://yg.huanxung.cn

cmd > out.log 2>&1
来源：http://gr.jctech888.com.cn

[R40] 追加写日志
来源：http://uc.yuexingan06.cn

echo "log" >> out.log
来源：http://fe.nszjky.cn

[R41] 丢弃输出
来源：http://tw.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://dy.szsharing.cn

[R42] 输入重定向
来源：http://pz.haigaiapp.cn

wc -l < a.txt
来源：http://vo.panjiajie.cn

[R43] 按名字查找文件
来源：http://cm.panjiajie.cn

find . -name "*.log" -type f
来源：http://df.huanxung.cn

[R44] 按修改时间查找
来源：http://gf.huanxung.cn

find . -mtime -7 -type f
来源：http://nq.shxzukj.cn

[R45] 批量删除
来源：http://gm.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://zl.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://yq.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ty.huanxung.cn

[R47] sed 单行替换
来源：http://xi.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lp.hnjuh.cn

[R48] awk 取指定列
来源：http://pu.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://tt.521024.cn

[R49] awk 带条件
来源：http://oe.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://td.yuexingan06.cn

[R50] awk 求和
来源：http://ri.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uz.gzmigu.cn

[R51] 排序去重取前几
来源：http://lz.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ei.panjiajie.cn

[R52] 统计行数
来源：http://ua.hahajie.cn

wc -l a.txt
来源：http://ik.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://qp.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mm.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://al.bookmarksfly.cn

diff a.txt b.txt
来源：http://br.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://za.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kh.bookmarksfly.cn

[R56] 远程拷贝
来源：http://xa.521024.cn

scp file user@host:/path/
来源：http://we.newstarts.cn

[R57] 远程执行命令
来源：http://fs.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://ru.newstarts.cn

[R58] 下载文件
来源：http://wz.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dx.yuexingan06.cn

[R59] 发 POST JSON
来源：http://em.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ra.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://tr.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wa.9csxet.cn

[R61] 磁盘占用
来源：http://zf.yuexingan06.cn

df -h;  du -sh *
来源：http://fs.521024.cn

[R62] 找最占空间的文件
来源：http://hr.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://im.bjjhwx.cn

[R63] 内存与进程
来源：http://xa.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://zt.haigaiapp.cn

[R64] 结束进程
来源：http://mt.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ra.bjjhwx.cn

[R65] 查看端口占用
来源：http://fd.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wy.newstarts.cn

[R66] 定时任务
来源：http://fy.wgjwhj.cn

crontab -e;  crontab -l
来源：http://nu.nicolike.cn

[R67] 生成随机十六进制串
来源：http://lh.shtwfgs.cn

openssl rand -hex 16
来源：http://or.yuexingan06.cn

[R68] 计算文件校验值
来源：http://im.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cy.shtwfgs.cn

[R69] 生成随机密码
来源：http://mc.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://dh.lnxyls.cn

[R70] 时间戳与互转
来源：http://gw.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://aw.jctech888.com.cn

[R71] 日期格式化
来源：http://dl.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lp.gzmigu.cn

[R72] 等待端口就绪
来源：http://yz.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xb.bjjhwx.cn

[R73] 分割大日志
来源：http://go.hahajie.cn

split -l 1000 big.log part_
来源：http://jq.huixiangedu.cn

[R74] 批量重命名
来源：http://gs.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nd.9csxet.cn

[R75] 导出环境变量
来源：http://hu.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://qa.shxzukj.cn

[R76] 使用临时文件
来源：http://jt.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://px.haigaiapp.cn

[R77] 读取用户输入
来源：http://gr.9csxet.cn

read -rp "请输入: " ans
来源：http://au.asd995.cn

[R78] 交互式菜单
来源：http://cx.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hp.panjiajie.cn

[R79] 解析命令行选项
来源：http://fr.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dq.yuntaijiaju.cn

[R80] 查看脚本执行耗时
来源：http://cf.chemitech.net.cn

time ./run.sh
来源：http://kf.muxihuayi.cn

================================================================================
来源：http://af.muxihuayi.cn

S. C / C++ 专题
来源：http://qr.huanxung.cn

================================================================================
来源：http://ko.haigaiapp.cn

[S01] C：Hello World
来源：http://vr.haigaiapp.cn

#include <stdio.h>
来源：http://xw.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nd.521024.cn

[S02] C：变量与格式化输出
来源：http://xh.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://td.yuexingan06.cn

[S03] C：读入整数
来源：http://as.521024.cn

int x; scanf("%d", &x);
来源：http://dl.bookmarksfly.cn

[S04] C：字符串复制
来源：http://un.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nj.shxzskj.cn

[S05] C：字符串长度
来源：http://ax.muxihuayi.cn

strlen(s)
来源：http://ha.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://oh.bjjhwx.cn

strcmp(a, b) == 0
来源：http://py.lnxyls.cn

[S07] C：数组遍历求和
来源：http://sn.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qa.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://li.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eh.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://ra.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hg.shxzskj.cn

[S10] C：指针与解引用
来源：http://aj.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://ds.jctech888.com.cn

[S11] C：逐行读文件
来源：http://au.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://cp.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lw.jianghongdianzi.cn

fclose(f);
来源：http://ah.gzmigu.cn

[S12] C：写文件
来源：http://yj.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wy.9csxet.cn

[S13] C：宏定义
来源：http://jg.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tu.szsharing.cn

[S14] C：枚举
来源：http://al.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://dl.wgjwhj.cn

[S15] C：类型转换
来源：http://ec.bookmarksfly.cn

(double) a / b
来源：http://is.colortex.cn

[S16] C：位操作置位
来源：http://ry.yuntaijiaju.cn

x |= (1 << 3);
来源：http://he.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://it.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://md.jctech888.com.cn

[S18] C：命令行参数
来源：http://kg.asd995.cn

int main(int argc, char **argv)
来源：http://ai.jctech888.com.cn

[S19] C：快速排序
来源：http://eu.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ou.jctech888.com.cn

[S20] C：二分查找
来源：http://bg.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pf.bjjhwx.cn

[S21] C：字符类别判断
来源：http://qr.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ue.newstarts.cn

[S22] C：字符串转数字
来源：http://td.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rd.nicolike.cn

[S23] C：随机数
来源：http://pt.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kv.lnxyls.cn

[S24] C：获取本地时间
来源：http://fp.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://me.shtwfgs.cn

[S25] C：内存拷贝
来源：http://up.9csxet.cn

memcpy(dst, src, n);
来源：http://hi.bookmarksfly.cn

[S26] C：内存清零
来源：http://ij.9csxet.cn

memset(a, 0, sizeof a);
来源：http://dc.hahajie.cn

[S27] C：定义常量
来源：http://jp.521024.cn

const double PI = 3.14159;
来源：http://xv.lnxyls.cn

[S28] C：静态变量
来源：http://yy.huixiangedu.cn

static int counter = 0;
来源：http://tr.bookmarksfly.cn

[S29] C：变参函数
来源：http://tk.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yd.chemitech.net.cn

[S30] C：头文件保护
来源：http://jk.jctech888.com.cn

#ifndef X_H
来源：http://zj.wgjwhj.cn

#define X_H
来源：http://aj.lnxyls.cn

#endif
来源：http://an.szsharing.cn

[S31] C++：Hello World
来源：http://rh.huanxung.cn

#include <iostream>
来源：http://hk.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://pw.chemitech.net.cn

[S32] C++：字符串
来源：http://ft.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://bn.shtwfgs.cn

[S33] C++：vector 增删
来源：http://oi.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nu.shxzskj.cn

[S34] C++：遍历 vector
来源：http://zf.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://dn.asd995.cn

[S35] C++：map
来源：http://cn.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fs.shxzukj.cn

[S36] C++：unordered_map
来源：http://pg.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fb.chemitech.net.cn

[S37] C++：set
来源：http://me.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tm.521024.cn

[S38] C++：排序
来源：http://dd.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://ac.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://qv.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wz.bookmarksfly.cn

[S40] C++：查找元素
来源：http://yf.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qd.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://fi.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nz.hahajie.cn

[S42] C++：继承与虚函数
来源：http://bg.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://vb.huanxung.cn

[S43] C++：智能指针
来源：http://ms.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://io.yuexingan06.cn

[S44] C++：引用传参
来源：http://ym.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://db.wgjwhj.cn

[S45] C++：lambda
来源：http://vt.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bt.bjjhwx.cn

[S46] C++：函数模板
来源：http://cg.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vp.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://ej.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fk.shxzskj.cn

[S48] C++：逐行读文件
来源：http://sj.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ek.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://cz.huixiangedu.cn

[S49] C++：写文件
来源：http://tp.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mk.huixiangedu.cn

[S50] C++：格式化数字
来源：http://wy.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ge.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://kr.hahajie.cn

static_cast<double>(a) / b
来源：http://lf.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://fe.colortex.cn

int size() const noexcept { return n_; }
来源：http://ze.szxytkj.cn

[S53] C++：移动语义
来源：http://kh.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://hd.nszjky.cn

[S54] C++：异常处理
来源：http://sb.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pl.hahajie.cn

[S55] C++：结构化绑定
来源：http://zg.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sj.jianghongdianzi.cn

[S56] C++：optional
来源：http://fb.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kc.jctech888.com.cn

[S57] C++：编译期常量
来源：http://tt.9csxet.cn

constexpr int N = 10;
来源：http://ts.nicolike.cn

[S58] C++：命名空间
来源：http://nk.521024.cn


<!-- 参考信息 -->