代发 wailian999

);
来源：http://yn.newstarts.cn

[Q03] 增加列
来源：http://dh.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kk.yuexingan06.cn

[Q04] 修改列类型
来源：http://rd.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sv.jianghongdianzi.cn

[Q05] 重命名列
来源：http://id.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dk.colortex.cn

[Q06] 删除列
来源：http://rc.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sm.muxihuayi.cn

[Q07] 删除表
来源：http://le.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://qa.haigaiapp.cn

[Q08] 创建普通索引
来源：http://gh.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xw.521024.cn

[Q09] 创建唯一索引
来源：http://tz.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qm.shxzskj.cn

[Q10] 插入单行
来源：http://kt.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ey.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://xm.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pw.colortex.cn

[Q12] 插入后取自增 ID
来源：http://ot.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yi.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qa.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://rf.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ij.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://xg.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hm.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jt.jianghongdianzi.cn

[Q15] 查询全部
来源：http://gq.shxzukj.cn

SELECT * FROM users;
来源：http://yz.huanxung.cn

[Q16] 查询指定列
来源：http://ic.asd995.cn

SELECT id, name FROM users;
来源：http://pl.shtwfgs.cn

[Q17] 条件查询
来源：http://jo.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://em.haigaiapp.cn

[Q18] 模糊匹配
来源：http://jr.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ag.huixinmuqiang.cn

[Q19] 范围查询
来源：http://my.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lc.newstarts.cn

[Q20] IN 列表
来源：http://aj.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ko.haigaiapp.cn

[Q21] 空值判断
来源：http://os.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tw.shtwfgs.cn

[Q22] 排序
来源：http://nz.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bz.colortex.cn

[Q23] 分页
来源：http://vw.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mg.panjiajie.cn

[Q24] 去重
来源：http://uu.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://mj.szsharing.cn

[Q25] 只取前 N 条
来源：http://bx.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fq.szxytkj.cn

[Q26] 计数
来源：http://mf.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://yy.9csxet.cn

[Q27] 条件计数
来源：http://gw.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://po.wgjwhj.cn

[Q28] 求和与平均
来源：http://qr.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eq.nicolike.cn

[Q29] 最大最小值
来源：http://gc.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hk.jctech888.com.cn

[Q30] 分组统计
来源：http://gb.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lf.colortex.cn

[Q31] 分组后过滤
来源：http://ql.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lw.szsharing.cn

[Q32] 分组拼接字符串
来源：http://aw.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oe.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uz.gzmigu.cn

[Q33] 多列分组
来源：http://zc.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uq.521024.cn

[Q34] 每组取第一条
来源：http://ov.haigaiapp.cn

SELECT * FROM (
来源：http://kx.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tu.nszjky.cn

) t WHERE rn = 1;
来源：http://gf.newstarts.cn

[Q35] 内连接
来源：http://gm.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pp.szxytkj.cn

[Q36] 左连接
来源：http://ml.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kg.hahajie.cn

[Q37] 右连接
来源：http://oh.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wz.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rh.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jo.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://wh.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lq.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zi.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vu.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://to.gzmigu.cn

[Q41] 多表连接
来源：http://ev.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nb.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://rk.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://bg.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://jr.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://qv.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ir.newstarts.cn

[Q43] 标量子查询
来源：http://ca.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xg.colortex.cn

[Q44] IN 子查询
来源：http://lu.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ui.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://lq.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zg.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pj.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://um.gzmigu.cn

[Q47] 与平均值比较
来源：http://ed.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ds.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://jq.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rw.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://co.hnjuh.cn

[Q49] 更新单行
来源：http://oe.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nz.shxzskj.cn

[Q50] 批量更新
来源：http://ff.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fn.chemitech.net.cn

[Q51] 用子查询更新
来源：http://uk.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xn.newstarts.cn

[Q52] 删除指定行
来源：http://zr.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://ml.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://ra.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wk.shtwfgs.cn

[Q54] 清空表
来源：http://be.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://gp.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://rr.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uq.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://qm.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oi.521024.cn

[Q57] 行号
来源：http://tg.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mm.shxzukj.cn

[Q58] 累计求和
来源：http://pb.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zy.nicolike.cn

[Q59] 分组内累计
来源：http://gi.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ug.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://bq.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ss.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xk.shxzskj.cn

[Q61] 移动平均
来源：http://lr.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://to.panjiajie.cn

[Q62] 分组占比
来源：http://vl.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wo.huixinmuqiang.cn

[Q63] 开启事务
来源：http://ac.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ft.colortex.cn

[Q64] 提交事务
来源：http://pf.haigaiapp.cn

COMMIT;
来源：http://it.9csxet.cn

[Q65] 回滚事务
来源：http://pv.9csxet.cn

ROLLBACK;
来源：http://wk.gzmigu.cn

[Q66] 行锁查询
来源：http://cx.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nu.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://ix.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rx.lnxyls.cn

[Q68] 保存点
来源：http://jq.jctech888.com.cn

SAVEPOINT sp1;
来源：http://vd.newstarts.cn

ROLLBACK TO sp1;
来源：http://ms.panjiajie.cn

[Q69] 查看执行计划
来源：http://qz.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ln.huixiangedu.cn

[Q70] 更新统计信息
来源：http://zv.asd995.cn

ANALYZE TABLE users;
来源：http://tz.asd995.cn

[Q71] 查看建表语句
来源：http://as.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tr.huanxung.cn

[Q72] 查看索引
来源：http://jk.szxytkj.cn

SHOW INDEX FROM users;
来源：http://ye.521024.cn

[Q73] 查看表状态
来源：http://tb.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ww.lnxyls.cn

[Q74] 强制使用索引
来源：http://vs.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ru.szxytkj.cn

[Q75] 日期格式化
来源：http://nr.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cz.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uf.9csxet.cn

[Q76] 按天统计
来源：http://rv.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://au.szsharing.cn

[Q77] 时间加减
来源：http://tt.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ha.asd995.cn

[Q78] 当前时间
来源：http://bj.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://de.chemitech.net.cn

[Q79] 字符串拼接
来源：http://bs.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jx.chemitech.net.cn

[Q80] 字符串截取
来源：http://dp.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ir.chemitech.net.cn

[Q81] 字符串替换
来源：http://un.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ow.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://zl.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uy.szxytkj.cn

[Q83] 大小写转换
来源：http://hi.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://li.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://xz.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://de.huixinmuqiang.cn

[Q85] 数值取整
来源：http://tw.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jk.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://cp.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pq.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://lf.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rs.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://dw.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://np.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eo.szxytkj.cn

[Q89] 判断表是否存在
来源：http://po.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nh.shtwfgs.cn

[Q90] 生成序号列
来源：http://ua.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qp.huixinmuqiang.cn

================================================================================
来源：http://xp.yuexingan06.cn

R. Bash 专题
来源：http://iz.521024.cn

================================================================================
来源：http://ei.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://mn.szsharing.cn

#!/usr/bin/env bash
来源：http://ii.shxzukj.cn

set -euo pipefail
来源：http://gf.shxzskj.cn

[R02] 变量赋值与使用
来源：http://yc.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://tp.nicolike.cn

[R03] 只读变量
来源：http://kw.huanxung.cn

readonly PI=3.14
来源：http://cx.hahajie.cn

[R04] 位置参数
来源：http://sa.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pd.asd995.cn

[R05] 参数默认值
来源：http://nh.newstarts.cn

name="${1:-default}"
来源：http://ii.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://dq.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ww.lnxyls.cn

[R07] if 判断文件
来源：http://sv.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://id.muxihuayi.cn

[R08] 数值比较
来源：http://pb.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bw.nicolike.cn

[R09] 字符串比较
来源：http://xs.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ic.asd995.cn

[R10] 正则匹配
来源：http://dh.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lv.yuexingan06.cn

[R11] case 多分支
来源：http://wv.asd995.cn

case "$1" in
来源：http://dn.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://ga.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://cg.asd995.cn

*)     echo "未知命令" ;;
来源：http://so.lnxyls.cn

esac
来源：http://zy.haigaiapp.cn

[R12] for 遍历文件
来源：http://hp.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://kp.jianghongdianzi.cn

[R13] for 计数循环
来源：http://bw.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://vh.9csxet.cn

[R14] C 风格 for
来源：http://mq.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wp.haigaiapp.cn

[R15] while 逐行读文件
来源：http://pb.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eb.asd995.cn

[R16] until 等待条件
来源：http://gk.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jy.shtwfgs.cn

[R17] 数组定义与取值
来源：http://ej.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ud.chemitech.net.cn

[R18] 遍历数组
来源：http://dx.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wb.panjiajie.cn

[R19] 数组长度
来源：http://cz.newstarts.cn

echo "${#arr[@]}"
来源：http://zx.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://cc.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uo.hnjuh.cn

[R21] 字符串长度
来源：http://ze.lnxyls.cn

echo "${#s}"
来源：http://or.shxzukj.cn

[R22] 截取子串
来源：http://ah.jctech888.com.cn

echo "${s:0:5}"
来源：http://vd.haigaiapp.cn

[R23] 字符串替换
来源：http://zv.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cr.nicolike.cn

[R24] 大小写转换
来源：http://xv.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nl.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://dp.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://de.wgjwhj.cn

[R26] 命令替换
来源：http://cg.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://df.hnjuh.cn

[R27] 算术展开
来源：http://tm.yuexingan06.cn

echo $((1 + 2 * 3))
来源：http://pu.jianghongdianzi.cn

[R28] 浮点运算
来源：http://qi.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://ta.nicolike.cn

[R29] 定义函数
来源：http://rv.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fo.nszjky.cn

[R30] 函数返回状态码
来源：http://eq.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://cc.gzmigu.cn

[R31] 局部变量
来源：http://gk.bjjhwx.cn

f() { local x=1; echo "$x"; }
来源：http://kl.huixiangedu.cn

[R32] 参数个数校验
来源：http://rq.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hy.colortex.cn

[R33] 捕获错误并提示行号
来源：http://xa.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ol.panjiajie.cn

[R34] 退出时清理
来源：http://jc.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sz.hahajie.cn

[R35] 后台执行并等待
来源：http://ks.asd995.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://os.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://xc.newstarts.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://he.asd995.cn

[R37] 把输出赋给变量
来源：http://yt.bjjhwx.cn

files=$(ls -1)
来源：http://ra.lnxyls.cn

[R38] 管道串联
来源：http://rb.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://wz.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://ln.yuntaijiaju.cn

cmd > out.log 2>&1
来源：http://mf.chemitech.net.cn

[R40] 追加写日志
来源：http://sp.colortex.cn

echo "log" >> out.log
来源：http://la.muxihuayi.cn

[R41] 丢弃输出
来源：http://zf.hahajie.cn

cmd >/dev/null 2>&1
来源：http://ri.9csxet.cn

[R42] 输入重定向
来源：http://xs.asd995.cn

wc -l < a.txt
来源：http://ra.muxihuayi.cn

[R43] 按名字查找文件
来源：http://os.nszjky.cn

find . -name "*.log" -type f
来源：http://xl.521024.cn

[R44] 按修改时间查找
来源：http://se.lnxyls.cn

find . -mtime -7 -type f
来源：http://mq.lnxyls.cn

[R45] 批量删除
来源：http://kt.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://tm.yuexingan06.cn

[R46] 递归替换文件内容
来源：http://nn.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sy.asd995.cn

[R47] sed 单行替换
来源：http://ce.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ds.521024.cn

[R48] awk 取指定列
来源：http://wz.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://jg.asd995.cn

[R49] awk 带条件
来源：http://db.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ll.huanxung.cn

[R50] awk 求和
来源：http://kn.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sj.haigaiapp.cn

[R51] 排序去重取前几
来源：http://ns.haigaiapp.cn


<!-- 参考信息 -->