代发 wailian999

[Q78] 当前时间
来源：http://qg.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pq.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://gi.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ih.gzmigu.cn

[Q80] 字符串截取
来源：http://tj.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jt.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://bh.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uc.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://bq.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fw.521024.cn

[Q83] 大小写转换
来源：http://tm.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ek.colortex.cn

[Q84] 去除首尾空格
来源：http://tn.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://gg.9csxet.cn

[Q85] 数值取整
来源：http://xq.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fu.asd995.cn

[Q86] 读取 JSON 字段
来源：http://hs.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lz.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://ja.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pm.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://rg.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cj.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uf.newstarts.cn

[Q89] 判断表是否存在
来源：http://mb.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ey.9csxet.cn

[Q90] 生成序号列
来源：http://xc.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tg.szsharing.cn

================================================================================
来源：http://gh.bookmarksfly.cn

R. Bash 专题
来源：http://fo.9csxet.cn

================================================================================
来源：http://hg.gzmigu.cn

[R01] shebang 与严格模式
来源：http://yp.9csxet.cn

#!/usr/bin/env bash
来源：http://fh.gzmigu.cn

set -euo pipefail
来源：http://rr.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://iu.szxytkj.cn

name="Tom"; echo "$name"
来源：http://hn.nszjky.cn

[R03] 只读变量
来源：http://dp.yuntaijiaju.cn

readonly PI=3.14
来源：http://no.szsharing.cn

[R04] 位置参数
来源：http://yu.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fj.gzmigu.cn

[R05] 参数默认值
来源：http://gy.yuntaijiaju.cn

name="${1:-default}"
来源：http://gx.szxytkj.cn

[R06] 判断命令是否存在
来源：http://gq.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://le.yuexingan06.cn

[R07] if 判断文件
来源：http://yt.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fw.huanxung.cn

[R08] 数值比较
来源：http://bu.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://if.yuntaijiaju.cn

[R09] 字符串比较
来源：http://xo.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xp.hahajie.cn

[R10] 正则匹配
来源：http://mg.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ev.bjjhwx.cn

[R11] case 多分支
来源：http://vh.shxzukj.cn

case "$1" in
来源：http://rg.chemitech.net.cn

start) echo "启动" ;;
来源：http://ac.asd995.cn

stop)  echo "停止" ;;
来源：http://dq.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://wc.chemitech.net.cn

esac
来源：http://je.hnjuh.cn

[R12] for 遍历文件
来源：http://fs.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://mz.chemitech.net.cn

[R13] for 计数循环
来源：http://ii.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://lk.newstarts.cn

[R14] C 风格 for
来源：http://gw.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fy.szxytkj.cn

[R15] while 逐行读文件
来源：http://sl.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gs.chemitech.net.cn

[R16] until 等待条件
来源：http://de.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pe.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://mp.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mk.muxihuayi.cn

[R18] 遍历数组
来源：http://bq.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://st.yuntaijiaju.cn

[R19] 数组长度
来源：http://rn.yuexingan06.cn

echo "${#arr[@]}"
来源：http://bf.szsharing.cn

[R20] 关联数组（字典）
来源：http://hf.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ea.wgjwhj.cn

[R21] 字符串长度
来源：http://sz.newstarts.cn

echo "${#s}"
来源：http://ok.yuntaijiaju.cn

[R22] 截取子串
来源：http://fh.haigaiapp.cn

echo "${s:0:5}"
来源：http://sy.colortex.cn

[R23] 字符串替换
来源：http://fb.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sg.wgjwhj.cn

[R24] 大小写转换
来源：http://nr.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rb.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://rv.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nj.chemitech.net.cn

[R26] 命令替换
来源：http://ro.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://ms.yuexingan06.cn

[R27] 算术展开
来源：http://we.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://yo.muxihuayi.cn

[R28] 浮点运算
来源：http://wk.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://pp.9csxet.cn

[R29] 定义函数
来源：http://sq.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gi.muxihuayi.cn

[R30] 函数返回状态码
来源：http://dh.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://uj.szsharing.cn

[R31] 局部变量
来源：http://us.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://wk.szxytkj.cn

[R32] 参数个数校验
来源：http://ju.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kz.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://mb.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lt.jianghongdianzi.cn

[R34] 退出时清理
来源：http://sc.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ga.hnjuh.cn

[R35] 后台执行并等待
来源：http://vv.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cz.lnxyls.cn

[R36] 并发执行多个任务
来源：http://iq.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zj.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://oe.yuntaijiaju.cn

files=$(ls -1)
来源：http://ol.jianghongdianzi.cn

[R38] 管道串联
来源：http://mp.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://zy.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://we.chemitech.net.cn

cmd > out.log 2>&1
来源：http://zu.muxihuayi.cn

[R40] 追加写日志
来源：http://nr.bookmarksfly.cn

echo "log" >> out.log
来源：http://kq.panjiajie.cn

[R41] 丢弃输出
来源：http://gq.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://kd.newstarts.cn

[R42] 输入重定向
来源：http://mp.bookmarksfly.cn

wc -l < a.txt
来源：http://dr.shtwfgs.cn

[R43] 按名字查找文件
来源：http://rw.nszjky.cn

find . -name "*.log" -type f
来源：http://bn.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://gp.521024.cn

find . -mtime -7 -type f
来源：http://mr.hnjuh.cn

[R45] 批量删除
来源：http://cb.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://qj.huanxung.cn

[R46] 递归替换文件内容
来源：http://pu.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ci.hnjuh.cn

[R47] sed 单行替换
来源：http://mq.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lo.521024.cn

[R48] awk 取指定列
来源：http://kf.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://vq.haigaiapp.cn

[R49] awk 带条件
来源：http://fb.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pl.newstarts.cn

[R50] awk 求和
来源：http://ne.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dy.bjjhwx.cn

[R51] 排序去重取前几
来源：http://ii.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gs.newstarts.cn

[R52] 统计行数
来源：http://kj.jctech888.com.cn

wc -l a.txt
来源：http://ra.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://si.panjiajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://he.521024.cn

[R54] 比较两个文件
来源：http://gg.huixinmuqiang.cn

diff a.txt b.txt
来源：http://pt.shxzskj.cn

[R55] 压缩与解压
来源：http://zr.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ng.panjiajie.cn

[R56] 远程拷贝
来源：http://bg.huanxung.cn

scp file user@host:/path/
来源：http://la.panjiajie.cn

[R57] 远程执行命令
来源：http://yj.nszjky.cn

ssh user@host 'uptime'
来源：http://gu.yuexingan06.cn

[R58] 下载文件
来源：http://iv.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xx.colortex.cn

[R59] 发 POST JSON
来源：http://cq.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fs.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://sa.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pc.yuexingan06.cn

[R61] 磁盘占用
来源：http://lm.jctech888.com.cn

df -h;  du -sh *
来源：http://qj.nszjky.cn

[R62] 找最占空间的文件
来源：http://gp.colortex.cn

du -ah . | sort -rh | head -10
来源：http://uw.yuntaijiaju.cn

[R63] 内存与进程
来源：http://ls.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://sh.haigaiapp.cn

[R64] 结束进程
来源：http://xm.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://sr.shtwfgs.cn

[R65] 查看端口占用
来源：http://nb.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wt.colortex.cn

[R66] 定时任务
来源：http://ck.lnxyls.cn

crontab -e;  crontab -l
来源：http://il.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://xm.haigaiapp.cn

openssl rand -hex 16
来源：http://lw.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://wc.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rv.nszjky.cn

[R69] 生成随机密码
来源：http://dg.521024.cn

head -c 16 /dev/urandom | base64
来源：http://kx.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://oo.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://hp.hnjuh.cn

[R71] 日期格式化
来源：http://nc.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lh.wgjwhj.cn

[R72] 等待端口就绪
来源：http://hd.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dd.gzmigu.cn

[R73] 分割大日志
来源：http://hd.chemitech.net.cn

split -l 1000 big.log part_
来源：http://ka.colortex.cn

[R74] 批量重命名
来源：http://lh.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://py.newstarts.cn

[R75] 导出环境变量
来源：http://hi.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://vl.bookmarksfly.cn

[R76] 使用临时文件
来源：http://rd.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fa.lnxyls.cn

[R77] 读取用户输入
来源：http://nm.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://cz.bookmarksfly.cn

[R78] 交互式菜单
来源：http://hs.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rr.shtwfgs.cn

[R79] 解析命令行选项
来源：http://td.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xv.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://zi.szsharing.cn

time ./run.sh
来源：http://qv.nicolike.cn

================================================================================
来源：http://iu.huixinmuqiang.cn

S. C / C++ 专题
来源：http://pj.szxytkj.cn

================================================================================
来源：http://yr.bjjhwx.cn

[S01] C：Hello World
来源：http://pt.huixinmuqiang.cn

#include <stdio.h>
来源：http://hz.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cw.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://uy.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://lw.panjiajie.cn

[S03] C：读入整数
来源：http://vk.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://cd.shxzukj.cn

[S04] C：字符串复制
来源：http://wb.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://te.huanxung.cn

[S05] C：字符串长度
来源：http://ft.521024.cn

strlen(s)
来源：http://iw.yuexingan06.cn

[S06] C：字符串比较
来源：http://pw.panjiajie.cn

strcmp(a, b) == 0
来源：http://nv.asd995.cn

[S07] C：数组遍历求和
来源：http://vd.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nt.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://lp.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qj.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://ru.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sw.haigaiapp.cn

[S10] C：指针与解引用
来源：http://ho.newstarts.cn

int *p = &a;  *p = 5;
来源：http://lj.szsharing.cn

[S11] C：逐行读文件
来源：http://be.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://wt.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dh.yuntaijiaju.cn

fclose(f);
来源：http://nk.newstarts.cn

[S12] C：写文件
来源：http://cu.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tu.bookmarksfly.cn

[S13] C：宏定义
来源：http://uq.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xr.lnxyls.cn

[S14] C：枚举
来源：http://fr.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://mg.lnxyls.cn

[S15] C：类型转换
来源：http://zv.panjiajie.cn

(double) a / b
来源：http://zm.bjjhwx.cn

[S16] C：位操作置位
来源：http://qw.jianghongdianzi.cn

x |= (1 << 3);
来源：http://nu.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://ok.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://av.newstarts.cn

[S18] C：命令行参数
来源：http://ud.bjjhwx.cn

int main(int argc, char **argv)
来源：http://cb.wgjwhj.cn

[S19] C：快速排序
来源：http://ln.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cm.shtwfgs.cn

[S20] C：二分查找
来源：http://vd.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eq.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://ka.shtwfgs.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://af.hahajie.cn

[S22] C：字符串转数字
来源：http://ns.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rx.jianghongdianzi.cn

[S23] C：随机数
来源：http://sa.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jr.shxzukj.cn

[S24] C：获取本地时间
来源：http://em.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hp.nszjky.cn

[S25] C：内存拷贝
来源：http://az.muxihuayi.cn

memcpy(dst, src, n);
来源：http://tk.hnjuh.cn

[S26] C：内存清零
来源：http://bv.hahajie.cn

memset(a, 0, sizeof a);
来源：http://bm.jctech888.com.cn

[S27] C：定义常量
来源：http://wk.nszjky.cn

const double PI = 3.14159;
来源：http://zs.huixiangedu.cn

[S28] C：静态变量
来源：http://ks.chemitech.net.cn

static int counter = 0;
来源：http://ex.9csxet.cn

[S29] C：变参函数
来源：http://wz.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gx.9csxet.cn

[S30] C：头文件保护
来源：http://ot.szxytkj.cn

#ifndef X_H
来源：http://bx.bookmarksfly.cn

#define X_H
来源：http://nf.9csxet.cn

#endif
来源：http://ph.szsharing.cn

[S31] C++：Hello World
来源：http://sp.chemitech.net.cn

#include <iostream>
来源：http://fg.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://cp.lnxyls.cn

[S32] C++：字符串
来源：http://ke.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://ik.shtwfgs.cn

[S33] C++：vector 增删
来源：http://zc.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zl.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://tr.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://uv.asd995.cn

[S35] C++：map
来源：http://lt.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ri.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://qn.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mt.haigaiapp.cn

[S37] C++：set
来源：http://rm.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fb.wgjwhj.cn

[S38] C++：排序
来源：http://sa.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://qv.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://hl.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tq.asd995.cn

[S40] C++：查找元素
来源：http://kn.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qn.shxzskj.cn

[S41] C++：类与构造函数
来源：http://fw.shtwfgs.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gz.asd995.cn

[S42] C++：继承与虚函数
来源：http://jv.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://nc.haigaiapp.cn

[S43] C++：智能指针
来源：http://zi.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://qn.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://la.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://cn.haigaiapp.cn

[S45] C++：lambda
来源：http://ni.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://si.hahajie.cn

[S46] C++：函数模板
来源：http://rx.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://if.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://ay.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://es.nicolike.cn

[S48] C++：逐行读文件
来源：http://zf.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pj.haigaiapp.cn


<!-- 参考信息 -->