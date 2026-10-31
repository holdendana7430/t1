代发 wailian999

[Q84] 去除首尾空格
来源：http://ov.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://ci.asd995.cn

[Q85] 数值取整
来源：http://fv.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ny.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://zz.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vt.hahajie.cn

[Q87] JSON 字段做条件
来源：http://ib.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jb.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://yf.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nz.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fy.hahajie.cn

[Q89] 判断表是否存在
来源：http://lh.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cr.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://ym.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zh.nicolike.cn

================================================================================
来源：http://ag.shxzukj.cn

R. Bash 专题
来源：http://rd.huanxung.cn

================================================================================
来源：http://hj.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://ht.nicolike.cn

#!/usr/bin/env bash
来源：http://vk.newstarts.cn

set -euo pipefail
来源：http://zc.nszjky.cn

[R02] 变量赋值与使用
来源：http://kw.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://xo.yuexingan06.cn

[R03] 只读变量
来源：http://ux.gzmigu.cn

readonly PI=3.14
来源：http://lz.yuntaijiaju.cn

[R04] 位置参数
来源：http://go.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://az.nicolike.cn

[R05] 参数默认值
来源：http://ly.szsharing.cn

name="${1:-default}"
来源：http://jg.shxzskj.cn

[R06] 判断命令是否存在
来源：http://hk.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://er.shxzukj.cn

[R07] if 判断文件
来源：http://pz.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rk.newstarts.cn

[R08] 数值比较
来源：http://fh.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ui.yuexingan06.cn

[R09] 字符串比较
来源：http://zt.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zu.huanxung.cn

[R10] 正则匹配
来源：http://tz.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rh.shxzskj.cn

[R11] case 多分支
来源：http://ne.bjjhwx.cn

case "$1" in
来源：http://lm.colortex.cn

start) echo "启动" ;;
来源：http://jr.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://ua.asd995.cn

*)     echo "未知命令" ;;
来源：http://fp.bookmarksfly.cn

esac
来源：http://vh.huixiangedu.cn

[R12] for 遍历文件
来源：http://ts.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://bd.colortex.cn

[R13] for 计数循环
来源：http://by.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://yo.szxytkj.cn

[R14] C 风格 for
来源：http://me.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ki.wgjwhj.cn

[R15] while 逐行读文件
来源：http://oi.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mi.huanxung.cn

[R16] until 等待条件
来源：http://jf.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fd.yuexingan06.cn

[R17] 数组定义与取值
来源：http://hv.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://le.muxihuayi.cn

[R18] 遍历数组
来源：http://zm.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xw.szxytkj.cn

[R19] 数组长度
来源：http://wj.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://ok.asd995.cn

[R20] 关联数组（字典）
来源：http://kl.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ft.nszjky.cn

[R21] 字符串长度
来源：http://vf.yuexingan06.cn

echo "${#s}"
来源：http://ik.521024.cn

[R22] 截取子串
来源：http://fj.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://hq.huixinmuqiang.cn

[R23] 字符串替换
来源：http://vu.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nj.huanxung.cn

[R24] 大小写转换
来源：http://uf.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kf.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://yf.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jg.colortex.cn

[R26] 命令替换
来源：http://rz.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://dq.nszjky.cn

[R27] 算术展开
来源：http://qm.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://lu.521024.cn

[R28] 浮点运算
来源：http://ft.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://eo.szxytkj.cn

[R29] 定义函数
来源：http://ig.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rj.lnxyls.cn

[R30] 函数返回状态码
来源：http://pz.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://dw.huixinmuqiang.cn

[R31] 局部变量
来源：http://bw.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://kk.panjiajie.cn

[R32] 参数个数校验
来源：http://he.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ka.chemitech.net.cn

[R33] 捕获错误并提示行号
来源：http://xh.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tb.colortex.cn

[R34] 退出时清理
来源：http://rb.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zn.nicolike.cn

[R35] 后台执行并等待
来源：http://pb.nszjky.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gy.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://dc.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ea.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://eo.wgjwhj.cn

files=$(ls -1)
来源：http://hu.jianghongdianzi.cn

[R38] 管道串联
来源：http://lf.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://al.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://yh.jctech888.com.cn

cmd > out.log 2>&1
来源：http://ek.hnjuh.cn

[R40] 追加写日志
来源：http://jd.bjjhwx.cn

echo "log" >> out.log
来源：http://an.shxzskj.cn

[R41] 丢弃输出
来源：http://ta.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://hj.haigaiapp.cn

[R42] 输入重定向
来源：http://pl.nicolike.cn

wc -l < a.txt
来源：http://zl.shxzukj.cn

[R43] 按名字查找文件
来源：http://jc.panjiajie.cn

find . -name "*.log" -type f
来源：http://fh.shtwfgs.cn

[R44] 按修改时间查找
来源：http://as.shxzskj.cn

find . -mtime -7 -type f
来源：http://nm.colortex.cn

[R45] 批量删除
来源：http://ze.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://vz.nszjky.cn

[R46] 递归替换文件内容
来源：http://gy.9csxet.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ca.huixiangedu.cn

[R47] sed 单行替换
来源：http://hq.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nk.hahajie.cn

[R48] awk 取指定列
来源：http://al.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://gm.bookmarksfly.cn

[R49] awk 带条件
来源：http://em.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nv.yuntaijiaju.cn

[R50] awk 求和
来源：http://ap.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gj.chemitech.net.cn

[R51] 排序去重取前几
来源：http://wo.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lz.lnxyls.cn

[R52] 统计行数
来源：http://pf.yuexingan06.cn

wc -l a.txt
来源：http://qz.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://zg.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fu.shtwfgs.cn

[R54] 比较两个文件
来源：http://bh.bjjhwx.cn

diff a.txt b.txt
来源：http://gb.szsharing.cn

[R55] 压缩与解压
来源：http://xm.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zw.lnxyls.cn

[R56] 远程拷贝
来源：http://sc.newstarts.cn

scp file user@host:/path/
来源：http://fq.lnxyls.cn

[R57] 远程执行命令
来源：http://vm.jctech888.com.cn

ssh user@host 'uptime'
来源：http://wv.nszjky.cn

[R58] 下载文件
来源：http://wa.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mf.9csxet.cn

[R59] 发 POST JSON
来源：http://qv.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rw.jianghongdianzi.cn

[R60] 只看 HTTP 状态码
来源：http://az.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mo.muxihuayi.cn

[R61] 磁盘占用
来源：http://vx.shxzskj.cn

df -h;  du -sh *
来源：http://zv.gzmigu.cn

[R62] 找最占空间的文件
来源：http://xd.9csxet.cn

du -ah . | sort -rh | head -10
来源：http://wb.nicolike.cn

[R63] 内存与进程
来源：http://fl.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://ty.hnjuh.cn

[R64] 结束进程
来源：http://dn.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://ld.hnjuh.cn

[R65] 查看端口占用
来源：http://sb.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cs.yuntaijiaju.cn

[R66] 定时任务
来源：http://jg.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://nc.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://eb.huixinmuqiang.cn

openssl rand -hex 16
来源：http://hb.huanxung.cn

[R68] 计算文件校验值
来源：http://kf.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://of.haigaiapp.cn

[R69] 生成随机密码
来源：http://qd.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://sz.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://hd.nicolike.cn

date +%s;  date -d @1700000000
来源：http://sj.jianghongdianzi.cn

[R71] 日期格式化
来源：http://jh.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sb.nicolike.cn

[R72] 等待端口就绪
来源：http://df.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sk.colortex.cn

[R73] 分割大日志
来源：http://mu.lnxyls.cn

split -l 1000 big.log part_
来源：http://xg.huixiangedu.cn

[R74] 批量重命名
来源：http://wa.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kh.szxytkj.cn

[R75] 导出环境变量
来源：http://iu.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://zx.wgjwhj.cn

[R76] 使用临时文件
来源：http://pe.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lq.newstarts.cn

[R77] 读取用户输入
来源：http://el.521024.cn

read -rp "请输入: " ans
来源：http://te.521024.cn

[R78] 交互式菜单
来源：http://wx.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ly.chemitech.net.cn

[R79] 解析命令行选项
来源：http://hj.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kn.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://uu.yuexingan06.cn

time ./run.sh
来源：http://lc.chemitech.net.cn

================================================================================
来源：http://po.9csxet.cn

S. C / C++ 专题
来源：http://lw.jctech888.com.cn

================================================================================
来源：http://cd.muxihuayi.cn

[S01] C：Hello World
来源：http://cu.chemitech.net.cn

#include <stdio.h>
来源：http://gu.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cp.szsharing.cn

[S02] C：变量与格式化输出
来源：http://mr.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://lk.hahajie.cn

[S03] C：读入整数
来源：http://ox.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://up.nicolike.cn

[S04] C：字符串复制
来源：http://ch.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oz.panjiajie.cn

[S05] C：字符串长度
来源：http://ji.nicolike.cn

strlen(s)
来源：http://op.muxihuayi.cn

[S06] C：字符串比较
来源：http://ch.nszjky.cn

strcmp(a, b) == 0
来源：http://me.hnjuh.cn

[S07] C：数组遍历求和
来源：http://yb.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fh.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://fo.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ul.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://na.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fe.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://zo.colortex.cn

int *p = &a;  *p = 5;
来源：http://gi.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://fg.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://ji.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ar.jianghongdianzi.cn

fclose(f);
来源：http://dl.yuntaijiaju.cn

[S12] C：写文件
来源：http://bs.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jz.lnxyls.cn

[S13] C：宏定义
来源：http://wi.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ll.lnxyls.cn

[S14] C：枚举
来源：http://ke.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://bf.bookmarksfly.cn

[S15] C：类型转换
来源：http://sq.nszjky.cn

(double) a / b
来源：http://bj.muxihuayi.cn

[S16] C：位操作置位
来源：http://qm.9csxet.cn

x |= (1 << 3);
来源：http://zo.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://ll.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://in.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://sg.huanxung.cn

int main(int argc, char **argv)
来源：http://jb.asd995.cn

[S19] C：快速排序
来源：http://zl.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wy.szxytkj.cn

[S20] C：二分查找
来源：http://mn.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://io.shxzskj.cn

[S21] C：字符类别判断
来源：http://me.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ee.hahajie.cn

[S22] C：字符串转数字
来源：http://ls.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pk.asd995.cn

[S23] C：随机数
来源：http://nd.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lg.jctech888.com.cn

[S24] C：获取本地时间
来源：http://lu.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ao.521024.cn

[S25] C：内存拷贝
来源：http://cf.jctech888.com.cn

memcpy(dst, src, n);
来源：http://dg.haigaiapp.cn

[S26] C：内存清零
来源：http://ex.nszjky.cn

memset(a, 0, sizeof a);
来源：http://sj.newstarts.cn

[S27] C：定义常量
来源：http://bz.shxzukj.cn

const double PI = 3.14159;
来源：http://qs.bjjhwx.cn

[S28] C：静态变量
来源：http://kd.jctech888.com.cn

static int counter = 0;
来源：http://li.colortex.cn

[S29] C：变参函数
来源：http://pk.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://om.muxihuayi.cn

[S30] C：头文件保护
来源：http://lb.shxzskj.cn

#ifndef X_H
来源：http://uo.wgjwhj.cn

#define X_H
来源：http://pm.colortex.cn

#endif
来源：http://xq.hnjuh.cn

[S31] C++：Hello World
来源：http://mj.panjiajie.cn

#include <iostream>
来源：http://yy.yuexingan06.cn

int main() { std::cout << "Hello\n"; }
来源：http://qj.haigaiapp.cn

[S32] C++：字符串
来源：http://tq.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ne.muxihuayi.cn

[S33] C++：vector 增删
来源：http://zj.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ct.gzmigu.cn

[S34] C++：遍历 vector
来源：http://me.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ic.panjiajie.cn

[S35] C++：map
来源：http://wn.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aa.shxzukj.cn

[S36] C++：unordered_map
来源：http://aq.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ll.panjiajie.cn

[S37] C++：set
来源：http://iw.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://al.szxytkj.cn

[S38] C++：排序
来源：http://xv.asd995.cn

std::sort(v.begin(), v.end());
来源：http://gk.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://fr.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dw.shxzskj.cn

[S40] C++：查找元素
来源：http://tp.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jg.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://tp.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lv.nszjky.cn

[S42] C++：继承与虚函数
来源：http://pc.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://sw.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://tg.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://sd.521024.cn

[S44] C++：引用传参
来源：http://yy.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://je.newstarts.cn

[S45] C++：lambda
来源：http://mm.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zk.hahajie.cn

[S46] C++：函数模板
来源：http://cd.huixinmuqiang.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lx.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://ah.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nv.szsharing.cn

[S48] C++：逐行读文件
来源：http://mk.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yw.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://ex.newstarts.cn

[S49] C++：写文件
来源：http://lf.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yt.newstarts.cn

[S50] C++：格式化数字
来源：http://rv.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tn.hnjuh.cn

[S51] C++：显式类型转换
来源：http://fq.haigaiapp.cn

static_cast<double>(a) / b
来源：http://tv.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://vu.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://cy.hnjuh.cn

[S53] C++：移动语义
来源：http://cn.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://un.chemitech.net.cn

[S54] C++：异常处理
来源：http://vd.lnxyls.cn


<!-- 参考信息 -->