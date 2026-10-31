代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kb.521024.cn

C#:   if (x is null) {}
来源：http://hl.panjiajie.cn

[P07] 防抖与节流
来源：http://qm.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zx.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://jv.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ua.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yq.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rq.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nz.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ss.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nh.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://et.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xx.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ex.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sr.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gz.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://df.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sd.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cw.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mt.huixinmuqiang.cn

================================================================================
来源：http://wk.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ek.nicolike.cn

================================================================================
来源：http://oi.nicolike.cn

[Q01] 创建表
来源：http://uq.newstarts.cn

CREATE TABLE users (
来源：http://ku.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eu.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://op.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://xe.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bf.wgjwhj.cn

);
来源：http://ap.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://jy.nszjky.cn

CREATE TABLE orders (
来源：http://ix.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vw.huanxung.cn

user_id INT NOT NULL,
来源：http://dq.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://yp.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ya.gzmigu.cn

);
来源：http://wo.muxihuayi.cn

[Q03] 增加列
来源：http://bz.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jr.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://sc.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vb.colortex.cn

[Q05] 重命名列
来源：http://gj.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qo.wgjwhj.cn

[Q06] 删除列
来源：http://ee.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hz.huanxung.cn

[Q07] 删除表
来源：http://fc.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://qe.yuexingan06.cn

[Q08] 创建普通索引
来源：http://ki.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ok.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://db.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fp.newstarts.cn

[Q10] 插入单行
来源：http://yl.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ij.asd995.cn

[Q11] 一次插入多行
来源：http://bn.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oy.521024.cn

[Q12] 插入后取自增 ID
来源：http://ue.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ss.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eb.huanxung.cn

[Q13] 忽略重复插入
来源：http://wz.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xr.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://ub.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tf.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://za.colortex.cn

[Q15] 查询全部
来源：http://fx.muxihuayi.cn

SELECT * FROM users;
来源：http://ub.bjjhwx.cn

[Q16] 查询指定列
来源：http://xt.szsharing.cn

SELECT id, name FROM users;
来源：http://kl.9csxet.cn

[Q17] 条件查询
来源：http://do.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fp.haigaiapp.cn

[Q18] 模糊匹配
来源：http://hv.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zv.jctech888.com.cn

[Q19] 范围查询
来源：http://qu.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://of.nicolike.cn

[Q20] IN 列表
来源：http://xd.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tc.colortex.cn

[Q21] 空值判断
来源：http://gp.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vw.gzmigu.cn

[Q22] 排序
来源：http://ya.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tw.chemitech.net.cn

[Q23] 分页
来源：http://qf.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fk.shxzskj.cn

[Q24] 去重
来源：http://nt.jctech888.com.cn

SELECT DISTINCT city FROM users;
来源：http://pl.lnxyls.cn

[Q25] 只取前 N 条
来源：http://eb.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xt.szxytkj.cn

[Q26] 计数
来源：http://et.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://pa.jianghongdianzi.cn

[Q27] 条件计数
来源：http://ro.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vb.chemitech.net.cn

[Q28] 求和与平均
来源：http://sv.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uq.newstarts.cn

[Q29] 最大最小值
来源：http://jk.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tz.hnjuh.cn

[Q30] 分组统计
来源：http://tr.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cs.nszjky.cn

[Q31] 分组后过滤
来源：http://gg.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xq.szsharing.cn

[Q32] 分组拼接字符串
来源：http://hv.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zp.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sh.huixinmuqiang.cn

[Q33] 多列分组
来源：http://fy.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ve.muxihuayi.cn

[Q34] 每组取第一条
来源：http://nl.asd995.cn

SELECT * FROM (
来源：http://hz.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hn.hahajie.cn

) t WHERE rn = 1;
来源：http://qh.newstarts.cn

[Q35] 内连接
来源：http://zm.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wh.bjjhwx.cn

[Q36] 左连接
来源：http://nr.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zl.nicolike.cn

[Q37] 右连接
来源：http://tj.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://la.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sw.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fx.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://gk.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sz.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ff.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kt.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://si.bookmarksfly.cn

[Q41] 多表连接
来源：http://by.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jj.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://wa.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://yx.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://qi.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://sf.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bl.newstarts.cn

[Q43] 标量子查询
来源：http://mi.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ii.chemitech.net.cn

[Q44] IN 子查询
来源：http://cv.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pu.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://zs.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eo.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lg.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gl.hnjuh.cn

[Q47] 与平均值比较
来源：http://nj.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gk.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://nn.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bi.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://os.bookmarksfly.cn

[Q49] 更新单行
来源：http://el.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tx.yuexingan06.cn

[Q50] 批量更新
来源：http://ms.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://av.nszjky.cn

[Q51] 用子查询更新
来源：http://hy.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yv.shtwfgs.cn

[Q52] 删除指定行
来源：http://fx.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://in.wgjwhj.cn

[Q53] 按条件删除
来源：http://bt.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bn.hahajie.cn

[Q54] 清空表
来源：http://tj.nicolike.cn

TRUNCATE TABLE logs;
来源：http://nz.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://on.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mz.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://bg.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bq.nicolike.cn

[Q57] 行号
来源：http://ng.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ap.szsharing.cn

[Q58] 累计求和
来源：http://ex.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ye.gzmigu.cn

[Q59] 分组内累计
来源：http://mr.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sa.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://no.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zk.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ht.bjjhwx.cn

[Q61] 移动平均
来源：http://oe.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yz.colortex.cn

[Q62] 分组占比
来源：http://ge.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qt.shxzukj.cn

[Q63] 开启事务
来源：http://uz.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qe.bookmarksfly.cn

[Q64] 提交事务
来源：http://dv.bookmarksfly.cn

COMMIT;
来源：http://ya.shtwfgs.cn

[Q65] 回滚事务
来源：http://nm.wgjwhj.cn

ROLLBACK;
来源：http://la.hahajie.cn

[Q66] 行锁查询
来源：http://bf.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sg.colortex.cn

[Q67] 设置隔离级别
来源：http://xq.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zy.nicolike.cn

[Q68] 保存点
来源：http://kr.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://yd.newstarts.cn

ROLLBACK TO sp1;
来源：http://wd.asd995.cn

[Q69] 查看执行计划
来源：http://oy.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rb.szxytkj.cn

[Q70] 更新统计信息
来源：http://qk.gzmigu.cn

ANALYZE TABLE users;
来源：http://os.asd995.cn

[Q71] 查看建表语句
来源：http://wz.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ex.szsharing.cn

[Q72] 查看索引
来源：http://rm.521024.cn

SHOW INDEX FROM users;
来源：http://zj.newstarts.cn

[Q73] 查看表状态
来源：http://sa.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nf.shxzukj.cn

[Q74] 强制使用索引
来源：http://ei.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qk.hnjuh.cn

[Q75] 日期格式化
来源：http://ki.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uw.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ef.haigaiapp.cn

[Q76] 按天统计
来源：http://zb.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ys.9csxet.cn

[Q77] 时间加减
来源：http://yw.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vh.yuexingan06.cn

[Q78] 当前时间
来源：http://id.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://se.9csxet.cn

[Q79] 字符串拼接
来源：http://xg.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qf.lnxyls.cn

[Q80] 字符串截取
来源：http://jq.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dz.huanxung.cn

[Q81] 字符串替换
来源：http://bd.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ky.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://xw.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zv.colortex.cn

[Q83] 大小写转换
来源：http://ml.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sc.lnxyls.cn

[Q84] 去除首尾空格
来源：http://jj.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://ii.haigaiapp.cn

[Q85] 数值取整
来源：http://wk.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://os.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://tz.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jg.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://rx.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fy.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://et.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ni.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://np.newstarts.cn

[Q89] 判断表是否存在
来源：http://dl.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zv.huixiangedu.cn

[Q90] 生成序号列
来源：http://sr.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qa.newstarts.cn

================================================================================
来源：http://ho.wgjwhj.cn

R. Bash 专题
来源：http://oj.gzmigu.cn

================================================================================
来源：http://yc.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://jj.szxytkj.cn

#!/usr/bin/env bash
来源：http://kb.shtwfgs.cn

set -euo pipefail
来源：http://bl.huixiangedu.cn

[R02] 变量赋值与使用
来源：http://nm.szxytkj.cn

name="Tom"; echo "$name"
来源：http://ng.shtwfgs.cn

[R03] 只读变量
来源：http://vw.jianghongdianzi.cn

readonly PI=3.14
来源：http://vz.szsharing.cn

[R04] 位置参数
来源：http://zg.bjjhwx.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kj.huanxung.cn

[R05] 参数默认值
来源：http://zl.colortex.cn

name="${1:-default}"
来源：http://ed.nicolike.cn

[R06] 判断命令是否存在
来源：http://yu.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zu.nszjky.cn

[R07] if 判断文件
来源：http://wb.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hc.huixiangedu.cn

[R08] 数值比较
来源：http://cq.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oc.colortex.cn

[R09] 字符串比较
来源：http://ds.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://op.hahajie.cn

[R10] 正则匹配
来源：http://ev.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cw.newstarts.cn

[R11] case 多分支
来源：http://jh.shtwfgs.cn

case "$1" in
来源：http://gh.asd995.cn

start) echo "启动" ;;
来源：http://ll.nszjky.cn

stop)  echo "停止" ;;
来源：http://yd.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://tr.nszjky.cn

esac
来源：http://xi.shtwfgs.cn

[R12] for 遍历文件
来源：http://vx.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://ra.hahajie.cn

[R13] for 计数循环
来源：http://qv.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ca.wgjwhj.cn

[R14] C 风格 for
来源：http://nx.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ad.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://qu.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tv.9csxet.cn

[R16] until 等待条件
来源：http://wp.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qh.nicolike.cn

[R17] 数组定义与取值
来源：http://cv.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bg.haigaiapp.cn

[R18] 遍历数组
来源：http://sh.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ei.haigaiapp.cn

[R19] 数组长度
来源：http://qu.newstarts.cn

echo "${#arr[@]}"
来源：http://ll.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://ye.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ef.huixiangedu.cn

[R21] 字符串长度
来源：http://qs.nicolike.cn

echo "${#s}"
来源：http://ep.gzmigu.cn

[R22] 截取子串
来源：http://jw.panjiajie.cn

echo "${s:0:5}"
来源：http://ww.haigaiapp.cn

[R23] 字符串替换
来源：http://yx.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://al.huixinmuqiang.cn

[R24] 大小写转换
来源：http://qb.nszjky.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cv.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://uc.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pq.shtwfgs.cn

[R26] 命令替换
来源：http://nf.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://um.shxzukj.cn

[R27] 算术展开
来源：http://yc.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ss.huixiangedu.cn

[R28] 浮点运算
来源：http://dv.bjjhwx.cn

echo "scale=2; 10/3" | bc
来源：http://eb.yuntaijiaju.cn

[R29] 定义函数
来源：http://zv.wgjwhj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yu.newstarts.cn

[R30] 函数返回状态码
来源：http://us.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://bu.shxzukj.cn

[R31] 局部变量
来源：http://yy.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://db.bookmarksfly.cn

[R32] 参数个数校验
来源：http://jt.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uw.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://yy.9csxet.cn


<!-- 参考信息 -->