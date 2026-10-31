代发 wailian999

PHP:  // 手写时间戳比较
来源：http://nl.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pg.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tx.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uo.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yc.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://th.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vf.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://mz.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xv.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xs.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hq.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hi.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mf.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qy.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gj.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fy.shxzskj.cn

================================================================================
来源：http://ds.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wl.gzmigu.cn

================================================================================
来源：http://by.hnjuh.cn

[Q01] 创建表
来源：http://ju.lnxyls.cn

CREATE TABLE users (
来源：http://cs.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bq.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ey.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://wo.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qg.521024.cn

);
来源：http://mb.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://zn.bookmarksfly.cn

CREATE TABLE orders (
来源：http://sg.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://or.colortex.cn

user_id INT NOT NULL,
来源：http://js.521024.cn

amount DECIMAL(10, 2),
来源：http://jx.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lk.bookmarksfly.cn

);
来源：http://ed.521024.cn

[Q03] 增加列
来源：http://lq.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iy.haigaiapp.cn

[Q04] 修改列类型
来源：http://jg.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://su.szsharing.cn

[Q05] 重命名列
来源：http://gf.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wg.huixinmuqiang.cn

[Q06] 删除列
来源：http://ih.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gs.wgjwhj.cn

[Q07] 删除表
来源：http://rh.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://kn.shxzukj.cn

[Q08] 创建普通索引
来源：http://rj.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dw.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://pc.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lu.bookmarksfly.cn

[Q10] 插入单行
来源：http://oe.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wr.shxzskj.cn

[Q11] 一次插入多行
来源：http://km.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vv.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://nf.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fv.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zc.nicolike.cn

[Q13] 忽略重复插入
来源：http://xz.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://it.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://ld.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lq.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ih.yuntaijiaju.cn

[Q15] 查询全部
来源：http://la.bjjhwx.cn

SELECT * FROM users;
来源：http://wd.shxzukj.cn

[Q16] 查询指定列
来源：http://vd.bjjhwx.cn

SELECT id, name FROM users;
来源：http://ws.nicolike.cn

[Q17] 条件查询
来源：http://gx.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jv.haigaiapp.cn

[Q18] 模糊匹配
来源：http://qt.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rq.huixiangedu.cn

[Q19] 范围查询
来源：http://rc.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sl.gzmigu.cn

[Q20] IN 列表
来源：http://gz.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rw.haigaiapp.cn

[Q21] 空值判断
来源：http://qn.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xo.hahajie.cn

[Q22] 排序
来源：http://zq.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wi.bjjhwx.cn

[Q23] 分页
来源：http://mn.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hk.bjjhwx.cn

[Q24] 去重
来源：http://if.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://kl.hahajie.cn

[Q25] 只取前 N 条
来源：http://fp.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ck.muxihuayi.cn

[Q26] 计数
来源：http://at.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://wa.shtwfgs.cn

[Q27] 条件计数
来源：http://rp.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aa.gzmigu.cn

[Q28] 求和与平均
来源：http://gd.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iu.gzmigu.cn

[Q29] 最大最小值
来源：http://vk.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gy.huixinmuqiang.cn

[Q30] 分组统计
来源：http://mx.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pn.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://vp.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jo.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://xh.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vh.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hk.jianghongdianzi.cn

[Q33] 多列分组
来源：http://vk.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tv.hahajie.cn

[Q34] 每组取第一条
来源：http://ay.huixiangedu.cn

SELECT * FROM (
来源：http://ls.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tl.muxihuayi.cn

) t WHERE rn = 1;
来源：http://fx.szxytkj.cn

[Q35] 内连接
来源：http://bc.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wv.muxihuayi.cn

[Q36] 左连接
来源：http://ge.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ou.muxihuayi.cn

[Q37] 右连接
来源：http://ol.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bf.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jx.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kt.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://sr.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://su.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ee.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://as.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ch.gzmigu.cn

[Q41] 多表连接
来源：http://il.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mv.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://em.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://jy.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://gv.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://hf.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hh.bookmarksfly.cn

[Q43] 标量子查询
来源：http://qg.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wz.colortex.cn

[Q44] IN 子查询
来源：http://gx.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fa.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://lt.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dg.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rm.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mv.shxzukj.cn

[Q47] 与平均值比较
来源：http://gw.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wh.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://hd.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mo.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://dv.9csxet.cn

[Q49] 更新单行
来源：http://yu.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wt.lnxyls.cn

[Q50] 批量更新
来源：http://nq.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pa.bjjhwx.cn

[Q51] 用子查询更新
来源：http://mp.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wn.bjjhwx.cn

[Q52] 删除指定行
来源：http://am.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://pc.muxihuayi.cn

[Q53] 按条件删除
来源：http://yl.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gj.yuntaijiaju.cn

[Q54] 清空表
来源：http://nb.9csxet.cn

TRUNCATE TABLE logs;
来源：http://nf.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://he.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://co.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://kk.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yv.huanxung.cn

[Q57] 行号
来源：http://vm.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gi.jianghongdianzi.cn

[Q58] 累计求和
来源：http://pe.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yf.nszjky.cn

[Q59] 分组内累计
来源：http://qw.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://db.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://ju.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ix.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rp.chemitech.net.cn

[Q61] 移动平均
来源：http://fs.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dr.huixiangedu.cn

[Q62] 分组占比
来源：http://bi.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ze.yuntaijiaju.cn

[Q63] 开启事务
来源：http://fu.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iu.lnxyls.cn

[Q64] 提交事务
来源：http://jd.gzmigu.cn

COMMIT;
来源：http://ow.wgjwhj.cn

[Q65] 回滚事务
来源：http://vf.huanxung.cn

ROLLBACK;
来源：http://kw.chemitech.net.cn

[Q66] 行锁查询
来源：http://oy.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nc.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://nn.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zn.huixiangedu.cn

[Q68] 保存点
来源：http://iu.szsharing.cn

SAVEPOINT sp1;
来源：http://wn.huanxung.cn

ROLLBACK TO sp1;
来源：http://dh.newstarts.cn

[Q69] 查看执行计划
来源：http://rd.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://is.szsharing.cn

[Q70] 更新统计信息
来源：http://km.hahajie.cn

ANALYZE TABLE users;
来源：http://hv.521024.cn

[Q71] 查看建表语句
来源：http://qg.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nq.wgjwhj.cn

[Q72] 查看索引
来源：http://ml.521024.cn

SHOW INDEX FROM users;
来源：http://lq.asd995.cn

[Q73] 查看表状态
来源：http://dy.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rl.521024.cn

[Q74] 强制使用索引
来源：http://eu.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cs.9csxet.cn

[Q75] 日期格式化
来源：http://hi.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vo.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nd.hnjuh.cn

[Q76] 按天统计
来源：http://ms.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zs.shxzukj.cn

[Q77] 时间加减
来源：http://rj.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zl.huixinmuqiang.cn

[Q78] 当前时间
来源：http://ec.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dv.asd995.cn

[Q79] 字符串拼接
来源：http://ck.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dr.szsharing.cn

[Q80] 字符串截取
来源：http://zv.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gk.gzmigu.cn

[Q81] 字符串替换
来源：http://ln.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yv.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://gz.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yp.nicolike.cn

[Q83] 大小写转换
来源：http://ki.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ld.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://sl.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://gl.shxzskj.cn

[Q85] 数值取整
来源：http://vy.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ga.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://cb.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jt.nszjky.cn

[Q87] JSON 字段做条件
来源：http://ju.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qv.muxihuayi.cn

[Q88] 行转列（条件聚合）
来源：http://mq.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zj.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gs.colortex.cn

[Q89] 判断表是否存在
来源：http://se.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ye.szsharing.cn

[Q90] 生成序号列
来源：http://qa.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xf.huixinmuqiang.cn

================================================================================
来源：http://ht.huixiangedu.cn

R. Bash 专题
来源：http://av.shxzukj.cn

================================================================================
来源：http://yo.nszjky.cn

[R01] shebang 与严格模式
来源：http://bx.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://ze.wgjwhj.cn

set -euo pipefail
来源：http://hs.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://ue.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://iy.huixiangedu.cn

[R03] 只读变量
来源：http://vp.521024.cn

readonly PI=3.14
来源：http://ly.jianghongdianzi.cn

[R04] 位置参数
来源：http://dx.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ep.szsharing.cn

[R05] 参数默认值
来源：http://bz.bookmarksfly.cn

name="${1:-default}"
来源：http://oq.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://cx.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jr.nicolike.cn

[R07] if 判断文件
来源：http://zp.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ri.szxytkj.cn

[R08] 数值比较
来源：http://ar.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xc.521024.cn

[R09] 字符串比较
来源：http://ly.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://si.newstarts.cn

[R10] 正则匹配
来源：http://wp.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vz.szsharing.cn

[R11] case 多分支
来源：http://pw.shtwfgs.cn

case "$1" in
来源：http://ru.newstarts.cn

start) echo "启动" ;;
来源：http://pe.hahajie.cn

stop)  echo "停止" ;;
来源：http://mr.521024.cn

*)     echo "未知命令" ;;
来源：http://lc.shxzukj.cn

esac
来源：http://cl.szsharing.cn

[R12] for 遍历文件
来源：http://nw.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://lp.521024.cn

[R13] for 计数循环
来源：http://su.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://hu.nszjky.cn

[R14] C 风格 for
来源：http://iv.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ck.huanxung.cn

[R15] while 逐行读文件
来源：http://oe.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ef.9csxet.cn

[R16] until 等待条件
来源：http://ma.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ra.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://wy.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ue.521024.cn

[R18] 遍历数组
来源：http://uw.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jz.wgjwhj.cn

[R19] 数组长度
来源：http://be.gzmigu.cn

echo "${#arr[@]}"
来源：http://xf.huanxung.cn

[R20] 关联数组（字典）
来源：http://gh.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://py.jctech888.com.cn

[R21] 字符串长度
来源：http://ec.huanxung.cn

echo "${#s}"
来源：http://gu.shtwfgs.cn

[R22] 截取子串
来源：http://ds.9csxet.cn

echo "${s:0:5}"
来源：http://au.asd995.cn

[R23] 字符串替换
来源：http://iu.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://up.asd995.cn

[R24] 大小写转换
来源：http://qn.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nk.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://ja.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ip.bookmarksfly.cn

[R26] 命令替换
来源：http://qv.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://st.jianghongdianzi.cn

[R27] 算术展开
来源：http://yl.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://zi.panjiajie.cn

[R28] 浮点运算
来源：http://kr.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://xh.lnxyls.cn

[R29] 定义函数
来源：http://wq.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nx.shtwfgs.cn

[R30] 函数返回状态码
来源：http://dt.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://fc.gzmigu.cn

[R31] 局部变量
来源：http://pj.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://ub.haigaiapp.cn

[R32] 参数个数校验
来源：http://dl.jianghongdianzi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://st.colortex.cn

[R33] 捕获错误并提示行号
来源：http://cz.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yw.panjiajie.cn

[R34] 退出时清理
来源：http://kj.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tz.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://fl.jctech888.com.cn


<!-- 参考信息 -->