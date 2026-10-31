代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zt.521024.cn

TS:   if (x == null) {}
来源：http://ul.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xr.newstarts.cn

Go:   if x == nil {}
来源：http://ab.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jt.9csxet.cn

C#:   if (x is null) {}
来源：http://xl.lnxyls.cn

[P07] 防抖与节流
来源：http://op.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pq.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://xa.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rs.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lk.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jm.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hq.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tg.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pi.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://cc.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xp.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ny.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bp.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ki.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wf.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fm.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bj.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ao.colortex.cn

================================================================================
来源：http://op.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zn.nszjky.cn

================================================================================
来源：http://pl.shxzskj.cn

[Q01] 创建表
来源：http://wy.szsharing.cn

CREATE TABLE users (
来源：http://oo.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xu.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://cj.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://bw.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://op.521024.cn

);
来源：http://zq.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://ro.hnjuh.cn

CREATE TABLE orders (
来源：http://zc.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eh.panjiajie.cn

user_id INT NOT NULL,
来源：http://mi.huanxung.cn

amount DECIMAL(10, 2),
来源：http://af.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bl.asd995.cn

);
来源：http://na.9csxet.cn

[Q03] 增加列
来源：http://bb.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pa.bookmarksfly.cn

[Q04] 修改列类型
来源：http://gv.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ca.chemitech.net.cn

[Q05] 重命名列
来源：http://bq.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://po.szsharing.cn

[Q06] 删除列
来源：http://vo.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vv.shxzskj.cn

[Q07] 删除表
来源：http://sv.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://ds.wgjwhj.cn

[Q08] 创建普通索引
来源：http://mt.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gn.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://ax.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rw.bjjhwx.cn

[Q10] 插入单行
来源：http://xx.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://du.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://or.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bu.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://ok.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ez.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oe.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://gp.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://in.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ij.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ge.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kj.wgjwhj.cn

[Q15] 查询全部
来源：http://ru.yuntaijiaju.cn

SELECT * FROM users;
来源：http://rn.szsharing.cn

[Q16] 查询指定列
来源：http://lu.hahajie.cn

SELECT id, name FROM users;
来源：http://ni.newstarts.cn

[Q17] 条件查询
来源：http://jr.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mo.jctech888.com.cn

[Q18] 模糊匹配
来源：http://ue.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xi.szxytkj.cn

[Q19] 范围查询
来源：http://rg.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mf.shtwfgs.cn

[Q20] IN 列表
来源：http://vp.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wy.huanxung.cn

[Q21] 空值判断
来源：http://wh.hnjuh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mp.chemitech.net.cn

[Q22] 排序
来源：http://lo.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nw.szsharing.cn

[Q23] 分页
来源：http://mg.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hm.colortex.cn

[Q24] 去重
来源：http://ej.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://gf.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://ju.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ux.colortex.cn

[Q26] 计数
来源：http://bh.521024.cn

SELECT COUNT(*) FROM users;
来源：http://qd.haigaiapp.cn

[Q27] 条件计数
来源：http://xc.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xl.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://qs.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rx.yuexingan06.cn

[Q29] 最大最小值
来源：http://wh.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://no.muxihuayi.cn

[Q30] 分组统计
来源：http://ok.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ge.9csxet.cn

[Q31] 分组后过滤
来源：http://vv.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fv.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://ji.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sk.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yj.huanxung.cn

[Q33] 多列分组
来源：http://xu.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nj.huanxung.cn

[Q34] 每组取第一条
来源：http://eo.colortex.cn

SELECT * FROM (
来源：http://vb.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yf.szxytkj.cn

) t WHERE rn = 1;
来源：http://gr.huixinmuqiang.cn

[Q35] 内连接
来源：http://yc.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rq.yuexingan06.cn

[Q36] 左连接
来源：http://vt.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pv.newstarts.cn

[Q37] 右连接
来源：http://zo.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tc.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://an.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ga.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://ay.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mh.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gi.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://og.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sv.9csxet.cn

[Q41] 多表连接
来源：http://pm.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lj.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://px.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://hy.asd995.cn

[Q42] 连接条件附加过滤
来源：http://zx.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://re.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dv.huanxung.cn

[Q43] 标量子查询
来源：http://ov.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qu.bjjhwx.cn

[Q44] IN 子查询
来源：http://vs.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xa.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://jh.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nv.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pf.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gl.wgjwhj.cn

[Q47] 与平均值比较
来源：http://vp.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dp.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://ua.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ec.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://fu.huanxung.cn

[Q49] 更新单行
来源：http://vb.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nj.newstarts.cn

[Q50] 批量更新
来源：http://tl.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yl.chemitech.net.cn

[Q51] 用子查询更新
来源：http://na.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ad.szxytkj.cn

[Q52] 删除指定行
来源：http://to.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://dc.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://wo.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zj.9csxet.cn

[Q54] 清空表
来源：http://ln.asd995.cn

TRUNCATE TABLE logs;
来源：http://ww.asd995.cn

[Q55] 排名（并列占位）
来源：http://rz.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aq.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://di.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oq.muxihuayi.cn

[Q57] 行号
来源：http://oq.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://em.muxihuayi.cn

[Q58] 累计求和
来源：http://aw.lnxyls.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bm.newstarts.cn

[Q59] 分组内累计
来源：http://ob.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mu.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://rr.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zv.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mn.gzmigu.cn

[Q61] 移动平均
来源：http://od.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vq.asd995.cn

[Q62] 分组占比
来源：http://ml.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xn.colortex.cn

[Q63] 开启事务
来源：http://sc.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ue.wgjwhj.cn

[Q64] 提交事务
来源：http://sj.shxzukj.cn

COMMIT;
来源：http://nq.jctech888.com.cn

[Q65] 回滚事务
来源：http://cx.9csxet.cn

ROLLBACK;
来源：http://oy.gzmigu.cn

[Q66] 行锁查询
来源：http://uf.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://ic.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ss.shxzskj.cn

[Q68] 保存点
来源：http://mg.haigaiapp.cn

SAVEPOINT sp1;
来源：http://qf.panjiajie.cn

ROLLBACK TO sp1;
来源：http://pd.huanxung.cn

[Q69] 查看执行计划
来源：http://vs.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wl.haigaiapp.cn

[Q70] 更新统计信息
来源：http://ud.shxzukj.cn

ANALYZE TABLE users;
来源：http://py.hahajie.cn

[Q71] 查看建表语句
来源：http://ui.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yv.gzmigu.cn

[Q72] 查看索引
来源：http://gk.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://eu.yuexingan06.cn

[Q73] 查看表状态
来源：http://tx.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bm.hahajie.cn

[Q74] 强制使用索引
来源：http://cp.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bd.shxzskj.cn

[Q75] 日期格式化
来源：http://eh.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zg.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rz.asd995.cn

[Q76] 按天统计
来源：http://sb.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gs.521024.cn

[Q77] 时间加减
来源：http://yb.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pr.wgjwhj.cn

[Q78] 当前时间
来源：http://bm.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yv.gzmigu.cn

[Q79] 字符串拼接
来源：http://tl.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sm.panjiajie.cn

[Q80] 字符串截取
来源：http://xj.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ye.colortex.cn

[Q81] 字符串替换
来源：http://lt.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fh.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://mf.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://au.bookmarksfly.cn

[Q83] 大小写转换
来源：http://fp.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qq.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://bi.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://hh.lnxyls.cn

[Q85] 数值取整
来源：http://qc.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zv.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://um.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dz.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://ko.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ie.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://si.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tz.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ji.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://ck.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://st.shxzukj.cn

[Q90] 生成序号列
来源：http://ke.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ze.hahajie.cn

================================================================================
来源：http://ri.shxzskj.cn

R. Bash 专题
来源：http://ej.huixiangedu.cn

================================================================================
来源：http://mx.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://zk.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://gs.huixinmuqiang.cn

set -euo pipefail
来源：http://yr.521024.cn

[R02] 变量赋值与使用
来源：http://it.lnxyls.cn

name="Tom"; echo "$name"
来源：http://qy.szsharing.cn

[R03] 只读变量
来源：http://ol.muxihuayi.cn

readonly PI=3.14
来源：http://zz.bjjhwx.cn

[R04] 位置参数
来源：http://gh.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ja.szsharing.cn

[R05] 参数默认值
来源：http://fq.nicolike.cn

name="${1:-default}"
来源：http://vq.huanxung.cn

[R06] 判断命令是否存在
来源：http://lc.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rz.huanxung.cn

[R07] if 判断文件
来源：http://ff.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qj.shtwfgs.cn

[R08] 数值比较
来源：http://ju.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qt.hahajie.cn

[R09] 字符串比较
来源：http://zt.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hs.gzmigu.cn

[R10] 正则匹配
来源：http://do.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ix.521024.cn

[R11] case 多分支
来源：http://wp.9csxet.cn

case "$1" in
来源：http://dg.bjjhwx.cn

start) echo "启动" ;;
来源：http://nd.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://av.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://yp.hahajie.cn

esac
来源：http://qo.szxytkj.cn

[R12] for 遍历文件
来源：http://lv.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://lf.haigaiapp.cn

[R13] for 计数循环
来源：http://ra.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://np.shtwfgs.cn

[R14] C 风格 for
来源：http://bu.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kv.521024.cn

[R15] while 逐行读文件
来源：http://oq.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zf.huixinmuqiang.cn

[R16] until 等待条件
来源：http://ba.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ue.yuexingan06.cn

[R17] 数组定义与取值
来源：http://ba.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aq.yuexingan06.cn

[R18] 遍历数组
来源：http://ys.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vp.haigaiapp.cn

[R19] 数组长度
来源：http://gu.huixiangedu.cn

echo "${#arr[@]}"
来源：http://cv.shxzskj.cn

[R20] 关联数组（字典）
来源：http://qe.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yt.huixiangedu.cn

[R21] 字符串长度
来源：http://hj.szxytkj.cn

echo "${#s}"
来源：http://mh.yuexingan06.cn

[R22] 截取子串
来源：http://xh.hahajie.cn

echo "${s:0:5}"
来源：http://az.hnjuh.cn

[R23] 字符串替换
来源：http://wi.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ju.jctech888.com.cn

[R24] 大小写转换
来源：http://nz.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sv.jctech888.com.cn

[R25] 去后缀 / 去前缀
来源：http://gm.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lg.9csxet.cn

[R26] 命令替换
来源：http://qn.colortex.cn

now=$(date +%F); echo "$now"
来源：http://dc.huixiangedu.cn

[R27] 算术展开
来源：http://ho.jctech888.com.cn

echo $((1 + 2 * 3))
来源：http://lo.hahajie.cn

[R28] 浮点运算
来源：http://ix.521024.cn

echo "scale=2; 10/3" | bc
来源：http://zx.colortex.cn

[R29] 定义函数
来源：http://ax.haigaiapp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kn.shtwfgs.cn

[R30] 函数返回状态码
来源：http://dy.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://ea.chemitech.net.cn

[R31] 局部变量
来源：http://zy.shxzukj.cn


<!-- 参考信息 -->