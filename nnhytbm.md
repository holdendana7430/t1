代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yx.asd995.cn

TS:   if (x == null) {}
来源：http://qf.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mc.panjiajie.cn

Go:   if x == nil {}
来源：http://ja.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dk.hahajie.cn

C#:   if (x is null) {}
来源：http://us.lnxyls.cn

[P07] 防抖与节流
来源：http://rc.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wt.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://so.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xi.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fs.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hk.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mz.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ol.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fr.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://vw.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uo.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mg.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ai.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vw.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nv.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iv.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nr.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sq.huixiangedu.cn

================================================================================
来源：http://hz.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sg.huixiangedu.cn

================================================================================
来源：http://ab.nicolike.cn

[Q01] 创建表
来源：http://nf.bjjhwx.cn

CREATE TABLE users (
来源：http://jg.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ug.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://wg.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://ne.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ho.wgjwhj.cn

);
来源：http://nd.shxzskj.cn

[Q02] 创建带外键的表
来源：http://he.szsharing.cn

CREATE TABLE orders (
来源：http://wt.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sw.bjjhwx.cn

user_id INT NOT NULL,
来源：http://db.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://qr.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ba.haigaiapp.cn

);
来源：http://yx.muxihuayi.cn

[Q03] 增加列
来源：http://lg.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ib.muxihuayi.cn

[Q04] 修改列类型
来源：http://ig.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wo.muxihuayi.cn

[Q05] 重命名列
来源：http://fv.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ep.gzmigu.cn

[Q06] 删除列
来源：http://bw.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://le.huanxung.cn

[Q07] 删除表
来源：http://kq.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://ac.shxzukj.cn

[Q08] 创建普通索引
来源：http://dn.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://my.huanxung.cn

[Q09] 创建唯一索引
来源：http://ib.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rb.jianghongdianzi.cn

[Q10] 插入单行
来源：http://lg.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pu.shxzskj.cn

[Q11] 一次插入多行
来源：http://iy.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qs.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://gd.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hu.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fz.asd995.cn

[Q13] 忽略重复插入
来源：http://ss.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lz.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://gg.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xh.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pf.bookmarksfly.cn

[Q15] 查询全部
来源：http://dd.huixiangedu.cn

SELECT * FROM users;
来源：http://qq.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://su.szsharing.cn

SELECT id, name FROM users;
来源：http://iz.muxihuayi.cn

[Q17] 条件查询
来源：http://xz.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vq.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://wt.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bn.nicolike.cn

[Q19] 范围查询
来源：http://qu.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vh.szsharing.cn

[Q20] IN 列表
来源：http://qk.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yc.szxytkj.cn

[Q21] 空值判断
来源：http://hf.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qp.yuexingan06.cn

[Q22] 排序
来源：http://jv.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qj.shxzskj.cn

[Q23] 分页
来源：http://rk.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eu.huanxung.cn

[Q24] 去重
来源：http://an.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://jf.hahajie.cn

[Q25] 只取前 N 条
来源：http://jb.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zu.nszjky.cn

[Q26] 计数
来源：http://lg.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://jr.gzmigu.cn

[Q27] 条件计数
来源：http://dg.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oy.bjjhwx.cn

[Q28] 求和与平均
来源：http://vk.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pd.newstarts.cn

[Q29] 最大最小值
来源：http://yu.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bi.gzmigu.cn

[Q30] 分组统计
来源：http://ol.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cm.asd995.cn

[Q31] 分组后过滤
来源：http://nv.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ka.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://up.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aa.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sw.huanxung.cn

[Q33] 多列分组
来源：http://xg.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yw.shxzskj.cn

[Q34] 每组取第一条
来源：http://lm.nszjky.cn

SELECT * FROM (
来源：http://bb.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ro.yuexingan06.cn

) t WHERE rn = 1;
来源：http://om.huanxung.cn

[Q35] 内连接
来源：http://qu.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qp.shxzukj.cn

[Q36] 左连接
来源：http://nu.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vy.hahajie.cn

[Q37] 右连接
来源：http://me.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bw.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yb.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jf.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://cu.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pr.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zb.hahajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tj.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vl.lnxyls.cn

[Q41] 多表连接
来源：http://vl.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sx.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://bj.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://ij.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://py.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://zg.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bb.gzmigu.cn

[Q43] 标量子查询
来源：http://ek.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://er.shtwfgs.cn

[Q44] IN 子查询
来源：http://on.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ff.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://sh.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zg.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oc.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jb.newstarts.cn

[Q47] 与平均值比较
来源：http://qr.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sk.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://ny.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xj.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://qo.shtwfgs.cn

[Q49] 更新单行
来源：http://qh.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hd.yuexingan06.cn

[Q50] 批量更新
来源：http://xu.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zp.haigaiapp.cn

[Q51] 用子查询更新
来源：http://ct.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://al.colortex.cn

[Q52] 删除指定行
来源：http://hd.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://cs.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://mg.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://az.jianghongdianzi.cn

[Q54] 清空表
来源：http://zs.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://nh.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://ok.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vk.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://gr.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eu.chemitech.net.cn

[Q57] 行号
来源：http://ri.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sd.wgjwhj.cn

[Q58] 累计求和
来源：http://cy.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wp.wgjwhj.cn

[Q59] 分组内累计
来源：http://qh.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aw.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://ky.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ec.hnjuh.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fr.colortex.cn

[Q61] 移动平均
来源：http://bf.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://og.bookmarksfly.cn

[Q62] 分组占比
来源：http://gq.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yv.chemitech.net.cn

[Q63] 开启事务
来源：http://su.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mg.hnjuh.cn

[Q64] 提交事务
来源：http://es.asd995.cn

COMMIT;
来源：http://pv.shtwfgs.cn

[Q65] 回滚事务
来源：http://ij.huanxung.cn

ROLLBACK;
来源：http://rm.hnjuh.cn

[Q66] 行锁查询
来源：http://fq.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dd.nicolike.cn

[Q67] 设置隔离级别
来源：http://dv.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kr.chemitech.net.cn

[Q68] 保存点
来源：http://jt.hahajie.cn

SAVEPOINT sp1;
来源：http://et.hnjuh.cn

ROLLBACK TO sp1;
来源：http://ta.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://nz.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bi.wgjwhj.cn

[Q70] 更新统计信息
来源：http://wj.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://oq.yuexingan06.cn

[Q71] 查看建表语句
来源：http://lb.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sb.shxzskj.cn

[Q72] 查看索引
来源：http://pv.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://hm.szxytkj.cn

[Q73] 查看表状态
来源：http://eg.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hx.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://ys.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tt.shxzskj.cn

[Q75] 日期格式化
来源：http://ih.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mg.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xj.huixinmuqiang.cn

[Q76] 按天统计
来源：http://da.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ux.9csxet.cn

[Q77] 时间加减
来源：http://ex.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mt.huixiangedu.cn

[Q78] 当前时间
来源：http://ba.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://in.szxytkj.cn

[Q79] 字符串拼接
来源：http://py.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xu.shxzukj.cn

[Q80] 字符串截取
来源：http://lf.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hk.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://gn.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aj.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://ld.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ej.huanxung.cn

[Q83] 大小写转换
来源：http://kb.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kz.hnjuh.cn

[Q84] 去除首尾空格
来源：http://bc.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://fq.chemitech.net.cn

[Q85] 数值取整
来源：http://qe.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yu.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://rh.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gy.newstarts.cn

[Q87] JSON 字段做条件
来源：http://gp.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://le.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://jv.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ao.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tw.colortex.cn

[Q89] 判断表是否存在
来源：http://cv.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cp.wgjwhj.cn

[Q90] 生成序号列
来源：http://fv.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hd.nicolike.cn

================================================================================
来源：http://wg.haigaiapp.cn

R. Bash 专题
来源：http://md.huixinmuqiang.cn

================================================================================
来源：http://dk.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://oe.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://pb.jctech888.com.cn

set -euo pipefail
来源：http://wy.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://pz.huanxung.cn

name="Tom"; echo "$name"
来源：http://dq.szxytkj.cn

[R03] 只读变量
来源：http://jq.chemitech.net.cn

readonly PI=3.14
来源：http://pu.nszjky.cn

[R04] 位置参数
来源：http://ns.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sy.521024.cn

[R05] 参数默认值
来源：http://qn.shxzukj.cn

name="${1:-default}"
来源：http://fl.shxzskj.cn

[R06] 判断命令是否存在
来源：http://hh.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ep.bjjhwx.cn

[R07] if 判断文件
来源：http://bh.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ru.jianghongdianzi.cn

[R08] 数值比较
来源：http://ug.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bj.huixinmuqiang.cn

[R09] 字符串比较
来源：http://tx.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yq.hahajie.cn

[R10] 正则匹配
来源：http://ii.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fr.huixiangedu.cn

[R11] case 多分支
来源：http://iz.szsharing.cn

case "$1" in
来源：http://cm.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://fw.szxytkj.cn

stop)  echo "停止" ;;
来源：http://az.9csxet.cn

*)     echo "未知命令" ;;
来源：http://lw.9csxet.cn

esac
来源：http://cu.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://fn.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://oa.jianghongdianzi.cn

[R13] for 计数循环
来源：http://bi.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://kz.jianghongdianzi.cn

[R14] C 风格 for
来源：http://vm.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bg.lnxyls.cn

[R15] while 逐行读文件
来源：http://bq.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lo.nicolike.cn

[R16] until 等待条件
来源：http://sy.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oq.wgjwhj.cn

[R17] 数组定义与取值
来源：http://jo.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jc.jctech888.com.cn

[R18] 遍历数组
来源：http://nb.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://is.bookmarksfly.cn

[R19] 数组长度
来源：http://al.wgjwhj.cn

echo "${#arr[@]}"
来源：http://ck.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://vl.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://la.wgjwhj.cn

[R21] 字符串长度
来源：http://xv.bjjhwx.cn

echo "${#s}"
来源：http://go.szsharing.cn

[R22] 截取子串
来源：http://ev.panjiajie.cn

echo "${s:0:5}"
来源：http://jo.huanxung.cn

[R23] 字符串替换
来源：http://lv.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nd.chemitech.net.cn

[R24] 大小写转换
来源：http://bs.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tm.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://lx.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://na.bookmarksfly.cn

[R26] 命令替换
来源：http://gb.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://xd.shxzskj.cn

[R27] 算术展开
来源：http://sn.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://wc.szxytkj.cn

[R28] 浮点运算
来源：http://xg.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://so.muxihuayi.cn

[R29] 定义函数
来源：http://ta.muxihuayi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vn.asd995.cn

[R30] 函数返回状态码
来源：http://xx.jctech888.com.cn

f() { return 0; }; f || echo "失败了"
来源：http://tk.chemitech.net.cn

[R31] 局部变量
来源：http://ee.chemitech.net.cn


<!-- 参考信息 -->