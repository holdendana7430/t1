代发 wailian999

ANALYZE TABLE users;
来源：http://bb.szxytkj.cn

[Q71] 查看建表语句
来源：http://zy.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yh.asd995.cn

[Q72] 查看索引
来源：http://fi.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://bv.nszjky.cn

[Q73] 查看表状态
来源：http://ox.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ow.huixiangedu.cn

[Q74] 强制使用索引
来源：http://fe.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cn.521024.cn

[Q75] 日期格式化
来源：http://bi.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xw.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://go.nszjky.cn

[Q76] 按天统计
来源：http://pr.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tr.bookmarksfly.cn

[Q77] 时间加减
来源：http://nl.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zy.9csxet.cn

[Q78] 当前时间
来源：http://tn.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wf.panjiajie.cn

[Q79] 字符串拼接
来源：http://ps.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mw.panjiajie.cn

[Q80] 字符串截取
来源：http://py.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://su.asd995.cn

[Q81] 字符串替换
来源：http://kl.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kw.521024.cn

[Q82] 字符长度与字节长度
来源：http://vi.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gp.521024.cn

[Q83] 大小写转换
来源：http://gr.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mr.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://bh.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://tj.hahajie.cn

[Q85] 数值取整
来源：http://mu.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tl.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://me.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ee.nszjky.cn

[Q87] JSON 字段做条件
来源：http://zd.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wy.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://tq.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vk.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ry.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://xw.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uh.yuexingan06.cn

[Q90] 生成序号列
来源：http://aw.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://th.lnxyls.cn

================================================================================
来源：http://kh.huixinmuqiang.cn

R. Bash 专题
来源：http://rj.haigaiapp.cn

================================================================================
来源：http://mp.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://jc.hnjuh.cn

#!/usr/bin/env bash
来源：http://yb.yuntaijiaju.cn

set -euo pipefail
来源：http://dm.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://kf.newstarts.cn

name="Tom"; echo "$name"
来源：http://eb.hnjuh.cn

[R03] 只读变量
来源：http://ik.lnxyls.cn

readonly PI=3.14
来源：http://sf.asd995.cn

[R04] 位置参数
来源：http://lg.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zt.huanxung.cn

[R05] 参数默认值
来源：http://bk.haigaiapp.cn

name="${1:-default}"
来源：http://so.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://wn.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yk.bjjhwx.cn

[R07] if 判断文件
来源：http://kh.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zs.wgjwhj.cn

[R08] 数值比较
来源：http://km.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zn.shxzukj.cn

[R09] 字符串比较
来源：http://zd.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xg.gzmigu.cn

[R10] 正则匹配
来源：http://lp.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uq.521024.cn

[R11] case 多分支
来源：http://sw.muxihuayi.cn

case "$1" in
来源：http://lh.9csxet.cn

start) echo "启动" ;;
来源：http://nu.panjiajie.cn

stop)  echo "停止" ;;
来源：http://ol.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://ws.yuexingan06.cn

esac
来源：http://wu.hnjuh.cn

[R12] for 遍历文件
来源：http://su.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://lv.shxzskj.cn

[R13] for 计数循环
来源：http://wj.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://wr.muxihuayi.cn

[R14] C 风格 for
来源：http://rh.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vg.newstarts.cn

[R15] while 逐行读文件
来源：http://sl.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pj.gzmigu.cn

[R16] until 等待条件
来源：http://ij.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ug.nszjky.cn

[R17] 数组定义与取值
来源：http://av.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://px.huixiangedu.cn

[R18] 遍历数组
来源：http://ih.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ef.asd995.cn

[R19] 数组长度
来源：http://xq.colortex.cn

echo "${#arr[@]}"
来源：http://iy.shxzskj.cn

[R20] 关联数组（字典）
来源：http://hp.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lu.wgjwhj.cn

[R21] 字符串长度
来源：http://qv.521024.cn

echo "${#s}"
来源：http://js.newstarts.cn

[R22] 截取子串
来源：http://nw.szsharing.cn

echo "${s:0:5}"
来源：http://aj.yuexingan06.cn

[R23] 字符串替换
来源：http://vb.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ub.gzmigu.cn

[R24] 大小写转换
来源：http://zu.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ly.521024.cn

[R25] 去后缀 / 去前缀
来源：http://fm.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tp.9csxet.cn

[R26] 命令替换
来源：http://eq.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://fn.gzmigu.cn

[R27] 算术展开
来源：http://yt.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://ag.bookmarksfly.cn

[R28] 浮点运算
来源：http://ma.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://fx.panjiajie.cn

[R29] 定义函数
来源：http://ei.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://au.yuexingan06.cn

[R30] 函数返回状态码
来源：http://mv.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://vh.wgjwhj.cn

[R31] 局部变量
来源：http://ym.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://oa.lnxyls.cn

[R32] 参数个数校验
来源：http://jr.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xe.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://um.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sa.wgjwhj.cn

[R34] 退出时清理
来源：http://pq.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qa.haigaiapp.cn

[R35] 后台执行并等待
来源：http://bk.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zi.nszjky.cn

[R36] 并发执行多个任务
来源：http://au.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qs.asd995.cn

[R37] 把输出赋给变量
来源：http://ic.jianghongdianzi.cn

files=$(ls -1)
来源：http://tj.gzmigu.cn

[R38] 管道串联
来源：http://fu.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://cy.huixinmuqiang.cn

[R39] 重定向标准输出与错误
来源：http://iv.9csxet.cn

cmd > out.log 2>&1
来源：http://us.jianghongdianzi.cn

[R40] 追加写日志
来源：http://ug.yuntaijiaju.cn

echo "log" >> out.log
来源：http://bl.panjiajie.cn

[R41] 丢弃输出
来源：http://mf.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://wq.huanxung.cn

[R42] 输入重定向
来源：http://eb.szxytkj.cn

wc -l < a.txt
来源：http://eg.szxytkj.cn

[R43] 按名字查找文件
来源：http://ks.huanxung.cn

find . -name "*.log" -type f
来源：http://gn.huanxung.cn

[R44] 按修改时间查找
来源：http://ef.huixiangedu.cn

find . -mtime -7 -type f
来源：http://mr.nszjky.cn

[R45] 批量删除
来源：http://mp.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://ec.szsharing.cn

[R46] 递归替换文件内容
来源：http://jl.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yi.shtwfgs.cn

[R47] sed 单行替换
来源：http://sr.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ck.hnjuh.cn

[R48] awk 取指定列
来源：http://wo.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://nh.wgjwhj.cn

[R49] awk 带条件
来源：http://ag.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vd.muxihuayi.cn

[R50] awk 求和
来源：http://vm.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xx.shtwfgs.cn

[R51] 排序去重取前几
来源：http://ae.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ta.hahajie.cn

[R52] 统计行数
来源：http://lm.9csxet.cn

wc -l a.txt
来源：http://oe.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://zg.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://es.shxzukj.cn

[R54] 比较两个文件
来源：http://vs.haigaiapp.cn

diff a.txt b.txt
来源：http://cj.newstarts.cn

[R55] 压缩与解压
来源：http://bd.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://je.huanxung.cn

[R56] 远程拷贝
来源：http://lt.hnjuh.cn

scp file user@host:/path/
来源：http://qh.9csxet.cn

[R57] 远程执行命令
来源：http://cp.nicolike.cn

ssh user@host 'uptime'
来源：http://xl.chemitech.net.cn

[R58] 下载文件
来源：http://ka.shxzukj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ol.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://ba.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tp.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://mk.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tz.colortex.cn

[R61] 磁盘占用
来源：http://bg.hnjuh.cn

df -h;  du -sh *
来源：http://wa.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://cq.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://dh.hahajie.cn

[R63] 内存与进程
来源：http://kn.jianghongdianzi.cn

free -h;  ps aux | grep nginx
来源：http://hp.huixinmuqiang.cn

[R64] 结束进程
来源：http://gq.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://wx.shxzukj.cn

[R65] 查看端口占用
来源：http://ff.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uo.colortex.cn

[R66] 定时任务
来源：http://rl.wgjwhj.cn

crontab -e;  crontab -l
来源：http://op.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://vw.szsharing.cn

openssl rand -hex 16
来源：http://ax.wgjwhj.cn

[R68] 计算文件校验值
来源：http://zb.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ht.szxytkj.cn

[R69] 生成随机密码
来源：http://jl.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://ty.lnxyls.cn

[R70] 时间戳与互转
来源：http://ux.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://fc.muxihuayi.cn

[R71] 日期格式化
来源：http://pz.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kk.muxihuayi.cn

[R72] 等待端口就绪
来源：http://st.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jk.jctech888.com.cn

[R73] 分割大日志
来源：http://bh.wgjwhj.cn

split -l 1000 big.log part_
来源：http://rw.shtwfgs.cn

[R74] 批量重命名
来源：http://tp.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pn.shxzskj.cn

[R75] 导出环境变量
来源：http://dq.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://nu.yuexingan06.cn

[R76] 使用临时文件
来源：http://br.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://st.haigaiapp.cn

[R77] 读取用户输入
来源：http://br.haigaiapp.cn

read -rp "请输入: " ans
来源：http://hi.521024.cn

[R78] 交互式菜单
来源：http://hr.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eg.muxihuayi.cn

[R79] 解析命令行选项
来源：http://dc.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ou.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://ei.panjiajie.cn

time ./run.sh
来源：http://qn.huixinmuqiang.cn

================================================================================
来源：http://uk.huanxung.cn

S. C / C++ 专题
来源：http://nf.bookmarksfly.cn

================================================================================
来源：http://gf.lnxyls.cn

[S01] C：Hello World
来源：http://df.jianghongdianzi.cn

#include <stdio.h>
来源：http://ef.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rm.9csxet.cn

[S02] C：变量与格式化输出
来源：http://la.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://xp.wgjwhj.cn

[S03] C：读入整数
来源：http://td.9csxet.cn

int x; scanf("%d", &x);
来源：http://mn.jctech888.com.cn

[S04] C：字符串复制
来源：http://kf.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iy.wgjwhj.cn

[S05] C：字符串长度
来源：http://fx.newstarts.cn

strlen(s)
来源：http://oz.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://xr.chemitech.net.cn

strcmp(a, b) == 0
来源：http://lz.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://zc.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bx.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://le.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://il.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://tt.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://or.lnxyls.cn

[S10] C：指针与解引用
来源：http://pd.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://fe.jctech888.com.cn

[S11] C：逐行读文件
来源：http://mw.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://vg.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xg.newstarts.cn

fclose(f);
来源：http://tl.wgjwhj.cn

[S12] C：写文件
来源：http://os.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zu.haigaiapp.cn

[S13] C：宏定义
来源：http://yd.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ux.szsharing.cn

[S14] C：枚举
来源：http://in.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://nn.nicolike.cn

[S15] C：类型转换
来源：http://rc.jctech888.com.cn

(double) a / b
来源：http://ei.panjiajie.cn

[S16] C：位操作置位
来源：http://cm.huixiangedu.cn

x |= (1 << 3);
来源：http://oi.hahajie.cn

[S17] C：安全拼接字符串
来源：http://bu.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wk.yuexingan06.cn

[S18] C：命令行参数
来源：http://cs.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ny.shxzskj.cn

[S19] C：快速排序
来源：http://pp.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hk.wgjwhj.cn

[S20] C：二分查找
来源：http://lu.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sb.huanxung.cn

[S21] C：字符类别判断
来源：http://in.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gp.haigaiapp.cn

[S22] C：字符串转数字
来源：http://xh.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://an.newstarts.cn

[S23] C：随机数
来源：http://cf.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ao.haigaiapp.cn

[S24] C：获取本地时间
来源：http://dg.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zj.chemitech.net.cn

[S25] C：内存拷贝
来源：http://lh.shtwfgs.cn

memcpy(dst, src, n);
来源：http://wc.shtwfgs.cn

[S26] C：内存清零
来源：http://ej.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://gy.szsharing.cn

[S27] C：定义常量
来源：http://oi.huanxung.cn

const double PI = 3.14159;
来源：http://wk.haigaiapp.cn

[S28] C：静态变量
来源：http://zm.chemitech.net.cn

static int counter = 0;
来源：http://qm.colortex.cn

[S29] C：变参函数
来源：http://ia.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qn.asd995.cn

[S30] C：头文件保护
来源：http://sq.asd995.cn

#ifndef X_H
来源：http://pn.bookmarksfly.cn

#define X_H
来源：http://nq.asd995.cn

#endif
来源：http://qn.newstarts.cn

[S31] C++：Hello World
来源：http://jq.yuexingan06.cn

#include <iostream>
来源：http://zh.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://ac.nszjky.cn

[S32] C++：字符串
来源：http://rc.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://da.szsharing.cn

[S33] C++：vector 增删
来源：http://qu.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://di.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ij.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://in.jctech888.com.cn

[S35] C++：map
来源：http://rh.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lp.panjiajie.cn

[S36] C++：unordered_map
来源：http://ox.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sf.yuntaijiaju.cn

[S37] C++：set
来源：http://hv.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rc.lnxyls.cn

[S38] C++：排序
来源：http://sc.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://ko.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://og.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nl.panjiajie.cn

[S40] C++：查找元素
来源：http://hd.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dj.bookmarksfly.cn


<!-- 参考信息 -->