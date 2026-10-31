代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://nv.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ua.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ib.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ry.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iu.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://io.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kd.newstarts.cn

Ruby: a == b
来源：http://sd.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bp.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zb.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nb.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://jq.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zl.jctech888.com.cn

TS:   if (x == null) {}
来源：http://sa.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gf.bjjhwx.cn

Go:   if x == nil {}
来源：http://ox.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xd.nicolike.cn

C#:   if (x is null) {}
来源：http://wy.asd995.cn

[P07] 防抖与节流
来源：http://pc.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nj.521024.cn

PHP:  // 手写时间戳比较
来源：http://bs.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vq.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://de.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eh.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bn.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://op.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dp.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://jr.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ny.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qt.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pc.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kn.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mj.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xi.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dk.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ct.newstarts.cn

================================================================================
来源：http://ht.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gg.521024.cn

================================================================================
来源：http://lq.bookmarksfly.cn

[Q01] 创建表
来源：http://pi.muxihuayi.cn

CREATE TABLE users (
来源：http://mt.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hy.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://rq.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://xt.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ye.jctech888.com.cn

);
来源：http://ra.hahajie.cn

[Q02] 创建带外键的表
来源：http://hn.huanxung.cn

CREATE TABLE orders (
来源：http://pc.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cg.yuexingan06.cn

user_id INT NOT NULL,
来源：http://rw.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://jc.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qk.chemitech.net.cn

);
来源：http://vo.bookmarksfly.cn

[Q03] 增加列
来源：http://aj.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qg.colortex.cn

[Q04] 修改列类型
来源：http://bh.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bc.huixiangedu.cn

[Q05] 重命名列
来源：http://jk.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gr.chemitech.net.cn

[Q06] 删除列
来源：http://un.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oe.szxytkj.cn

[Q07] 删除表
来源：http://ao.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://qh.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://by.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://er.asd995.cn

[Q09] 创建唯一索引
来源：http://sl.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dq.bjjhwx.cn

[Q10] 插入单行
来源：http://pb.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://la.asd995.cn

[Q11] 一次插入多行
来源：http://bk.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tj.521024.cn

[Q12] 插入后取自增 ID
来源：http://jv.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kv.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mu.9csxet.cn

[Q13] 忽略重复插入
来源：http://nd.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ws.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://tk.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://so.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://am.nicolike.cn

[Q15] 查询全部
来源：http://ug.bjjhwx.cn

SELECT * FROM users;
来源：http://rx.haigaiapp.cn

[Q16] 查询指定列
来源：http://im.yuexingan06.cn

SELECT id, name FROM users;
来源：http://ue.huixiangedu.cn

[Q17] 条件查询
来源：http://eu.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xo.szsharing.cn

[Q18] 模糊匹配
来源：http://dp.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rf.hnjuh.cn

[Q19] 范围查询
来源：http://dg.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xh.9csxet.cn

[Q20] IN 列表
来源：http://rc.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pp.hnjuh.cn

[Q21] 空值判断
来源：http://jh.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ns.szsharing.cn

[Q22] 排序
来源：http://an.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yz.huanxung.cn

[Q23] 分页
来源：http://km.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uz.nszjky.cn

[Q24] 去重
来源：http://do.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://yx.shxzskj.cn

[Q25] 只取前 N 条
来源：http://hu.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fv.colortex.cn

[Q26] 计数
来源：http://gh.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://vz.colortex.cn

[Q27] 条件计数
来源：http://mv.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ou.gzmigu.cn

[Q28] 求和与平均
来源：http://rv.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://no.hnjuh.cn

[Q29] 最大最小值
来源：http://ho.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iz.szxytkj.cn

[Q30] 分组统计
来源：http://sg.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://np.muxihuayi.cn

[Q31] 分组后过滤
来源：http://ue.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wu.9csxet.cn

[Q32] 分组拼接字符串
来源：http://uy.hahajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wl.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bd.shxzskj.cn

[Q33] 多列分组
来源：http://ra.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ol.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://eh.szsharing.cn

SELECT * FROM (
来源：http://ga.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ls.szsharing.cn

) t WHERE rn = 1;
来源：http://rf.chemitech.net.cn

[Q35] 内连接
来源：http://ec.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ra.nicolike.cn

[Q36] 左连接
来源：http://ih.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hm.nicolike.cn

[Q37] 右连接
来源：http://ez.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xw.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yt.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ex.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://bg.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ud.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hb.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cq.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://op.nszjky.cn

[Q41] 多表连接
来源：http://zy.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vm.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://oq.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://df.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://ud.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://ka.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yi.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://ac.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cc.huixiangedu.cn

[Q44] IN 子查询
来源：http://mt.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yo.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://qb.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://li.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vv.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fk.shxzskj.cn

[Q47] 与平均值比较
来源：http://nn.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oa.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://uu.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://be.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://jd.nszjky.cn

[Q49] 更新单行
来源：http://ov.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bw.shxzskj.cn

[Q50] 批量更新
来源：http://ln.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ky.panjiajie.cn

[Q51] 用子查询更新
来源：http://wa.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hs.nszjky.cn

[Q52] 删除指定行
来源：http://qy.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://lp.521024.cn

[Q53] 按条件删除
来源：http://cz.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mw.colortex.cn

[Q54] 清空表
来源：http://af.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://im.9csxet.cn

[Q55] 排名（并列占位）
来源：http://ea.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://de.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://st.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://er.shtwfgs.cn

[Q57] 行号
来源：http://cc.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ep.newstarts.cn

[Q58] 累计求和
来源：http://iw.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qu.lnxyls.cn

[Q59] 分组内累计
来源：http://od.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gv.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://lr.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pg.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fl.haigaiapp.cn

[Q61] 移动平均
来源：http://xr.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ts.chemitech.net.cn

[Q62] 分组占比
来源：http://pp.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lk.panjiajie.cn

[Q63] 开启事务
来源：http://ts.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://na.muxihuayi.cn

[Q64] 提交事务
来源：http://vc.szxytkj.cn

COMMIT;
来源：http://uf.huanxung.cn

[Q65] 回滚事务
来源：http://eu.hnjuh.cn

ROLLBACK;
来源：http://rh.shxzukj.cn

[Q66] 行锁查询
来源：http://rk.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vl.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://dg.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://it.szsharing.cn

[Q68] 保存点
来源：http://bk.huanxung.cn

SAVEPOINT sp1;
来源：http://np.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://jy.hnjuh.cn

[Q69] 查看执行计划
来源：http://ya.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vi.colortex.cn

[Q70] 更新统计信息
来源：http://ht.asd995.cn

ANALYZE TABLE users;
来源：http://sa.shxzskj.cn

[Q71] 查看建表语句
来源：http://lp.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tk.jctech888.com.cn

[Q72] 查看索引
来源：http://rs.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://hu.panjiajie.cn

[Q73] 查看表状态
来源：http://fz.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ut.haigaiapp.cn

[Q74] 强制使用索引
来源：http://ko.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qy.muxihuayi.cn

[Q75] 日期格式化
来源：http://im.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ia.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ua.huixiangedu.cn

[Q76] 按天统计
来源：http://nr.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yw.szxytkj.cn

[Q77] 时间加减
来源：http://fu.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zv.huixinmuqiang.cn

[Q78] 当前时间
来源：http://tn.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vx.huixiangedu.cn

[Q79] 字符串拼接
来源：http://vp.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pu.shxzukj.cn

[Q80] 字符串截取
来源：http://xa.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://it.chemitech.net.cn

[Q81] 字符串替换
来源：http://rh.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fm.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://ai.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wd.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://py.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fn.gzmigu.cn

[Q84] 去除首尾空格
来源：http://vj.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://wq.szsharing.cn

[Q85] 数值取整
来源：http://pv.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://im.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://jf.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zl.nicolike.cn

[Q87] JSON 字段做条件
来源：http://zj.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fb.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://nt.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ql.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tw.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://av.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nu.colortex.cn

[Q90] 生成序号列
来源：http://zs.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xd.jianghongdianzi.cn

================================================================================
来源：http://nl.huixinmuqiang.cn

R. Bash 专题
来源：http://fu.shxzskj.cn

================================================================================
来源：http://pl.szxytkj.cn

[R01] shebang 与严格模式
来源：http://pr.haigaiapp.cn

#!/usr/bin/env bash
来源：http://ea.colortex.cn

set -euo pipefail
来源：http://go.asd995.cn

[R02] 变量赋值与使用
来源：http://gh.shxzukj.cn

name="Tom"; echo "$name"
来源：http://qj.shtwfgs.cn

[R03] 只读变量
来源：http://ti.lnxyls.cn

readonly PI=3.14
来源：http://qd.jctech888.com.cn

[R04] 位置参数
来源：http://vf.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fm.shxzukj.cn

[R05] 参数默认值
来源：http://su.huanxung.cn

name="${1:-default}"
来源：http://wc.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://db.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jl.jctech888.com.cn

[R07] if 判断文件
来源：http://ao.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ef.hahajie.cn

[R08] 数值比较
来源：http://wi.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ki.nicolike.cn

[R09] 字符串比较
来源：http://oj.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pc.521024.cn

[R10] 正则匹配
来源：http://ao.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qb.yuexingan06.cn

[R11] case 多分支
来源：http://oj.nicolike.cn

case "$1" in
来源：http://or.nszjky.cn

start) echo "启动" ;;
来源：http://nv.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://pf.asd995.cn

*)     echo "未知命令" ;;
来源：http://wi.hnjuh.cn

esac
来源：http://xt.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://ra.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://fr.huanxung.cn

[R13] for 计数循环
来源：http://hf.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://ty.hahajie.cn

[R14] C 风格 for
来源：http://gf.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pu.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://dr.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kp.nicolike.cn

[R16] until 等待条件
来源：http://tv.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ny.hahajie.cn

[R17] 数组定义与取值
来源：http://cs.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zn.asd995.cn

[R18] 遍历数组
来源：http://vl.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ne.shxzskj.cn

[R19] 数组长度
来源：http://cm.shtwfgs.cn

echo "${#arr[@]}"
来源：http://rd.nszjky.cn

[R20] 关联数组（字典）
来源：http://qh.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tq.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ix.jctech888.com.cn

echo "${#s}"
来源：http://ec.huixinmuqiang.cn

[R22] 截取子串
来源：http://ul.jctech888.com.cn

echo "${s:0:5}"
来源：http://kx.shtwfgs.cn

[R23] 字符串替换
来源：http://lm.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://za.521024.cn

[R24] 大小写转换
来源：http://mh.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gs.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://ya.521024.cn


<!-- 参考信息 -->