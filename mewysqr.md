代发 wailian999

PHP:  // 手写时间戳比较
来源：http://te.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oh.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fc.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ri.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vs.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ks.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dr.huanxung.cn

[P08] 处理浮点精度问题
来源：http://ii.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jl.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://im.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://un.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ty.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ne.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ws.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jn.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qi.nszjky.cn

================================================================================
来源：http://us.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rx.chemitech.net.cn

================================================================================
来源：http://pv.yuntaijiaju.cn

[Q01] 创建表
来源：http://lw.chemitech.net.cn

CREATE TABLE users (
来源：http://qx.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jd.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://lz.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://fq.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bx.hnjuh.cn

);
来源：http://aj.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://yl.muxihuayi.cn

CREATE TABLE orders (
来源：http://mr.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fy.nicolike.cn

user_id INT NOT NULL,
来源：http://dy.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://rb.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yi.szxytkj.cn

);
来源：http://ek.yuexingan06.cn

[Q03] 增加列
来源：http://zi.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mc.szxytkj.cn

[Q04] 修改列类型
来源：http://oy.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zd.nicolike.cn

[Q05] 重命名列
来源：http://pf.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xk.muxihuayi.cn

[Q06] 删除列
来源：http://gr.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ah.szsharing.cn

[Q07] 删除表
来源：http://wx.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://es.colortex.cn

[Q08] 创建普通索引
来源：http://ii.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ce.colortex.cn

[Q09] 创建唯一索引
来源：http://ru.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yj.nszjky.cn

[Q10] 插入单行
来源：http://fn.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ua.muxihuayi.cn

[Q11] 一次插入多行
来源：http://pg.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zc.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://al.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://il.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gv.newstarts.cn

[Q13] 忽略重复插入
来源：http://wr.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ip.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://rj.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gp.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://du.yuntaijiaju.cn

[Q15] 查询全部
来源：http://hu.huixiangedu.cn

SELECT * FROM users;
来源：http://kb.bookmarksfly.cn

[Q16] 查询指定列
来源：http://zg.panjiajie.cn

SELECT id, name FROM users;
来源：http://yf.asd995.cn

[Q17] 条件查询
来源：http://fx.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hx.huixiangedu.cn

[Q18] 模糊匹配
来源：http://xr.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rw.hahajie.cn

[Q19] 范围查询
来源：http://mz.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ue.yuexingan06.cn

[Q20] IN 列表
来源：http://rd.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ew.gzmigu.cn

[Q21] 空值判断
来源：http://zz.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vd.521024.cn

[Q22] 排序
来源：http://cb.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hb.jianghongdianzi.cn

[Q23] 分页
来源：http://pl.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jl.huixinmuqiang.cn

[Q24] 去重
来源：http://hh.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://ku.szsharing.cn

[Q25] 只取前 N 条
来源：http://ck.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fd.9csxet.cn

[Q26] 计数
来源：http://ii.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://dn.shxzskj.cn

[Q27] 条件计数
来源：http://lk.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fn.gzmigu.cn

[Q28] 求和与平均
来源：http://ju.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wc.hnjuh.cn

[Q29] 最大最小值
来源：http://fc.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ar.yuexingan06.cn

[Q30] 分组统计
来源：http://ps.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rs.nszjky.cn

[Q31] 分组后过滤
来源：http://fh.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xh.colortex.cn

[Q32] 分组拼接字符串
来源：http://xv.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ke.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jm.hahajie.cn

[Q33] 多列分组
来源：http://lw.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pz.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://cr.hahajie.cn

SELECT * FROM (
来源：http://ks.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yj.hnjuh.cn

) t WHERE rn = 1;
来源：http://ek.chemitech.net.cn

[Q35] 内连接
来源：http://yl.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cx.nszjky.cn

[Q36] 左连接
来源：http://ih.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zc.newstarts.cn

[Q37] 右连接
来源：http://fi.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pr.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://or.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hg.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://la.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ih.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wf.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hq.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xo.hahajie.cn

[Q41] 多表连接
来源：http://lg.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ro.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://js.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://xp.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ic.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://tx.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mj.521024.cn

[Q43] 标量子查询
来源：http://cy.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xa.shxzukj.cn

[Q44] IN 子查询
来源：http://kn.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ox.asd995.cn

[Q45] EXISTS 判断存在
来源：http://xz.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uc.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qt.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mm.panjiajie.cn

[Q47] 与平均值比较
来源：http://eb.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ik.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://cj.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uc.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://vp.shxzukj.cn

[Q49] 更新单行
来源：http://vh.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gw.huixinmuqiang.cn

[Q50] 批量更新
来源：http://mr.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dj.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://yj.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cy.szsharing.cn

[Q52] 删除指定行
来源：http://oh.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://ew.szxytkj.cn

[Q53] 按条件删除
来源：http://nd.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gh.gzmigu.cn

[Q54] 清空表
来源：http://ni.colortex.cn

TRUNCATE TABLE logs;
来源：http://us.colortex.cn

[Q55] 排名（并列占位）
来源：http://et.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://as.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://ju.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yh.haigaiapp.cn

[Q57] 行号
来源：http://ly.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cs.yuntaijiaju.cn

[Q58] 累计求和
来源：http://zs.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lj.colortex.cn

[Q59] 分组内累计
来源：http://gf.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ze.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://tm.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ti.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jt.shtwfgs.cn

[Q61] 移动平均
来源：http://jo.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://na.jianghongdianzi.cn

[Q62] 分组占比
来源：http://zs.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fu.huixiangedu.cn

[Q63] 开启事务
来源：http://rq.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jj.shxzukj.cn

[Q64] 提交事务
来源：http://fd.jctech888.com.cn

COMMIT;
来源：http://qs.521024.cn

[Q65] 回滚事务
来源：http://fp.huixiangedu.cn

ROLLBACK;
来源：http://wj.bjjhwx.cn

[Q66] 行锁查询
来源：http://iv.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bp.newstarts.cn

[Q67] 设置隔离级别
来源：http://am.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yu.521024.cn

[Q68] 保存点
来源：http://bl.chemitech.net.cn

SAVEPOINT sp1;
来源：http://wv.9csxet.cn

ROLLBACK TO sp1;
来源：http://vx.huanxung.cn

[Q69] 查看执行计划
来源：http://bs.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ch.shxzukj.cn

[Q70] 更新统计信息
来源：http://ey.521024.cn

ANALYZE TABLE users;
来源：http://qj.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://nd.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hx.huixinmuqiang.cn

[Q72] 查看索引
来源：http://mt.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://ef.bookmarksfly.cn

[Q73] 查看表状态
来源：http://dy.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qk.newstarts.cn

[Q74] 强制使用索引
来源：http://pa.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qh.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://md.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://co.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mt.9csxet.cn

[Q76] 按天统计
来源：http://ix.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eu.shxzskj.cn

[Q77] 时间加减
来源：http://dj.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hc.chemitech.net.cn

[Q78] 当前时间
来源：http://vr.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fu.521024.cn

[Q79] 字符串拼接
来源：http://vq.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ij.colortex.cn

[Q80] 字符串截取
来源：http://fv.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qn.asd995.cn

[Q81] 字符串替换
来源：http://nn.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oz.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://fq.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zn.szsharing.cn

[Q83] 大小写转换
来源：http://nm.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yi.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://lx.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://dr.9csxet.cn

[Q85] 数值取整
来源：http://gu.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ye.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://pf.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yq.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://yf.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pi.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://kq.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pn.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bo.521024.cn

[Q89] 判断表是否存在
来源：http://hn.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bu.szxytkj.cn

[Q90] 生成序号列
来源：http://oo.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nj.huixinmuqiang.cn

================================================================================
来源：http://jh.chemitech.net.cn

R. Bash 专题
来源：http://ru.yuexingan06.cn

================================================================================
来源：http://xc.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://ve.shxzukj.cn

#!/usr/bin/env bash
来源：http://ow.huixinmuqiang.cn

set -euo pipefail
来源：http://dh.521024.cn

[R02] 变量赋值与使用
来源：http://ut.9csxet.cn

name="Tom"; echo "$name"
来源：http://wk.szxytkj.cn

[R03] 只读变量
来源：http://uc.lnxyls.cn

readonly PI=3.14
来源：http://pm.huixinmuqiang.cn

[R04] 位置参数
来源：http://qf.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sq.9csxet.cn

[R05] 参数默认值
来源：http://iu.jctech888.com.cn

name="${1:-default}"
来源：http://wz.colortex.cn

[R06] 判断命令是否存在
来源：http://yh.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mi.jianghongdianzi.cn

[R07] if 判断文件
来源：http://tp.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cm.szsharing.cn

[R08] 数值比较
来源：http://pl.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kh.szsharing.cn

[R09] 字符串比较
来源：http://jj.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mj.newstarts.cn

[R10] 正则匹配
来源：http://fi.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qq.szsharing.cn

[R11] case 多分支
来源：http://lp.huixinmuqiang.cn

case "$1" in
来源：http://kh.521024.cn

start) echo "启动" ;;
来源：http://jl.lnxyls.cn

stop)  echo "停止" ;;
来源：http://hi.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://lj.jctech888.com.cn

esac
来源：http://bj.wgjwhj.cn

[R12] for 遍历文件
来源：http://yd.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://lw.nicolike.cn

[R13] for 计数循环
来源：http://dp.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://yo.huixinmuqiang.cn

[R14] C 风格 for
来源：http://wq.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cu.521024.cn

[R15] while 逐行读文件
来源：http://lk.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cy.szxytkj.cn

[R16] until 等待条件
来源：http://tg.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tw.panjiajie.cn

[R17] 数组定义与取值
来源：http://to.bjjhwx.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qj.bjjhwx.cn

[R18] 遍历数组
来源：http://cd.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ug.shxzukj.cn

[R19] 数组长度
来源：http://ot.huixiangedu.cn

echo "${#arr[@]}"
来源：http://rt.asd995.cn

[R20] 关联数组（字典）
来源：http://ce.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qz.bjjhwx.cn

[R21] 字符串长度
来源：http://pk.hahajie.cn

echo "${#s}"
来源：http://rk.panjiajie.cn

[R22] 截取子串
来源：http://tz.szxytkj.cn

echo "${s:0:5}"
来源：http://nl.szsharing.cn

[R23] 字符串替换
来源：http://cm.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jt.lnxyls.cn

[R24] 大小写转换
来源：http://dl.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://go.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://qf.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yw.muxihuayi.cn

[R26] 命令替换
来源：http://fy.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://rf.521024.cn

[R27] 算术展开
来源：http://oj.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://el.hnjuh.cn

[R28] 浮点运算
来源：http://ml.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://fb.jianghongdianzi.cn

[R29] 定义函数
来源：http://gr.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dg.newstarts.cn

[R30] 函数返回状态码
来源：http://us.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://ff.huanxung.cn

[R31] 局部变量
来源：http://ne.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://rc.jctech888.com.cn

[R32] 参数个数校验
来源：http://mr.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qn.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://sp.521024.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xg.asd995.cn

[R34] 退出时清理
来源：http://ph.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qo.shtwfgs.cn

[R35] 后台执行并等待
来源：http://dh.521024.cn


<!-- 参考信息 -->