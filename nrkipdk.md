代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cu.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yo.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wq.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://lx.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ss.szxytkj.cn

TS:   if (x == null) {}
来源：http://hw.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ej.colortex.cn

Go:   if x == nil {}
来源：http://dz.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yw.nicolike.cn

C#:   if (x is null) {}
来源：http://aw.shxzskj.cn

[P07] 防抖与节流
来源：http://tu.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lj.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://si.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uc.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dd.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://od.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qm.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ph.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qc.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://vd.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jo.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kw.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wr.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bm.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xt.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cd.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bo.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qu.chemitech.net.cn

================================================================================
来源：http://fu.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mz.shtwfgs.cn

================================================================================
来源：http://ge.newstarts.cn

[Q01] 创建表
来源：http://jf.gzmigu.cn

CREATE TABLE users (
来源：http://lj.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yx.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://xi.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://nx.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bs.shxzskj.cn

);
来源：http://ol.szxytkj.cn

[Q02] 创建带外键的表
来源：http://ob.panjiajie.cn

CREATE TABLE orders (
来源：http://mm.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://da.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://px.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://ul.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ll.nszjky.cn

);
来源：http://bf.muxihuayi.cn

[Q03] 增加列
来源：http://fv.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vy.bjjhwx.cn

[Q04] 修改列类型
来源：http://tp.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vs.newstarts.cn

[Q05] 重命名列
来源：http://wc.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jw.shxzukj.cn

[Q06] 删除列
来源：http://gu.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hu.jctech888.com.cn

[Q07] 删除表
来源：http://bm.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://vv.haigaiapp.cn

[Q08] 创建普通索引
来源：http://uu.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ur.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://zz.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ie.panjiajie.cn

[Q10] 插入单行
来源：http://wq.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vg.chemitech.net.cn

[Q11] 一次插入多行
来源：http://vg.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tp.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://ov.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xq.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://am.szsharing.cn

[Q13] 忽略重复插入
来源：http://id.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sj.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://bi.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ib.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gg.hnjuh.cn

[Q15] 查询全部
来源：http://bh.nszjky.cn

SELECT * FROM users;
来源：http://vp.szxytkj.cn

[Q16] 查询指定列
来源：http://qj.9csxet.cn

SELECT id, name FROM users;
来源：http://tf.wgjwhj.cn

[Q17] 条件查询
来源：http://st.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xp.chemitech.net.cn

[Q18] 模糊匹配
来源：http://gc.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qy.nicolike.cn

[Q19] 范围查询
来源：http://ki.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://un.yuexingan06.cn

[Q20] IN 列表
来源：http://ax.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bo.gzmigu.cn

[Q21] 空值判断
来源：http://sh.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ep.hahajie.cn

[Q22] 排序
来源：http://rp.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://io.bjjhwx.cn

[Q23] 分页
来源：http://ic.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ij.szxytkj.cn

[Q24] 去重
来源：http://to.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://tj.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://ej.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oa.nszjky.cn

[Q26] 计数
来源：http://by.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://dc.yuexingan06.cn

[Q27] 条件计数
来源：http://dn.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sa.gzmigu.cn

[Q28] 求和与平均
来源：http://za.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xv.shtwfgs.cn

[Q29] 最大最小值
来源：http://zu.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hb.chemitech.net.cn

[Q30] 分组统计
来源：http://kx.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ks.newstarts.cn

[Q31] 分组后过滤
来源：http://ff.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cs.huanxung.cn

[Q32] 分组拼接字符串
来源：http://hj.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wk.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zn.gzmigu.cn

[Q33] 多列分组
来源：http://ve.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xd.jctech888.com.cn

[Q34] 每组取第一条
来源：http://rq.muxihuayi.cn

SELECT * FROM (
来源：http://ry.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nz.colortex.cn

) t WHERE rn = 1;
来源：http://ix.shxzskj.cn

[Q35] 内连接
来源：http://lf.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eo.shxzukj.cn

[Q36] 左连接
来源：http://xh.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://si.newstarts.cn

[Q37] 右连接
来源：http://vz.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gd.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wg.haigaiapp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://um.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://jn.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gb.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wp.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yk.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zl.521024.cn

[Q41] 多表连接
来源：http://zh.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ld.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://lg.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ab.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://kq.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://sr.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hf.hnjuh.cn

[Q43] 标量子查询
来源：http://uy.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ln.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://pj.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://np.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://fd.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://do.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pu.yuexingan06.cn

[Q47] 与平均值比较
来源：http://cj.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gg.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://vu.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cl.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://bc.nszjky.cn

[Q49] 更新单行
来源：http://rv.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wf.shtwfgs.cn

[Q50] 批量更新
来源：http://ph.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wj.lnxyls.cn

[Q51] 用子查询更新
来源：http://ak.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jr.shxzukj.cn

[Q52] 删除指定行
来源：http://lh.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://ut.bookmarksfly.cn

[Q53] 按条件删除
来源：http://ev.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bb.haigaiapp.cn

[Q54] 清空表
来源：http://xh.yuexingan06.cn

TRUNCATE TABLE logs;
来源：http://ql.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://uk.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jl.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://pi.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ee.lnxyls.cn

[Q57] 行号
来源：http://gw.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pm.wgjwhj.cn

[Q58] 累计求和
来源：http://hp.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jw.gzmigu.cn

[Q59] 分组内累计
来源：http://ki.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ax.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://zc.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mn.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tz.haigaiapp.cn

[Q61] 移动平均
来源：http://hn.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gy.jianghongdianzi.cn

[Q62] 分组占比
来源：http://ov.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://of.haigaiapp.cn

[Q63] 开启事务
来源：http://ss.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yj.asd995.cn

[Q64] 提交事务
来源：http://sh.chemitech.net.cn

COMMIT;
来源：http://bm.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://yf.hnjuh.cn

ROLLBACK;
来源：http://kr.nszjky.cn

[Q66] 行锁查询
来源：http://fa.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://to.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://lb.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gw.wgjwhj.cn

[Q68] 保存点
来源：http://wz.szsharing.cn

SAVEPOINT sp1;
来源：http://ss.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://nf.szxytkj.cn

[Q69] 查看执行计划
来源：http://oh.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://do.szxytkj.cn

[Q70] 更新统计信息
来源：http://jz.jctech888.com.cn

ANALYZE TABLE users;
来源：http://zc.haigaiapp.cn

[Q71] 查看建表语句
来源：http://lh.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://br.yuexingan06.cn

[Q72] 查看索引
来源：http://pa.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://zd.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://bt.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lo.lnxyls.cn

[Q74] 强制使用索引
来源：http://cb.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sp.hahajie.cn

[Q75] 日期格式化
来源：http://qz.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hu.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ib.bookmarksfly.cn

[Q76] 按天统计
来源：http://hb.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ai.gzmigu.cn

[Q77] 时间加减
来源：http://ac.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pm.huanxung.cn

[Q78] 当前时间
来源：http://ka.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wg.gzmigu.cn

[Q79] 字符串拼接
来源：http://nn.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://if.szxytkj.cn

[Q80] 字符串截取
来源：http://jm.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cu.jctech888.com.cn

[Q81] 字符串替换
来源：http://bs.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gd.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://hl.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ch.colortex.cn

[Q83] 大小写转换
来源：http://fz.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lj.szsharing.cn

[Q84] 去除首尾空格
来源：http://wi.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://na.huixinmuqiang.cn

[Q85] 数值取整
来源：http://ez.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zg.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://rb.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vx.9csxet.cn

[Q87] JSON 字段做条件
来源：http://zg.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://se.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://ui.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ac.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zs.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://gf.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://js.bjjhwx.cn

[Q90] 生成序号列
来源：http://dn.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ax.colortex.cn

================================================================================
来源：http://ve.gzmigu.cn

R. Bash 专题
来源：http://rk.jctech888.com.cn

================================================================================
来源：http://wa.newstarts.cn

[R01] shebang 与严格模式
来源：http://vz.szxytkj.cn

#!/usr/bin/env bash
来源：http://fb.shxzskj.cn

set -euo pipefail
来源：http://uq.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://nw.nicolike.cn

name="Tom"; echo "$name"
来源：http://oy.haigaiapp.cn

[R03] 只读变量
来源：http://pk.shxzukj.cn

readonly PI=3.14
来源：http://ma.colortex.cn

[R04] 位置参数
来源：http://qv.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sy.521024.cn

[R05] 参数默认值
来源：http://rh.chemitech.net.cn

name="${1:-default}"
来源：http://se.nicolike.cn

[R06] 判断命令是否存在
来源：http://no.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jk.9csxet.cn

[R07] if 判断文件
来源：http://se.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qk.lnxyls.cn

[R08] 数值比较
来源：http://tr.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kq.hnjuh.cn

[R09] 字符串比较
来源：http://jk.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uy.bjjhwx.cn

[R10] 正则匹配
来源：http://nn.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nu.bjjhwx.cn

[R11] case 多分支
来源：http://sr.szsharing.cn

case "$1" in
来源：http://ek.wgjwhj.cn

start) echo "启动" ;;
来源：http://wc.huanxung.cn

stop)  echo "停止" ;;
来源：http://xx.szsharing.cn

*)     echo "未知命令" ;;
来源：http://un.huixiangedu.cn

esac
来源：http://qv.muxihuayi.cn

[R12] for 遍历文件
来源：http://cj.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://pt.shxzskj.cn

[R13] for 计数循环
来源：http://rd.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://de.521024.cn

[R14] C 风格 for
来源：http://jn.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://na.9csxet.cn

[R15] while 逐行读文件
来源：http://dp.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ww.asd995.cn

[R16] until 等待条件
来源：http://fg.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://am.hnjuh.cn

[R17] 数组定义与取值
来源：http://sj.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uq.lnxyls.cn

[R18] 遍历数组
来源：http://br.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xd.gzmigu.cn

[R19] 数组长度
来源：http://bt.nicolike.cn

echo "${#arr[@]}"
来源：http://ei.hnjuh.cn

[R20] 关联数组（字典）
来源：http://nq.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vt.bookmarksfly.cn

[R21] 字符串长度
来源：http://sj.chemitech.net.cn

echo "${#s}"
来源：http://oi.huixiangedu.cn

[R22] 截取子串
来源：http://ms.haigaiapp.cn

echo "${s:0:5}"
来源：http://qt.asd995.cn

[R23] 字符串替换
来源：http://fu.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://io.chemitech.net.cn

[R24] 大小写转换
来源：http://gb.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zh.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://xm.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yr.jianghongdianzi.cn

[R26] 命令替换
来源：http://kc.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://dw.asd995.cn

[R27] 算术展开
来源：http://hc.colortex.cn

echo $((1 + 2 * 3))
来源：http://jy.colortex.cn

[R28] 浮点运算
来源：http://bx.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://zh.colortex.cn

[R29] 定义函数
来源：http://sv.jianghongdianzi.cn


<!-- 参考信息 -->