代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://pi.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ro.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bs.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kz.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ng.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yo.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pt.9csxet.cn

Ruby: a == b
来源：http://fm.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rm.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mi.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ql.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://va.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yr.huixiangedu.cn

TS:   if (x == null) {}
来源：http://en.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xk.yuexingan06.cn

Go:   if x == nil {}
来源：http://df.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gt.newstarts.cn

C#:   if (x is null) {}
来源：http://uq.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://dj.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wr.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://qh.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zh.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rp.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ni.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zw.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ez.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ko.asd995.cn

[P08] 处理浮点精度问题
来源：http://uq.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sd.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dd.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ag.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cn.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mv.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nn.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zx.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dw.huixinmuqiang.cn

================================================================================
来源：http://ut.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mm.huixiangedu.cn

================================================================================
来源：http://wz.colortex.cn

[Q01] 创建表
来源：http://qj.yuntaijiaju.cn

CREATE TABLE users (
来源：http://mx.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pz.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://pj.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://if.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qq.szxytkj.cn

);
来源：http://lm.hahajie.cn

[Q02] 创建带外键的表
来源：http://th.shxzskj.cn

CREATE TABLE orders (
来源：http://sr.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pu.shtwfgs.cn

user_id INT NOT NULL,
来源：http://fd.nszjky.cn

amount DECIMAL(10, 2),
来源：http://ap.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://td.shxzskj.cn

);
来源：http://wk.nicolike.cn

[Q03] 增加列
来源：http://oc.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ll.lnxyls.cn

[Q04] 修改列类型
来源：http://ru.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fh.jctech888.com.cn

[Q05] 重命名列
来源：http://cw.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nb.huixiangedu.cn

[Q06] 删除列
来源：http://dz.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vk.chemitech.net.cn

[Q07] 删除表
来源：http://zj.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://jj.chemitech.net.cn

[Q08] 创建普通索引
来源：http://vm.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bb.szxytkj.cn

[Q09] 创建唯一索引
来源：http://dq.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xa.bookmarksfly.cn

[Q10] 插入单行
来源：http://wl.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gh.panjiajie.cn

[Q11] 一次插入多行
来源：http://tj.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pw.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://yh.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qq.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://id.asd995.cn

[Q13] 忽略重复插入
来源：http://en.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://df.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://in.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xp.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xq.muxihuayi.cn

[Q15] 查询全部
来源：http://wv.jctech888.com.cn

SELECT * FROM users;
来源：http://xi.shxzukj.cn

[Q16] 查询指定列
来源：http://qw.gzmigu.cn

SELECT id, name FROM users;
来源：http://ap.shtwfgs.cn

[Q17] 条件查询
来源：http://fo.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oi.hnjuh.cn

[Q18] 模糊匹配
来源：http://qz.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://du.huixiangedu.cn

[Q19] 范围查询
来源：http://bt.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cr.panjiajie.cn

[Q20] IN 列表
来源：http://ns.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gv.szsharing.cn

[Q21] 空值判断
来源：http://dc.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wr.bookmarksfly.cn

[Q22] 排序
来源：http://wn.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kb.bjjhwx.cn

[Q23] 分页
来源：http://ok.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hp.colortex.cn

[Q24] 去重
来源：http://hu.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://eg.huanxung.cn

[Q25] 只取前 N 条
来源：http://ye.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ya.lnxyls.cn

[Q26] 计数
来源：http://fm.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://fs.panjiajie.cn

[Q27] 条件计数
来源：http://tl.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zq.hnjuh.cn

[Q28] 求和与平均
来源：http://nt.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nh.nicolike.cn

[Q29] 最大最小值
来源：http://oc.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://na.szxytkj.cn

[Q30] 分组统计
来源：http://dn.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dt.hnjuh.cn

[Q31] 分组后过滤
来源：http://rg.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qf.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://tv.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iw.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gy.jianghongdianzi.cn

[Q33] 多列分组
来源：http://oo.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ie.lnxyls.cn

[Q34] 每组取第一条
来源：http://lp.muxihuayi.cn

SELECT * FROM (
来源：http://sk.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rl.szxytkj.cn

) t WHERE rn = 1;
来源：http://pw.szxytkj.cn

[Q35] 内连接
来源：http://yu.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://un.9csxet.cn

[Q36] 左连接
来源：http://pq.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tr.huixinmuqiang.cn

[Q37] 右连接
来源：http://dk.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xt.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tc.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ds.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://aq.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jz.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yg.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://db.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lk.jctech888.com.cn

[Q41] 多表连接
来源：http://xb.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yv.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://bj.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://iy.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://qy.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://gi.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uc.521024.cn

[Q43] 标量子查询
来源：http://ju.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://no.jctech888.com.cn

[Q44] IN 子查询
来源：http://wn.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bc.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://mg.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wf.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eu.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vb.hahajie.cn

[Q47] 与平均值比较
来源：http://kn.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wm.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://lv.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qx.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://pw.huixiangedu.cn

[Q49] 更新单行
来源：http://pv.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xm.haigaiapp.cn

[Q50] 批量更新
来源：http://it.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fq.haigaiapp.cn

[Q51] 用子查询更新
来源：http://jo.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ta.huanxung.cn

[Q52] 删除指定行
来源：http://od.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://cd.muxihuayi.cn

[Q53] 按条件删除
来源：http://sm.wgjwhj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bi.wgjwhj.cn

[Q54] 清空表
来源：http://hf.hahajie.cn

TRUNCATE TABLE logs;
来源：http://jy.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://fw.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nr.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://rd.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ou.521024.cn

[Q57] 行号
来源：http://tr.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vx.nicolike.cn

[Q58] 累计求和
来源：http://xa.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ll.szxytkj.cn

[Q59] 分组内累计
来源：http://hj.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ng.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://df.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rc.huixinmuqiang.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jn.shxzskj.cn

[Q61] 移动平均
来源：http://wj.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ul.asd995.cn

[Q62] 分组占比
来源：http://gv.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vp.colortex.cn

[Q63] 开启事务
来源：http://pf.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://am.haigaiapp.cn

[Q64] 提交事务
来源：http://oz.huanxung.cn

COMMIT;
来源：http://bc.panjiajie.cn

[Q65] 回滚事务
来源：http://dp.shtwfgs.cn

ROLLBACK;
来源：http://mu.szxytkj.cn

[Q66] 行锁查询
来源：http://wx.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jq.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://fd.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nu.lnxyls.cn

[Q68] 保存点
来源：http://vh.huixiangedu.cn

SAVEPOINT sp1;
来源：http://ux.szsharing.cn

ROLLBACK TO sp1;
来源：http://uj.9csxet.cn

[Q69] 查看执行计划
来源：http://ee.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rt.szsharing.cn

[Q70] 更新统计信息
来源：http://iw.colortex.cn

ANALYZE TABLE users;
来源：http://ls.shtwfgs.cn

[Q71] 查看建表语句
来源：http://fi.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nd.shxzskj.cn

[Q72] 查看索引
来源：http://dj.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://oc.nszjky.cn

[Q73] 查看表状态
来源：http://nj.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mm.yuexingan06.cn

[Q74] 强制使用索引
来源：http://rp.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hx.chemitech.net.cn

[Q75] 日期格式化
来源：http://jt.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://na.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nc.bookmarksfly.cn

[Q76] 按天统计
来源：http://hm.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hs.wgjwhj.cn

[Q77] 时间加减
来源：http://ge.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wv.bjjhwx.cn

[Q78] 当前时间
来源：http://da.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jw.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://pn.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dk.9csxet.cn

[Q80] 字符串截取
来源：http://fj.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wk.muxihuayi.cn

[Q81] 字符串替换
来源：http://tw.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://el.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://mh.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ks.9csxet.cn

[Q83] 大小写转换
来源：http://sm.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gt.shxzukj.cn

[Q84] 去除首尾空格
来源：http://vj.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://qw.huanxung.cn

[Q85] 数值取整
来源：http://nn.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://go.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://uj.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qu.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://uu.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pa.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://kf.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yb.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aq.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://ya.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://um.yuexingan06.cn

[Q90] 生成序号列
来源：http://cs.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nl.521024.cn

================================================================================
来源：http://ff.huanxung.cn

R. Bash 专题
来源：http://tt.9csxet.cn

================================================================================
来源：http://ip.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://vz.huanxung.cn

#!/usr/bin/env bash
来源：http://om.nicolike.cn

set -euo pipefail
来源：http://tn.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://yv.9csxet.cn

name="Tom"; echo "$name"
来源：http://as.bookmarksfly.cn

[R03] 只读变量
来源：http://sz.szxytkj.cn

readonly PI=3.14
来源：http://kj.huixiangedu.cn

[R04] 位置参数
来源：http://lj.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dg.shxzukj.cn

[R05] 参数默认值
来源：http://od.gzmigu.cn

name="${1:-default}"
来源：http://cc.nicolike.cn

[R06] 判断命令是否存在
来源：http://tb.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rh.shxzskj.cn

[R07] if 判断文件
来源：http://ek.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tx.szsharing.cn

[R08] 数值比较
来源：http://kt.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oz.shtwfgs.cn

[R09] 字符串比较
来源：http://yp.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://df.panjiajie.cn

[R10] 正则匹配
来源：http://cg.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yr.bjjhwx.cn

[R11] case 多分支
来源：http://tf.lnxyls.cn

case "$1" in
来源：http://na.colortex.cn

start) echo "启动" ;;
来源：http://ay.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://iw.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://ne.nszjky.cn

esac
来源：http://fs.gzmigu.cn

[R12] for 遍历文件
来源：http://lu.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://pm.nszjky.cn

[R13] for 计数循环
来源：http://kp.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ph.shtwfgs.cn

[R14] C 风格 for
来源：http://hk.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yj.chemitech.net.cn

[R15] while 逐行读文件
来源：http://lq.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qd.lnxyls.cn

[R16] until 等待条件
来源：http://hr.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vo.wgjwhj.cn

[R17] 数组定义与取值
来源：http://jo.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zs.bookmarksfly.cn

[R18] 遍历数组
来源：http://ff.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pa.nicolike.cn

[R19] 数组长度
来源：http://qj.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://qw.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://le.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tw.newstarts.cn

[R21] 字符串长度
来源：http://ra.newstarts.cn

echo "${#s}"
来源：http://nr.newstarts.cn

[R22] 截取子串
来源：http://ep.szxytkj.cn

echo "${s:0:5}"
来源：http://wq.huanxung.cn

[R23] 字符串替换
来源：http://mi.bjjhwx.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cz.huixiangedu.cn

[R24] 大小写转换
来源：http://ml.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hn.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://jt.huanxung.cn


<!-- 参考信息 -->