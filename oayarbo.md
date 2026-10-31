代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://id.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://an.shtwfgs.cn

[Q43] 标量子查询
来源：http://sb.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gu.wgjwhj.cn

[Q44] IN 子查询
来源：http://za.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jv.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://ru.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jj.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ov.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sg.521024.cn

[Q47] 与平均值比较
来源：http://eq.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oa.jctech888.com.cn

[Q48] CTE 公用表表达式
来源：http://ws.lnxyls.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iq.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://ba.muxihuayi.cn

[Q49] 更新单行
来源：http://ze.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jq.bookmarksfly.cn

[Q50] 批量更新
来源：http://qj.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rc.asd995.cn

[Q51] 用子查询更新
来源：http://ga.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zp.shtwfgs.cn

[Q52] 删除指定行
来源：http://rl.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://gw.bookmarksfly.cn

[Q53] 按条件删除
来源：http://vf.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mq.lnxyls.cn

[Q54] 清空表
来源：http://fb.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://az.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://qp.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vy.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://va.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fb.panjiajie.cn

[Q57] 行号
来源：http://vh.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ut.bjjhwx.cn

[Q58] 累计求和
来源：http://ss.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lj.newstarts.cn

[Q59] 分组内累计
来源：http://ql.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pq.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://ge.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ch.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dn.hnjuh.cn

[Q61] 移动平均
来源：http://lo.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jh.colortex.cn

[Q62] 分组占比
来源：http://cn.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://by.lnxyls.cn

[Q63] 开启事务
来源：http://ty.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://am.shxzukj.cn

[Q64] 提交事务
来源：http://ei.hnjuh.cn

COMMIT;
来源：http://eu.asd995.cn

[Q65] 回滚事务
来源：http://rq.chemitech.net.cn

ROLLBACK;
来源：http://zc.gzmigu.cn

[Q66] 行锁查询
来源：http://rz.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ql.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://bo.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kq.521024.cn

[Q68] 保存点
来源：http://bs.shtwfgs.cn

SAVEPOINT sp1;
来源：http://hz.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://jx.hnjuh.cn

[Q69] 查看执行计划
来源：http://sr.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ev.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://rf.asd995.cn

ANALYZE TABLE users;
来源：http://gg.szxytkj.cn

[Q71] 查看建表语句
来源：http://fp.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dw.newstarts.cn

[Q72] 查看索引
来源：http://du.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://jw.nszjky.cn

[Q73] 查看表状态
来源：http://sm.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hn.jctech888.com.cn

[Q74] 强制使用索引
来源：http://bv.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ye.lnxyls.cn

[Q75] 日期格式化
来源：http://wf.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oo.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ql.wgjwhj.cn

[Q76] 按天统计
来源：http://vk.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dm.colortex.cn

[Q77] 时间加减
来源：http://vs.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oa.szsharing.cn

[Q78] 当前时间
来源：http://fx.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qk.shtwfgs.cn

[Q79] 字符串拼接
来源：http://hi.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oh.panjiajie.cn

[Q80] 字符串截取
来源：http://vk.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ye.9csxet.cn

[Q81] 字符串替换
来源：http://af.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ja.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://aq.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ad.panjiajie.cn

[Q83] 大小写转换
来源：http://wi.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fn.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://st.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://pl.nszjky.cn

[Q85] 数值取整
来源：http://ns.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fg.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://af.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fk.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://gj.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vl.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://bq.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://os.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fk.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://kj.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pn.yuexingan06.cn

[Q90] 生成序号列
来源：http://mj.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fn.muxihuayi.cn

================================================================================
来源：http://mm.hnjuh.cn

R. Bash 专题
来源：http://bu.shxzskj.cn

================================================================================
来源：http://bk.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://ib.521024.cn

#!/usr/bin/env bash
来源：http://fd.wgjwhj.cn

set -euo pipefail
来源：http://qo.521024.cn

[R02] 变量赋值与使用
来源：http://cd.shxzskj.cn

name="Tom"; echo "$name"
来源：http://hv.shxzukj.cn

[R03] 只读变量
来源：http://sa.521024.cn

readonly PI=3.14
来源：http://tg.jianghongdianzi.cn

[R04] 位置参数
来源：http://kv.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ul.szxytkj.cn

[R05] 参数默认值
来源：http://kx.colortex.cn

name="${1:-default}"
来源：http://qg.asd995.cn

[R06] 判断命令是否存在
来源：http://nh.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yi.muxihuayi.cn

[R07] if 判断文件
来源：http://rr.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gw.muxihuayi.cn

[R08] 数值比较
来源：http://sb.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ij.nicolike.cn

[R09] 字符串比较
来源：http://qw.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ar.colortex.cn

[R10] 正则匹配
来源：http://sc.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sq.huixiangedu.cn

[R11] case 多分支
来源：http://oi.huixinmuqiang.cn

case "$1" in
来源：http://pg.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://nb.newstarts.cn

stop)  echo "停止" ;;
来源：http://cj.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://bf.gzmigu.cn

esac
来源：http://zt.nszjky.cn

[R12] for 遍历文件
来源：http://db.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://nh.huixiangedu.cn

[R13] for 计数循环
来源：http://ux.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://sa.haigaiapp.cn

[R14] C 风格 for
来源：http://kp.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vm.huixiangedu.cn

[R15] while 逐行读文件
来源：http://qy.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wm.jctech888.com.cn

[R16] until 等待条件
来源：http://qe.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ij.jctech888.com.cn

[R17] 数组定义与取值
来源：http://iq.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lp.shtwfgs.cn

[R18] 遍历数组
来源：http://lu.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cy.yuexingan06.cn

[R19] 数组长度
来源：http://zv.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://qn.huanxung.cn

[R20] 关联数组（字典）
来源：http://jr.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://su.9csxet.cn

[R21] 字符串长度
来源：http://dr.szxytkj.cn

echo "${#s}"
来源：http://dg.wgjwhj.cn

[R22] 截取子串
来源：http://aa.lnxyls.cn

echo "${s:0:5}"
来源：http://ch.huixinmuqiang.cn

[R23] 字符串替换
来源：http://zt.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kz.szxytkj.cn

[R24] 大小写转换
来源：http://az.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://og.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://gd.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mg.chemitech.net.cn

[R26] 命令替换
来源：http://xc.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://hz.bjjhwx.cn

[R27] 算术展开
来源：http://jj.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://jk.huixinmuqiang.cn

[R28] 浮点运算
来源：http://uz.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://ge.jianghongdianzi.cn

[R29] 定义函数
来源：http://ek.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mr.9csxet.cn

[R30] 函数返回状态码
来源：http://mm.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://zv.colortex.cn

[R31] 局部变量
来源：http://nf.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://vc.bookmarksfly.cn

[R32] 参数个数校验
来源：http://oj.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fo.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://yy.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mm.hnjuh.cn

[R34] 退出时清理
来源：http://sk.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sn.shxzukj.cn

[R35] 后台执行并等待
来源：http://jc.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ab.panjiajie.cn

[R36] 并发执行多个任务
来源：http://pn.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wp.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://xp.huanxung.cn

files=$(ls -1)
来源：http://yg.shtwfgs.cn

[R38] 管道串联
来源：http://ap.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://hr.jianghongdianzi.cn

[R39] 重定向标准输出与错误
来源：http://nj.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://zm.huixinmuqiang.cn

[R40] 追加写日志
来源：http://fk.huanxung.cn

echo "log" >> out.log
来源：http://xh.newstarts.cn

[R41] 丢弃输出
来源：http://ma.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://zo.szxytkj.cn

[R42] 输入重定向
来源：http://ru.jianghongdianzi.cn

wc -l < a.txt
来源：http://hn.yuexingan06.cn

[R43] 按名字查找文件
来源：http://os.shtwfgs.cn

find . -name "*.log" -type f
来源：http://ac.wgjwhj.cn

[R44] 按修改时间查找
来源：http://du.shtwfgs.cn

find . -mtime -7 -type f
来源：http://ut.jianghongdianzi.cn

[R45] 批量删除
来源：http://gv.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://qm.newstarts.cn

[R46] 递归替换文件内容
来源：http://wi.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hx.chemitech.net.cn

[R47] sed 单行替换
来源：http://js.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xp.nicolike.cn

[R48] awk 取指定列
来源：http://qz.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://xw.yuexingan06.cn

[R49] awk 带条件
来源：http://oe.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iv.bookmarksfly.cn

[R50] awk 求和
来源：http://zr.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gs.yuexingan06.cn

[R51] 排序去重取前几
来源：http://zo.panjiajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xo.hnjuh.cn

[R52] 统计行数
来源：http://bz.yuexingan06.cn

wc -l a.txt
来源：http://vv.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://zf.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sw.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://fj.shtwfgs.cn

diff a.txt b.txt
来源：http://zi.wgjwhj.cn

[R55] 压缩与解压
来源：http://xg.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cw.newstarts.cn

[R56] 远程拷贝
来源：http://px.bjjhwx.cn

scp file user@host:/path/
来源：http://dd.shxzskj.cn

[R57] 远程执行命令
来源：http://dh.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://kd.jianghongdianzi.cn

[R58] 下载文件
来源：http://zz.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ar.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://op.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jm.521024.cn

[R60] 只看 HTTP 状态码
来源：http://jh.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vt.bookmarksfly.cn

[R61] 磁盘占用
来源：http://fe.jctech888.com.cn

df -h;  du -sh *
来源：http://ed.shxzskj.cn

[R62] 找最占空间的文件
来源：http://mx.asd995.cn

du -ah . | sort -rh | head -10
来源：http://ds.nszjky.cn

[R63] 内存与进程
来源：http://ax.wgjwhj.cn

free -h;  ps aux | grep nginx
来源：http://ez.panjiajie.cn

[R64] 结束进程
来源：http://lz.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://wl.shxzskj.cn

[R65] 查看端口占用
来源：http://ii.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fz.colortex.cn

[R66] 定时任务
来源：http://jj.asd995.cn

crontab -e;  crontab -l
来源：http://vi.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://va.hnjuh.cn

openssl rand -hex 16
来源：http://cb.muxihuayi.cn

[R68] 计算文件校验值
来源：http://tm.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ps.newstarts.cn

[R69] 生成随机密码
来源：http://nd.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://uf.chemitech.net.cn

[R70] 时间戳与互转
来源：http://fb.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://hr.haigaiapp.cn

[R71] 日期格式化
来源：http://zv.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qr.haigaiapp.cn

[R72] 等待端口就绪
来源：http://gp.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cr.shxzskj.cn

[R73] 分割大日志
来源：http://jp.asd995.cn

split -l 1000 big.log part_
来源：http://gk.jianghongdianzi.cn

[R74] 批量重命名
来源：http://rx.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mz.newstarts.cn

[R75] 导出环境变量
来源：http://gw.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://pt.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://av.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fd.bookmarksfly.cn

[R77] 读取用户输入
来源：http://ck.chemitech.net.cn

read -rp "请输入: " ans
来源：http://ck.chemitech.net.cn

[R78] 交互式菜单
来源：http://wl.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nw.shtwfgs.cn

[R79] 解析命令行选项
来源：http://sr.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yy.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://bx.szxytkj.cn

time ./run.sh
来源：http://pm.nicolike.cn

================================================================================
来源：http://oi.bookmarksfly.cn

S. C / C++ 专题
来源：http://ts.nicolike.cn

================================================================================
来源：http://hc.yuntaijiaju.cn

[S01] C：Hello World
来源：http://to.hahajie.cn

#include <stdio.h>
来源：http://nd.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rf.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://nt.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://ej.hnjuh.cn

[S03] C：读入整数
来源：http://ej.9csxet.cn

int x; scanf("%d", &x);
来源：http://ze.521024.cn

[S04] C：字符串复制
来源：http://kq.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xz.bjjhwx.cn

[S05] C：字符串长度
来源：http://rs.huixinmuqiang.cn

strlen(s)
来源：http://yj.yuexingan06.cn

[S06] C：字符串比较
来源：http://fk.szsharing.cn

strcmp(a, b) == 0
来源：http://cv.colortex.cn

[S07] C：数组遍历求和
来源：http://aw.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://al.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://eu.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uj.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://bo.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wy.szsharing.cn

[S10] C：指针与解引用
来源：http://sj.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://do.bjjhwx.cn

[S11] C：逐行读文件
来源：http://zk.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://pf.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ti.newstarts.cn

fclose(f);
来源：http://vk.lnxyls.cn

[S12] C：写文件
来源：http://ez.hnjuh.cn


<!-- 参考信息 -->