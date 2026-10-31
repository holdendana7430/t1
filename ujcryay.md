代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vq.huixinmuqiang.cn

[Q24] 去重
来源：http://gq.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://go.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://of.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cd.521024.cn

[Q26] 计数
来源：http://in.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://fy.jianghongdianzi.cn

[Q27] 条件计数
来源：http://pq.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lr.shxzskj.cn

[Q28] 求和与平均
来源：http://hu.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ag.huanxung.cn

[Q29] 最大最小值
来源：http://ga.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cw.szsharing.cn

[Q30] 分组统计
来源：http://yd.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sn.muxihuayi.cn

[Q31] 分组后过滤
来源：http://wq.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pv.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://ja.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wq.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bj.gzmigu.cn

[Q33] 多列分组
来源：http://lu.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sq.shxzskj.cn

[Q34] 每组取第一条
来源：http://gj.haigaiapp.cn

SELECT * FROM (
来源：http://fu.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ae.lnxyls.cn

) t WHERE rn = 1;
来源：http://jn.wgjwhj.cn

[Q35] 内连接
来源：http://al.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bh.haigaiapp.cn

[Q36] 左连接
来源：http://dx.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ej.9csxet.cn

[Q37] 右连接
来源：http://tm.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cq.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ae.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wx.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://li.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://su.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zh.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qn.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://la.huixinmuqiang.cn

[Q41] 多表连接
来源：http://xm.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iv.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://wt.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://bn.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://vx.panjiajie.cn

SELECT u.name, o.amount FROM users u
来源：http://yh.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wn.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://os.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://on.asd995.cn

[Q44] IN 子查询
来源：http://rb.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ad.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://rb.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jl.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ns.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vj.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://rx.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xy.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://gd.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oi.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://es.521024.cn

[Q49] 更新单行
来源：http://er.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bl.hnjuh.cn

[Q50] 批量更新
来源：http://tj.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hs.colortex.cn

[Q51] 用子查询更新
来源：http://pa.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pn.szxytkj.cn

[Q52] 删除指定行
来源：http://th.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://tb.huanxung.cn

[Q53] 按条件删除
来源：http://pf.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aw.lnxyls.cn

[Q54] 清空表
来源：http://tf.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://du.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://ob.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kk.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://sf.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://df.colortex.cn

[Q57] 行号
来源：http://hb.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ja.newstarts.cn

[Q58] 累计求和
来源：http://dh.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://di.asd995.cn

[Q59] 分组内累计
来源：http://vr.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xt.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://dt.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vd.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qx.szxytkj.cn

[Q61] 移动平均
来源：http://to.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oj.yuexingan06.cn

[Q62] 分组占比
来源：http://dy.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fo.huixiangedu.cn

[Q63] 开启事务
来源：http://gs.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qx.521024.cn

[Q64] 提交事务
来源：http://cb.huixiangedu.cn

COMMIT;
来源：http://ap.gzmigu.cn

[Q65] 回滚事务
来源：http://xp.chemitech.net.cn

ROLLBACK;
来源：http://jv.huanxung.cn

[Q66] 行锁查询
来源：http://de.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tz.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://qr.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gh.bjjhwx.cn

[Q68] 保存点
来源：http://qm.jctech888.com.cn

SAVEPOINT sp1;
来源：http://dy.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://lt.newstarts.cn

[Q69] 查看执行计划
来源：http://wl.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ju.yuexingan06.cn

[Q70] 更新统计信息
来源：http://eb.shxzskj.cn

ANALYZE TABLE users;
来源：http://nj.huixiangedu.cn

[Q71] 查看建表语句
来源：http://jb.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ly.shtwfgs.cn

[Q72] 查看索引
来源：http://ld.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://hu.panjiajie.cn

[Q73] 查看表状态
来源：http://di.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://az.szxytkj.cn

[Q74] 强制使用索引
来源：http://uk.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aa.shxzskj.cn

[Q75] 日期格式化
来源：http://ks.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fr.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tk.colortex.cn

[Q76] 按天统计
来源：http://xu.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cw.jctech888.com.cn

[Q77] 时间加减
来源：http://lv.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lj.yuntaijiaju.cn

[Q78] 当前时间
来源：http://yb.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gj.shtwfgs.cn

[Q79] 字符串拼接
来源：http://vb.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zb.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://lb.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lq.newstarts.cn

[Q81] 字符串替换
来源：http://hu.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gy.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://sv.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dp.gzmigu.cn

[Q83] 大小写转换
来源：http://cv.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wl.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://rz.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://ow.shtwfgs.cn

[Q85] 数值取整
来源：http://gb.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gz.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://ip.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bs.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://ql.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iu.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://sf.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ye.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gx.shxzskj.cn

[Q89] 判断表是否存在
来源：http://tx.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sv.huanxung.cn

[Q90] 生成序号列
来源：http://ig.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://og.hahajie.cn

================================================================================
来源：http://cm.haigaiapp.cn

R. Bash 专题
来源：http://kw.bjjhwx.cn

================================================================================
来源：http://iu.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://xx.colortex.cn

#!/usr/bin/env bash
来源：http://vp.panjiajie.cn

set -euo pipefail
来源：http://ah.panjiajie.cn

[R02] 变量赋值与使用
来源：http://wr.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://co.huanxung.cn

[R03] 只读变量
来源：http://ku.bookmarksfly.cn

readonly PI=3.14
来源：http://bu.nszjky.cn

[R04] 位置参数
来源：http://ux.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jp.huixinmuqiang.cn

[R05] 参数默认值
来源：http://vq.muxihuayi.cn

name="${1:-default}"
来源：http://vc.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://ex.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rh.huanxung.cn

[R07] if 判断文件
来源：http://nl.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gv.colortex.cn

[R08] 数值比较
来源：http://kv.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jw.haigaiapp.cn

[R09] 字符串比较
来源：http://py.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ia.jctech888.com.cn

[R10] 正则匹配
来源：http://kc.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aw.jianghongdianzi.cn

[R11] case 多分支
来源：http://pc.bjjhwx.cn

case "$1" in
来源：http://id.jctech888.com.cn

start) echo "启动" ;;
来源：http://mj.nszjky.cn

stop)  echo "停止" ;;
来源：http://hh.colortex.cn

*)     echo "未知命令" ;;
来源：http://tg.huanxung.cn

esac
来源：http://ym.hnjuh.cn

[R12] for 遍历文件
来源：http://av.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://jj.szxytkj.cn

[R13] for 计数循环
来源：http://xv.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://kc.9csxet.cn

[R14] C 风格 for
来源：http://oz.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dc.hahajie.cn

[R15] while 逐行读文件
来源：http://fr.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wy.jianghongdianzi.cn

[R16] until 等待条件
来源：http://rj.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://du.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://de.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gb.shtwfgs.cn

[R18] 遍历数组
来源：http://ch.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lm.chemitech.net.cn

[R19] 数组长度
来源：http://gm.hnjuh.cn

echo "${#arr[@]}"
来源：http://og.521024.cn

[R20] 关联数组（字典）
来源：http://ol.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ho.shxzskj.cn

[R21] 字符串长度
来源：http://hl.521024.cn

echo "${#s}"
来源：http://lb.haigaiapp.cn

[R22] 截取子串
来源：http://pp.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://ns.shtwfgs.cn

[R23] 字符串替换
来源：http://qy.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rq.lnxyls.cn

[R24] 大小写转换
来源：http://zh.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fh.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://ce.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://to.wgjwhj.cn

[R26] 命令替换
来源：http://ky.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://yu.huixiangedu.cn

[R27] 算术展开
来源：http://jz.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://yv.yuexingan06.cn

[R28] 浮点运算
来源：http://kh.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://ak.shxzskj.cn

[R29] 定义函数
来源：http://yp.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://da.colortex.cn

[R30] 函数返回状态码
来源：http://le.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://rz.yuntaijiaju.cn

[R31] 局部变量
来源：http://jt.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://zr.newstarts.cn

[R32] 参数个数校验
来源：http://ex.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fd.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://dy.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tp.bjjhwx.cn

[R34] 退出时清理
来源：http://al.chemitech.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ff.newstarts.cn

[R35] 后台执行并等待
来源：http://uh.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ts.hnjuh.cn

[R36] 并发执行多个任务
来源：http://jx.colortex.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gz.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://cr.yuexingan06.cn

files=$(ls -1)
来源：http://kq.jianghongdianzi.cn

[R38] 管道串联
来源：http://kj.jianghongdianzi.cn

cat a.txt | grep -i error | wc -l
来源：http://iu.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://oq.jctech888.com.cn

cmd > out.log 2>&1
来源：http://pj.bjjhwx.cn

[R40] 追加写日志
来源：http://hp.gzmigu.cn

echo "log" >> out.log
来源：http://iz.lnxyls.cn

[R41] 丢弃输出
来源：http://ne.huixinmuqiang.cn

cmd >/dev/null 2>&1
来源：http://ca.yuexingan06.cn

[R42] 输入重定向
来源：http://yw.gzmigu.cn

wc -l < a.txt
来源：http://bl.shxzukj.cn

[R43] 按名字查找文件
来源：http://dh.muxihuayi.cn

find . -name "*.log" -type f
来源：http://tt.shxzskj.cn

[R44] 按修改时间查找
来源：http://fb.nszjky.cn

find . -mtime -7 -type f
来源：http://xh.shxzskj.cn

[R45] 批量删除
来源：http://yd.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://qe.panjiajie.cn

[R46] 递归替换文件内容
来源：http://ng.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yj.huanxung.cn

[R47] sed 单行替换
来源：http://ik.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iu.shxzukj.cn

[R48] awk 取指定列
来源：http://ue.nicolike.cn

awk '{print $1, $3}' a.txt
来源：http://fk.lnxyls.cn

[R49] awk 带条件
来源：http://wi.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kd.szxytkj.cn

[R50] awk 求和
来源：http://ft.nicolike.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bn.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://io.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ip.hahajie.cn

[R52] 统计行数
来源：http://ml.szxytkj.cn

wc -l a.txt
来源：http://pu.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://uq.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://js.colortex.cn

[R54] 比较两个文件
来源：http://oi.colortex.cn

diff a.txt b.txt
来源：http://aw.521024.cn

[R55] 压缩与解压
来源：http://by.hahajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zd.9csxet.cn

[R56] 远程拷贝
来源：http://hy.szxytkj.cn

scp file user@host:/path/
来源：http://td.9csxet.cn

[R57] 远程执行命令
来源：http://wi.asd995.cn

ssh user@host 'uptime'
来源：http://ba.muxihuayi.cn

[R58] 下载文件
来源：http://eo.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bz.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://zw.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qc.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://sp.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jh.shtwfgs.cn

[R61] 磁盘占用
来源：http://wz.yuexingan06.cn

df -h;  du -sh *
来源：http://mq.hnjuh.cn

[R62] 找最占空间的文件
来源：http://cl.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://vl.jctech888.com.cn

[R63] 内存与进程
来源：http://rm.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://ak.shxzskj.cn

[R64] 结束进程
来源：http://kf.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://bq.nicolike.cn

[R65] 查看端口占用
来源：http://fz.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vb.yuntaijiaju.cn

[R66] 定时任务
来源：http://zb.nszjky.cn

crontab -e;  crontab -l
来源：http://pr.9csxet.cn

[R67] 生成随机十六进制串
来源：http://jz.chemitech.net.cn

openssl rand -hex 16
来源：http://ms.huixiangedu.cn

[R68] 计算文件校验值
来源：http://wx.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mm.9csxet.cn

[R69] 生成随机密码
来源：http://xv.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://zo.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://le.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://wp.asd995.cn

[R71] 日期格式化
来源：http://nf.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ik.nszjky.cn

[R72] 等待端口就绪
来源：http://rk.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mr.shtwfgs.cn

[R73] 分割大日志
来源：http://dy.yuntaijiaju.cn


<!-- 参考信息 -->