代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pf.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lx.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eb.nszjky.cn

Ruby: a == b
来源：http://hw.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ak.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gt.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ga.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://ie.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://im.9csxet.cn

TS:   if (x == null) {}
来源：http://it.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ys.shxzukj.cn

Go:   if x == nil {}
来源：http://xk.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oq.nszjky.cn

C#:   if (x is null) {}
来源：http://sv.hahajie.cn

[P07] 防抖与节流
来源：http://er.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rl.521024.cn

PHP:  // 手写时间戳比较
来源：http://vr.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ba.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mk.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sn.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://an.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iq.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jr.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://pd.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xv.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vo.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yt.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mj.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ft.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qc.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lv.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eh.bjjhwx.cn

================================================================================
来源：http://kz.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zr.szxytkj.cn

================================================================================
来源：http://sz.gzmigu.cn

[Q01] 创建表
来源：http://gy.bjjhwx.cn

CREATE TABLE users (
来源：http://qa.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://un.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://ki.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://xy.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bp.yuntaijiaju.cn

);
来源：http://iw.shxzskj.cn

[Q02] 创建带外键的表
来源：http://vs.hnjuh.cn

CREATE TABLE orders (
来源：http://le.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kd.szsharing.cn

user_id INT NOT NULL,
来源：http://hv.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://hf.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wf.hnjuh.cn

);
来源：http://ga.jctech888.com.cn

[Q03] 增加列
来源：http://yn.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ss.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://rg.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ql.huixinmuqiang.cn

[Q05] 重命名列
来源：http://yc.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ll.chemitech.net.cn

[Q06] 删除列
来源：http://lp.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ja.nicolike.cn

[Q07] 删除表
来源：http://kb.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://hs.huixiangedu.cn

[Q08] 创建普通索引
来源：http://og.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ru.gzmigu.cn

[Q09] 创建唯一索引
来源：http://nt.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fx.jianghongdianzi.cn

[Q10] 插入单行
来源：http://zn.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sk.jctech888.com.cn

[Q11] 一次插入多行
来源：http://pd.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fd.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://cw.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tu.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ma.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://wu.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mm.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://rv.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jc.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vg.colortex.cn

[Q15] 查询全部
来源：http://xg.colortex.cn

SELECT * FROM users;
来源：http://xp.asd995.cn

[Q16] 查询指定列
来源：http://kb.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://ui.shxzskj.cn

[Q17] 条件查询
来源：http://lb.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ae.nszjky.cn

[Q18] 模糊匹配
来源：http://no.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oj.521024.cn

[Q19] 范围查询
来源：http://mr.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hn.huixiangedu.cn

[Q20] IN 列表
来源：http://ai.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uv.shxzskj.cn

[Q21] 空值判断
来源：http://zo.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gl.shtwfgs.cn

[Q22] 排序
来源：http://gc.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gq.szsharing.cn

[Q23] 分页
来源：http://lf.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zl.lnxyls.cn

[Q24] 去重
来源：http://rw.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://vb.shxzukj.cn

[Q25] 只取前 N 条
来源：http://ju.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fw.szxytkj.cn

[Q26] 计数
来源：http://ku.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ms.huixiangedu.cn

[Q27] 条件计数
来源：http://hy.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xw.szsharing.cn

[Q28] 求和与平均
来源：http://qs.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ui.panjiajie.cn

[Q29] 最大最小值
来源：http://zn.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rl.hahajie.cn

[Q30] 分组统计
来源：http://cp.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wx.wgjwhj.cn

[Q31] 分组后过滤
来源：http://xv.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sg.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://ke.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bf.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rg.yuntaijiaju.cn

[Q33] 多列分组
来源：http://nd.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nw.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://dh.huixinmuqiang.cn

SELECT * FROM (
来源：http://ff.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vp.panjiajie.cn

) t WHERE rn = 1;
来源：http://in.shxzskj.cn

[Q35] 内连接
来源：http://sp.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xg.bookmarksfly.cn

[Q36] 左连接
来源：http://zl.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://da.shxzskj.cn

[Q37] 右连接
来源：http://uv.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nv.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wb.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vh.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://xa.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ce.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xv.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://es.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ft.haigaiapp.cn

[Q41] 多表连接
来源：http://al.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://er.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://nk.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://mt.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://md.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://nn.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hw.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://ba.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ol.521024.cn

[Q44] IN 子查询
来源：http://jc.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ky.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://vd.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vt.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pr.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vi.chemitech.net.cn

[Q47] 与平均值比较
来源：http://tp.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ky.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://si.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pu.bjjhwx.cn

SELECT * FROM t WHERE c > 5;
来源：http://vb.bjjhwx.cn

[Q49] 更新单行
来源：http://ry.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bo.yuexingan06.cn

[Q50] 批量更新
来源：http://rn.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mq.panjiajie.cn

[Q51] 用子查询更新
来源：http://aj.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://in.shtwfgs.cn

[Q52] 删除指定行
来源：http://aq.yuntaijiaju.cn

DELETE FROM users WHERE id = 10;
来源：http://hn.shxzukj.cn

[Q53] 按条件删除
来源：http://jd.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ed.gzmigu.cn

[Q54] 清空表
来源：http://dl.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://cx.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://ro.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zm.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://im.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dw.nszjky.cn

[Q57] 行号
来源：http://yf.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jw.shxzskj.cn

[Q58] 累计求和
来源：http://ap.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://np.haigaiapp.cn

[Q59] 分组内累计
来源：http://vk.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ki.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://dc.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jo.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ec.bjjhwx.cn

[Q61] 移动平均
来源：http://fd.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bh.jianghongdianzi.cn

[Q62] 分组占比
来源：http://pm.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aw.haigaiapp.cn

[Q63] 开启事务
来源：http://oo.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ca.asd995.cn

[Q64] 提交事务
来源：http://kh.huixinmuqiang.cn

COMMIT;
来源：http://lu.huixiangedu.cn

[Q65] 回滚事务
来源：http://zh.huanxung.cn

ROLLBACK;
来源：http://mw.haigaiapp.cn

[Q66] 行锁查询
来源：http://dd.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ee.colortex.cn

[Q67] 设置隔离级别
来源：http://ax.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gp.chemitech.net.cn

[Q68] 保存点
来源：http://sb.9csxet.cn

SAVEPOINT sp1;
来源：http://ii.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://jw.shxzskj.cn

[Q69] 查看执行计划
来源：http://tc.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aa.huixiangedu.cn

[Q70] 更新统计信息
来源：http://aj.huanxung.cn

ANALYZE TABLE users;
来源：http://xp.szxytkj.cn

[Q71] 查看建表语句
来源：http://nd.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zk.jianghongdianzi.cn

[Q72] 查看索引
来源：http://km.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://sh.hahajie.cn

[Q73] 查看表状态
来源：http://rl.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wq.9csxet.cn

[Q74] 强制使用索引
来源：http://qe.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ft.panjiajie.cn

[Q75] 日期格式化
来源：http://gx.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://re.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rz.asd995.cn

[Q76] 按天统计
来源：http://nx.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ko.521024.cn

[Q77] 时间加减
来源：http://du.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://si.newstarts.cn

[Q78] 当前时间
来源：http://km.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rh.hahajie.cn

[Q79] 字符串拼接
来源：http://ec.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xp.bjjhwx.cn

[Q80] 字符串截取
来源：http://lk.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jj.huanxung.cn

[Q81] 字符串替换
来源：http://py.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iz.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://vi.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fe.wgjwhj.cn

[Q83] 大小写转换
来源：http://xm.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aa.colortex.cn

[Q84] 去除首尾空格
来源：http://ls.521024.cn

SELECT TRIM(name) FROM users;
来源：http://di.wgjwhj.cn

[Q85] 数值取整
来源：http://xi.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jk.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://in.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nn.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ou.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qh.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://yl.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hd.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ua.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://ht.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://js.bookmarksfly.cn

[Q90] 生成序号列
来源：http://ft.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gi.jianghongdianzi.cn

================================================================================
来源：http://ry.newstarts.cn

R. Bash 专题
来源：http://pe.huanxung.cn

================================================================================
来源：http://wa.newstarts.cn

[R01] shebang 与严格模式
来源：http://bx.chemitech.net.cn

#!/usr/bin/env bash
来源：http://av.gzmigu.cn

set -euo pipefail
来源：http://ei.shxzskj.cn

[R02] 变量赋值与使用
来源：http://kp.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://md.521024.cn

[R03] 只读变量
来源：http://oh.shxzskj.cn

readonly PI=3.14
来源：http://om.yuntaijiaju.cn

[R04] 位置参数
来源：http://ip.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ab.huixiangedu.cn

[R05] 参数默认值
来源：http://ay.colortex.cn

name="${1:-default}"
来源：http://mh.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://dg.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://al.hahajie.cn

[R07] if 判断文件
来源：http://fg.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://de.colortex.cn

[R08] 数值比较
来源：http://wh.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://to.szxytkj.cn

[R09] 字符串比较
来源：http://jt.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://za.huixiangedu.cn

[R10] 正则匹配
来源：http://ks.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gn.haigaiapp.cn

[R11] case 多分支
来源：http://lm.shxzukj.cn

case "$1" in
来源：http://gy.shxzukj.cn

start) echo "启动" ;;
来源：http://lu.szxytkj.cn

stop)  echo "停止" ;;
来源：http://of.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://oc.panjiajie.cn

esac
来源：http://br.yuexingan06.cn

[R12] for 遍历文件
来源：http://ne.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://lw.muxihuayi.cn

[R13] for 计数循环
来源：http://qf.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://vp.chemitech.net.cn

[R14] C 风格 for
来源：http://yj.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fs.asd995.cn

[R15] while 逐行读文件
来源：http://my.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pi.huanxung.cn

[R16] until 等待条件
来源：http://rt.bookmarksfly.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://za.jctech888.com.cn

[R17] 数组定义与取值
来源：http://sv.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lu.huixinmuqiang.cn

[R18] 遍历数组
来源：http://we.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vx.bookmarksfly.cn

[R19] 数组长度
来源：http://cx.colortex.cn

echo "${#arr[@]}"
来源：http://hl.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://bs.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tf.shtwfgs.cn

[R21] 字符串长度
来源：http://ge.yuexingan06.cn

echo "${#s}"
来源：http://uo.newstarts.cn

[R22] 截取子串
来源：http://ti.hahajie.cn

echo "${s:0:5}"
来源：http://bk.bookmarksfly.cn

[R23] 字符串替换
来源：http://ot.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rk.jctech888.com.cn

[R24] 大小写转换
来源：http://pt.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qu.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://qv.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sl.panjiajie.cn

[R26] 命令替换
来源：http://mp.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://mm.yuntaijiaju.cn

[R27] 算术展开
来源：http://mc.jctech888.com.cn


<!-- 参考信息 -->