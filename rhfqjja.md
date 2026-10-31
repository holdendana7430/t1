代发 wailian999

[Q67] 设置隔离级别
来源：http://zm.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wj.yuexingan06.cn

[Q68] 保存点
来源：http://bm.shxzskj.cn

SAVEPOINT sp1;
来源：http://vz.nicolike.cn

ROLLBACK TO sp1;
来源：http://nt.hahajie.cn

[Q69] 查看执行计划
来源：http://wl.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gz.muxihuayi.cn

[Q70] 更新统计信息
来源：http://iy.colortex.cn

ANALYZE TABLE users;
来源：http://bw.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://dd.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://la.shtwfgs.cn

[Q72] 查看索引
来源：http://ng.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://jy.newstarts.cn

[Q73] 查看表状态
来源：http://xn.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ve.nszjky.cn

[Q74] 强制使用索引
来源：http://zd.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hu.9csxet.cn

[Q75] 日期格式化
来源：http://ri.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ib.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ay.szsharing.cn

[Q76] 按天统计
来源：http://bz.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xx.newstarts.cn

[Q77] 时间加减
来源：http://if.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tx.huixiangedu.cn

[Q78] 当前时间
来源：http://cr.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qw.haigaiapp.cn

[Q79] 字符串拼接
来源：http://dw.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sz.shxzskj.cn

[Q80] 字符串截取
来源：http://ic.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yt.haigaiapp.cn

[Q81] 字符串替换
来源：http://ei.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ez.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://zp.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zl.chemitech.net.cn

[Q83] 大小写转换
来源：http://qn.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ke.newstarts.cn

[Q84] 去除首尾空格
来源：http://sc.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://xf.yuexingan06.cn

[Q85] 数值取整
来源：http://cw.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jj.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://si.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ky.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ix.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eg.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://kx.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ko.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xk.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://vz.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://be.bookmarksfly.cn

[Q90] 生成序号列
来源：http://zk.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kv.panjiajie.cn

================================================================================
来源：http://iu.haigaiapp.cn

R. Bash 专题
来源：http://ib.521024.cn

================================================================================
来源：http://wm.newstarts.cn

[R01] shebang 与严格模式
来源：http://kb.hnjuh.cn

#!/usr/bin/env bash
来源：http://iz.huanxung.cn

set -euo pipefail
来源：http://ce.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://oy.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://fa.yuntaijiaju.cn

[R03] 只读变量
来源：http://aq.gzmigu.cn

readonly PI=3.14
来源：http://at.huixinmuqiang.cn

[R04] 位置参数
来源：http://dx.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fg.panjiajie.cn

[R05] 参数默认值
来源：http://hh.haigaiapp.cn

name="${1:-default}"
来源：http://sw.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://se.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vk.yuntaijiaju.cn

[R07] if 判断文件
来源：http://gu.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mp.shtwfgs.cn

[R08] 数值比较
来源：http://yi.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nh.huixiangedu.cn

[R09] 字符串比较
来源：http://ea.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wn.bjjhwx.cn

[R10] 正则匹配
来源：http://ct.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bs.lnxyls.cn

[R11] case 多分支
来源：http://hp.huixiangedu.cn

case "$1" in
来源：http://im.newstarts.cn

start) echo "启动" ;;
来源：http://nq.9csxet.cn

stop)  echo "停止" ;;
来源：http://jw.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://lk.shxzukj.cn

esac
来源：http://vh.hahajie.cn

[R12] for 遍历文件
来源：http://qn.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://bd.9csxet.cn

[R13] for 计数循环
来源：http://ag.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://nx.asd995.cn

[R14] C 风格 for
来源：http://nk.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xv.yuexingan06.cn

[R15] while 逐行读文件
来源：http://ey.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zk.yuexingan06.cn

[R16] until 等待条件
来源：http://so.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gr.9csxet.cn

[R17] 数组定义与取值
来源：http://qg.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tf.huanxung.cn

[R18] 遍历数组
来源：http://od.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ho.newstarts.cn

[R19] 数组长度
来源：http://nd.jctech888.com.cn

echo "${#arr[@]}"
来源：http://sf.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://es.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qj.shxzskj.cn

[R21] 字符串长度
来源：http://dd.szsharing.cn

echo "${#s}"
来源：http://cm.hnjuh.cn

[R22] 截取子串
来源：http://yn.colortex.cn

echo "${s:0:5}"
来源：http://fw.wgjwhj.cn

[R23] 字符串替换
来源：http://ip.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hc.bjjhwx.cn

[R24] 大小写转换
来源：http://fe.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bm.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://vl.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://aa.szsharing.cn

[R26] 命令替换
来源：http://gu.asd995.cn

now=$(date +%F); echo "$now"
来源：http://cl.szxytkj.cn

[R27] 算术展开
来源：http://dl.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://wn.shxzskj.cn

[R28] 浮点运算
来源：http://ot.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://nx.wgjwhj.cn

[R29] 定义函数
来源：http://ju.hnjuh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kw.szxytkj.cn

[R30] 函数返回状态码
来源：http://ut.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://xu.szsharing.cn

[R31] 局部变量
来源：http://gj.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://aj.shtwfgs.cn

[R32] 参数个数校验
来源：http://zg.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pr.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://gw.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sv.huixiangedu.cn

[R34] 退出时清理
来源：http://ao.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mv.9csxet.cn

[R35] 后台执行并等待
来源：http://gz.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hb.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://gk.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nj.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://ef.szsharing.cn

files=$(ls -1)
来源：http://zg.szxytkj.cn

[R38] 管道串联
来源：http://jv.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://rl.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://mj.521024.cn

cmd > out.log 2>&1
来源：http://tn.huanxung.cn

[R40] 追加写日志
来源：http://vw.wgjwhj.cn

echo "log" >> out.log
来源：http://wf.chemitech.net.cn

[R41] 丢弃输出
来源：http://wz.nszjky.cn

cmd >/dev/null 2>&1
来源：http://kc.bjjhwx.cn

[R42] 输入重定向
来源：http://ma.9csxet.cn

wc -l < a.txt
来源：http://pn.bjjhwx.cn

[R43] 按名字查找文件
来源：http://mj.huixiangedu.cn

find . -name "*.log" -type f
来源：http://sm.szsharing.cn

[R44] 按修改时间查找
来源：http://ze.panjiajie.cn

find . -mtime -7 -type f
来源：http://uk.9csxet.cn

[R45] 批量删除
来源：http://uc.9csxet.cn

find . -name "*.tmp" -delete
来源：http://tf.lnxyls.cn

[R46] 递归替换文件内容
来源：http://ue.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zc.asd995.cn

[R47] sed 单行替换
来源：http://rg.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://et.newstarts.cn

[R48] awk 取指定列
来源：http://lv.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://mj.muxihuayi.cn

[R49] awk 带条件
来源：http://ia.muxihuayi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pd.521024.cn

[R50] awk 求和
来源：http://xc.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wl.521024.cn

[R51] 排序去重取前几
来源：http://sx.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tc.yuntaijiaju.cn

[R52] 统计行数
来源：http://sd.jianghongdianzi.cn

wc -l a.txt
来源：http://yq.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://rv.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jo.hahajie.cn

[R54] 比较两个文件
来源：http://pm.shxzukj.cn

diff a.txt b.txt
来源：http://vh.bjjhwx.cn

[R55] 压缩与解压
来源：http://pg.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://an.huanxung.cn

[R56] 远程拷贝
来源：http://qt.haigaiapp.cn

scp file user@host:/path/
来源：http://dm.jianghongdianzi.cn

[R57] 远程执行命令
来源：http://ke.9csxet.cn

ssh user@host 'uptime'
来源：http://bf.lnxyls.cn

[R58] 下载文件
来源：http://ai.nicolike.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://us.nicolike.cn

[R59] 发 POST JSON
来源：http://ih.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xq.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://gf.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sx.huixiangedu.cn

[R61] 磁盘占用
来源：http://jr.jianghongdianzi.cn

df -h;  du -sh *
来源：http://vv.huixinmuqiang.cn

[R62] 找最占空间的文件
来源：http://lm.521024.cn

du -ah . | sort -rh | head -10
来源：http://cp.gzmigu.cn

[R63] 内存与进程
来源：http://wb.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://qm.huixinmuqiang.cn

[R64] 结束进程
来源：http://fo.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://ay.yuexingan06.cn

[R65] 查看端口占用
来源：http://nv.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tl.521024.cn

[R66] 定时任务
来源：http://vj.nszjky.cn

crontab -e;  crontab -l
来源：http://vs.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://qu.jctech888.com.cn

openssl rand -hex 16
来源：http://ob.newstarts.cn

[R68] 计算文件校验值
来源：http://vg.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xg.colortex.cn

[R69] 生成随机密码
来源：http://yv.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://wm.colortex.cn

[R70] 时间戳与互转
来源：http://ya.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://iy.colortex.cn

[R71] 日期格式化
来源：http://eq.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iv.huanxung.cn

[R72] 等待端口就绪
来源：http://mi.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sk.yuntaijiaju.cn

[R73] 分割大日志
来源：http://ap.hahajie.cn

split -l 1000 big.log part_
来源：http://pn.gzmigu.cn

[R74] 批量重命名
来源：http://mh.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://st.muxihuayi.cn

[R75] 导出环境变量
来源：http://me.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://fm.asd995.cn

[R76] 使用临时文件
来源：http://qm.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tt.bjjhwx.cn

[R77] 读取用户输入
来源：http://wm.hnjuh.cn

read -rp "请输入: " ans
来源：http://nq.bookmarksfly.cn

[R78] 交互式菜单
来源：http://un.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fb.lnxyls.cn

[R79] 解析命令行选项
来源：http://ln.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kc.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://ss.huixinmuqiang.cn

time ./run.sh
来源：http://fp.yuntaijiaju.cn

================================================================================
来源：http://bh.wgjwhj.cn

S. C / C++ 专题
来源：http://ap.lnxyls.cn

================================================================================
来源：http://cp.bjjhwx.cn

[S01] C：Hello World
来源：http://yc.haigaiapp.cn

#include <stdio.h>
来源：http://xm.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ps.newstarts.cn

[S02] C：变量与格式化输出
来源：http://xl.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://xs.nszjky.cn

[S03] C：读入整数
来源：http://da.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://oc.szxytkj.cn

[S04] C：字符串复制
来源：http://bx.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ea.colortex.cn

[S05] C：字符串长度
来源：http://gh.nicolike.cn

strlen(s)
来源：http://gi.szxytkj.cn

[S06] C：字符串比较
来源：http://dt.nicolike.cn

strcmp(a, b) == 0
来源：http://rz.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://bz.521024.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://is.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://iv.jctech888.com.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gx.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://qo.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bl.huanxung.cn

[S10] C：指针与解引用
来源：http://hq.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://up.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ni.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://wb.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cy.yuexingan06.cn

fclose(f);
来源：http://rz.huixinmuqiang.cn

[S12] C：写文件
来源：http://rw.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yy.wgjwhj.cn

[S13] C：宏定义
来源：http://hw.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mb.yuntaijiaju.cn

[S14] C：枚举
来源：http://fu.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://sl.chemitech.net.cn

[S15] C：类型转换
来源：http://mu.chemitech.net.cn

(double) a / b
来源：http://zf.hahajie.cn

[S16] C：位操作置位
来源：http://ly.lnxyls.cn

x |= (1 << 3);
来源：http://rw.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://ho.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xh.haigaiapp.cn

[S18] C：命令行参数
来源：http://ts.asd995.cn

int main(int argc, char **argv)
来源：http://fy.yuntaijiaju.cn

[S19] C：快速排序
来源：http://da.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mn.huanxung.cn

[S20] C：二分查找
来源：http://uv.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gw.chemitech.net.cn

[S21] C：字符类别判断
来源：http://eu.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://db.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://lc.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lk.bookmarksfly.cn

[S23] C：随机数
来源：http://hc.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nz.huanxung.cn

[S24] C：获取本地时间
来源：http://eq.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bs.szxytkj.cn

[S25] C：内存拷贝
来源：http://ff.muxihuayi.cn

memcpy(dst, src, n);
来源：http://pz.jianghongdianzi.cn

[S26] C：内存清零
来源：http://ot.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://li.hnjuh.cn

[S27] C：定义常量
来源：http://zq.huixiangedu.cn

const double PI = 3.14159;
来源：http://ho.shxzskj.cn

[S28] C：静态变量
来源：http://cf.yuntaijiaju.cn

static int counter = 0;
来源：http://js.gzmigu.cn

[S29] C：变参函数
来源：http://qq.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ha.newstarts.cn

[S30] C：头文件保护
来源：http://jf.shtwfgs.cn

#ifndef X_H
来源：http://yk.bookmarksfly.cn

#define X_H
来源：http://pe.szxytkj.cn

#endif
来源：http://vj.bookmarksfly.cn

[S31] C++：Hello World
来源：http://vk.gzmigu.cn

#include <iostream>
来源：http://lf.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://pc.hnjuh.cn

[S32] C++：字符串
来源：http://dx.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://oz.wgjwhj.cn

[S33] C++：vector 增删
来源：http://qg.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lh.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://rp.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://dy.hahajie.cn

[S35] C++：map
来源：http://bq.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cd.lnxyls.cn

[S36] C++：unordered_map
来源：http://gy.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nb.asd995.cn


<!-- 参考信息 -->