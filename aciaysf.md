代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://em.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://vj.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qf.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://je.bjjhwx.cn

[Q61] 移动平均
来源：http://oh.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pb.muxihuayi.cn

[Q62] 分组占比
来源：http://mi.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sy.yuexingan06.cn

[Q63] 开启事务
来源：http://ln.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sj.jianghongdianzi.cn

[Q64] 提交事务
来源：http://rd.nicolike.cn

COMMIT;
来源：http://se.chemitech.net.cn

[Q65] 回滚事务
来源：http://ur.shxzukj.cn

ROLLBACK;
来源：http://si.newstarts.cn

[Q66] 行锁查询
来源：http://nu.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iz.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://fs.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dk.yuntaijiaju.cn

[Q68] 保存点
来源：http://mq.shxzskj.cn

SAVEPOINT sp1;
来源：http://cd.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://qq.shxzukj.cn

[Q69] 查看执行计划
来源：http://wk.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dv.lnxyls.cn

[Q70] 更新统计信息
来源：http://bi.muxihuayi.cn

ANALYZE TABLE users;
来源：http://bl.9csxet.cn

[Q71] 查看建表语句
来源：http://bd.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jg.panjiajie.cn

[Q72] 查看索引
来源：http://qi.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://gj.gzmigu.cn

[Q73] 查看表状态
来源：http://yn.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://op.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://gt.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fc.gzmigu.cn

[Q75] 日期格式化
来源：http://zj.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tq.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ec.huixiangedu.cn

[Q76] 按天统计
来源：http://qk.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vk.muxihuayi.cn

[Q77] 时间加减
来源：http://sz.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://na.shtwfgs.cn

[Q78] 当前时间
来源：http://in.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qo.colortex.cn

[Q79] 字符串拼接
来源：http://to.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zm.shtwfgs.cn

[Q80] 字符串截取
来源：http://tv.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wo.huanxung.cn

[Q81] 字符串替换
来源：http://vr.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bu.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://ij.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tr.521024.cn

[Q83] 大小写转换
来源：http://ao.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wn.colortex.cn

[Q84] 去除首尾空格
来源：http://zj.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://rl.yuexingan06.cn

[Q85] 数值取整
来源：http://jp.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ov.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://bg.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ha.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://nj.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lt.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://zf.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jm.gzmigu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zd.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://bv.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bj.hahajie.cn

[Q90] 生成序号列
来源：http://dp.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ph.lnxyls.cn

================================================================================
来源：http://ki.shxzskj.cn

R. Bash 专题
来源：http://nc.haigaiapp.cn

================================================================================
来源：http://dm.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://vk.haigaiapp.cn

#!/usr/bin/env bash
来源：http://ch.colortex.cn

set -euo pipefail
来源：http://sz.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://ik.newstarts.cn

name="Tom"; echo "$name"
来源：http://id.nicolike.cn

[R03] 只读变量
来源：http://fm.panjiajie.cn

readonly PI=3.14
来源：http://vf.hahajie.cn

[R04] 位置参数
来源：http://ai.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tm.9csxet.cn

[R05] 参数默认值
来源：http://to.hnjuh.cn

name="${1:-default}"
来源：http://el.szsharing.cn

[R06] 判断命令是否存在
来源：http://ht.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gr.hahajie.cn

[R07] if 判断文件
来源：http://vz.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uh.521024.cn

[R08] 数值比较
来源：http://yg.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ts.hahajie.cn

[R09] 字符串比较
来源：http://pn.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sr.szsharing.cn

[R10] 正则匹配
来源：http://ru.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qu.newstarts.cn

[R11] case 多分支
来源：http://tl.yuexingan06.cn

case "$1" in
来源：http://tu.asd995.cn

start) echo "启动" ;;
来源：http://hy.colortex.cn

stop)  echo "停止" ;;
来源：http://xq.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://qa.panjiajie.cn

esac
来源：http://oa.huixiangedu.cn

[R12] for 遍历文件
来源：http://uo.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://mv.nszjky.cn

[R13] for 计数循环
来源：http://ks.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://ps.asd995.cn

[R14] C 风格 for
来源：http://sr.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yv.hahajie.cn

[R15] while 逐行读文件
来源：http://es.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ta.asd995.cn

[R16] until 等待条件
来源：http://eh.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://au.chemitech.net.cn

[R17] 数组定义与取值
来源：http://pm.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dd.panjiajie.cn

[R18] 遍历数组
来源：http://ci.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://av.hnjuh.cn

[R19] 数组长度
来源：http://ud.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://mp.asd995.cn

[R20] 关联数组（字典）
来源：http://pf.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ua.lnxyls.cn

[R21] 字符串长度
来源：http://ng.yuntaijiaju.cn

echo "${#s}"
来源：http://te.lnxyls.cn

[R22] 截取子串
来源：http://dx.szxytkj.cn

echo "${s:0:5}"
来源：http://ka.nicolike.cn

[R23] 字符串替换
来源：http://xz.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ul.shxzskj.cn

[R24] 大小写转换
来源：http://rl.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nt.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://ow.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zv.huanxung.cn

[R26] 命令替换
来源：http://zl.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://ka.shtwfgs.cn

[R27] 算术展开
来源：http://jz.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://cx.shxzskj.cn

[R28] 浮点运算
来源：http://oz.muxihuayi.cn

echo "scale=2; 10/3" | bc
来源：http://af.bjjhwx.cn

[R29] 定义函数
来源：http://yg.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pq.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://bu.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://nh.yuntaijiaju.cn

[R31] 局部变量
来源：http://nq.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://bc.bjjhwx.cn

[R32] 参数个数校验
来源：http://hh.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ei.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://zd.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uk.huanxung.cn

[R34] 退出时清理
来源：http://sd.newstarts.cn

trap 'rm -f "$tmp"' EXIT
来源：http://av.521024.cn

[R35] 后台执行并等待
来源：http://ju.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qw.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://oy.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kv.hnjuh.cn

[R37] 把输出赋给变量
来源：http://he.wgjwhj.cn

files=$(ls -1)
来源：http://dy.521024.cn

[R38] 管道串联
来源：http://zc.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://wb.asd995.cn

[R39] 重定向标准输出与错误
来源：http://jq.hnjuh.cn

cmd > out.log 2>&1
来源：http://zf.yuntaijiaju.cn

[R40] 追加写日志
来源：http://qx.szsharing.cn

echo "log" >> out.log
来源：http://lk.gzmigu.cn

[R41] 丢弃输出
来源：http://kr.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://nh.shtwfgs.cn

[R42] 输入重定向
来源：http://zf.chemitech.net.cn

wc -l < a.txt
来源：http://od.gzmigu.cn

[R43] 按名字查找文件
来源：http://sp.wgjwhj.cn

find . -name "*.log" -type f
来源：http://yv.nicolike.cn

[R44] 按修改时间查找
来源：http://lr.shtwfgs.cn

find . -mtime -7 -type f
来源：http://zv.chemitech.net.cn

[R45] 批量删除
来源：http://la.nicolike.cn

find . -name "*.tmp" -delete
来源：http://gv.nszjky.cn

[R46] 递归替换文件内容
来源：http://zz.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bd.9csxet.cn

[R47] sed 单行替换
来源：http://kb.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hb.shxzskj.cn

[R48] awk 取指定列
来源：http://cs.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://ry.panjiajie.cn

[R49] awk 带条件
来源：http://zv.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lq.521024.cn

[R50] awk 求和
来源：http://um.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vw.521024.cn

[R51] 排序去重取前几
来源：http://pg.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vf.jctech888.com.cn

[R52] 统计行数
来源：http://ar.lnxyls.cn

wc -l a.txt
来源：http://gr.521024.cn

[R53] 查看文件头与实时尾
来源：http://fv.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zj.9csxet.cn

[R54] 比较两个文件
来源：http://py.huixinmuqiang.cn

diff a.txt b.txt
来源：http://qq.hahajie.cn

[R55] 压缩与解压
来源：http://ln.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fo.colortex.cn

[R56] 远程拷贝
来源：http://nc.bookmarksfly.cn

scp file user@host:/path/
来源：http://rj.521024.cn

[R57] 远程执行命令
来源：http://iz.chemitech.net.cn

ssh user@host 'uptime'
来源：http://of.shxzukj.cn

[R58] 下载文件
来源：http://js.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dd.huanxung.cn

[R59] 发 POST JSON
来源：http://zq.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ur.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://am.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ql.szsharing.cn

[R61] 磁盘占用
来源：http://nv.szxytkj.cn

df -h;  du -sh *
来源：http://ql.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://ch.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://gj.jianghongdianzi.cn

[R63] 内存与进程
来源：http://qn.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://gf.huixiangedu.cn

[R64] 结束进程
来源：http://bl.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://vr.jctech888.com.cn

[R65] 查看端口占用
来源：http://lp.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xi.newstarts.cn

[R66] 定时任务
来源：http://vh.lnxyls.cn

crontab -e;  crontab -l
来源：http://rd.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://zd.chemitech.net.cn

openssl rand -hex 16
来源：http://fl.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://lf.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xj.szxytkj.cn

[R69] 生成随机密码
来源：http://ik.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://at.szxytkj.cn

[R70] 时间戳与互转
来源：http://mj.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://ej.huanxung.cn

[R71] 日期格式化
来源：http://zp.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cw.yuexingan06.cn

[R72] 等待端口就绪
来源：http://fo.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cz.521024.cn

[R73] 分割大日志
来源：http://gq.shxzskj.cn

split -l 1000 big.log part_
来源：http://cq.haigaiapp.cn

[R74] 批量重命名
来源：http://kx.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lz.haigaiapp.cn

[R75] 导出环境变量
来源：http://oq.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://fm.huixiangedu.cn

[R76] 使用临时文件
来源：http://gj.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ca.bookmarksfly.cn

[R77] 读取用户输入
来源：http://jm.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://es.huanxung.cn

[R78] 交互式菜单
来源：http://to.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ei.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://jw.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hx.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://qe.newstarts.cn

time ./run.sh
来源：http://cs.chemitech.net.cn

================================================================================
来源：http://hq.yuexingan06.cn

S. C / C++ 专题
来源：http://zh.muxihuayi.cn

================================================================================
来源：http://aj.panjiajie.cn

[S01] C：Hello World
来源：http://mq.colortex.cn

#include <stdio.h>
来源：http://ew.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dt.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://ml.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://of.asd995.cn

[S03] C：读入整数
来源：http://hh.colortex.cn

int x; scanf("%d", &x);
来源：http://mq.bjjhwx.cn

[S04] C：字符串复制
来源：http://jo.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ic.muxihuayi.cn

[S05] C：字符串长度
来源：http://ak.huixinmuqiang.cn

strlen(s)
来源：http://wg.shtwfgs.cn

[S06] C：字符串比较
来源：http://uo.nszjky.cn

strcmp(a, b) == 0
来源：http://bz.newstarts.cn

[S07] C：数组遍历求和
来源：http://eg.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vk.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://jz.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sj.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://nh.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ft.hnjuh.cn

[S10] C：指针与解引用
来源：http://cc.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://sk.gzmigu.cn

[S11] C：逐行读文件
来源：http://sx.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ts.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tn.haigaiapp.cn

fclose(f);
来源：http://wg.nicolike.cn

[S12] C：写文件
来源：http://za.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qi.hahajie.cn

[S13] C：宏定义
来源：http://dy.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dd.huixiangedu.cn

[S14] C：枚举
来源：http://ps.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ff.shtwfgs.cn

[S15] C：类型转换
来源：http://wj.jianghongdianzi.cn

(double) a / b
来源：http://gg.bjjhwx.cn

[S16] C：位操作置位
来源：http://su.szsharing.cn

x |= (1 << 3);
来源：http://dl.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://kv.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oc.shxzukj.cn

[S18] C：命令行参数
来源：http://zv.shxzskj.cn

int main(int argc, char **argv)
来源：http://ag.521024.cn

[S19] C：快速排序
来源：http://ep.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fa.521024.cn

[S20] C：二分查找
来源：http://ec.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ls.shxzukj.cn

[S21] C：字符类别判断
来源：http://nx.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hx.chemitech.net.cn

[S22] C：字符串转数字
来源：http://lp.gzmigu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vc.asd995.cn

[S23] C：随机数
来源：http://tr.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ba.wgjwhj.cn

[S24] C：获取本地时间
来源：http://fb.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jz.9csxet.cn

[S25] C：内存拷贝
来源：http://at.szxytkj.cn

memcpy(dst, src, n);
来源：http://pi.lnxyls.cn

[S26] C：内存清零
来源：http://vy.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://al.newstarts.cn

[S27] C：定义常量
来源：http://zq.szsharing.cn

const double PI = 3.14159;
来源：http://pm.szsharing.cn

[S28] C：静态变量
来源：http://ve.szxytkj.cn

static int counter = 0;
来源：http://rg.hahajie.cn

[S29] C：变参函数
来源：http://xw.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ls.asd995.cn

[S30] C：头文件保护
来源：http://un.muxihuayi.cn


<!-- 参考信息 -->