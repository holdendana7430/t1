代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://st.colortex.cn

C#:   if (x is null) {}
来源：http://yo.lnxyls.cn

[P07] 防抖与节流
来源：http://my.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lh.asd995.cn

PHP:  // 手写时间戳比较
来源：http://oo.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gp.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wn.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ry.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zz.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gp.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yz.9csxet.cn

[P08] 处理浮点精度问题
来源：http://ze.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lt.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vz.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gn.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ov.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dq.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zd.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nf.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lr.muxihuayi.cn

================================================================================
来源：http://ao.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lp.szxytkj.cn

================================================================================
来源：http://po.newstarts.cn

[Q01] 创建表
来源：http://sc.huixiangedu.cn

CREATE TABLE users (
来源：http://vn.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oh.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://cc.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://av.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://is.lnxyls.cn

);
来源：http://hg.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://ga.hnjuh.cn

CREATE TABLE orders (
来源：http://iw.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://md.haigaiapp.cn

user_id INT NOT NULL,
来源：http://im.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://zd.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qo.hnjuh.cn

);
来源：http://gw.lnxyls.cn

[Q03] 增加列
来源：http://of.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.521024.cn

[Q04] 修改列类型
来源：http://bp.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dx.szxytkj.cn

[Q05] 重命名列
来源：http://dx.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dz.9csxet.cn

[Q06] 删除列
来源：http://vw.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kf.nicolike.cn

[Q07] 删除表
来源：http://ag.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://tt.nicolike.cn

[Q08] 创建普通索引
来源：http://gd.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fc.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://qf.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rx.chemitech.net.cn

[Q10] 插入单行
来源：http://nz.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ah.muxihuayi.cn

[Q11] 一次插入多行
来源：http://sy.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mz.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://dj.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ov.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mx.panjiajie.cn

[Q13] 忽略重复插入
来源：http://wd.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tx.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://rj.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://og.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ab.wgjwhj.cn

[Q15] 查询全部
来源：http://pu.haigaiapp.cn

SELECT * FROM users;
来源：http://ce.asd995.cn

[Q16] 查询指定列
来源：http://oe.hahajie.cn

SELECT id, name FROM users;
来源：http://ks.huanxung.cn

[Q17] 条件查询
来源：http://tw.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vr.gzmigu.cn

[Q18] 模糊匹配
来源：http://cu.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sh.bjjhwx.cn

[Q19] 范围查询
来源：http://ew.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dq.colortex.cn

[Q20] IN 列表
来源：http://zy.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bg.hahajie.cn

[Q21] 空值判断
来源：http://hx.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oz.hnjuh.cn

[Q22] 排序
来源：http://fg.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://or.newstarts.cn

[Q23] 分页
来源：http://mb.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fv.wgjwhj.cn

[Q24] 去重
来源：http://ez.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://oi.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://ph.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yj.asd995.cn

[Q26] 计数
来源：http://vc.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://fp.chemitech.net.cn

[Q27] 条件计数
来源：http://rn.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://az.nszjky.cn

[Q28] 求和与平均
来源：http://fs.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zn.panjiajie.cn

[Q29] 最大最小值
来源：http://yq.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yq.shxzskj.cn

[Q30] 分组统计
来源：http://st.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vg.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ja.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xu.9csxet.cn

[Q32] 分组拼接字符串
来源：http://pq.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ig.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tf.chemitech.net.cn

[Q33] 多列分组
来源：http://jr.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wg.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://ir.hahajie.cn

SELECT * FROM (
来源：http://jn.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pq.lnxyls.cn

) t WHERE rn = 1;
来源：http://rd.colortex.cn

[Q35] 内连接
来源：http://qv.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pw.521024.cn

[Q36] 左连接
来源：http://kc.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qa.huixiangedu.cn

[Q37] 右连接
来源：http://tj.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cm.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qj.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bx.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://eg.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://is.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zk.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fs.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ui.bjjhwx.cn

[Q41] 多表连接
来源：http://hj.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ji.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://wo.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://rr.asd995.cn

[Q42] 连接条件附加过滤
来源：http://sw.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://yb.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ho.nszjky.cn

[Q43] 标量子查询
来源：http://cn.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gx.nszjky.cn

[Q44] IN 子查询
来源：http://il.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xj.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ct.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jl.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://to.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jd.wgjwhj.cn

[Q47] 与平均值比较
来源：http://ua.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bh.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://km.yuntaijiaju.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nu.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://az.bookmarksfly.cn

[Q49] 更新单行
来源：http://zh.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uw.nszjky.cn

[Q50] 批量更新
来源：http://hx.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xj.hahajie.cn

[Q51] 用子查询更新
来源：http://ci.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rx.hnjuh.cn

[Q52] 删除指定行
来源：http://qk.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://pw.huanxung.cn

[Q53] 按条件删除
来源：http://nq.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fv.newstarts.cn

[Q54] 清空表
来源：http://od.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://gh.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://it.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vn.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://mu.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://td.huixiangedu.cn

[Q57] 行号
来源：http://cq.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sk.hnjuh.cn

[Q58] 累计求和
来源：http://rq.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jr.newstarts.cn

[Q59] 分组内累计
来源：http://hj.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ss.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://he.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ad.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jg.newstarts.cn

[Q61] 移动平均
来源：http://sd.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yu.szsharing.cn

[Q62] 分组占比
来源：http://hl.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ru.9csxet.cn

[Q63] 开启事务
来源：http://bm.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://js.panjiajie.cn

[Q64] 提交事务
来源：http://ti.wgjwhj.cn

COMMIT;
来源：http://ow.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://sd.shtwfgs.cn

ROLLBACK;
来源：http://hk.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://va.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://do.gzmigu.cn

[Q67] 设置隔离级别
来源：http://pf.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rf.muxihuayi.cn

[Q68] 保存点
来源：http://fx.haigaiapp.cn

SAVEPOINT sp1;
来源：http://mr.colortex.cn

ROLLBACK TO sp1;
来源：http://pe.jctech888.com.cn

[Q69] 查看执行计划
来源：http://yr.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://de.szsharing.cn

[Q70] 更新统计信息
来源：http://ns.hnjuh.cn

ANALYZE TABLE users;
来源：http://ef.szsharing.cn

[Q71] 查看建表语句
来源：http://wr.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cl.szxytkj.cn

[Q72] 查看索引
来源：http://co.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://ae.haigaiapp.cn

[Q73] 查看表状态
来源：http://br.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xh.chemitech.net.cn

[Q74] 强制使用索引
来源：http://cv.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vw.haigaiapp.cn

[Q75] 日期格式化
来源：http://st.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sj.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sw.yuntaijiaju.cn

[Q76] 按天统计
来源：http://mq.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vg.muxihuayi.cn

[Q77] 时间加减
来源：http://sz.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://la.huixiangedu.cn

[Q78] 当前时间
来源：http://vg.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yr.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://pg.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wd.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://pr.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zg.huanxung.cn

[Q81] 字符串替换
来源：http://je.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://at.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://ie.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ls.hahajie.cn

[Q83] 大小写转换
来源：http://ta.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tu.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://vi.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://cf.gzmigu.cn

[Q85] 数值取整
来源：http://on.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zb.asd995.cn

[Q86] 读取 JSON 字段
来源：http://lo.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hf.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://vz.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://de.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://bh.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cd.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mk.shxzskj.cn

[Q89] 判断表是否存在
来源：http://qp.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fu.hnjuh.cn

[Q90] 生成序号列
来源：http://ji.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zp.jianghongdianzi.cn

================================================================================
来源：http://qa.521024.cn

R. Bash 专题
来源：http://bd.9csxet.cn

================================================================================
来源：http://bv.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ih.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://nb.gzmigu.cn

set -euo pipefail
来源：http://kc.panjiajie.cn

[R02] 变量赋值与使用
来源：http://vp.szsharing.cn

name="Tom"; echo "$name"
来源：http://dz.asd995.cn

[R03] 只读变量
来源：http://uq.szxytkj.cn

readonly PI=3.14
来源：http://wd.panjiajie.cn

[R04] 位置参数
来源：http://hn.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zw.bjjhwx.cn

[R05] 参数默认值
来源：http://tn.521024.cn

name="${1:-default}"
来源：http://uq.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://mj.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vy.yuexingan06.cn

[R07] if 判断文件
来源：http://pk.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tn.szxytkj.cn

[R08] 数值比较
来源：http://qw.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ax.muxihuayi.cn

[R09] 字符串比较
来源：http://gz.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lu.szxytkj.cn

[R10] 正则匹配
来源：http://cl.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sg.gzmigu.cn

[R11] case 多分支
来源：http://qn.chemitech.net.cn

case "$1" in
来源：http://di.chemitech.net.cn

start) echo "启动" ;;
来源：http://zv.shxzukj.cn

stop)  echo "停止" ;;
来源：http://fh.nszjky.cn

*)     echo "未知命令" ;;
来源：http://zu.nicolike.cn

esac
来源：http://ry.huixiangedu.cn

[R12] for 遍历文件
来源：http://tg.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://pj.chemitech.net.cn

[R13] for 计数循环
来源：http://ui.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://dk.gzmigu.cn

[R14] C 风格 for
来源：http://ef.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ea.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://fd.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rq.yuexingan06.cn

[R16] until 等待条件
来源：http://uh.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dg.9csxet.cn

[R17] 数组定义与取值
来源：http://jt.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sl.jianghongdianzi.cn

[R18] 遍历数组
来源：http://kw.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ku.lnxyls.cn

[R19] 数组长度
来源：http://hd.szxytkj.cn

echo "${#arr[@]}"
来源：http://du.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://wc.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zs.nszjky.cn

[R21] 字符串长度
来源：http://ij.hahajie.cn

echo "${#s}"
来源：http://lx.nszjky.cn

[R22] 截取子串
来源：http://gn.yuexingan06.cn

echo "${s:0:5}"
来源：http://ej.panjiajie.cn

[R23] 字符串替换
来源：http://un.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://be.9csxet.cn

[R24] 大小写转换
来源：http://bi.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ed.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://ao.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fj.haigaiapp.cn

[R26] 命令替换
来源：http://vy.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://vo.9csxet.cn

[R27] 算术展开
来源：http://bf.nszjky.cn

echo $((1 + 2 * 3))
来源：http://nb.521024.cn

[R28] 浮点运算
来源：http://tx.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://zi.9csxet.cn

[R29] 定义函数
来源：http://lb.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://av.szsharing.cn

[R30] 函数返回状态码
来源：http://ln.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ft.9csxet.cn

[R31] 局部变量
来源：http://ne.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://tp.lnxyls.cn

[R32] 参数个数校验
来源：http://vy.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pn.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://ew.muxihuayi.cn


<!-- 参考信息 -->