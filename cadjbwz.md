代发 wailian999

PHP:  // 手写时间戳比较
来源：http://yd.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ah.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lb.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tj.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vz.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qv.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qo.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://vp.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jl.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mz.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pq.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hq.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lp.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zn.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ia.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kj.9csxet.cn

================================================================================
来源：http://kl.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://za.huixiangedu.cn

================================================================================
来源：http://cz.szsharing.cn

[Q01] 创建表
来源：http://tf.shtwfgs.cn

CREATE TABLE users (
来源：http://pp.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yr.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://va.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://ic.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://he.yuntaijiaju.cn

);
来源：http://it.gzmigu.cn

[Q02] 创建带外键的表
来源：http://xf.yuexingan06.cn

CREATE TABLE orders (
来源：http://zv.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ek.hnjuh.cn

user_id INT NOT NULL,
来源：http://dq.521024.cn

amount DECIMAL(10, 2),
来源：http://sp.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ix.huanxung.cn

);
来源：http://nf.szsharing.cn

[Q03] 增加列
来源：http://fo.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mr.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://mr.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cv.shxzskj.cn

[Q05] 重命名列
来源：http://om.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uw.newstarts.cn

[Q06] 删除列
来源：http://hr.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wl.jianghongdianzi.cn

[Q07] 删除表
来源：http://di.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://em.szsharing.cn

[Q08] 创建普通索引
来源：http://ru.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qr.colortex.cn

[Q09] 创建唯一索引
来源：http://li.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hc.huanxung.cn

[Q10] 插入单行
来源：http://cc.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ep.wgjwhj.cn

[Q11] 一次插入多行
来源：http://ek.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yp.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://ol.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xj.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://su.lnxyls.cn

[Q13] 忽略重复插入
来源：http://tp.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://db.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://tw.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wm.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iw.jianghongdianzi.cn

[Q15] 查询全部
来源：http://wn.gzmigu.cn

SELECT * FROM users;
来源：http://dq.panjiajie.cn

[Q16] 查询指定列
来源：http://zg.bjjhwx.cn

SELECT id, name FROM users;
来源：http://mv.lnxyls.cn

[Q17] 条件查询
来源：http://gg.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://li.asd995.cn

[Q18] 模糊匹配
来源：http://ly.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pl.9csxet.cn

[Q19] 范围查询
来源：http://od.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kp.yuexingan06.cn

[Q20] IN 列表
来源：http://ot.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ki.huixiangedu.cn

[Q21] 空值判断
来源：http://oi.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bx.chemitech.net.cn

[Q22] 排序
来源：http://ls.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ec.haigaiapp.cn

[Q23] 分页
来源：http://ot.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jr.521024.cn

[Q24] 去重
来源：http://ao.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://hw.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://cb.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ln.szxytkj.cn

[Q26] 计数
来源：http://kd.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://ww.newstarts.cn

[Q27] 条件计数
来源：http://dh.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kl.panjiajie.cn

[Q28] 求和与平均
来源：http://sl.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vc.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://vr.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzmigu.cn

[Q30] 分组统计
来源：http://by.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rr.yuexingan06.cn

[Q31] 分组后过滤
来源：http://iz.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nl.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://eg.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qu.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wp.chemitech.net.cn

[Q33] 多列分组
来源：http://ft.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ar.asd995.cn

[Q34] 每组取第一条
来源：http://go.hahajie.cn

SELECT * FROM (
来源：http://vt.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fe.nicolike.cn

) t WHERE rn = 1;
来源：http://ua.shxzukj.cn

[Q35] 内连接
来源：http://wc.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eb.jctech888.com.cn

[Q36] 左连接
来源：http://wa.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kt.lnxyls.cn

[Q37] 右连接
来源：http://uc.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ef.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yd.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hd.521024.cn

[Q39] 自连接（查上下级）
来源：http://xh.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nj.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bq.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ip.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fh.asd995.cn

[Q41] 多表连接
来源：http://an.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sj.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://eq.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://fu.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://tk.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://js.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ow.yuexingan06.cn

[Q43] 标量子查询
来源：http://cf.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zk.yuexingan06.cn

[Q44] IN 子查询
来源：http://ei.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zw.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://mf.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ye.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gb.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://te.shxzskj.cn

[Q47] 与平均值比较
来源：http://fm.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ca.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://lj.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rb.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://dx.521024.cn

[Q49] 更新单行
来源：http://tn.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hk.bookmarksfly.cn

[Q50] 批量更新
来源：http://tl.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pi.gzmigu.cn

[Q51] 用子查询更新
来源：http://qk.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nx.szsharing.cn

[Q52] 删除指定行
来源：http://hm.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://lo.panjiajie.cn

[Q53] 按条件删除
来源：http://dw.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zf.jianghongdianzi.cn

[Q54] 清空表
来源：http://np.hahajie.cn

TRUNCATE TABLE logs;
来源：http://lp.szsharing.cn

[Q55] 排名（并列占位）
来源：http://pq.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nr.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://sz.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lh.jianghongdianzi.cn

[Q57] 行号
来源：http://ai.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fj.gzmigu.cn

[Q58] 累计求和
来源：http://qk.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fx.szsharing.cn

[Q59] 分组内累计
来源：http://we.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hi.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ww.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xx.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dn.jctech888.com.cn

[Q61] 移动平均
来源：http://iw.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fq.panjiajie.cn

[Q62] 分组占比
来源：http://lb.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://du.bookmarksfly.cn

[Q63] 开启事务
来源：http://cz.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jh.szxytkj.cn

[Q64] 提交事务
来源：http://ev.huixinmuqiang.cn

COMMIT;
来源：http://gg.szsharing.cn

[Q65] 回滚事务
来源：http://zm.wgjwhj.cn

ROLLBACK;
来源：http://hi.huanxung.cn

[Q66] 行锁查询
来源：http://zf.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qs.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://rk.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yi.9csxet.cn

[Q68] 保存点
来源：http://dr.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://qd.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://zi.hahajie.cn

[Q69] 查看执行计划
来源：http://qj.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ef.colortex.cn

[Q70] 更新统计信息
来源：http://uy.shxzukj.cn

ANALYZE TABLE users;
来源：http://xp.shtwfgs.cn

[Q71] 查看建表语句
来源：http://vb.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lf.shxzskj.cn

[Q72] 查看索引
来源：http://qw.nicolike.cn

SHOW INDEX FROM users;
来源：http://xl.nicolike.cn

[Q73] 查看表状态
来源：http://qe.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mp.hahajie.cn

[Q74] 强制使用索引
来源：http://ao.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zs.hahajie.cn

[Q75] 日期格式化
来源：http://gc.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cg.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fy.muxihuayi.cn

[Q76] 按天统计
来源：http://id.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lf.huixiangedu.cn

[Q77] 时间加减
来源：http://bn.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vi.asd995.cn

[Q78] 当前时间
来源：http://oy.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hv.hnjuh.cn

[Q79] 字符串拼接
来源：http://iv.shxzukj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oh.szsharing.cn

[Q80] 字符串截取
来源：http://kh.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fz.hnjuh.cn

[Q81] 字符串替换
来源：http://wn.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qb.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://vl.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cj.szsharing.cn

[Q83] 大小写转换
来源：http://to.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://be.gzmigu.cn

[Q84] 去除首尾空格
来源：http://um.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://tg.nszjky.cn

[Q85] 数值取整
来源：http://mw.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lx.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://xi.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://it.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://cm.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ot.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://np.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pb.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pi.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://jg.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yo.panjiajie.cn

[Q90] 生成序号列
来源：http://ce.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jt.panjiajie.cn

================================================================================
来源：http://en.szxytkj.cn

R. Bash 专题
来源：http://um.muxihuayi.cn

================================================================================
来源：http://wg.asd995.cn

[R01] shebang 与严格模式
来源：http://kd.huanxung.cn

#!/usr/bin/env bash
来源：http://aj.newstarts.cn

set -euo pipefail
来源：http://yz.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://by.shxzskj.cn

name="Tom"; echo "$name"
来源：http://fv.colortex.cn

[R03] 只读变量
来源：http://cu.nszjky.cn

readonly PI=3.14
来源：http://ex.nicolike.cn

[R04] 位置参数
来源：http://nm.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lg.9csxet.cn

[R05] 参数默认值
来源：http://uw.huixiangedu.cn

name="${1:-default}"
来源：http://bd.nszjky.cn

[R06] 判断命令是否存在
来源：http://yk.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bo.wgjwhj.cn

[R07] if 判断文件
来源：http://sj.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rn.szxytkj.cn

[R08] 数值比较
来源：http://rr.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zy.jianghongdianzi.cn

[R09] 字符串比较
来源：http://pp.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mm.9csxet.cn

[R10] 正则匹配
来源：http://rb.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tn.huixinmuqiang.cn

[R11] case 多分支
来源：http://yq.shxzukj.cn

case "$1" in
来源：http://av.asd995.cn

start) echo "启动" ;;
来源：http://hw.hnjuh.cn

stop)  echo "停止" ;;
来源：http://vh.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://gw.shtwfgs.cn

esac
来源：http://yp.521024.cn

[R12] for 遍历文件
来源：http://ct.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://va.shtwfgs.cn

[R13] for 计数循环
来源：http://jn.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://ur.wgjwhj.cn

[R14] C 风格 for
来源：http://cn.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sr.newstarts.cn

[R15] while 逐行读文件
来源：http://ra.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fu.chemitech.net.cn

[R16] until 等待条件
来源：http://rh.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gx.chemitech.net.cn

[R17] 数组定义与取值
来源：http://pf.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eg.bjjhwx.cn

[R18] 遍历数组
来源：http://ih.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wy.nicolike.cn

[R19] 数组长度
来源：http://du.hahajie.cn

echo "${#arr[@]}"
来源：http://nd.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://li.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://un.colortex.cn

[R21] 字符串长度
来源：http://fr.huixinmuqiang.cn

echo "${#s}"
来源：http://eg.nicolike.cn

[R22] 截取子串
来源：http://iy.wgjwhj.cn

echo "${s:0:5}"
来源：http://st.9csxet.cn

[R23] 字符串替换
来源：http://el.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dh.yuntaijiaju.cn

[R24] 大小写转换
来源：http://fi.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ik.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://og.shxzukj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ki.shxzukj.cn

[R26] 命令替换
来源：http://ah.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://on.huanxung.cn

[R27] 算术展开
来源：http://il.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://hg.huixinmuqiang.cn

[R28] 浮点运算
来源：http://yj.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://ps.shxzukj.cn

[R29] 定义函数
来源：http://qn.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zs.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://nm.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://cm.nszjky.cn

[R31] 局部变量
来源：http://ms.nicolike.cn

f() { local x=1; echo "$x"; }
来源：http://kr.huixinmuqiang.cn

[R32] 参数个数校验
来源：http://dq.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tc.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://dj.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rt.shxzukj.cn

[R34] 退出时清理
来源：http://yg.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tg.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://tk.newstarts.cn


<!-- 参考信息 -->