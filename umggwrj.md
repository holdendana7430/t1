代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fn.newstarts.cn

TS:   if (x == null) {}
来源：http://pk.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vw.huanxung.cn

Go:   if x == nil {}
来源：http://qu.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ys.hnjuh.cn

C#:   if (x is null) {}
来源：http://hw.jctech888.com.cn

[P07] 防抖与节流
来源：http://kl.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://re.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://pw.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nx.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://or.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iz.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ic.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nc.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vw.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://nd.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jf.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wv.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ho.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oa.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ej.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nz.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ae.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pg.huixinmuqiang.cn

================================================================================
来源：http://ev.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oy.521024.cn

================================================================================
来源：http://ea.muxihuayi.cn

[Q01] 创建表
来源：http://iq.chemitech.net.cn

CREATE TABLE users (
来源：http://ks.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mh.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://iy.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://uo.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wd.lnxyls.cn

);
来源：http://uu.hahajie.cn

[Q02] 创建带外键的表
来源：http://cc.colortex.cn

CREATE TABLE orders (
来源：http://fy.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tk.hahajie.cn

user_id INT NOT NULL,
来源：http://gt.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://nf.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zp.521024.cn

);
来源：http://om.colortex.cn

[Q03] 增加列
来源：http://ew.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kp.nicolike.cn

[Q04] 修改列类型
来源：http://po.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://as.haigaiapp.cn

[Q05] 重命名列
来源：http://xk.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dt.chemitech.net.cn

[Q06] 删除列
来源：http://wb.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bh.jctech888.com.cn

[Q07] 删除表
来源：http://de.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://ix.lnxyls.cn

[Q08] 创建普通索引
来源：http://ko.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hg.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://hq.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iw.hnjuh.cn

[Q10] 插入单行
来源：http://ep.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dx.hnjuh.cn

[Q11] 一次插入多行
来源：http://tf.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sc.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://fl.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hi.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eu.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://nw.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ko.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://dg.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ho.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ej.huanxung.cn

[Q15] 查询全部
来源：http://ev.nicolike.cn

SELECT * FROM users;
来源：http://nt.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://az.shxzukj.cn

SELECT id, name FROM users;
来源：http://yx.gzmigu.cn

[Q17] 条件查询
来源：http://wi.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rq.haigaiapp.cn

[Q18] 模糊匹配
来源：http://vw.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://un.bjjhwx.cn

[Q19] 范围查询
来源：http://bj.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lu.shtwfgs.cn

[Q20] IN 列表
来源：http://rq.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oe.haigaiapp.cn

[Q21] 空值判断
来源：http://gx.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yu.szsharing.cn

[Q22] 排序
来源：http://zn.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nn.bjjhwx.cn

[Q23] 分页
来源：http://pn.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yu.panjiajie.cn

[Q24] 去重
来源：http://fm.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://zt.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://rl.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sc.panjiajie.cn

[Q26] 计数
来源：http://fn.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://rx.nszjky.cn

[Q27] 条件计数
来源：http://ud.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qt.wgjwhj.cn

[Q28] 求和与平均
来源：http://eg.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jp.9csxet.cn

[Q29] 最大最小值
来源：http://tt.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oi.haigaiapp.cn

[Q30] 分组统计
来源：http://mc.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fq.muxihuayi.cn

[Q31] 分组后过滤
来源：http://di.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kp.9csxet.cn

[Q32] 分组拼接字符串
来源：http://cy.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yz.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://io.szsharing.cn

[Q33] 多列分组
来源：http://pt.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jo.muxihuayi.cn

[Q34] 每组取第一条
来源：http://hp.nszjky.cn

SELECT * FROM (
来源：http://ni.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pf.haigaiapp.cn

) t WHERE rn = 1;
来源：http://uh.muxihuayi.cn

[Q35] 内连接
来源：http://ke.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wv.huanxung.cn

[Q36] 左连接
来源：http://bs.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bf.asd995.cn

[Q37] 右连接
来源：http://gr.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bt.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cw.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ep.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://ss.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://se.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gr.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ss.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cm.szsharing.cn

[Q41] 多表连接
来源：http://uo.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ee.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ea.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://mw.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://la.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://qf.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lw.shxzukj.cn

[Q43] 标量子查询
来源：http://oc.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hf.wgjwhj.cn

[Q44] IN 子查询
来源：http://uj.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sw.colortex.cn

[Q45] EXISTS 判断存在
来源：http://ii.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kt.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cz.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zs.gzmigu.cn

[Q47] 与平均值比较
来源：http://pn.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rv.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://bk.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ny.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://qz.jctech888.com.cn

[Q49] 更新单行
来源：http://bo.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yo.shxzukj.cn

[Q50] 批量更新
来源：http://nt.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nk.nszjky.cn

[Q51] 用子查询更新
来源：http://iu.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dy.szxytkj.cn

[Q52] 删除指定行
来源：http://ir.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://wx.jctech888.com.cn

[Q53] 按条件删除
来源：http://cb.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qb.yuexingan06.cn

[Q54] 清空表
来源：http://ot.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://hw.huanxung.cn

[Q55] 排名（并列占位）
来源：http://vg.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gj.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://xn.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qb.jctech888.com.cn

[Q57] 行号
来源：http://rq.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hi.szsharing.cn

[Q58] 累计求和
来源：http://ln.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pk.jctech888.com.cn

[Q59] 分组内累计
来源：http://ii.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sa.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://ii.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wp.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ug.huixiangedu.cn

[Q61] 移动平均
来源：http://zl.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cj.nicolike.cn

[Q62] 分组占比
来源：http://pn.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pj.bjjhwx.cn

[Q63] 开启事务
来源：http://mm.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sf.9csxet.cn

[Q64] 提交事务
来源：http://ck.gzmigu.cn

COMMIT;
来源：http://xe.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://si.asd995.cn

ROLLBACK;
来源：http://qp.hnjuh.cn

[Q66] 行锁查询
来源：http://yd.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jj.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://yh.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ao.chemitech.net.cn

[Q68] 保存点
来源：http://ob.asd995.cn

SAVEPOINT sp1;
来源：http://tu.521024.cn

ROLLBACK TO sp1;
来源：http://yf.shxzukj.cn

[Q69] 查看执行计划
来源：http://ym.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gn.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://kl.hnjuh.cn

ANALYZE TABLE users;
来源：http://ef.gzmigu.cn

[Q71] 查看建表语句
来源：http://bo.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dr.lnxyls.cn

[Q72] 查看索引
来源：http://xj.huanxung.cn

SHOW INDEX FROM users;
来源：http://wt.hahajie.cn

[Q73] 查看表状态
来源：http://db.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pq.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://px.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bl.yuexingan06.cn

[Q75] 日期格式化
来源：http://fn.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bc.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fw.nicolike.cn

[Q76] 按天统计
来源：http://rn.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ii.colortex.cn

[Q77] 时间加减
来源：http://mo.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kc.colortex.cn

[Q78] 当前时间
来源：http://nh.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iu.hnjuh.cn

[Q79] 字符串拼接
来源：http://sh.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jk.colortex.cn

[Q80] 字符串截取
来源：http://re.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bi.lnxyls.cn

[Q81] 字符串替换
来源：http://br.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iw.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://zs.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mu.nszjky.cn

[Q83] 大小写转换
来源：http://ow.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rf.nicolike.cn

[Q84] 去除首尾空格
来源：http://mw.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://rh.bjjhwx.cn

[Q85] 数值取整
来源：http://gu.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://kl.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://to.newstarts.cn

[Q87] JSON 字段做条件
来源：http://bm.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gi.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://rk.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jx.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mt.hahajie.cn

[Q89] 判断表是否存在
来源：http://he.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vy.9csxet.cn

[Q90] 生成序号列
来源：http://ny.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gk.huixiangedu.cn

================================================================================
来源：http://jb.huixiangedu.cn

R. Bash 专题
来源：http://jb.wgjwhj.cn

================================================================================
来源：http://ky.shxzukj.cn

[R01] shebang 与严格模式
来源：http://vc.shxzskj.cn

#!/usr/bin/env bash
来源：http://gn.shxzskj.cn

set -euo pipefail
来源：http://cv.9csxet.cn

[R02] 变量赋值与使用
来源：http://vr.hahajie.cn

name="Tom"; echo "$name"
来源：http://ou.wgjwhj.cn

[R03] 只读变量
来源：http://oj.gzmigu.cn

readonly PI=3.14
来源：http://du.521024.cn

[R04] 位置参数
来源：http://fb.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bj.colortex.cn

[R05] 参数默认值
来源：http://tc.bookmarksfly.cn

name="${1:-default}"
来源：http://ax.panjiajie.cn

[R06] 判断命令是否存在
来源：http://co.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://id.gzmigu.cn

[R07] if 判断文件
来源：http://to.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eg.bookmarksfly.cn

[R08] 数值比较
来源：http://xv.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fs.muxihuayi.cn

[R09] 字符串比较
来源：http://kn.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qe.wgjwhj.cn

[R10] 正则匹配
来源：http://pu.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cl.hahajie.cn

[R11] case 多分支
来源：http://ug.nicolike.cn

case "$1" in
来源：http://ms.9csxet.cn

start) echo "启动" ;;
来源：http://cp.hahajie.cn

stop)  echo "停止" ;;
来源：http://xr.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://mt.huixinmuqiang.cn

esac
来源：http://bz.colortex.cn

[R12] for 遍历文件
来源：http://ja.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://yk.521024.cn

[R13] for 计数循环
来源：http://wn.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://te.521024.cn

[R14] C 风格 for
来源：http://da.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pm.hnjuh.cn

[R15] while 逐行读文件
来源：http://et.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ih.gzmigu.cn

[R16] until 等待条件
来源：http://zx.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://at.newstarts.cn

[R17] 数组定义与取值
来源：http://oe.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zs.newstarts.cn

[R18] 遍历数组
来源：http://pq.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dm.hahajie.cn

[R19] 数组长度
来源：http://ny.szsharing.cn

echo "${#arr[@]}"
来源：http://qw.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://sb.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lf.asd995.cn

[R21] 字符串长度
来源：http://ol.shxzskj.cn

echo "${#s}"
来源：http://wm.szxytkj.cn

[R22] 截取子串
来源：http://nu.jctech888.com.cn

echo "${s:0:5}"
来源：http://ou.nszjky.cn

[R23] 字符串替换
来源：http://fi.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gq.chemitech.net.cn

[R24] 大小写转换
来源：http://ra.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ex.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://hj.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uk.shxzskj.cn

[R26] 命令替换
来源：http://tg.jianghongdianzi.cn

now=$(date +%F); echo "$now"
来源：http://yx.wgjwhj.cn

[R27] 算术展开
来源：http://uf.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://ml.shxzukj.cn

[R28] 浮点运算
来源：http://xz.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://aj.wgjwhj.cn

[R29] 定义函数
来源：http://kp.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sm.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://wg.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://dz.bookmarksfly.cn

[R31] 局部变量
来源：http://of.wgjwhj.cn


<!-- 参考信息 -->