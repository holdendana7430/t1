代发 wailian999

);
来源：http://vt.muxihuayi.cn

[Q03] 增加列
来源：http://eb.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ck.gzmigu.cn

[Q04] 修改列类型
来源：http://pf.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://do.yuexingan06.cn

[Q05] 重命名列
来源：http://vz.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://to.newstarts.cn

[Q06] 删除列
来源：http://sx.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fn.haigaiapp.cn

[Q07] 删除表
来源：http://hc.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://rf.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://qm.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pr.nszjky.cn

[Q09] 创建唯一索引
来源：http://sa.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://og.asd995.cn

[Q10] 插入单行
来源：http://de.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rb.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://dz.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qn.asd995.cn

[Q12] 插入后取自增 ID
来源：http://ml.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jp.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sd.hahajie.cn

[Q13] 忽略重复插入
来源：http://zq.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qj.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://tb.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://my.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ll.lnxyls.cn

[Q15] 查询全部
来源：http://eo.szxytkj.cn

SELECT * FROM users;
来源：http://jx.jctech888.com.cn

[Q16] 查询指定列
来源：http://hz.hahajie.cn

SELECT id, name FROM users;
来源：http://ms.gzmigu.cn

[Q17] 条件查询
来源：http://tx.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://im.gzmigu.cn

[Q18] 模糊匹配
来源：http://bm.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yi.shtwfgs.cn

[Q19] 范围查询
来源：http://oz.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uv.asd995.cn

[Q20] IN 列表
来源：http://zb.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ql.szxytkj.cn

[Q21] 空值判断
来源：http://ko.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hv.huixiangedu.cn

[Q22] 排序
来源：http://xy.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tf.gzmigu.cn

[Q23] 分页
来源：http://ay.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pp.nicolike.cn

[Q24] 去重
来源：http://ws.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://gw.szsharing.cn

[Q25] 只取前 N 条
来源：http://ko.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eu.hnjuh.cn

[Q26] 计数
来源：http://ho.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://th.521024.cn

[Q27] 条件计数
来源：http://ff.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yi.chemitech.net.cn

[Q28] 求和与平均
来源：http://nr.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cr.gzmigu.cn

[Q29] 最大最小值
来源：http://jc.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eq.wgjwhj.cn

[Q30] 分组统计
来源：http://ls.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nt.huixiangedu.cn

[Q31] 分组后过滤
来源：http://gy.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cq.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://si.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ae.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fp.yuntaijiaju.cn

[Q33] 多列分组
来源：http://fc.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tz.chemitech.net.cn

[Q34] 每组取第一条
来源：http://it.hnjuh.cn

SELECT * FROM (
来源：http://ie.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cx.muxihuayi.cn

) t WHERE rn = 1;
来源：http://sj.shxzukj.cn

[Q35] 内连接
来源：http://yj.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ed.bookmarksfly.cn

[Q36] 左连接
来源：http://te.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://en.asd995.cn

[Q37] 右连接
来源：http://sy.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yc.huixinmuqiang.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kv.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jc.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://zj.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ws.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sq.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ax.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xt.bookmarksfly.cn

[Q41] 多表连接
来源：http://iz.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://po.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://pz.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://jm.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://rp.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://ro.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rb.jctech888.com.cn

[Q43] 标量子查询
来源：http://ed.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yg.shtwfgs.cn

[Q44] IN 子查询
来源：http://ov.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sw.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://hu.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://po.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ax.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zy.huanxung.cn

[Q47] 与平均值比较
来源：http://pp.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ro.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://xr.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qh.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://ac.muxihuayi.cn

[Q49] 更新单行
来源：http://mb.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lt.hahajie.cn

[Q50] 批量更新
来源：http://ks.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qq.szsharing.cn

[Q51] 用子查询更新
来源：http://rc.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ix.bjjhwx.cn

[Q52] 删除指定行
来源：http://fa.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://up.jctech888.com.cn

[Q53] 按条件删除
来源：http://ab.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ib.asd995.cn

[Q54] 清空表
来源：http://uy.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://bv.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://pz.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lk.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://mx.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yo.nszjky.cn

[Q57] 行号
来源：http://wj.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jc.shtwfgs.cn

[Q58] 累计求和
来源：http://ls.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ji.yuexingan06.cn

[Q59] 分组内累计
来源：http://qg.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pc.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://ts.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gb.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jo.colortex.cn

[Q61] 移动平均
来源：http://og.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://al.shxzukj.cn

[Q62] 分组占比
来源：http://sr.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mo.asd995.cn

[Q63] 开启事务
来源：http://az.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lp.huanxung.cn

[Q64] 提交事务
来源：http://nw.521024.cn

COMMIT;
来源：http://qq.huixiangedu.cn

[Q65] 回滚事务
来源：http://gi.muxihuayi.cn

ROLLBACK;
来源：http://ij.521024.cn

[Q66] 行锁查询
来源：http://ya.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xg.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://dv.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fq.gzmigu.cn

[Q68] 保存点
来源：http://je.colortex.cn

SAVEPOINT sp1;
来源：http://nz.9csxet.cn

ROLLBACK TO sp1;
来源：http://ui.wgjwhj.cn

[Q69] 查看执行计划
来源：http://oe.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ih.panjiajie.cn

[Q70] 更新统计信息
来源：http://nk.shxzukj.cn

ANALYZE TABLE users;
来源：http://wg.bjjhwx.cn

[Q71] 查看建表语句
来源：http://vn.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rq.shxzukj.cn

[Q72] 查看索引
来源：http://qq.asd995.cn

SHOW INDEX FROM users;
来源：http://yg.chemitech.net.cn

[Q73] 查看表状态
来源：http://bi.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ff.nicolike.cn

[Q74] 强制使用索引
来源：http://yv.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sm.asd995.cn

[Q75] 日期格式化
来源：http://gw.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ot.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ip.nicolike.cn

[Q76] 按天统计
来源：http://mj.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qz.newstarts.cn

[Q77] 时间加减
来源：http://zm.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vw.szxytkj.cn

[Q78] 当前时间
来源：http://in.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tr.lnxyls.cn

[Q79] 字符串拼接
来源：http://wf.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ul.yuexingan06.cn

[Q80] 字符串截取
来源：http://vd.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jp.huixiangedu.cn

[Q81] 字符串替换
来源：http://rn.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tw.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://iz.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://an.hahajie.cn

[Q83] 大小写转换
来源：http://lc.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tr.shxzskj.cn

[Q84] 去除首尾空格
来源：http://sb.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://fo.hnjuh.cn

[Q85] 数值取整
来源：http://fk.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dn.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://cw.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://la.nicolike.cn

[Q87] JSON 字段做条件
来源：http://pr.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mk.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://ir.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ep.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ps.asd995.cn

[Q89] 判断表是否存在
来源：http://ak.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ht.wgjwhj.cn

[Q90] 生成序号列
来源：http://dn.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://px.nszjky.cn

================================================================================
来源：http://qb.shtwfgs.cn

R. Bash 专题
来源：http://zd.521024.cn

================================================================================
来源：http://jj.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://sc.shxzukj.cn

#!/usr/bin/env bash
来源：http://tb.shxzskj.cn

set -euo pipefail
来源：http://hz.9csxet.cn

[R02] 变量赋值与使用
来源：http://la.gzmigu.cn

name="Tom"; echo "$name"
来源：http://sw.shxzskj.cn

[R03] 只读变量
来源：http://lo.yuexingan06.cn

readonly PI=3.14
来源：http://ut.haigaiapp.cn

[R04] 位置参数
来源：http://up.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bb.9csxet.cn

[R05] 参数默认值
来源：http://of.colortex.cn

name="${1:-default}"
来源：http://qf.9csxet.cn

[R06] 判断命令是否存在
来源：http://nr.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wi.yuexingan06.cn

[R07] if 判断文件
来源：http://ar.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bs.9csxet.cn

[R08] 数值比较
来源：http://vr.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ws.szsharing.cn

[R09] 字符串比较
来源：http://af.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ag.bookmarksfly.cn

[R10] 正则匹配
来源：http://it.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ns.lnxyls.cn

[R11] case 多分支
来源：http://vx.szxytkj.cn

case "$1" in
来源：http://wf.jctech888.com.cn

start) echo "启动" ;;
来源：http://aa.asd995.cn

stop)  echo "停止" ;;
来源：http://co.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://os.asd995.cn

esac
来源：http://zp.huanxung.cn

[R12] for 遍历文件
来源：http://ju.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://gy.jianghongdianzi.cn

[R13] for 计数循环
来源：http://ki.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://cz.shxzukj.cn

[R14] C 风格 for
来源：http://dt.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gn.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://av.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zt.yuntaijiaju.cn

[R16] until 等待条件
来源：http://ax.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://td.nicolike.cn

[R17] 数组定义与取值
来源：http://js.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ao.shxzskj.cn

[R18] 遍历数组
来源：http://ts.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uj.gzmigu.cn

[R19] 数组长度
来源：http://ky.jctech888.com.cn

echo "${#arr[@]}"
来源：http://fi.shxzukj.cn

[R20] 关联数组（字典）
来源：http://cn.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ci.bookmarksfly.cn

[R21] 字符串长度
来源：http://gd.panjiajie.cn

echo "${#s}"
来源：http://zm.lnxyls.cn

[R22] 截取子串
来源：http://qv.haigaiapp.cn

echo "${s:0:5}"
来源：http://yb.bjjhwx.cn

[R23] 字符串替换
来源：http://dr.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qs.nszjky.cn

[R24] 大小写转换
来源：http://ck.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://za.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://jd.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ee.huixiangedu.cn

[R26] 命令替换
来源：http://fc.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://so.hnjuh.cn

[R27] 算术展开
来源：http://uk.colortex.cn

echo $((1 + 2 * 3))
来源：http://eo.shxzskj.cn

[R28] 浮点运算
来源：http://ax.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://qr.newstarts.cn

[R29] 定义函数
来源：http://lf.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ua.hahajie.cn

[R30] 函数返回状态码
来源：http://ud.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://ot.shxzukj.cn

[R31] 局部变量
来源：http://np.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://od.hnjuh.cn

[R32] 参数个数校验
来源：http://ar.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ww.szsharing.cn

[R33] 捕获错误并提示行号
来源：http://es.szxytkj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jo.szsharing.cn

[R34] 退出时清理
来源：http://aw.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://we.szsharing.cn

[R35] 后台执行并等待
来源：http://tc.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://om.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://vq.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://me.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://hp.bjjhwx.cn

files=$(ls -1)
来源：http://yi.bookmarksfly.cn

[R38] 管道串联
来源：http://ms.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://yt.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://xc.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://ac.nszjky.cn

[R40] 追加写日志
来源：http://jz.huanxung.cn

echo "log" >> out.log
来源：http://ab.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://jl.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://no.szxytkj.cn

[R42] 输入重定向
来源：http://ci.bjjhwx.cn

wc -l < a.txt
来源：http://ss.chemitech.net.cn

[R43] 按名字查找文件
来源：http://md.lnxyls.cn

find . -name "*.log" -type f
来源：http://ba.panjiajie.cn

[R44] 按修改时间查找
来源：http://ug.hahajie.cn

find . -mtime -7 -type f
来源：http://fk.nicolike.cn

[R45] 批量删除
来源：http://fg.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://lz.szsharing.cn

[R46] 递归替换文件内容
来源：http://hn.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://os.yuexingan06.cn

[R47] sed 单行替换
来源：http://wa.bookmarksfly.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hu.wgjwhj.cn

[R48] awk 取指定列
来源：http://jk.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://rv.jctech888.com.cn

[R49] awk 带条件
来源：http://bg.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xe.panjiajie.cn

[R50] awk 求和
来源：http://dr.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ke.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ep.chemitech.net.cn


<!-- 参考信息 -->