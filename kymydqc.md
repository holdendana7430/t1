代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vu.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vl.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dq.9csxet.cn

Ruby: a == b
来源：http://ud.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://od.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qh.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pd.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://ky.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hc.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://ff.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bz.shtwfgs.cn

Go:   if x == nil {}
来源：http://yy.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://go.yuexingan06.cn

C#:   if (x is null) {}
来源：http://af.521024.cn

[P07] 防抖与节流
来源：http://kc.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ic.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://rx.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hh.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://si.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://st.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gn.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gv.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dg.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://kg.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zz.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ah.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qr.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hm.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tu.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cs.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ec.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zf.yuexingan06.cn

================================================================================
来源：http://zn.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lf.shxzukj.cn

================================================================================
来源：http://kr.bjjhwx.cn

[Q01] 创建表
来源：http://rk.shxzskj.cn

CREATE TABLE users (
来源：http://rx.nszjky.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nd.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ct.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://rd.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://op.newstarts.cn

);
来源：http://am.panjiajie.cn

[Q02] 创建带外键的表
来源：http://ee.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://nm.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hr.lnxyls.cn

user_id INT NOT NULL,
来源：http://re.newstarts.cn

amount DECIMAL(10, 2),
来源：http://bi.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ot.yuntaijiaju.cn

);
来源：http://ln.shxzukj.cn

[Q03] 增加列
来源：http://vq.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gc.muxihuayi.cn

[Q04] 修改列类型
来源：http://ri.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gl.szsharing.cn

[Q05] 重命名列
来源：http://su.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kn.jctech888.com.cn

[Q06] 删除列
来源：http://ep.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fn.wgjwhj.cn

[Q07] 删除表
来源：http://qk.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://qs.huanxung.cn

[Q08] 创建普通索引
来源：http://ye.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://as.nicolike.cn

[Q09] 创建唯一索引
来源：http://ai.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lq.bjjhwx.cn

[Q10] 插入单行
来源：http://mo.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ov.nszjky.cn

[Q11] 一次插入多行
来源：http://qr.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bb.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://ob.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jc.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://br.lnxyls.cn

[Q13] 忽略重复插入
来源：http://fs.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wz.521024.cn

[Q14] 存在则更新（upsert）
来源：http://cj.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kl.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kh.hahajie.cn

[Q15] 查询全部
来源：http://hm.bookmarksfly.cn

SELECT * FROM users;
来源：http://yw.shxzskj.cn

[Q16] 查询指定列
来源：http://oq.muxihuayi.cn

SELECT id, name FROM users;
来源：http://vi.lnxyls.cn

[Q17] 条件查询
来源：http://jr.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wq.wgjwhj.cn

[Q18] 模糊匹配
来源：http://df.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xn.jianghongdianzi.cn

[Q19] 范围查询
来源：http://pe.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nu.huixinmuqiang.cn

[Q20] IN 列表
来源：http://ek.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ep.hahajie.cn

[Q21] 空值判断
来源：http://no.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rs.asd995.cn

[Q22] 排序
来源：http://bs.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://un.muxihuayi.cn

[Q23] 分页
来源：http://ji.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vk.jctech888.com.cn

[Q24] 去重
来源：http://vk.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://ah.huanxung.cn

[Q25] 只取前 N 条
来源：http://cd.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qp.newstarts.cn

[Q26] 计数
来源：http://oj.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://sn.hnjuh.cn

[Q27] 条件计数
来源：http://bd.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ts.bookmarksfly.cn

[Q28] 求和与平均
来源：http://tc.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sl.bjjhwx.cn

[Q29] 最大最小值
来源：http://ng.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wx.panjiajie.cn

[Q30] 分组统计
来源：http://fa.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ny.huanxung.cn

[Q31] 分组后过滤
来源：http://cl.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gm.nszjky.cn

[Q32] 分组拼接字符串
来源：http://al.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ii.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pm.szsharing.cn

[Q33] 多列分组
来源：http://pw.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pu.yuexingan06.cn

[Q34] 每组取第一条
来源：http://ct.shxzskj.cn

SELECT * FROM (
来源：http://nt.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oj.yuexingan06.cn

) t WHERE rn = 1;
来源：http://vy.muxihuayi.cn

[Q35] 内连接
来源：http://sh.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fc.shxzskj.cn

[Q36] 左连接
来源：http://rt.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rw.gzmigu.cn

[Q37] 右连接
来源：http://jo.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kr.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ii.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://co.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://yx.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xf.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hq.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bi.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xl.jctech888.com.cn

[Q41] 多表连接
来源：http://mu.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wh.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://mq.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://qp.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://ak.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://kw.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ic.muxihuayi.cn

[Q43] 标量子查询
来源：http://qw.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wx.9csxet.cn

[Q44] IN 子查询
来源：http://ol.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xx.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://iu.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vy.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sp.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mq.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://zv.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xa.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://vc.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ha.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://vj.haigaiapp.cn

[Q49] 更新单行
来源：http://wf.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wj.bookmarksfly.cn

[Q50] 批量更新
来源：http://gy.huixiangedu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yx.hnjuh.cn

[Q51] 用子查询更新
来源：http://aj.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kg.chemitech.net.cn

[Q52] 删除指定行
来源：http://cj.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://il.nicolike.cn

[Q53] 按条件删除
来源：http://qt.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ng.shtwfgs.cn

[Q54] 清空表
来源：http://me.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://qf.9csxet.cn

[Q55] 排名（并列占位）
来源：http://yg.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rk.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://ox.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://js.yuntaijiaju.cn

[Q57] 行号
来源：http://hm.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zq.chemitech.net.cn

[Q58] 累计求和
来源：http://ox.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://re.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://vm.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tw.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://ct.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gu.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yh.szxytkj.cn

[Q61] 移动平均
来源：http://ef.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lq.colortex.cn

[Q62] 分组占比
来源：http://aq.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mz.muxihuayi.cn

[Q63] 开启事务
来源：http://ml.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qq.9csxet.cn

[Q64] 提交事务
来源：http://vi.shxzskj.cn

COMMIT;
来源：http://ni.lnxyls.cn

[Q65] 回滚事务
来源：http://zi.gzmigu.cn

ROLLBACK;
来源：http://yq.huixiangedu.cn

[Q66] 行锁查询
来源：http://lv.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xe.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://gn.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vz.chemitech.net.cn

[Q68] 保存点
来源：http://dy.hahajie.cn

SAVEPOINT sp1;
来源：http://eh.nszjky.cn

ROLLBACK TO sp1;
来源：http://ug.gzmigu.cn

[Q69] 查看执行计划
来源：http://uk.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eh.colortex.cn

[Q70] 更新统计信息
来源：http://wp.panjiajie.cn

ANALYZE TABLE users;
来源：http://ck.panjiajie.cn

[Q71] 查看建表语句
来源：http://mc.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ty.shxzukj.cn

[Q72] 查看索引
来源：http://tk.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://bh.huixiangedu.cn

[Q73] 查看表状态
来源：http://gj.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ac.szxytkj.cn

[Q74] 强制使用索引
来源：http://nt.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rt.9csxet.cn

[Q75] 日期格式化
来源：http://li.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xd.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tf.szsharing.cn

[Q76] 按天统计
来源：http://zi.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://et.nicolike.cn

[Q77] 时间加减
来源：http://ev.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dk.panjiajie.cn

[Q78] 当前时间
来源：http://ni.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sf.szxytkj.cn

[Q79] 字符串拼接
来源：http://vr.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pj.colortex.cn

[Q80] 字符串截取
来源：http://yg.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ld.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://ku.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uz.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://rt.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ro.panjiajie.cn

[Q83] 大小写转换
来源：http://yd.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ja.asd995.cn

[Q84] 去除首尾空格
来源：http://xb.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://ys.shxzukj.cn

[Q85] 数值取整
来源：http://oe.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qr.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://rw.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lf.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://sl.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zy.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://bu.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zf.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ox.newstarts.cn

[Q89] 判断表是否存在
来源：http://xh.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ve.huixiangedu.cn

[Q90] 生成序号列
来源：http://ad.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qs.szsharing.cn

================================================================================
来源：http://rf.muxihuayi.cn

R. Bash 专题
来源：http://ul.hnjuh.cn

================================================================================
来源：http://jv.nszjky.cn

[R01] shebang 与严格模式
来源：http://ms.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://wo.szsharing.cn

set -euo pipefail
来源：http://gu.521024.cn

[R02] 变量赋值与使用
来源：http://uq.shxzukj.cn

name="Tom"; echo "$name"
来源：http://pk.shxzukj.cn

[R03] 只读变量
来源：http://tm.newstarts.cn

readonly PI=3.14
来源：http://sl.gzmigu.cn

[R04] 位置参数
来源：http://sy.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ez.yuexingan06.cn

[R05] 参数默认值
来源：http://ms.yuntaijiaju.cn

name="${1:-default}"
来源：http://ig.9csxet.cn

[R06] 判断命令是否存在
来源：http://om.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://et.szsharing.cn

[R07] if 判断文件
来源：http://mn.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xy.colortex.cn

[R08] 数值比较
来源：http://kv.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aw.huixinmuqiang.cn

[R09] 字符串比较
来源：http://go.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://th.haigaiapp.cn

[R10] 正则匹配
来源：http://hq.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kb.yuntaijiaju.cn

[R11] case 多分支
来源：http://vh.9csxet.cn

case "$1" in
来源：http://ul.nicolike.cn

start) echo "启动" ;;
来源：http://si.panjiajie.cn

stop)  echo "停止" ;;
来源：http://hr.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://lv.colortex.cn

esac
来源：http://rz.wgjwhj.cn

[R12] for 遍历文件
来源：http://uo.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://fa.jianghongdianzi.cn

[R13] for 计数循环
来源：http://bi.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://vv.jianghongdianzi.cn

[R14] C 风格 for
来源：http://gj.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xf.newstarts.cn

[R15] while 逐行读文件
来源：http://pp.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xp.lnxyls.cn

[R16] until 等待条件
来源：http://tc.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jv.wgjwhj.cn

[R17] 数组定义与取值
来源：http://hz.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tq.chemitech.net.cn

[R18] 遍历数组
来源：http://xi.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aw.bookmarksfly.cn

[R19] 数组长度
来源：http://mg.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://nq.newstarts.cn

[R20] 关联数组（字典）
来源：http://yk.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wu.yuntaijiaju.cn

[R21] 字符串长度
来源：http://nt.szsharing.cn

echo "${#s}"
来源：http://my.shxzskj.cn

[R22] 截取子串
来源：http://cj.shxzukj.cn

echo "${s:0:5}"
来源：http://dc.muxihuayi.cn

[R23] 字符串替换
来源：http://cr.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://by.panjiajie.cn

[R24] 大小写转换
来源：http://hb.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xh.521024.cn

[R25] 去后缀 / 去前缀
来源：http://jx.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://at.panjiajie.cn

[R26] 命令替换
来源：http://ok.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://ky.nicolike.cn

[R27] 算术展开
来源：http://cq.huanxung.cn


<!-- 参考信息 -->