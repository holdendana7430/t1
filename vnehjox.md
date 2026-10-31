代发 wailian999

PHP:  // 手写时间戳比较
来源：http://sx.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rp.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ul.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fo.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://by.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bg.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ae.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://vm.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nt.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jr.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hd.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rh.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rs.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ck.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fz.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dp.yuexingan06.cn

================================================================================
来源：http://fu.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yu.shxzskj.cn

================================================================================
来源：http://el.jianghongdianzi.cn

[Q01] 创建表
来源：http://vq.521024.cn

CREATE TABLE users (
来源：http://ly.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xx.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://ay.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://zq.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xs.huanxung.cn

);
来源：http://sr.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://yj.wgjwhj.cn

CREATE TABLE orders (
来源：http://it.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dl.yuexingan06.cn

user_id INT NOT NULL,
来源：http://ic.asd995.cn

amount DECIMAL(10, 2),
来源：http://ve.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bq.jctech888.com.cn

);
来源：http://sr.huixiangedu.cn

[Q03] 增加列
来源：http://ks.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gv.shtwfgs.cn

[Q04] 修改列类型
来源：http://bd.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rp.shxzukj.cn

[Q05] 重命名列
来源：http://na.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jo.521024.cn

[Q06] 删除列
来源：http://tz.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://in.yuexingan06.cn

[Q07] 删除表
来源：http://pt.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://ww.nszjky.cn

[Q08] 创建普通索引
来源：http://gz.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nz.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://bb.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hx.asd995.cn

[Q10] 插入单行
来源：http://iv.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ev.chemitech.net.cn

[Q11] 一次插入多行
来源：http://bw.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fp.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://io.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ce.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dx.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://vf.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rw.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://tn.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ud.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dz.hahajie.cn

[Q15] 查询全部
来源：http://mm.szsharing.cn

SELECT * FROM users;
来源：http://vo.lnxyls.cn

[Q16] 查询指定列
来源：http://ol.9csxet.cn

SELECT id, name FROM users;
来源：http://wq.yuexingan06.cn

[Q17] 条件查询
来源：http://qx.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lm.wgjwhj.cn

[Q18] 模糊匹配
来源：http://ms.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pl.shtwfgs.cn

[Q19] 范围查询
来源：http://ut.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xp.bookmarksfly.cn

[Q20] IN 列表
来源：http://zb.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ig.chemitech.net.cn

[Q21] 空值判断
来源：http://op.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ua.shxzskj.cn

[Q22] 排序
来源：http://ga.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ct.bjjhwx.cn

[Q23] 分页
来源：http://pu.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lr.bjjhwx.cn

[Q24] 去重
来源：http://ia.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://wc.colortex.cn

[Q25] 只取前 N 条
来源：http://zm.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bf.jctech888.com.cn

[Q26] 计数
来源：http://au.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://mc.muxihuayi.cn

[Q27] 条件计数
来源：http://zd.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vr.wgjwhj.cn

[Q28] 求和与平均
来源：http://st.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nj.wgjwhj.cn

[Q29] 最大最小值
来源：http://fj.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://be.hahajie.cn

[Q30] 分组统计
来源：http://iy.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sx.jctech888.com.cn

[Q31] 分组后过滤
来源：http://po.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fo.szsharing.cn

[Q32] 分组拼接字符串
来源：http://es.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ed.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kl.haigaiapp.cn

[Q33] 多列分组
来源：http://ba.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dv.newstarts.cn

[Q34] 每组取第一条
来源：http://do.lnxyls.cn

SELECT * FROM (
来源：http://ru.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nd.szxytkj.cn

) t WHERE rn = 1;
来源：http://sl.haigaiapp.cn

[Q35] 内连接
来源：http://he.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vj.hahajie.cn

[Q36] 左连接
来源：http://xb.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lm.yuntaijiaju.cn

[Q37] 右连接
来源：http://zu.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ar.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pq.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zc.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://fk.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vm.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ke.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dx.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pa.hnjuh.cn

[Q41] 多表连接
来源：http://wf.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://it.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://eb.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://hh.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://ky.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://ct.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nr.newstarts.cn

[Q43] 标量子查询
来源：http://tz.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rc.bookmarksfly.cn

[Q44] IN 子查询
来源：http://ay.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rp.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://rp.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://be.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pr.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ck.shxzukj.cn

[Q47] 与平均值比较
来源：http://fv.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xf.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://kr.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bi.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://qc.muxihuayi.cn

[Q49] 更新单行
来源：http://ag.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gl.lnxyls.cn

[Q50] 批量更新
来源：http://dc.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ay.yuexingan06.cn

[Q51] 用子查询更新
来源：http://oy.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uy.haigaiapp.cn

[Q52] 删除指定行
来源：http://ab.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://ng.gzmigu.cn

[Q53] 按条件删除
来源：http://qk.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sf.huixiangedu.cn

[Q54] 清空表
来源：http://hi.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://fz.lnxyls.cn

[Q55] 排名（并列占位）
来源：http://mi.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://la.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://dr.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yl.haigaiapp.cn

[Q57] 行号
来源：http://pq.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nq.bookmarksfly.cn

[Q58] 累计求和
来源：http://xc.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cx.huanxung.cn

[Q59] 分组内累计
来源：http://om.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yb.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://ib.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wa.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vz.gzmigu.cn

[Q61] 移动平均
来源：http://or.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ih.shxzukj.cn

[Q62] 分组占比
来源：http://fh.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sb.gzmigu.cn

[Q63] 开启事务
来源：http://wq.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wi.szsharing.cn

[Q64] 提交事务
来源：http://ov.gzmigu.cn

COMMIT;
来源：http://nd.asd995.cn

[Q65] 回滚事务
来源：http://kv.jianghongdianzi.cn

ROLLBACK;
来源：http://wt.szsharing.cn

[Q66] 行锁查询
来源：http://yh.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ye.hahajie.cn

[Q67] 设置隔离级别
来源：http://cw.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ur.shxzukj.cn

[Q68] 保存点
来源：http://me.nszjky.cn

SAVEPOINT sp1;
来源：http://bw.newstarts.cn

ROLLBACK TO sp1;
来源：http://il.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://mt.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vk.hnjuh.cn

[Q70] 更新统计信息
来源：http://zl.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://bq.colortex.cn

[Q71] 查看建表语句
来源：http://bh.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hb.haigaiapp.cn

[Q72] 查看索引
来源：http://mq.newstarts.cn

SHOW INDEX FROM users;
来源：http://vc.haigaiapp.cn

[Q73] 查看表状态
来源：http://rl.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ng.muxihuayi.cn

[Q74] 强制使用索引
来源：http://bs.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kg.9csxet.cn

[Q75] 日期格式化
来源：http://au.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wx.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kt.huanxung.cn

[Q76] 按天统计
来源：http://qg.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ps.newstarts.cn

[Q77] 时间加减
来源：http://rn.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lm.jctech888.com.cn

[Q78] 当前时间
来源：http://yt.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qr.gzmigu.cn

[Q79] 字符串拼接
来源：http://zi.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yq.wgjwhj.cn

[Q80] 字符串截取
来源：http://pq.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wc.shxzukj.cn

[Q81] 字符串替换
来源：http://tm.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wr.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://dp.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://we.bookmarksfly.cn

[Q83] 大小写转换
来源：http://mo.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fx.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://tj.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://yw.panjiajie.cn

[Q85] 数值取整
来源：http://km.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kw.asd995.cn

[Q86] 读取 JSON 字段
来源：http://vx.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cd.huanxung.cn

[Q87] JSON 字段做条件
来源：http://qu.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mi.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://gp.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lg.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xo.szsharing.cn

[Q89] 判断表是否存在
来源：http://fd.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zn.szxytkj.cn

[Q90] 生成序号列
来源：http://ka.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bj.hahajie.cn

================================================================================
来源：http://wy.jianghongdianzi.cn

R. Bash 专题
来源：http://zc.gzmigu.cn

================================================================================
来源：http://yi.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://yn.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://cp.jianghongdianzi.cn

set -euo pipefail
来源：http://ul.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://pa.newstarts.cn

name="Tom"; echo "$name"
来源：http://je.panjiajie.cn

[R03] 只读变量
来源：http://sb.521024.cn

readonly PI=3.14
来源：http://gz.jianghongdianzi.cn

[R04] 位置参数
来源：http://js.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://es.bjjhwx.cn

[R05] 参数默认值
来源：http://ww.shtwfgs.cn

name="${1:-default}"
来源：http://go.nszjky.cn

[R06] 判断命令是否存在
来源：http://ot.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qw.bookmarksfly.cn

[R07] if 判断文件
来源：http://gx.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sp.shxzskj.cn

[R08] 数值比较
来源：http://qm.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wl.bjjhwx.cn

[R09] 字符串比较
来源：http://by.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ze.haigaiapp.cn

[R10] 正则匹配
来源：http://wt.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mg.shxzskj.cn

[R11] case 多分支
来源：http://iq.colortex.cn

case "$1" in
来源：http://aw.huixiangedu.cn

start) echo "启动" ;;
来源：http://rk.newstarts.cn

stop)  echo "停止" ;;
来源：http://jj.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://ne.haigaiapp.cn

esac
来源：http://my.newstarts.cn

[R12] for 遍历文件
来源：http://tm.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://qp.nicolike.cn

[R13] for 计数循环
来源：http://la.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://ia.huixiangedu.cn

[R14] C 风格 for
来源：http://mj.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ag.hnjuh.cn

[R15] while 逐行读文件
来源：http://lc.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ia.asd995.cn

[R16] until 等待条件
来源：http://dl.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://no.shxzskj.cn

[R17] 数组定义与取值
来源：http://pl.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ub.gzmigu.cn

[R18] 遍历数组
来源：http://er.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ua.9csxet.cn

[R19] 数组长度
来源：http://mq.hnjuh.cn

echo "${#arr[@]}"
来源：http://kb.huanxung.cn

[R20] 关联数组（字典）
来源：http://sy.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ew.shxzukj.cn

[R21] 字符串长度
来源：http://eu.9csxet.cn

echo "${#s}"
来源：http://uy.shxzukj.cn

[R22] 截取子串
来源：http://vm.wgjwhj.cn

echo "${s:0:5}"
来源：http://jn.haigaiapp.cn

[R23] 字符串替换
来源：http://es.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://to.9csxet.cn

[R24] 大小写转换
来源：http://jh.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ji.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://pc.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://so.gzmigu.cn

[R26] 命令替换
来源：http://ay.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://kf.panjiajie.cn

[R27] 算术展开
来源：http://uj.nszjky.cn

echo $((1 + 2 * 3))
来源：http://ru.szxytkj.cn

[R28] 浮点运算
来源：http://ca.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://is.huixinmuqiang.cn

[R29] 定义函数
来源：http://na.jctech888.com.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bs.hahajie.cn

[R30] 函数返回状态码
来源：http://iv.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://xw.521024.cn

[R31] 局部变量
来源：http://qd.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://fh.huixiangedu.cn

[R32] 参数个数校验
来源：http://qp.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zn.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://se.nszjky.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mv.shtwfgs.cn

[R34] 退出时清理
来源：http://wh.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yw.nicolike.cn

[R35] 后台执行并等待
来源：http://kw.huanxung.cn


<!-- 参考信息 -->