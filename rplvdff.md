代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hg.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eu.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xt.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oa.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zs.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://av.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xq.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://lf.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ng.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oo.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cj.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xw.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yd.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qy.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ld.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gu.bjjhwx.cn

================================================================================
来源：http://gh.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mw.wgjwhj.cn

================================================================================
来源：http://ae.hnjuh.cn

[Q01] 创建表
来源：http://uc.huixiangedu.cn

CREATE TABLE users (
来源：http://st.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zh.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ja.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://yb.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ad.bookmarksfly.cn

);
来源：http://pq.colortex.cn

[Q02] 创建带外键的表
来源：http://fm.huanxung.cn

CREATE TABLE orders (
来源：http://wr.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uc.huixiangedu.cn

user_id INT NOT NULL,
来源：http://ni.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://uq.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bc.bookmarksfly.cn

);
来源：http://oi.yuntaijiaju.cn

[Q03] 增加列
来源：http://yk.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qs.szxytkj.cn

[Q04] 修改列类型
来源：http://pu.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vr.yuexingan06.cn

[Q05] 重命名列
来源：http://hm.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uw.shxzukj.cn

[Q06] 删除列
来源：http://cb.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://me.bjjhwx.cn

[Q07] 删除表
来源：http://ic.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://oi.asd995.cn

[Q08] 创建普通索引
来源：http://nz.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dc.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://uy.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gv.jianghongdianzi.cn

[Q10] 插入单行
来源：http://eq.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pt.chemitech.net.cn

[Q11] 一次插入多行
来源：http://ow.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pl.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://tu.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mo.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vt.asd995.cn

[Q13] 忽略重复插入
来源：http://it.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ne.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://xq.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gj.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lr.hnjuh.cn

[Q15] 查询全部
来源：http://yp.haigaiapp.cn

SELECT * FROM users;
来源：http://yp.huanxung.cn

[Q16] 查询指定列
来源：http://qy.chemitech.net.cn

SELECT id, name FROM users;
来源：http://cz.9csxet.cn

[Q17] 条件查询
来源：http://wq.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lu.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://lm.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wc.hahajie.cn

[Q19] 范围查询
来源：http://vr.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fp.panjiajie.cn

[Q20] IN 列表
来源：http://cn.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nv.haigaiapp.cn

[Q21] 空值判断
来源：http://bz.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lx.szsharing.cn

[Q22] 排序
来源：http://pf.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hr.yuntaijiaju.cn

[Q23] 分页
来源：http://wu.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ls.huixinmuqiang.cn

[Q24] 去重
来源：http://ro.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://ob.panjiajie.cn

[Q25] 只取前 N 条
来源：http://yg.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fn.szsharing.cn

[Q26] 计数
来源：http://rz.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ng.huixinmuqiang.cn

[Q27] 条件计数
来源：http://ms.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xi.nszjky.cn

[Q28] 求和与平均
来源：http://sd.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gn.szsharing.cn

[Q29] 最大最小值
来源：http://ri.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rb.jctech888.com.cn

[Q30] 分组统计
来源：http://tn.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gd.colortex.cn

[Q31] 分组后过滤
来源：http://pl.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qk.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://vx.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mr.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://od.chemitech.net.cn

[Q33] 多列分组
来源：http://kn.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rm.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ad.asd995.cn

SELECT * FROM (
来源：http://sb.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jx.chemitech.net.cn

) t WHERE rn = 1;
来源：http://ry.haigaiapp.cn

[Q35] 内连接
来源：http://ix.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hb.nicolike.cn

[Q36] 左连接
来源：http://zz.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hx.hnjuh.cn

[Q37] 右连接
来源：http://bz.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dr.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mx.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fj.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://aq.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cg.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qp.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ni.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://by.9csxet.cn

[Q41] 多表连接
来源：http://ke.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://el.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://ay.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://gr.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://vs.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://sy.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jj.szsharing.cn

[Q43] 标量子查询
来源：http://ma.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sg.panjiajie.cn

[Q44] IN 子查询
来源：http://td.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sa.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://hf.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sw.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lj.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yy.nicolike.cn

[Q47] 与平均值比较
来源：http://pd.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oe.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://hd.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://po.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://tv.yuntaijiaju.cn

[Q49] 更新单行
来源：http://oi.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mq.huixinmuqiang.cn

[Q50] 批量更新
来源：http://dr.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rs.shxzskj.cn

[Q51] 用子查询更新
来源：http://hp.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ak.shxzukj.cn

[Q52] 删除指定行
来源：http://uz.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://vo.hahajie.cn

[Q53] 按条件删除
来源：http://we.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lk.muxihuayi.cn

[Q54] 清空表
来源：http://kl.newstarts.cn

TRUNCATE TABLE logs;
来源：http://bm.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://ym.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yv.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://rx.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://el.szsharing.cn

[Q57] 行号
来源：http://dm.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pf.jctech888.com.cn

[Q58] 累计求和
来源：http://lr.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cq.muxihuayi.cn

[Q59] 分组内累计
来源：http://bi.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qf.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://ny.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vo.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vs.bookmarksfly.cn

[Q61] 移动平均
来源：http://ds.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nh.wgjwhj.cn

[Q62] 分组占比
来源：http://bu.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pl.colortex.cn

[Q63] 开启事务
来源：http://pa.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ur.nszjky.cn

[Q64] 提交事务
来源：http://zd.gzmigu.cn

COMMIT;
来源：http://qt.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://qu.521024.cn

ROLLBACK;
来源：http://ce.hahajie.cn

[Q66] 行锁查询
来源：http://tt.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wq.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://ob.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gg.shxzskj.cn

[Q68] 保存点
来源：http://oo.shtwfgs.cn

SAVEPOINT sp1;
来源：http://nq.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://pm.nicolike.cn

[Q69] 查看执行计划
来源：http://df.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bb.shxzukj.cn

[Q70] 更新统计信息
来源：http://mq.521024.cn

ANALYZE TABLE users;
来源：http://qa.hnjuh.cn

[Q71] 查看建表语句
来源：http://rx.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ml.chemitech.net.cn

[Q72] 查看索引
来源：http://dw.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://rh.newstarts.cn

[Q73] 查看表状态
来源：http://py.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ay.huanxung.cn

[Q74] 强制使用索引
来源：http://sd.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://be.szxytkj.cn

[Q75] 日期格式化
来源：http://yp.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xw.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wu.bjjhwx.cn

[Q76] 按天统计
来源：http://xb.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qb.szxytkj.cn

[Q77] 时间加减
来源：http://bw.shxzukj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mw.panjiajie.cn

[Q78] 当前时间
来源：http://uv.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zf.hnjuh.cn

[Q79] 字符串拼接
来源：http://cc.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uf.yuexingan06.cn

[Q80] 字符串截取
来源：http://em.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kg.huixiangedu.cn

[Q81] 字符串替换
来源：http://tv.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pg.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://wd.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fi.nszjky.cn

[Q83] 大小写转换
来源：http://ke.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ef.huanxung.cn

[Q84] 去除首尾空格
来源：http://ov.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://xv.shxzukj.cn

[Q85] 数值取整
来源：http://ei.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wn.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://ue.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://es.9csxet.cn

[Q87] JSON 字段做条件
来源：http://nb.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://up.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://ax.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gq.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cu.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://op.szsharing.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bz.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://pq.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://da.jianghongdianzi.cn

================================================================================
来源：http://ih.panjiajie.cn

R. Bash 专题
来源：http://ac.nicolike.cn

================================================================================
来源：http://ch.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://lw.shxzskj.cn

#!/usr/bin/env bash
来源：http://ay.yuntaijiaju.cn

set -euo pipefail
来源：http://qn.gzmigu.cn

[R02] 变量赋值与使用
来源：http://sy.szsharing.cn

name="Tom"; echo "$name"
来源：http://ej.jctech888.com.cn

[R03] 只读变量
来源：http://jt.huixiangedu.cn

readonly PI=3.14
来源：http://te.lnxyls.cn

[R04] 位置参数
来源：http://xj.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gm.bookmarksfly.cn

[R05] 参数默认值
来源：http://ri.shxzskj.cn

name="${1:-default}"
来源：http://op.hahajie.cn

[R06] 判断命令是否存在
来源：http://wi.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mv.huanxung.cn

[R07] if 判断文件
来源：http://th.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fm.bookmarksfly.cn

[R08] 数值比较
来源：http://jj.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zi.nszjky.cn

[R09] 字符串比较
来源：http://rs.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pt.jctech888.com.cn

[R10] 正则匹配
来源：http://pt.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pm.haigaiapp.cn

[R11] case 多分支
来源：http://go.hahajie.cn

case "$1" in
来源：http://co.colortex.cn

start) echo "启动" ;;
来源：http://uf.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://af.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://pu.jctech888.com.cn

esac
来源：http://wb.szsharing.cn

[R12] for 遍历文件
来源：http://hs.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://gc.huanxung.cn

[R13] for 计数循环
来源：http://ox.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://md.szsharing.cn

[R14] C 风格 for
来源：http://hk.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hq.gzmigu.cn

[R15] while 逐行读文件
来源：http://iz.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sm.huixiangedu.cn

[R16] until 等待条件
来源：http://qf.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ya.panjiajie.cn

[R17] 数组定义与取值
来源：http://gp.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nb.jianghongdianzi.cn

[R18] 遍历数组
来源：http://mf.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zv.jctech888.com.cn

[R19] 数组长度
来源：http://sk.chemitech.net.cn

echo "${#arr[@]}"
来源：http://th.huanxung.cn

[R20] 关联数组（字典）
来源：http://uq.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yp.bookmarksfly.cn

[R21] 字符串长度
来源：http://tw.shtwfgs.cn

echo "${#s}"
来源：http://pr.huixinmuqiang.cn

[R22] 截取子串
来源：http://gs.huixiangedu.cn

echo "${s:0:5}"
来源：http://lt.nicolike.cn

[R23] 字符串替换
来源：http://qs.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uf.lnxyls.cn

[R24] 大小写转换
来源：http://qi.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rb.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://qg.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lz.szxytkj.cn

[R26] 命令替换
来源：http://od.asd995.cn

now=$(date +%F); echo "$now"
来源：http://ib.yuntaijiaju.cn

[R27] 算术展开
来源：http://uq.colortex.cn

echo $((1 + 2 * 3))
来源：http://pp.shxzskj.cn

[R28] 浮点运算
来源：http://zv.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://or.521024.cn

[R29] 定义函数
来源：http://bb.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sy.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://vr.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://er.bjjhwx.cn

[R31] 局部变量
来源：http://mg.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://qu.bjjhwx.cn

[R32] 参数个数校验
来源：http://op.wgjwhj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://be.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://yb.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zu.asd995.cn

[R34] 退出时清理
来源：http://wq.shxzukj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ja.521024.cn

[R35] 后台执行并等待
来源：http://nt.hnjuh.cn


<!-- 参考信息 -->