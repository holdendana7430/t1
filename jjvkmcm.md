代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mb.hahajie.cn

C#:   if (x is null) {}
来源：http://tm.colortex.cn

[P07] 防抖与节流
来源：http://yz.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zp.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://yz.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fn.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uq.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cm.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ak.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wo.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tq.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://fj.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mn.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://re.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bw.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wi.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wf.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vu.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://og.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uc.newstarts.cn

================================================================================
来源：http://xv.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dv.panjiajie.cn

================================================================================
来源：http://ds.colortex.cn

[Q01] 创建表
来源：http://ij.wgjwhj.cn

CREATE TABLE users (
来源：http://oy.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qp.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://an.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://ht.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ze.lnxyls.cn

);
来源：http://ad.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://ui.bjjhwx.cn

CREATE TABLE orders (
来源：http://cx.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bq.shxzskj.cn

user_id INT NOT NULL,
来源：http://ee.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://lw.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cu.huixinmuqiang.cn

);
来源：http://yk.nicolike.cn

[Q03] 增加列
来源：http://kx.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wm.colortex.cn

[Q04] 修改列类型
来源：http://vw.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ur.wgjwhj.cn

[Q05] 重命名列
来源：http://qq.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tn.shxzskj.cn

[Q06] 删除列
来源：http://cj.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rn.bookmarksfly.cn

[Q07] 删除表
来源：http://ls.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://ju.521024.cn

[Q08] 创建普通索引
来源：http://qd.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cn.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://gn.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ao.huanxung.cn

[Q10] 插入单行
来源：http://lw.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nh.lnxyls.cn

[Q11] 一次插入多行
来源：http://ul.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aa.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://qi.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gz.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sx.nszjky.cn

[Q13] 忽略重复插入
来源：http://rr.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ig.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://ec.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ea.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yy.nszjky.cn

[Q15] 查询全部
来源：http://uk.chemitech.net.cn

SELECT * FROM users;
来源：http://jh.hnjuh.cn

[Q16] 查询指定列
来源：http://pv.haigaiapp.cn

SELECT id, name FROM users;
来源：http://eh.huanxung.cn

[Q17] 条件查询
来源：http://qx.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rr.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://wy.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ah.jctech888.com.cn

[Q19] 范围查询
来源：http://tt.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ez.nszjky.cn

[Q20] IN 列表
来源：http://jg.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ge.shtwfgs.cn

[Q21] 空值判断
来源：http://go.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sb.nszjky.cn

[Q22] 排序
来源：http://pn.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tg.jianghongdianzi.cn

[Q23] 分页
来源：http://tq.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cy.muxihuayi.cn

[Q24] 去重
来源：http://dp.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://la.hahajie.cn

[Q25] 只取前 N 条
来源：http://fd.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://os.huanxung.cn

[Q26] 计数
来源：http://at.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://tb.colortex.cn

[Q27] 条件计数
来源：http://xm.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lt.bookmarksfly.cn

[Q28] 求和与平均
来源：http://db.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uc.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://sk.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pf.lnxyls.cn

[Q30] 分组统计
来源：http://au.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qv.colortex.cn

[Q31] 分组后过滤
来源：http://pn.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zf.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://ec.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mj.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xz.huanxung.cn

[Q33] 多列分组
来源：http://zu.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ix.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ka.521024.cn

SELECT * FROM (
来源：http://kj.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mq.jctech888.com.cn

) t WHERE rn = 1;
来源：http://oa.muxihuayi.cn

[Q35] 内连接
来源：http://hf.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://in.hnjuh.cn

[Q36] 左连接
来源：http://ra.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sc.szsharing.cn

[Q37] 右连接
来源：http://kb.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uh.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mr.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qa.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://tw.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oq.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mi.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nm.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ue.panjiajie.cn

[Q41] 多表连接
来源：http://px.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wn.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://cr.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://gf.nicolike.cn

[Q42] 连接条件附加过滤
来源：http://lg.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://db.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ge.hahajie.cn

[Q43] 标量子查询
来源：http://de.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pi.huanxung.cn

[Q44] IN 子查询
来源：http://hr.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zq.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://xm.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ah.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eh.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ag.yuntaijiaju.cn

[Q47] 与平均值比较
来源：http://fo.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pq.hahajie.cn

[Q48] CTE 公用表表达式
来源：http://hh.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kv.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://xs.muxihuayi.cn

[Q49] 更新单行
来源：http://by.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://no.newstarts.cn

[Q50] 批量更新
来源：http://lx.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bo.szsharing.cn

[Q51] 用子查询更新
来源：http://fo.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lj.bookmarksfly.cn

[Q52] 删除指定行
来源：http://eh.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://bk.gzmigu.cn

[Q53] 按条件删除
来源：http://rm.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qv.lnxyls.cn

[Q54] 清空表
来源：http://bi.nszjky.cn

TRUNCATE TABLE logs;
来源：http://sr.szsharing.cn

[Q55] 排名（并列占位）
来源：http://of.yuexingan06.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vh.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://gj.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nc.yuexingan06.cn

[Q57] 行号
来源：http://pf.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vl.huixiangedu.cn

[Q58] 累计求和
来源：http://gx.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://to.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://hx.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mc.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://os.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vb.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wg.szsharing.cn

[Q61] 移动平均
来源：http://fs.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fd.szxytkj.cn

[Q62] 分组占比
来源：http://aq.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ui.chemitech.net.cn

[Q63] 开启事务
来源：http://yq.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vk.szsharing.cn

[Q64] 提交事务
来源：http://fp.jianghongdianzi.cn

COMMIT;
来源：http://yo.newstarts.cn

[Q65] 回滚事务
来源：http://ck.asd995.cn

ROLLBACK;
来源：http://es.lnxyls.cn

[Q66] 行锁查询
来源：http://vc.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yt.shxzukj.cn

[Q67] 设置隔离级别
来源：http://eb.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aa.hnjuh.cn

[Q68] 保存点
来源：http://wv.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://kf.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://yd.shxzukj.cn

[Q69] 查看执行计划
来源：http://gj.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rr.jctech888.com.cn

[Q70] 更新统计信息
来源：http://hn.haigaiapp.cn

ANALYZE TABLE users;
来源：http://lh.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://ox.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cs.chemitech.net.cn

[Q72] 查看索引
来源：http://bb.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://rz.shxzukj.cn

[Q73] 查看表状态
来源：http://is.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rs.wgjwhj.cn

[Q74] 强制使用索引
来源：http://bw.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nx.shtwfgs.cn

[Q75] 日期格式化
来源：http://uf.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dt.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tw.haigaiapp.cn

[Q76] 按天统计
来源：http://za.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gd.muxihuayi.cn

[Q77] 时间加减
来源：http://ug.szxytkj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cg.nicolike.cn

[Q78] 当前时间
来源：http://nf.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dk.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://yy.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pj.lnxyls.cn

[Q80] 字符串截取
来源：http://qx.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hg.9csxet.cn

[Q81] 字符串替换
来源：http://nj.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://os.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://ph.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ta.chemitech.net.cn

[Q83] 大小写转换
来源：http://lc.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sb.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://ux.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://ex.shxzukj.cn

[Q85] 数值取整
来源：http://rc.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kx.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://qc.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ey.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://wf.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kz.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://ce.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ev.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lv.9csxet.cn

[Q89] 判断表是否存在
来源：http://xk.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zh.521024.cn

[Q90] 生成序号列
来源：http://rb.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pc.bookmarksfly.cn

================================================================================
来源：http://bu.521024.cn

R. Bash 专题
来源：http://id.hahajie.cn

================================================================================
来源：http://ir.shxzskj.cn

[R01] shebang 与严格模式
来源：http://ue.chemitech.net.cn

#!/usr/bin/env bash
来源：http://xt.hahajie.cn

set -euo pipefail
来源：http://tr.nicolike.cn

[R02] 变量赋值与使用
来源：http://an.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://sb.521024.cn

[R03] 只读变量
来源：http://vo.huixiangedu.cn

readonly PI=3.14
来源：http://xj.jianghongdianzi.cn

[R04] 位置参数
来源：http://oz.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ka.szxytkj.cn

[R05] 参数默认值
来源：http://jj.bjjhwx.cn

name="${1:-default}"
来源：http://vm.shxzskj.cn

[R06] 判断命令是否存在
来源：http://mo.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xj.newstarts.cn

[R07] if 判断文件
来源：http://qc.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ub.nszjky.cn

[R08] 数值比较
来源：http://wb.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wp.colortex.cn

[R09] 字符串比较
来源：http://dn.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zx.newstarts.cn

[R10] 正则匹配
来源：http://br.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ge.shxzukj.cn

[R11] case 多分支
来源：http://cn.jianghongdianzi.cn

case "$1" in
来源：http://gp.bookmarksfly.cn

start) echo "启动" ;;
来源：http://fq.huanxung.cn

stop)  echo "停止" ;;
来源：http://uh.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://sl.nszjky.cn

esac
来源：http://mb.gzmigu.cn

[R12] for 遍历文件
来源：http://hf.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://lf.asd995.cn

[R13] for 计数循环
来源：http://mq.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://hz.colortex.cn

[R14] C 风格 for
来源：http://no.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fb.haigaiapp.cn

[R15] while 逐行读文件
来源：http://vf.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kd.huanxung.cn

[R16] until 等待条件
来源：http://hr.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ij.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://sm.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bj.nicolike.cn

[R18] 遍历数组
来源：http://qe.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oi.wgjwhj.cn

[R19] 数组长度
来源：http://tz.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://kj.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://ey.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ly.chemitech.net.cn

[R21] 字符串长度
来源：http://hk.yuexingan06.cn

echo "${#s}"
来源：http://lg.szsharing.cn

[R22] 截取子串
来源：http://vo.nszjky.cn

echo "${s:0:5}"
来源：http://tb.nicolike.cn

[R23] 字符串替换
来源：http://ln.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tt.shxzskj.cn

[R24] 大小写转换
来源：http://te.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lj.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://vk.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vg.shtwfgs.cn

[R26] 命令替换
来源：http://wm.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://mo.bookmarksfly.cn

[R27] 算术展开
来源：http://cz.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://hu.hahajie.cn

[R28] 浮点运算
来源：http://kn.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://sr.shxzskj.cn

[R29] 定义函数
来源：http://jb.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://as.chemitech.net.cn

[R30] 函数返回状态码
来源：http://sp.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://by.jctech888.com.cn

[R31] 局部变量
来源：http://qv.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://jb.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://hv.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ue.521024.cn

[R33] 捕获错误并提示行号
来源：http://js.chemitech.net.cn


<!-- 参考信息 -->