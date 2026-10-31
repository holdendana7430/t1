代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yg.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://tz.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hw.haigaiapp.cn

Go:   if x == nil {}
来源：http://wa.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nn.hnjuh.cn

C#:   if (x is null) {}
来源：http://qa.hnjuh.cn

[P07] 防抖与节流
来源：http://yq.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xg.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://kn.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fc.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wr.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vl.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wx.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vc.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ut.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://xl.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ub.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sd.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jn.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ew.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mg.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nf.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ek.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ji.huixinmuqiang.cn

================================================================================
来源：http://jv.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vz.huixinmuqiang.cn

================================================================================
来源：http://bp.wgjwhj.cn

[Q01] 创建表
来源：http://ti.lnxyls.cn

CREATE TABLE users (
来源：http://qi.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hf.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://nv.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://hk.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dd.9csxet.cn

);
来源：http://hh.nicolike.cn

[Q02] 创建带外键的表
来源：http://cy.521024.cn

CREATE TABLE orders (
来源：http://nq.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sb.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://oo.asd995.cn

amount DECIMAL(10, 2),
来源：http://aq.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vk.nszjky.cn

);
来源：http://gc.szsharing.cn

[Q03] 增加列
来源：http://sx.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vl.szxytkj.cn

[Q04] 修改列类型
来源：http://px.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hk.yuexingan06.cn

[Q05] 重命名列
来源：http://fm.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lw.muxihuayi.cn

[Q06] 删除列
来源：http://bt.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hn.lnxyls.cn

[Q07] 删除表
来源：http://es.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://rr.shtwfgs.cn

[Q08] 创建普通索引
来源：http://id.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vw.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://he.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wo.gzmigu.cn

[Q10] 插入单行
来源：http://wv.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wf.asd995.cn

[Q11] 一次插入多行
来源：http://cz.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lx.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://vx.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ys.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fl.gzmigu.cn

[Q13] 忽略重复插入
来源：http://vm.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gb.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://rn.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://np.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nl.521024.cn

[Q15] 查询全部
来源：http://um.yuntaijiaju.cn

SELECT * FROM users;
来源：http://ce.jctech888.com.cn

[Q16] 查询指定列
来源：http://wp.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://xu.hnjuh.cn

[Q17] 条件查询
来源：http://cj.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vb.hahajie.cn

[Q18] 模糊匹配
来源：http://er.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vr.bjjhwx.cn

[Q19] 范围查询
来源：http://gn.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ib.haigaiapp.cn

[Q20] IN 列表
来源：http://gv.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://po.wgjwhj.cn

[Q21] 空值判断
来源：http://kn.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tc.lnxyls.cn

[Q22] 排序
来源：http://nw.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fx.panjiajie.cn

[Q23] 分页
来源：http://vx.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ce.nicolike.cn

[Q24] 去重
来源：http://rc.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://wp.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://sf.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yi.szxytkj.cn

[Q26] 计数
来源：http://xe.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://kz.bjjhwx.cn

[Q27] 条件计数
来源：http://jh.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ny.nszjky.cn

[Q28] 求和与平均
来源：http://qb.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://my.newstarts.cn

[Q29] 最大最小值
来源：http://jz.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rq.hahajie.cn

[Q30] 分组统计
来源：http://cc.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yf.newstarts.cn

[Q31] 分组后过滤
来源：http://lq.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ae.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://le.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lj.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qj.shxzskj.cn

[Q33] 多列分组
来源：http://uo.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nh.521024.cn

[Q34] 每组取第一条
来源：http://fi.wgjwhj.cn

SELECT * FROM (
来源：http://ax.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ej.jctech888.com.cn

) t WHERE rn = 1;
来源：http://jk.huanxung.cn

[Q35] 内连接
来源：http://pr.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lh.chemitech.net.cn

[Q36] 左连接
来源：http://zh.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xz.jianghongdianzi.cn

[Q37] 右连接
来源：http://qe.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zw.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zp.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jy.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://ez.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gw.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jn.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vx.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rh.9csxet.cn

[Q41] 多表连接
来源：http://oj.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ya.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://se.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://dm.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://ww.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://za.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yl.lnxyls.cn

[Q43] 标量子查询
来源：http://qe.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ic.shxzukj.cn

[Q44] IN 子查询
来源：http://ox.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ho.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://yg.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bb.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wj.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://en.gzmigu.cn

[Q47] 与平均值比较
来源：http://mc.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wv.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://rs.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cy.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://wc.haigaiapp.cn

[Q49] 更新单行
来源：http://fn.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ja.hahajie.cn

[Q50] 批量更新
来源：http://cd.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cp.521024.cn

[Q51] 用子查询更新
来源：http://rq.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uo.hnjuh.cn

[Q52] 删除指定行
来源：http://zr.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://rq.jctech888.com.cn

[Q53] 按条件删除
来源：http://gm.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rg.521024.cn

[Q54] 清空表
来源：http://xs.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://cl.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://vy.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ag.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ys.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zg.asd995.cn

[Q57] 行号
来源：http://pb.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://de.gzmigu.cn

[Q58] 累计求和
来源：http://jx.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fr.521024.cn

[Q59] 分组内累计
来源：http://rm.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jj.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://ld.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zr.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://at.szsharing.cn

[Q61] 移动平均
来源：http://wd.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ga.panjiajie.cn

[Q62] 分组占比
来源：http://ez.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ms.nicolike.cn

[Q63] 开启事务
来源：http://nt.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zk.wgjwhj.cn

[Q64] 提交事务
来源：http://ux.huixiangedu.cn

COMMIT;
来源：http://rk.newstarts.cn

[Q65] 回滚事务
来源：http://wx.shtwfgs.cn

ROLLBACK;
来源：http://vh.huanxung.cn

[Q66] 行锁查询
来源：http://fy.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yo.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://eh.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ts.bookmarksfly.cn

[Q68] 保存点
来源：http://mp.haigaiapp.cn

SAVEPOINT sp1;
来源：http://xp.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://dk.bjjhwx.cn

[Q69] 查看执行计划
来源：http://it.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://np.panjiajie.cn

[Q70] 更新统计信息
来源：http://ot.bjjhwx.cn

ANALYZE TABLE users;
来源：http://kr.bjjhwx.cn

[Q71] 查看建表语句
来源：http://wf.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iu.huixinmuqiang.cn

[Q72] 查看索引
来源：http://cl.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://jh.wgjwhj.cn

[Q73] 查看表状态
来源：http://bu.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ge.colortex.cn

[Q74] 强制使用索引
来源：http://vk.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jn.bookmarksfly.cn

[Q75] 日期格式化
来源：http://om.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tt.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jn.huixinmuqiang.cn

[Q76] 按天统计
来源：http://wt.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pr.shxzskj.cn

[Q77] 时间加减
来源：http://hn.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bn.jianghongdianzi.cn

[Q78] 当前时间
来源：http://sm.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jp.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://fa.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eu.9csxet.cn

[Q80] 字符串截取
来源：http://et.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sy.szsharing.cn

[Q81] 字符串替换
来源：http://ic.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ia.asd995.cn

[Q82] 字符长度与字节长度
来源：http://zm.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cj.nicolike.cn

[Q83] 大小写转换
来源：http://fc.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rt.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://ol.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://gh.muxihuayi.cn

[Q85] 数值取整
来源：http://qn.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bi.asd995.cn

[Q86] 读取 JSON 字段
来源：http://bh.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ef.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://jd.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kc.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://ow.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ob.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pj.nicolike.cn

[Q89] 判断表是否存在
来源：http://mr.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vr.9csxet.cn

[Q90] 生成序号列
来源：http://kw.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hh.shtwfgs.cn

================================================================================
来源：http://zn.nszjky.cn

R. Bash 专题
来源：http://hj.hahajie.cn

================================================================================
来源：http://fm.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://tg.yuexingan06.cn

#!/usr/bin/env bash
来源：http://ub.panjiajie.cn

set -euo pipefail
来源：http://yz.gzmigu.cn

[R02] 变量赋值与使用
来源：http://hz.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://ar.shxzukj.cn

[R03] 只读变量
来源：http://ng.bjjhwx.cn

readonly PI=3.14
来源：http://xs.asd995.cn

[R04] 位置参数
来源：http://lr.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://di.huanxung.cn

[R05] 参数默认值
来源：http://ah.shxzskj.cn

name="${1:-default}"
来源：http://eh.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://yr.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zn.huanxung.cn

[R07] if 判断文件
来源：http://ti.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gr.yuexingan06.cn

[R08] 数值比较
来源：http://ni.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vi.haigaiapp.cn

[R09] 字符串比较
来源：http://tx.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://du.muxihuayi.cn

[R10] 正则匹配
来源：http://yv.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ua.hahajie.cn

[R11] case 多分支
来源：http://ia.jctech888.com.cn

case "$1" in
来源：http://vy.shxzukj.cn

start) echo "启动" ;;
来源：http://pd.shxzskj.cn

stop)  echo "停止" ;;
来源：http://hf.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://cm.newstarts.cn

esac
来源：http://jj.bjjhwx.cn

[R12] for 遍历文件
来源：http://xm.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://ea.huixiangedu.cn

[R13] for 计数循环
来源：http://gn.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://lo.bjjhwx.cn

[R14] C 风格 for
来源：http://fo.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uh.yuexingan06.cn

[R15] while 逐行读文件
来源：http://dq.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wp.hnjuh.cn

[R16] until 等待条件
来源：http://io.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wn.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://og.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xy.9csxet.cn

[R18] 遍历数组
来源：http://ba.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hd.shxzskj.cn

[R19] 数组长度
来源：http://pt.521024.cn

echo "${#arr[@]}"
来源：http://bo.newstarts.cn

[R20] 关联数组（字典）
来源：http://cb.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rz.asd995.cn

[R21] 字符串长度
来源：http://os.nszjky.cn

echo "${#s}"
来源：http://kn.521024.cn

[R22] 截取子串
来源：http://gy.521024.cn

echo "${s:0:5}"
来源：http://mb.huanxung.cn

[R23] 字符串替换
来源：http://lt.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mm.muxihuayi.cn

[R24] 大小写转换
来源：http://ry.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iv.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://yb.9csxet.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mq.haigaiapp.cn

[R26] 命令替换
来源：http://uo.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://bh.nicolike.cn

[R27] 算术展开
来源：http://sz.9csxet.cn

echo $((1 + 2 * 3))
来源：http://aj.bjjhwx.cn

[R28] 浮点运算
来源：http://vl.shxzukj.cn

echo "scale=2; 10/3" | bc
来源：http://lu.jianghongdianzi.cn

[R29] 定义函数
来源：http://gm.szxytkj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://to.shtwfgs.cn

[R30] 函数返回状态码
来源：http://zd.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://zo.bjjhwx.cn

[R31] 局部变量
来源：http://cy.muxihuayi.cn


<!-- 参考信息 -->