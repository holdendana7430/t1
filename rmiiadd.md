代发 wailian999

PHP:  // 手写时间戳比较
来源：http://bt.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ns.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ov.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uy.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ch.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ur.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rr.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://qj.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kv.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wf.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cu.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hp.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://um.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ji.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oi.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zg.bookmarksfly.cn

================================================================================
来源：http://mq.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fq.lnxyls.cn

================================================================================
来源：http://pu.huixiangedu.cn

[Q01] 创建表
来源：http://ud.nicolike.cn

CREATE TABLE users (
来源：http://rz.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gq.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://gs.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://xh.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bo.shxzskj.cn

);
来源：http://vn.hnjuh.cn

[Q02] 创建带外键的表
来源：http://mc.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://ai.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ar.huanxung.cn

user_id INT NOT NULL,
来源：http://yx.huanxung.cn

amount DECIMAL(10, 2),
来源：http://wg.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uw.asd995.cn

);
来源：http://rp.bookmarksfly.cn

[Q03] 增加列
来源：http://yk.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://na.colortex.cn

[Q04] 修改列类型
来源：http://sr.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ue.nicolike.cn

[Q05] 重命名列
来源：http://av.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xf.bookmarksfly.cn

[Q06] 删除列
来源：http://uz.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tp.nszjky.cn

[Q07] 删除表
来源：http://yw.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://zf.newstarts.cn

[Q08] 创建普通索引
来源：http://kb.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oc.szxytkj.cn

[Q09] 创建唯一索引
来源：http://pd.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qq.shxzukj.cn

[Q10] 插入单行
来源：http://dk.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hm.muxihuayi.cn

[Q11] 一次插入多行
来源：http://cy.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ca.asd995.cn

[Q12] 插入后取自增 ID
来源：http://ja.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ug.nszjky.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://im.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://vm.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fk.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://em.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zv.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sa.521024.cn

[Q15] 查询全部
来源：http://yr.9csxet.cn

SELECT * FROM users;
来源：http://zq.chemitech.net.cn

[Q16] 查询指定列
来源：http://xt.hnjuh.cn

SELECT id, name FROM users;
来源：http://gq.nicolike.cn

[Q17] 条件查询
来源：http://zl.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://at.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://bj.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pc.huanxung.cn

[Q19] 范围查询
来源：http://dt.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dv.yuntaijiaju.cn

[Q20] IN 列表
来源：http://gi.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cf.jctech888.com.cn

[Q21] 空值判断
来源：http://mw.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ox.huixiangedu.cn

[Q22] 排序
来源：http://dh.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hx.521024.cn

[Q23] 分页
来源：http://hu.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sc.bookmarksfly.cn

[Q24] 去重
来源：http://fv.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ho.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://nr.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://su.panjiajie.cn

[Q26] 计数
来源：http://pb.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://pe.jctech888.com.cn

[Q27] 条件计数
来源：http://ht.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hj.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://nf.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tk.shxzskj.cn

[Q29] 最大最小值
来源：http://ky.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bq.9csxet.cn

[Q30] 分组统计
来源：http://nx.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qo.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://hq.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mv.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://xu.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rt.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xt.szxytkj.cn

[Q33] 多列分组
来源：http://he.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ej.chemitech.net.cn

[Q34] 每组取第一条
来源：http://bw.szsharing.cn

SELECT * FROM (
来源：http://hv.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wd.shtwfgs.cn

) t WHERE rn = 1;
来源：http://nd.nszjky.cn

[Q35] 内连接
来源：http://iq.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ss.9csxet.cn

[Q36] 左连接
来源：http://tw.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mr.asd995.cn

[Q37] 右连接
来源：http://qb.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ct.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lz.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jg.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ld.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cb.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wb.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xp.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://by.newstarts.cn

[Q41] 多表连接
来源：http://oo.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://km.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://kp.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ik.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://wk.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://zv.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eu.shxzskj.cn

[Q43] 标量子查询
来源：http://oj.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wr.lnxyls.cn

[Q44] IN 子查询
来源：http://gf.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sj.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://lj.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nl.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ms.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xz.muxihuayi.cn

[Q47] 与平均值比较
来源：http://nx.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rp.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://jl.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ew.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://tv.newstarts.cn

[Q49] 更新单行
来源：http://ka.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://om.hahajie.cn

[Q50] 批量更新
来源：http://nb.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hw.chemitech.net.cn

[Q51] 用子查询更新
来源：http://iy.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ao.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://wo.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://pt.yuexingan06.cn

[Q53] 按条件删除
来源：http://nj.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rb.bjjhwx.cn

[Q54] 清空表
来源：http://bd.nicolike.cn

TRUNCATE TABLE logs;
来源：http://mu.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://to.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xw.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://qv.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fm.yuntaijiaju.cn

[Q57] 行号
来源：http://tz.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ln.huixiangedu.cn

[Q58] 累计求和
来源：http://xk.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kh.nszjky.cn

[Q59] 分组内累计
来源：http://qp.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kf.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://dv.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jr.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ub.newstarts.cn

[Q61] 移动平均
来源：http://de.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iv.szxytkj.cn

[Q62] 分组占比
来源：http://fr.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gx.hnjuh.cn

[Q63] 开启事务
来源：http://ah.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://id.chemitech.net.cn

[Q64] 提交事务
来源：http://mq.bjjhwx.cn

COMMIT;
来源：http://hq.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://xx.asd995.cn

ROLLBACK;
来源：http://wx.chemitech.net.cn

[Q66] 行锁查询
来源：http://vm.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tc.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://yl.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wq.yuexingan06.cn

[Q68] 保存点
来源：http://tl.521024.cn

SAVEPOINT sp1;
来源：http://dy.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://im.nicolike.cn

[Q69] 查看执行计划
来源：http://am.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zy.lnxyls.cn

[Q70] 更新统计信息
来源：http://hp.lnxyls.cn

ANALYZE TABLE users;
来源：http://fv.huanxung.cn

[Q71] 查看建表语句
来源：http://fg.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bh.hnjuh.cn

[Q72] 查看索引
来源：http://xp.shxzskj.cn

SHOW INDEX FROM users;
来源：http://jo.newstarts.cn

[Q73] 查看表状态
来源：http://kd.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wu.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://pg.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xk.huixiangedu.cn

[Q75] 日期格式化
来源：http://ha.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vh.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sm.nicolike.cn

[Q76] 按天统计
来源：http://kf.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rc.gzmigu.cn

[Q77] 时间加减
来源：http://eu.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ju.hnjuh.cn

[Q78] 当前时间
来源：http://lc.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gl.lnxyls.cn

[Q79] 字符串拼接
来源：http://qv.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://be.asd995.cn

[Q80] 字符串截取
来源：http://ow.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ev.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://je.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zc.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://ge.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pj.newstarts.cn

[Q83] 大小写转换
来源：http://mu.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zb.nszjky.cn

[Q84] 去除首尾空格
来源：http://dy.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://om.nicolike.cn

[Q85] 数值取整
来源：http://ji.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jk.521024.cn

[Q86] 读取 JSON 字段
来源：http://gq.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kq.521024.cn

[Q87] JSON 字段做条件
来源：http://nb.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wt.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://aa.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rh.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rl.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://ld.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cs.wgjwhj.cn

[Q90] 生成序号列
来源：http://pv.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yy.lnxyls.cn

================================================================================
来源：http://xh.asd995.cn

R. Bash 专题
来源：http://vy.newstarts.cn

================================================================================
来源：http://kd.gzmigu.cn

[R01] shebang 与严格模式
来源：http://ak.panjiajie.cn

#!/usr/bin/env bash
来源：http://kt.hahajie.cn

set -euo pipefail
来源：http://jr.huanxung.cn

[R02] 变量赋值与使用
来源：http://jm.asd995.cn

name="Tom"; echo "$name"
来源：http://rr.yuntaijiaju.cn

[R03] 只读变量
来源：http://li.hnjuh.cn

readonly PI=3.14
来源：http://xq.yuntaijiaju.cn

[R04] 位置参数
来源：http://yj.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kv.panjiajie.cn

[R05] 参数默认值
来源：http://uc.nszjky.cn

name="${1:-default}"
来源：http://bp.521024.cn

[R06] 判断命令是否存在
来源：http://dl.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eq.chemitech.net.cn

[R07] if 判断文件
来源：http://zm.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rs.nicolike.cn

[R08] 数值比较
来源：http://gj.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xl.bookmarksfly.cn

[R09] 字符串比较
来源：http://ui.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wr.asd995.cn

[R10] 正则匹配
来源：http://xu.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://er.asd995.cn

[R11] case 多分支
来源：http://kh.lnxyls.cn

case "$1" in
来源：http://kp.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://ch.asd995.cn

stop)  echo "停止" ;;
来源：http://rd.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://bf.jianghongdianzi.cn

esac
来源：http://yt.shxzukj.cn

[R12] for 遍历文件
来源：http://as.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://gb.lnxyls.cn

[R13] for 计数循环
来源：http://gf.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://cq.szxytkj.cn

[R14] C 风格 for
来源：http://ni.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ls.shxzukj.cn

[R15] while 逐行读文件
来源：http://lc.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nj.haigaiapp.cn

[R16] until 等待条件
来源：http://lg.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nr.huixiangedu.cn

[R17] 数组定义与取值
来源：http://sr.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://la.9csxet.cn

[R18] 遍历数组
来源：http://oc.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://la.gzmigu.cn

[R19] 数组长度
来源：http://yr.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://ys.lnxyls.cn

[R20] 关联数组（字典）
来源：http://rl.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dc.panjiajie.cn

[R21] 字符串长度
来源：http://gq.haigaiapp.cn

echo "${#s}"
来源：http://ha.hnjuh.cn

[R22] 截取子串
来源：http://xb.wgjwhj.cn

echo "${s:0:5}"
来源：http://ec.huixiangedu.cn

[R23] 字符串替换
来源：http://bu.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lu.yuntaijiaju.cn

[R24] 大小写转换
来源：http://px.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fa.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://ri.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bu.hahajie.cn

[R26] 命令替换
来源：http://zc.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://vv.gzmigu.cn

[R27] 算术展开
来源：http://yp.9csxet.cn

echo $((1 + 2 * 3))
来源：http://uz.chemitech.net.cn

[R28] 浮点运算
来源：http://uj.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://pt.hahajie.cn

[R29] 定义函数
来源：http://sl.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wc.huixiangedu.cn

[R30] 函数返回状态码
来源：http://vs.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://hx.huixinmuqiang.cn

[R31] 局部变量
来源：http://eu.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://ca.gzmigu.cn

[R32] 参数个数校验
来源：http://oq.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jq.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://ad.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xi.bookmarksfly.cn

[R34] 退出时清理
来源：http://xj.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hi.newstarts.cn

[R35] 后台执行并等待
来源：http://ge.nicolike.cn


<!-- 参考信息 -->