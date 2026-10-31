代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bg.haigaiapp.cn

TS:   if (x == null) {}
来源：http://oz.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ye.nszjky.cn

Go:   if x == nil {}
来源：http://np.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://to.haigaiapp.cn

C#:   if (x is null) {}
来源：http://yl.nicolike.cn

[P07] 防抖与节流
来源：http://vl.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://li.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://qt.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ve.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://df.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fy.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fa.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iy.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ga.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://zk.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vt.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nu.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bx.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kh.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wc.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wj.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lb.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fi.gzmigu.cn

================================================================================
来源：http://xg.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://go.szxytkj.cn

================================================================================
来源：http://ta.jctech888.com.cn

[Q01] 创建表
来源：http://nk.huanxung.cn

CREATE TABLE users (
来源：http://dn.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nb.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://gn.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://wc.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rl.newstarts.cn

);
来源：http://zh.newstarts.cn

[Q02] 创建带外键的表
来源：http://rz.lnxyls.cn

CREATE TABLE orders (
来源：http://mn.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://es.hnjuh.cn

user_id INT NOT NULL,
来源：http://ax.nszjky.cn

amount DECIMAL(10, 2),
来源：http://gw.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xz.gzmigu.cn

);
来源：http://dj.szsharing.cn

[Q03] 增加列
来源：http://he.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wc.wgjwhj.cn

[Q04] 修改列类型
来源：http://ao.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qo.9csxet.cn

[Q05] 重命名列
来源：http://wr.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gc.shtwfgs.cn

[Q06] 删除列
来源：http://oo.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pc.jianghongdianzi.cn

[Q07] 删除表
来源：http://lt.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://gq.szxytkj.cn

[Q08] 创建普通索引
来源：http://vv.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sb.hnjuh.cn

[Q09] 创建唯一索引
来源：http://zs.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dx.jianghongdianzi.cn

[Q10] 插入单行
来源：http://zy.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gu.asd995.cn

[Q11] 一次插入多行
来源：http://gn.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uq.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://at.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pw.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ss.newstarts.cn

[Q13] 忽略重复插入
来源：http://pb.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wa.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://zp.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ez.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://py.jctech888.com.cn

[Q15] 查询全部
来源：http://rv.asd995.cn

SELECT * FROM users;
来源：http://nu.huanxung.cn

[Q16] 查询指定列
来源：http://kf.muxihuayi.cn

SELECT id, name FROM users;
来源：http://fo.huixinmuqiang.cn

[Q17] 条件查询
来源：http://ec.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hi.gzmigu.cn

[Q18] 模糊匹配
来源：http://yr.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://da.wgjwhj.cn

[Q19] 范围查询
来源：http://id.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ac.bjjhwx.cn

[Q20] IN 列表
来源：http://ln.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cv.jctech888.com.cn

[Q21] 空值判断
来源：http://wj.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nx.hnjuh.cn

[Q22] 排序
来源：http://zt.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zr.shxzskj.cn

[Q23] 分页
来源：http://rp.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ey.bookmarksfly.cn

[Q24] 去重
来源：http://zn.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://js.521024.cn

[Q25] 只取前 N 条
来源：http://ff.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hv.huanxung.cn

[Q26] 计数
来源：http://cm.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://sb.9csxet.cn

[Q27] 条件计数
来源：http://la.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cf.huixiangedu.cn

[Q28] 求和与平均
来源：http://wg.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uh.panjiajie.cn

[Q29] 最大最小值
来源：http://dt.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kp.szsharing.cn

[Q30] 分组统计
来源：http://wb.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ra.hahajie.cn

[Q31] 分组后过滤
来源：http://rh.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://be.nicolike.cn

[Q32] 分组拼接字符串
来源：http://cd.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ba.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ab.panjiajie.cn

[Q33] 多列分组
来源：http://od.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ok.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://mm.521024.cn

SELECT * FROM (
来源：http://lw.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fo.panjiajie.cn

) t WHERE rn = 1;
来源：http://ks.wgjwhj.cn

[Q35] 内连接
来源：http://yf.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mb.lnxyls.cn

[Q36] 左连接
来源：http://vq.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dc.521024.cn

[Q37] 右连接
来源：http://og.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tg.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fu.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bc.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://sn.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zh.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ea.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ac.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bl.yuntaijiaju.cn

[Q41] 多表连接
来源：http://ug.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kh.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://mb.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://uo.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://ex.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://uy.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ai.nszjky.cn

[Q43] 标量子查询
来源：http://fp.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ao.shxzskj.cn

[Q44] IN 子查询
来源：http://ib.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yu.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://cp.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ve.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rw.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hm.wgjwhj.cn

[Q47] 与平均值比较
来源：http://fr.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ec.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://jc.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nm.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://gg.wgjwhj.cn

[Q49] 更新单行
来源：http://jq.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lm.shxzskj.cn

[Q50] 批量更新
来源：http://nz.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fx.hahajie.cn

[Q51] 用子查询更新
来源：http://iq.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tt.bjjhwx.cn

[Q52] 删除指定行
来源：http://eg.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://ax.hnjuh.cn

[Q53] 按条件删除
来源：http://yi.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bf.gzmigu.cn

[Q54] 清空表
来源：http://el.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://sr.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://je.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ef.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://pw.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zl.newstarts.cn

[Q57] 行号
来源：http://fz.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lw.jctech888.com.cn

[Q58] 累计求和
来源：http://ze.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ua.9csxet.cn

[Q59] 分组内累计
来源：http://ar.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eh.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://bi.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dr.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xy.panjiajie.cn

[Q61] 移动平均
来源：http://gq.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iv.shxzukj.cn

[Q62] 分组占比
来源：http://tm.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://le.asd995.cn

[Q63] 开启事务
来源：http://vv.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qi.szsharing.cn

[Q64] 提交事务
来源：http://yq.huixinmuqiang.cn

COMMIT;
来源：http://ge.bjjhwx.cn

[Q65] 回滚事务
来源：http://gx.521024.cn

ROLLBACK;
来源：http://lm.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://wf.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hy.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://cl.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zm.haigaiapp.cn

[Q68] 保存点
来源：http://yj.panjiajie.cn

SAVEPOINT sp1;
来源：http://yr.lnxyls.cn

ROLLBACK TO sp1;
来源：http://lk.521024.cn

[Q69] 查看执行计划
来源：http://df.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://il.9csxet.cn

[Q70] 更新统计信息
来源：http://lu.huixiangedu.cn

ANALYZE TABLE users;
来源：http://rb.jctech888.com.cn

[Q71] 查看建表语句
来源：http://wl.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tz.yuntaijiaju.cn

[Q72] 查看索引
来源：http://fy.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://kp.newstarts.cn

[Q73] 查看表状态
来源：http://eg.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pk.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://qg.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ws.hnjuh.cn

[Q75] 日期格式化
来源：http://rj.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wd.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ue.huixiangedu.cn

[Q76] 按天统计
来源：http://oq.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bs.szsharing.cn

[Q77] 时间加减
来源：http://xt.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ty.lnxyls.cn

[Q78] 当前时间
来源：http://kb.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gb.muxihuayi.cn

[Q79] 字符串拼接
来源：http://uz.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lk.shxzukj.cn

[Q80] 字符串截取
来源：http://ng.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://op.asd995.cn

[Q81] 字符串替换
来源：http://wv.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lg.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://id.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uk.gzmigu.cn

[Q83] 大小写转换
来源：http://gm.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hk.nszjky.cn

[Q84] 去除首尾空格
来源：http://hj.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://yf.jctech888.com.cn

[Q85] 数值取整
来源：http://ea.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ii.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://rx.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gd.szsharing.cn

[Q87] JSON 字段做条件
来源：http://bz.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bw.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://rh.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zy.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gx.huanxung.cn

[Q89] 判断表是否存在
来源：http://vt.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lh.wgjwhj.cn

[Q90] 生成序号列
来源：http://zj.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dd.colortex.cn

================================================================================
来源：http://hi.huixinmuqiang.cn

R. Bash 专题
来源：http://hs.chemitech.net.cn

================================================================================
来源：http://jg.gzmigu.cn

[R01] shebang 与严格模式
来源：http://pe.huixiangedu.cn

#!/usr/bin/env bash
来源：http://cv.huixinmuqiang.cn

set -euo pipefail
来源：http://fo.hahajie.cn

[R02] 变量赋值与使用
来源：http://cl.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://gl.wgjwhj.cn

[R03] 只读变量
来源：http://ue.bjjhwx.cn

readonly PI=3.14
来源：http://sk.huixinmuqiang.cn

[R04] 位置参数
来源：http://ig.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tq.jctech888.com.cn

[R05] 参数默认值
来源：http://xr.colortex.cn

name="${1:-default}"
来源：http://vd.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://wi.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jt.szxytkj.cn

[R07] if 判断文件
来源：http://th.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://at.bookmarksfly.cn

[R08] 数值比较
来源：http://no.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wc.yuexingan06.cn

[R09] 字符串比较
来源：http://ja.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://us.hnjuh.cn

[R10] 正则匹配
来源：http://fo.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qj.bookmarksfly.cn

[R11] case 多分支
来源：http://mr.chemitech.net.cn

case "$1" in
来源：http://km.yuexingan06.cn

start) echo "启动" ;;
来源：http://ns.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://ev.hahajie.cn

*)     echo "未知命令" ;;
来源：http://xb.wgjwhj.cn

esac
来源：http://cd.szxytkj.cn

[R12] for 遍历文件
来源：http://nq.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://mr.jctech888.com.cn

[R13] for 计数循环
来源：http://uq.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://hc.huanxung.cn

[R14] C 风格 for
来源：http://cv.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wc.hahajie.cn

[R15] while 逐行读文件
来源：http://ek.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ag.huixinmuqiang.cn

[R16] until 等待条件
来源：http://pp.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ue.521024.cn

[R17] 数组定义与取值
来源：http://qk.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dz.hahajie.cn

[R18] 遍历数组
来源：http://sv.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qx.haigaiapp.cn

[R19] 数组长度
来源：http://op.asd995.cn

echo "${#arr[@]}"
来源：http://ij.panjiajie.cn

[R20] 关联数组（字典）
来源：http://ss.gzmigu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sq.nicolike.cn

[R21] 字符串长度
来源：http://nn.szsharing.cn

echo "${#s}"
来源：http://ty.jianghongdianzi.cn

[R22] 截取子串
来源：http://in.colortex.cn

echo "${s:0:5}"
来源：http://br.bjjhwx.cn

[R23] 字符串替换
来源：http://yh.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vc.nicolike.cn

[R24] 大小写转换
来源：http://bi.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zn.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://oz.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ct.chemitech.net.cn

[R26] 命令替换
来源：http://go.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://sl.yuexingan06.cn

[R27] 算术展开
来源：http://jc.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://tp.colortex.cn

[R28] 浮点运算
来源：http://hh.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://kb.gzmigu.cn

[R29] 定义函数
来源：http://qx.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ed.nszjky.cn

[R30] 函数返回状态码
来源：http://mt.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://ci.szxytkj.cn

[R31] 局部变量
来源：http://sv.newstarts.cn


<!-- 参考信息 -->