代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ob.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://td.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mj.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://by.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ba.haigaiapp.cn

TS:   if (x == null) {}
来源：http://wv.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sf.gzmigu.cn

Go:   if x == nil {}
来源：http://eq.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://if.muxihuayi.cn

C#:   if (x is null) {}
来源：http://iq.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://wl.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kh.colortex.cn

PHP:  // 手写时间戳比较
来源：http://ft.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tu.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://il.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rp.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fx.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bl.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yk.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://ip.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://de.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://es.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xm.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ds.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hv.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ie.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sc.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lj.huixiangedu.cn

================================================================================
来源：http://go.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://th.9csxet.cn

================================================================================
来源：http://ni.jctech888.com.cn

[Q01] 创建表
来源：http://mu.bjjhwx.cn

CREATE TABLE users (
来源：http://yg.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xe.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://rs.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://fy.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pp.szxytkj.cn

);
来源：http://qk.szsharing.cn

[Q02] 创建带外键的表
来源：http://db.szxytkj.cn

CREATE TABLE orders (
来源：http://fj.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gk.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://ct.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://vw.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tz.wgjwhj.cn

);
来源：http://ki.gzmigu.cn

[Q03] 增加列
来源：http://bo.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kz.hahajie.cn

[Q04] 修改列类型
来源：http://cw.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fp.nicolike.cn

[Q05] 重命名列
来源：http://xu.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mu.huanxung.cn

[Q06] 删除列
来源：http://ba.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xg.bjjhwx.cn

[Q07] 删除表
来源：http://ly.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://zy.huixiangedu.cn

[Q08] 创建普通索引
来源：http://ui.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iv.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://uu.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mv.shxzukj.cn

[Q10] 插入单行
来源：http://vr.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ol.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://gx.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aq.521024.cn

[Q12] 插入后取自增 ID
来源：http://ei.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ak.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qz.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://yj.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ss.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://pn.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yf.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kg.9csxet.cn

[Q15] 查询全部
来源：http://as.huixiangedu.cn

SELECT * FROM users;
来源：http://fa.muxihuayi.cn

[Q16] 查询指定列
来源：http://vj.bjjhwx.cn

SELECT id, name FROM users;
来源：http://vv.lnxyls.cn

[Q17] 条件查询
来源：http://pq.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oi.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://bv.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://as.521024.cn

[Q19] 范围查询
来源：http://kt.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fg.panjiajie.cn

[Q20] IN 列表
来源：http://ge.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vf.yuntaijiaju.cn

[Q21] 空值判断
来源：http://qf.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fs.nicolike.cn

[Q22] 排序
来源：http://bg.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ss.jctech888.com.cn

[Q23] 分页
来源：http://xv.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ee.nicolike.cn

[Q24] 去重
来源：http://kk.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://pf.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://xc.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uk.nszjky.cn

[Q26] 计数
来源：http://oc.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://jb.chemitech.net.cn

[Q27] 条件计数
来源：http://oy.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gt.lnxyls.cn

[Q28] 求和与平均
来源：http://hd.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sa.jctech888.com.cn

[Q29] 最大最小值
来源：http://dw.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bl.huanxung.cn

[Q30] 分组统计
来源：http://pn.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ip.szsharing.cn

[Q31] 分组后过滤
来源：http://iv.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tg.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://so.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yz.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ag.newstarts.cn

[Q33] 多列分组
来源：http://cx.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pb.wgjwhj.cn

[Q34] 每组取第一条
来源：http://ck.bookmarksfly.cn

SELECT * FROM (
来源：http://rs.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dc.huixiangedu.cn

) t WHERE rn = 1;
来源：http://dq.colortex.cn

[Q35] 内连接
来源：http://bn.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fo.jctech888.com.cn

[Q36] 左连接
来源：http://tg.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sc.huanxung.cn

[Q37] 右连接
来源：http://yy.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fw.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xq.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yc.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ga.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lf.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cr.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sf.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yx.szxytkj.cn

[Q41] 多表连接
来源：http://wl.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qv.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ek.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://sj.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://zf.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://jp.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ou.bjjhwx.cn

[Q43] 标量子查询
来源：http://cc.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sy.chemitech.net.cn

[Q44] IN 子查询
来源：http://np.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lp.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://iy.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hr.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://el.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zj.panjiajie.cn

[Q47] 与平均值比较
来源：http://rx.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ld.colortex.cn

[Q48] CTE 公用表表达式
来源：http://oe.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://am.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://ze.521024.cn

[Q49] 更新单行
来源：http://xm.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yi.bjjhwx.cn

[Q50] 批量更新
来源：http://ki.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vz.hnjuh.cn

[Q51] 用子查询更新
来源：http://sm.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xc.chemitech.net.cn

[Q52] 删除指定行
来源：http://iu.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://kv.szxytkj.cn

[Q53] 按条件删除
来源：http://co.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qf.bookmarksfly.cn

[Q54] 清空表
来源：http://zh.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://ha.nszjky.cn

[Q55] 排名（并列占位）
来源：http://kt.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ct.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ry.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pz.bookmarksfly.cn

[Q57] 行号
来源：http://ot.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jt.huanxung.cn

[Q58] 累计求和
来源：http://de.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sd.9csxet.cn

[Q59] 分组内累计
来源：http://wu.lnxyls.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uc.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://uc.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lq.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://in.nicolike.cn

[Q61] 移动平均
来源：http://gi.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://of.huanxung.cn

[Q62] 分组占比
来源：http://dk.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xz.yuexingan06.cn

[Q63] 开启事务
来源：http://lx.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ym.szxytkj.cn

[Q64] 提交事务
来源：http://tr.bjjhwx.cn

COMMIT;
来源：http://jb.shxzskj.cn

[Q65] 回滚事务
来源：http://gw.shxzskj.cn

ROLLBACK;
来源：http://dg.9csxet.cn

[Q66] 行锁查询
来源：http://os.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bl.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://zh.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zs.shtwfgs.cn

[Q68] 保存点
来源：http://ys.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://kc.shxzukj.cn

ROLLBACK TO sp1;
来源：http://vz.muxihuayi.cn

[Q69] 查看执行计划
来源：http://pf.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ud.shxzukj.cn

[Q70] 更新统计信息
来源：http://ad.chemitech.net.cn

ANALYZE TABLE users;
来源：http://ro.chemitech.net.cn

[Q71] 查看建表语句
来源：http://tn.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gw.hahajie.cn

[Q72] 查看索引
来源：http://mg.shxzskj.cn

SHOW INDEX FROM users;
来源：http://vy.huixiangedu.cn

[Q73] 查看表状态
来源：http://dc.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ni.haigaiapp.cn

[Q74] 强制使用索引
来源：http://wi.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aj.chemitech.net.cn

[Q75] 日期格式化
来源：http://eg.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mo.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rc.asd995.cn

[Q76] 按天统计
来源：http://km.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ua.huixiangedu.cn

[Q77] 时间加减
来源：http://pf.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ya.panjiajie.cn

[Q78] 当前时间
来源：http://jw.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gv.hnjuh.cn

[Q79] 字符串拼接
来源：http://re.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://il.nicolike.cn

[Q80] 字符串截取
来源：http://ut.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xf.nicolike.cn

[Q81] 字符串替换
来源：http://mv.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pn.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://zj.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kv.shxzukj.cn

[Q83] 大小写转换
来源：http://hj.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qx.szsharing.cn

[Q84] 去除首尾空格
来源：http://fy.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://dw.nicolike.cn

[Q85] 数值取整
来源：http://ia.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fe.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://ao.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ft.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://gs.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hq.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://zt.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kx.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kp.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://gd.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nc.bookmarksfly.cn

[Q90] 生成序号列
来源：http://hy.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ow.9csxet.cn

================================================================================
来源：http://fd.jianghongdianzi.cn

R. Bash 专题
来源：http://uk.haigaiapp.cn

================================================================================
来源：http://km.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://vx.gzmigu.cn

#!/usr/bin/env bash
来源：http://uc.521024.cn

set -euo pipefail
来源：http://ky.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://pm.panjiajie.cn

name="Tom"; echo "$name"
来源：http://sz.jianghongdianzi.cn

[R03] 只读变量
来源：http://sn.yuntaijiaju.cn

readonly PI=3.14
来源：http://eu.colortex.cn

[R04] 位置参数
来源：http://bu.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sv.muxihuayi.cn

[R05] 参数默认值
来源：http://xm.huixiangedu.cn

name="${1:-default}"
来源：http://xd.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://wf.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://am.bookmarksfly.cn

[R07] if 判断文件
来源：http://jc.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gw.bjjhwx.cn

[R08] 数值比较
来源：http://hz.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ya.panjiajie.cn

[R09] 字符串比较
来源：http://qx.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rk.colortex.cn

[R10] 正则匹配
来源：http://re.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ni.yuntaijiaju.cn

[R11] case 多分支
来源：http://em.huixinmuqiang.cn

case "$1" in
来源：http://yq.muxihuayi.cn

start) echo "启动" ;;
来源：http://aj.nicolike.cn

stop)  echo "停止" ;;
来源：http://ku.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://zt.lnxyls.cn

esac
来源：http://tk.panjiajie.cn

[R12] for 遍历文件
来源：http://no.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://os.shxzskj.cn

[R13] for 计数循环
来源：http://kz.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://bt.szxytkj.cn

[R14] C 风格 for
来源：http://iv.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pa.jctech888.com.cn

[R15] while 逐行读文件
来源：http://kg.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ta.gzmigu.cn

[R16] until 等待条件
来源：http://vh.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://da.9csxet.cn

[R17] 数组定义与取值
来源：http://ti.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mw.huixinmuqiang.cn

[R18] 遍历数组
来源：http://eo.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jy.szxytkj.cn

[R19] 数组长度
来源：http://tf.huanxung.cn

echo "${#arr[@]}"
来源：http://ij.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://ys.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vt.colortex.cn

[R21] 字符串长度
来源：http://mr.jctech888.com.cn

echo "${#s}"
来源：http://wr.szxytkj.cn

[R22] 截取子串
来源：http://kq.szsharing.cn

echo "${s:0:5}"
来源：http://xh.huanxung.cn

[R23] 字符串替换
来源：http://er.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wh.shtwfgs.cn

[R24] 大小写转换
来源：http://sw.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xk.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://bq.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ma.colortex.cn

[R26] 命令替换
来源：http://au.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://ic.muxihuayi.cn

[R27] 算术展开
来源：http://av.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://ek.szsharing.cn

[R28] 浮点运算
来源：http://fm.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://be.nicolike.cn

[R29] 定义函数
来源：http://li.newstarts.cn


<!-- 参考信息 -->