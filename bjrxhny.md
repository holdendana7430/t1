代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://we.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zo.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wn.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://rr.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://be.muxihuayi.cn

TS:   if (x == null) {}
来源：http://je.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rf.wgjwhj.cn

Go:   if x == nil {}
来源：http://om.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xc.huanxung.cn

C#:   if (x is null) {}
来源：http://wy.haigaiapp.cn

[P07] 防抖与节流
来源：http://nl.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hd.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://lq.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mq.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://az.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ff.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://er.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rk.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oa.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://qp.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pu.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://up.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hq.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wo.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rt.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qu.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rk.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gf.shxzukj.cn

================================================================================
来源：http://yi.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://en.asd995.cn

================================================================================
来源：http://rx.jianghongdianzi.cn

[Q01] 创建表
来源：http://nq.colortex.cn

CREATE TABLE users (
来源：http://oo.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xl.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://zr.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://iv.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ss.shxzskj.cn

);
来源：http://ta.asd995.cn

[Q02] 创建带外键的表
来源：http://sv.huanxung.cn

CREATE TABLE orders (
来源：http://rr.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pn.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://gg.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://ex.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tj.colortex.cn

);
来源：http://cu.huanxung.cn

[Q03] 增加列
来源：http://yi.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pd.lnxyls.cn

[Q04] 修改列类型
来源：http://gd.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dp.bjjhwx.cn

[Q05] 重命名列
来源：http://xj.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xn.shxzukj.cn

[Q06] 删除列
来源：http://gn.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kl.nicolike.cn

[Q07] 删除表
来源：http://lp.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://cj.huixiangedu.cn

[Q08] 创建普通索引
来源：http://qd.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zc.hnjuh.cn

[Q09] 创建唯一索引
来源：http://cy.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ez.shxzukj.cn

[Q10] 插入单行
来源：http://ix.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dm.jctech888.com.cn

[Q11] 一次插入多行
来源：http://eg.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iz.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://qc.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ep.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gh.hahajie.cn

[Q13] 忽略重复插入
来源：http://nw.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wr.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://cp.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lc.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jp.yuexingan06.cn

[Q15] 查询全部
来源：http://yd.huixiangedu.cn

SELECT * FROM users;
来源：http://mh.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://cd.chemitech.net.cn

SELECT id, name FROM users;
来源：http://qu.9csxet.cn

[Q17] 条件查询
来源：http://xo.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vv.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://td.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tl.shxzukj.cn

[Q19] 范围查询
来源：http://eb.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://be.bookmarksfly.cn

[Q20] IN 列表
来源：http://ia.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ih.huanxung.cn

[Q21] 空值判断
来源：http://gl.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aj.hahajie.cn

[Q22] 排序
来源：http://fl.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ct.panjiajie.cn

[Q23] 分页
来源：http://jr.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tu.huixinmuqiang.cn

[Q24] 去重
来源：http://we.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://kr.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://dt.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ce.hahajie.cn

[Q26] 计数
来源：http://hw.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://na.szxytkj.cn

[Q27] 条件计数
来源：http://pd.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://by.gzmigu.cn

[Q28] 求和与平均
来源：http://zh.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ll.wgjwhj.cn

[Q29] 最大最小值
来源：http://ph.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pq.szsharing.cn

[Q30] 分组统计
来源：http://nm.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vd.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://ig.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sh.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://tk.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ng.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://me.gzmigu.cn

[Q33] 多列分组
来源：http://cn.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dp.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://bd.jianghongdianzi.cn

SELECT * FROM (
来源：http://ri.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rd.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://gc.yuntaijiaju.cn

[Q35] 内连接
来源：http://vk.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xr.bjjhwx.cn

[Q36] 左连接
来源：http://nf.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xe.shxzukj.cn

[Q37] 右连接
来源：http://is.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cg.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xx.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lv.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://rv.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iy.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sa.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hu.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ln.nszjky.cn

[Q41] 多表连接
来源：http://kq.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ss.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://bj.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://aa.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://sd.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://zn.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xn.haigaiapp.cn

[Q43] 标量子查询
来源：http://lx.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jv.yuexingan06.cn

[Q44] IN 子查询
来源：http://ds.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fa.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://sm.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vv.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mo.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tq.asd995.cn

[Q47] 与平均值比较
来源：http://tz.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zw.asd995.cn

[Q48] CTE 公用表表达式
来源：http://ne.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jf.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://su.colortex.cn

[Q49] 更新单行
来源：http://th.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dr.hnjuh.cn

[Q50] 批量更新
来源：http://it.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pw.chemitech.net.cn

[Q51] 用子查询更新
来源：http://ns.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jm.shtwfgs.cn

[Q52] 删除指定行
来源：http://cu.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://ot.huanxung.cn

[Q53] 按条件删除
来源：http://yc.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wi.hahajie.cn

[Q54] 清空表
来源：http://by.shxzukj.cn

TRUNCATE TABLE logs;
来源：http://zb.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://pf.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ff.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://yl.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xf.jianghongdianzi.cn

[Q57] 行号
来源：http://cf.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vn.lnxyls.cn

[Q58] 累计求和
来源：http://hk.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sn.bookmarksfly.cn

[Q59] 分组内累计
来源：http://cf.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kn.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://xl.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sd.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rl.haigaiapp.cn

[Q61] 移动平均
来源：http://ns.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hn.9csxet.cn

[Q62] 分组占比
来源：http://iy.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gi.jctech888.com.cn

[Q63] 开启事务
来源：http://nr.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fc.9csxet.cn

[Q64] 提交事务
来源：http://fw.wgjwhj.cn

COMMIT;
来源：http://nw.muxihuayi.cn

[Q65] 回滚事务
来源：http://vm.nicolike.cn

ROLLBACK;
来源：http://va.huanxung.cn

[Q66] 行锁查询
来源：http://bo.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dv.hahajie.cn

[Q67] 设置隔离级别
来源：http://ao.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sm.hahajie.cn

[Q68] 保存点
来源：http://qd.521024.cn

SAVEPOINT sp1;
来源：http://sm.gzmigu.cn

ROLLBACK TO sp1;
来源：http://gj.shxzukj.cn

[Q69] 查看执行计划
来源：http://sc.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qb.colortex.cn

[Q70] 更新统计信息
来源：http://fv.haigaiapp.cn

ANALYZE TABLE users;
来源：http://kd.521024.cn

[Q71] 查看建表语句
来源：http://da.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jn.wgjwhj.cn

[Q72] 查看索引
来源：http://uj.hnjuh.cn

SHOW INDEX FROM users;
来源：http://ok.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://kv.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tr.lnxyls.cn

[Q74] 强制使用索引
来源：http://um.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gh.hahajie.cn

[Q75] 日期格式化
来源：http://lw.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://el.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hm.shxzukj.cn

[Q76] 按天统计
来源：http://yu.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ow.colortex.cn

[Q77] 时间加减
来源：http://kk.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://su.newstarts.cn

[Q78] 当前时间
来源：http://cr.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kk.521024.cn

[Q79] 字符串拼接
来源：http://sw.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ht.wgjwhj.cn

[Q80] 字符串截取
来源：http://up.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ae.huanxung.cn

[Q81] 字符串替换
来源：http://iu.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mh.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://lx.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wm.shxzskj.cn

[Q83] 大小写转换
来源：http://kc.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tu.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://rc.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://yk.huixinmuqiang.cn

[Q85] 数值取整
来源：http://ez.szxytkj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yo.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://lw.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ko.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://ro.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vd.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://ac.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iw.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wv.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://gu.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bt.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://ae.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gq.hahajie.cn

================================================================================
来源：http://yz.hnjuh.cn

R. Bash 专题
来源：http://wj.asd995.cn

================================================================================
来源：http://pp.shxzskj.cn

[R01] shebang 与严格模式
来源：http://we.chemitech.net.cn

#!/usr/bin/env bash
来源：http://ay.panjiajie.cn

set -euo pipefail
来源：http://fq.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://zf.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://kj.521024.cn

[R03] 只读变量
来源：http://ta.chemitech.net.cn

readonly PI=3.14
来源：http://zz.shtwfgs.cn

[R04] 位置参数
来源：http://an.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hs.hahajie.cn

[R05] 参数默认值
来源：http://bt.jianghongdianzi.cn

name="${1:-default}"
来源：http://li.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://zp.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bi.hnjuh.cn

[R07] if 判断文件
来源：http://ql.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ns.szsharing.cn

[R08] 数值比较
来源：http://vw.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mf.bjjhwx.cn

[R09] 字符串比较
来源：http://zz.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wf.panjiajie.cn

[R10] 正则匹配
来源：http://xc.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xs.newstarts.cn

[R11] case 多分支
来源：http://fp.huixiangedu.cn

case "$1" in
来源：http://ak.yuexingan06.cn

start) echo "启动" ;;
来源：http://xk.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://gx.szsharing.cn

*)     echo "未知命令" ;;
来源：http://ad.nicolike.cn

esac
来源：http://eh.nszjky.cn

[R12] for 遍历文件
来源：http://gt.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://eh.jianghongdianzi.cn

[R13] for 计数循环
来源：http://go.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://nc.lnxyls.cn

[R14] C 风格 for
来源：http://jg.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rc.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://zw.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bt.shxzukj.cn

[R16] until 等待条件
来源：http://us.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hi.hahajie.cn

[R17] 数组定义与取值
来源：http://ta.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vj.jctech888.com.cn

[R18] 遍历数组
来源：http://xu.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sf.szsharing.cn

[R19] 数组长度
来源：http://xr.shtwfgs.cn

echo "${#arr[@]}"
来源：http://kx.nszjky.cn

[R20] 关联数组（字典）
来源：http://zk.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://my.szxytkj.cn

[R21] 字符串长度
来源：http://lz.lnxyls.cn

echo "${#s}"
来源：http://jj.hahajie.cn

[R22] 截取子串
来源：http://lb.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://wg.jianghongdianzi.cn

[R23] 字符串替换
来源：http://cu.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eb.bookmarksfly.cn

[R24] 大小写转换
来源：http://el.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uo.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://av.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jj.521024.cn

[R26] 命令替换
来源：http://sy.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://fg.hnjuh.cn

[R27] 算术展开
来源：http://bw.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://av.huixiangedu.cn

[R28] 浮点运算
来源：http://cz.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://ii.jctech888.com.cn

[R29] 定义函数
来源：http://df.shtwfgs.cn


<!-- 参考信息 -->