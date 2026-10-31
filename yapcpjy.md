代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sx.asd995.cn

C#:   if (x is null) {}
来源：http://jn.asd995.cn

[P07] 防抖与节流
来源：http://ap.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eq.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://kl.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nx.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fu.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wb.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://he.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mw.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jc.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://eo.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ce.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://io.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rl.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pi.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gx.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zb.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gy.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jq.huixinmuqiang.cn

================================================================================
来源：http://ve.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ta.huixiangedu.cn

================================================================================
来源：http://lq.wgjwhj.cn

[Q01] 创建表
来源：http://ne.hahajie.cn

CREATE TABLE users (
来源：http://qy.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ae.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://sj.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ul.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ck.shxzskj.cn

);
来源：http://ii.szxytkj.cn

[Q02] 创建带外键的表
来源：http://zf.lnxyls.cn

CREATE TABLE orders (
来源：http://fr.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yl.jctech888.com.cn

user_id INT NOT NULL,
来源：http://li.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://ol.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oz.shxzukj.cn

);
来源：http://up.shtwfgs.cn

[Q03] 增加列
来源：http://rb.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://es.shxzskj.cn

[Q04] 修改列类型
来源：http://gf.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oi.521024.cn

[Q05] 重命名列
来源：http://ty.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pf.newstarts.cn

[Q06] 删除列
来源：http://ix.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sx.yuntaijiaju.cn

[Q07] 删除表
来源：http://cz.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://gq.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://ke.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ez.lnxyls.cn

[Q09] 创建唯一索引
来源：http://qs.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mv.nszjky.cn

[Q10] 插入单行
来源：http://zx.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aq.newstarts.cn

[Q11] 一次插入多行
来源：http://ab.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sv.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://ne.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://st.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rx.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://sc.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sg.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://an.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iq.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kr.shxzskj.cn

[Q15] 查询全部
来源：http://qw.huixiangedu.cn

SELECT * FROM users;
来源：http://ls.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://eh.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://vn.chemitech.net.cn

[Q17] 条件查询
来源：http://cd.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yk.shtwfgs.cn

[Q18] 模糊匹配
来源：http://ms.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sl.huixiangedu.cn

[Q19] 范围查询
来源：http://xb.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wi.colortex.cn

[Q20] IN 列表
来源：http://of.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://au.bookmarksfly.cn

[Q21] 空值判断
来源：http://my.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ca.shxzskj.cn

[Q22] 排序
来源：http://hm.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kz.yuexingan06.cn

[Q23] 分页
来源：http://uu.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://my.yuntaijiaju.cn

[Q24] 去重
来源：http://dz.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://ns.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://vl.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zs.wgjwhj.cn

[Q26] 计数
来源：http://au.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://ya.chemitech.net.cn

[Q27] 条件计数
来源：http://cs.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bf.newstarts.cn

[Q28] 求和与平均
来源：http://vt.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jr.chemitech.net.cn

[Q29] 最大最小值
来源：http://ir.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ht.shxzskj.cn

[Q30] 分组统计
来源：http://gh.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ab.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://xm.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://po.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://ep.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ds.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ft.colortex.cn

[Q33] 多列分组
来源：http://gw.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://md.hahajie.cn

[Q34] 每组取第一条
来源：http://qv.bjjhwx.cn

SELECT * FROM (
来源：http://dj.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ab.521024.cn

) t WHERE rn = 1;
来源：http://ip.yuexingan06.cn

[Q35] 内连接
来源：http://cv.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://py.nicolike.cn

[Q36] 左连接
来源：http://kt.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ij.newstarts.cn

[Q37] 右连接
来源：http://ir.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yj.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gl.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fw.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://ma.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mv.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yy.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ds.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://py.shxzukj.cn

[Q41] 多表连接
来源：http://zb.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ec.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://ln.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://bc.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ea.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://yp.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.lnxyls.cn

[Q43] 标量子查询
来源：http://da.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uo.nicolike.cn

[Q44] IN 子查询
来源：http://nk.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ax.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://kz.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dv.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gw.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oj.chemitech.net.cn

[Q47] 与平均值比较
来源：http://cw.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hl.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://lb.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fd.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://qk.asd995.cn

[Q49] 更新单行
来源：http://lk.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cu.chemitech.net.cn

[Q50] 批量更新
来源：http://ii.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yg.gzmigu.cn

[Q51] 用子查询更新
来源：http://er.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hw.haigaiapp.cn

[Q52] 删除指定行
来源：http://rf.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://vo.newstarts.cn

[Q53] 按条件删除
来源：http://op.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ai.huixinmuqiang.cn

[Q54] 清空表
来源：http://lw.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://os.hahajie.cn

[Q55] 排名（并列占位）
来源：http://fw.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://af.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://ro.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://us.shxzskj.cn

[Q57] 行号
来源：http://fx.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nv.yuexingan06.cn

[Q58] 累计求和
来源：http://us.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sn.colortex.cn

[Q59] 分组内累计
来源：http://ws.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ri.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://jo.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ht.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xn.hnjuh.cn

[Q61] 移动平均
来源：http://ta.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kn.colortex.cn

[Q62] 分组占比
来源：http://bn.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eq.panjiajie.cn

[Q63] 开启事务
来源：http://hd.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fy.bookmarksfly.cn

[Q64] 提交事务
来源：http://mj.yuntaijiaju.cn

COMMIT;
来源：http://vu.521024.cn

[Q65] 回滚事务
来源：http://kp.shtwfgs.cn

ROLLBACK;
来源：http://fn.yuexingan06.cn

[Q66] 行锁查询
来源：http://jq.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ra.gzmigu.cn

[Q67] 设置隔离级别
来源：http://nc.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wt.9csxet.cn

[Q68] 保存点
来源：http://he.shxzukj.cn

SAVEPOINT sp1;
来源：http://zp.panjiajie.cn

ROLLBACK TO sp1;
来源：http://vc.521024.cn

[Q69] 查看执行计划
来源：http://zg.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wo.lnxyls.cn

[Q70] 更新统计信息
来源：http://np.muxihuayi.cn

ANALYZE TABLE users;
来源：http://xk.asd995.cn

[Q71] 查看建表语句
来源：http://rc.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xy.newstarts.cn

[Q72] 查看索引
来源：http://cl.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://yz.9csxet.cn

[Q73] 查看表状态
来源：http://cm.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jq.haigaiapp.cn

[Q74] 强制使用索引
来源：http://dm.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ar.hahajie.cn

[Q75] 日期格式化
来源：http://rq.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://na.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://op.panjiajie.cn

[Q76] 按天统计
来源：http://gd.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fd.lnxyls.cn

[Q77] 时间加减
来源：http://ia.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://td.bookmarksfly.cn

[Q78] 当前时间
来源：http://oa.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ho.shxzskj.cn

[Q79] 字符串拼接
来源：http://qg.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ph.hnjuh.cn

[Q80] 字符串截取
来源：http://pg.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nq.yuexingan06.cn

[Q81] 字符串替换
来源：http://uk.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://we.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://lx.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xc.shtwfgs.cn

[Q83] 大小写转换
来源：http://cp.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ii.hahajie.cn

[Q84] 去除首尾空格
来源：http://go.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://wh.szsharing.cn

[Q85] 数值取整
来源：http://jc.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ey.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://yw.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fq.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://gu.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ke.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://er.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kj.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ym.nicolike.cn

[Q89] 判断表是否存在
来源：http://iz.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jn.wgjwhj.cn

[Q90] 生成序号列
来源：http://ef.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fj.panjiajie.cn

================================================================================
来源：http://te.szxytkj.cn

R. Bash 专题
来源：http://py.szxytkj.cn

================================================================================
来源：http://zt.huanxung.cn

[R01] shebang 与严格模式
来源：http://ub.chemitech.net.cn

#!/usr/bin/env bash
来源：http://hh.shtwfgs.cn

set -euo pipefail
来源：http://te.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://sj.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://kc.jctech888.com.cn

[R03] 只读变量
来源：http://na.shxzskj.cn

readonly PI=3.14
来源：http://ry.huanxung.cn

[R04] 位置参数
来源：http://zc.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pm.asd995.cn

[R05] 参数默认值
来源：http://ob.huixinmuqiang.cn

name="${1:-default}"
来源：http://yk.szxytkj.cn

[R06] 判断命令是否存在
来源：http://nb.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tw.panjiajie.cn

[R07] if 判断文件
来源：http://po.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://em.shxzukj.cn

[R08] 数值比较
来源：http://pb.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ck.chemitech.net.cn

[R09] 字符串比较
来源：http://pw.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kv.jctech888.com.cn

[R10] 正则匹配
来源：http://wj.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hj.colortex.cn

[R11] case 多分支
来源：http://pm.nicolike.cn

case "$1" in
来源：http://cr.panjiajie.cn

start) echo "启动" ;;
来源：http://hz.nicolike.cn

stop)  echo "停止" ;;
来源：http://rl.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://fd.panjiajie.cn

esac
来源：http://fk.huanxung.cn

[R12] for 遍历文件
来源：http://gb.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://mt.gzmigu.cn

[R13] for 计数循环
来源：http://ot.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://ni.521024.cn

[R14] C 风格 for
来源：http://jo.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oj.muxihuayi.cn

[R15] while 逐行读文件
来源：http://ws.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bu.bjjhwx.cn

[R16] until 等待条件
来源：http://np.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ej.panjiajie.cn

[R17] 数组定义与取值
来源：http://wt.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sq.huixiangedu.cn

[R18] 遍历数组
来源：http://qf.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ba.hnjuh.cn

[R19] 数组长度
来源：http://pp.chemitech.net.cn

echo "${#arr[@]}"
来源：http://aj.nicolike.cn

[R20] 关联数组（字典）
来源：http://lq.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://if.9csxet.cn

[R21] 字符串长度
来源：http://fm.huixiangedu.cn

echo "${#s}"
来源：http://js.bjjhwx.cn

[R22] 截取子串
来源：http://da.newstarts.cn

echo "${s:0:5}"
来源：http://ok.newstarts.cn

[R23] 字符串替换
来源：http://da.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fi.wgjwhj.cn

[R24] 大小写转换
来源：http://ok.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qd.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://xe.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dv.huanxung.cn

[R26] 命令替换
来源：http://hf.szsharing.cn

now=$(date +%F); echo "$now"
来源：http://rp.gzmigu.cn

[R27] 算术展开
来源：http://qy.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://rl.bookmarksfly.cn

[R28] 浮点运算
来源：http://hr.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://ex.bjjhwx.cn

[R29] 定义函数
来源：http://uq.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jz.shxzukj.cn

[R30] 函数返回状态码
来源：http://ak.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ap.521024.cn

[R31] 局部变量
来源：http://tb.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://fm.huixiangedu.cn

[R32] 参数个数校验
来源：http://qb.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://so.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://am.jctech888.com.cn


<!-- 参考信息 -->