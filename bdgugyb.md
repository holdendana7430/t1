代发 wailian999

[Q48] CTE 公用表表达式
来源：http://li.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vc.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://yk.panjiajie.cn

[Q49] 更新单行
来源：http://xz.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kv.haigaiapp.cn

[Q50] 批量更新
来源：http://cd.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://if.huanxung.cn

[Q51] 用子查询更新
来源：http://mj.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://go.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://fj.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://jp.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://ke.haigaiapp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lg.yuntaijiaju.cn

[Q54] 清空表
来源：http://fq.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://wz.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://eb.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ef.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://hh.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iu.chemitech.net.cn

[Q57] 行号
来源：http://pd.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rx.hnjuh.cn

[Q58] 累计求和
来源：http://xm.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jn.huixiangedu.cn

[Q59] 分组内累计
来源：http://ay.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sr.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://qa.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gg.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zi.huixinmuqiang.cn

[Q61] 移动平均
来源：http://xf.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ux.9csxet.cn

[Q62] 分组占比
来源：http://xg.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qr.chemitech.net.cn

[Q63] 开启事务
来源：http://jk.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://es.gzmigu.cn

[Q64] 提交事务
来源：http://sd.yuexingan06.cn

COMMIT;
来源：http://ej.asd995.cn

[Q65] 回滚事务
来源：http://ee.nszjky.cn

ROLLBACK;
来源：http://ps.nszjky.cn

[Q66] 行锁查询
来源：http://es.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nd.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://lx.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ma.nicolike.cn

[Q68] 保存点
来源：http://tv.hnjuh.cn

SAVEPOINT sp1;
来源：http://zo.asd995.cn

ROLLBACK TO sp1;
来源：http://ge.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://cv.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dr.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://qa.newstarts.cn

ANALYZE TABLE users;
来源：http://xd.jctech888.com.cn

[Q71] 查看建表语句
来源：http://ua.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lq.colortex.cn

[Q72] 查看索引
来源：http://zl.panjiajie.cn

SHOW INDEX FROM users;
来源：http://ag.521024.cn

[Q73] 查看表状态
来源：http://ds.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nh.lnxyls.cn

[Q74] 强制使用索引
来源：http://uv.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sp.shxzskj.cn

[Q75] 日期格式化
来源：http://tu.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ji.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yy.nszjky.cn

[Q76] 按天统计
来源：http://oa.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oy.newstarts.cn

[Q77] 时间加减
来源：http://sj.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xz.yuntaijiaju.cn

[Q78] 当前时间
来源：http://fj.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ak.9csxet.cn

[Q79] 字符串拼接
来源：http://zn.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sv.bookmarksfly.cn

[Q80] 字符串截取
来源：http://cl.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cj.chemitech.net.cn

[Q81] 字符串替换
来源：http://kj.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xb.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://bo.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mk.shtwfgs.cn

[Q83] 大小写转换
来源：http://ux.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zr.9csxet.cn

[Q84] 去除首尾空格
来源：http://ei.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://oi.huixinmuqiang.cn

[Q85] 数值取整
来源：http://tj.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ab.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://qe.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vh.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://kg.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ur.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://jc.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kz.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mx.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://ux.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qa.bookmarksfly.cn

[Q90] 生成序号列
来源：http://xy.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bm.colortex.cn

================================================================================
来源：http://jj.newstarts.cn

R. Bash 专题
来源：http://dl.huixiangedu.cn

================================================================================
来源：http://zh.nicolike.cn

[R01] shebang 与严格模式
来源：http://gl.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://ha.hnjuh.cn

set -euo pipefail
来源：http://ax.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://bo.colortex.cn

name="Tom"; echo "$name"
来源：http://wy.521024.cn

[R03] 只读变量
来源：http://xj.yuexingan06.cn

readonly PI=3.14
来源：http://zw.chemitech.net.cn

[R04] 位置参数
来源：http://oj.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qs.lnxyls.cn

[R05] 参数默认值
来源：http://tb.panjiajie.cn

name="${1:-default}"
来源：http://rx.panjiajie.cn

[R06] 判断命令是否存在
来源：http://qr.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cf.szsharing.cn

[R07] if 判断文件
来源：http://zs.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://df.panjiajie.cn

[R08] 数值比较
来源：http://ys.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://io.shxzukj.cn

[R09] 字符串比较
来源：http://ae.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ip.hahajie.cn

[R10] 正则匹配
来源：http://qu.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tp.szsharing.cn

[R11] case 多分支
来源：http://ze.panjiajie.cn

case "$1" in
来源：http://kf.haigaiapp.cn

start) echo "启动" ;;
来源：http://cl.szxytkj.cn

stop)  echo "停止" ;;
来源：http://cb.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://rs.lnxyls.cn

esac
来源：http://in.wgjwhj.cn

[R12] for 遍历文件
来源：http://re.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://xz.huixiangedu.cn

[R13] for 计数循环
来源：http://ay.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://uk.nicolike.cn

[R14] C 风格 for
来源：http://gk.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ro.panjiajie.cn

[R15] while 逐行读文件
来源：http://hi.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sz.lnxyls.cn

[R16] until 等待条件
来源：http://lv.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wu.szsharing.cn

[R17] 数组定义与取值
来源：http://pa.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fe.muxihuayi.cn

[R18] 遍历数组
来源：http://ve.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vq.szxytkj.cn

[R19] 数组长度
来源：http://kg.gzmigu.cn

echo "${#arr[@]}"
来源：http://nr.panjiajie.cn

[R20] 关联数组（字典）
来源：http://pk.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qz.huixinmuqiang.cn

[R21] 字符串长度
来源：http://yw.lnxyls.cn

echo "${#s}"
来源：http://ni.wgjwhj.cn

[R22] 截取子串
来源：http://kg.hnjuh.cn

echo "${s:0:5}"
来源：http://qy.panjiajie.cn

[R23] 字符串替换
来源：http://km.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gn.nicolike.cn

[R24] 大小写转换
来源：http://ip.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://li.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://yw.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tx.bookmarksfly.cn

[R26] 命令替换
来源：http://ck.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://xf.chemitech.net.cn

[R27] 算术展开
来源：http://au.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://vg.newstarts.cn

[R28] 浮点运算
来源：http://uu.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://qg.bookmarksfly.cn

[R29] 定义函数
来源：http://du.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pi.wgjwhj.cn

[R30] 函数返回状态码
来源：http://ya.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://ro.huanxung.cn

[R31] 局部变量
来源：http://nv.shtwfgs.cn

f() { local x=1; echo "$x"; }
来源：http://pq.szsharing.cn

[R32] 参数个数校验
来源：http://ks.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oh.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://py.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jd.bookmarksfly.cn

[R34] 退出时清理
来源：http://tq.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mt.huixiangedu.cn

[R35] 后台执行并等待
来源：http://ce.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gi.nicolike.cn

[R36] 并发执行多个任务
来源：http://dp.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nc.gzmigu.cn

[R37] 把输出赋给变量
来源：http://en.haigaiapp.cn

files=$(ls -1)
来源：http://fw.szsharing.cn

[R38] 管道串联
来源：http://jo.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://oa.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://wd.muxihuayi.cn

cmd > out.log 2>&1
来源：http://dp.shtwfgs.cn

[R40] 追加写日志
来源：http://wk.asd995.cn

echo "log" >> out.log
来源：http://ba.bookmarksfly.cn

[R41] 丢弃输出
来源：http://gn.gzmigu.cn

cmd >/dev/null 2>&1
来源：http://yw.shtwfgs.cn

[R42] 输入重定向
来源：http://si.wgjwhj.cn

wc -l < a.txt
来源：http://eb.huixiangedu.cn

[R43] 按名字查找文件
来源：http://vk.lnxyls.cn

find . -name "*.log" -type f
来源：http://dy.wgjwhj.cn

[R44] 按修改时间查找
来源：http://mx.gzmigu.cn

find . -mtime -7 -type f
来源：http://hf.asd995.cn

[R45] 批量删除
来源：http://lx.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://ob.hahajie.cn

[R46] 递归替换文件内容
来源：http://gp.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jt.asd995.cn

[R47] sed 单行替换
来源：http://rl.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ve.nicolike.cn

[R48] awk 取指定列
来源：http://cp.nszjky.cn

awk '{print $1, $3}' a.txt
来源：http://ql.chemitech.net.cn

[R49] awk 带条件
来源：http://ln.hahajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ec.haigaiapp.cn

[R50] awk 求和
来源：http://mv.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lz.lnxyls.cn

[R51] 排序去重取前几
来源：http://te.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bq.panjiajie.cn

[R52] 统计行数
来源：http://ls.bookmarksfly.cn

wc -l a.txt
来源：http://wj.asd995.cn

[R53] 查看文件头与实时尾
来源：http://ec.szsharing.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yc.yuexingan06.cn

[R54] 比较两个文件
来源：http://vw.colortex.cn

diff a.txt b.txt
来源：http://rm.nicolike.cn

[R55] 压缩与解压
来源：http://se.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ju.muxihuayi.cn

[R56] 远程拷贝
来源：http://ty.521024.cn

scp file user@host:/path/
来源：http://wd.9csxet.cn

[R57] 远程执行命令
来源：http://dp.wgjwhj.cn

ssh user@host 'uptime'
来源：http://ry.asd995.cn

[R58] 下载文件
来源：http://vx.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ga.9csxet.cn

[R59] 发 POST JSON
来源：http://rc.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fb.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://gp.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ga.huanxung.cn

[R61] 磁盘占用
来源：http://hz.wgjwhj.cn

df -h;  du -sh *
来源：http://uo.shxzukj.cn

[R62] 找最占空间的文件
来源：http://dh.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://ds.shxzukj.cn

[R63] 内存与进程
来源：http://so.521024.cn

free -h;  ps aux | grep nginx
来源：http://lz.yuntaijiaju.cn

[R64] 结束进程
来源：http://ln.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://lg.9csxet.cn

[R65] 查看端口占用
来源：http://ds.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hl.hnjuh.cn

[R66] 定时任务
来源：http://ia.hahajie.cn

crontab -e;  crontab -l
来源：http://ua.chemitech.net.cn

[R67] 生成随机十六进制串
来源：http://kx.huixinmuqiang.cn

openssl rand -hex 16
来源：http://fg.jctech888.com.cn

[R68] 计算文件校验值
来源：http://dd.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kv.szxytkj.cn

[R69] 生成随机密码
来源：http://hp.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ot.muxihuayi.cn

[R70] 时间戳与互转
来源：http://oo.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://ya.nszjky.cn

[R71] 日期格式化
来源：http://zd.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zd.shxzskj.cn

[R72] 等待端口就绪
来源：http://bs.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ht.wgjwhj.cn

[R73] 分割大日志
来源：http://pk.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://zy.shxzukj.cn

[R74] 批量重命名
来源：http://tg.nszjky.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ov.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ei.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://dc.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ym.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qd.huixiangedu.cn

[R77] 读取用户输入
来源：http://fc.huixiangedu.cn

read -rp "请输入: " ans
来源：http://cz.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://gp.huixinmuqiang.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eu.colortex.cn

[R79] 解析命令行选项
来源：http://dp.szsharing.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jt.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://es.colortex.cn

time ./run.sh
来源：http://fl.huixiangedu.cn

================================================================================
来源：http://mj.hnjuh.cn

S. C / C++ 专题
来源：http://nm.nszjky.cn

================================================================================
来源：http://ek.panjiajie.cn

[S01] C：Hello World
来源：http://hg.szsharing.cn

#include <stdio.h>
来源：http://jf.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mc.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://da.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://vq.bookmarksfly.cn

[S03] C：读入整数
来源：http://eu.nicolike.cn

int x; scanf("%d", &x);
来源：http://ra.bookmarksfly.cn

[S04] C：字符串复制
来源：http://dl.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xg.shxzukj.cn

[S05] C：字符串长度
来源：http://uu.hnjuh.cn

strlen(s)
来源：http://un.gzmigu.cn

[S06] C：字符串比较
来源：http://cx.newstarts.cn

strcmp(a, b) == 0
来源：http://jm.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://nc.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ao.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://tm.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gr.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://bt.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ri.jctech888.com.cn

[S10] C：指针与解引用
来源：http://ip.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://bq.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://ps.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://py.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gx.colortex.cn

fclose(f);
来源：http://mx.shxzskj.cn

[S12] C：写文件
来源：http://cx.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iq.huixiangedu.cn

[S13] C：宏定义
来源：http://wv.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zy.newstarts.cn

[S14] C：枚举
来源：http://lp.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://kt.huixinmuqiang.cn

[S15] C：类型转换
来源：http://jf.wgjwhj.cn

(double) a / b
来源：http://nd.panjiajie.cn

[S16] C：位操作置位
来源：http://kk.wgjwhj.cn

x |= (1 << 3);
来源：http://va.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://fa.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://un.521024.cn

[S18] C：命令行参数
来源：http://gm.chemitech.net.cn


<!-- 参考信息 -->