代发 wailian999

PHP:  // 手写时间戳比较
来源：http://sy.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qr.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xh.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://py.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zi.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hu.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nb.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://xb.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yh.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bf.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gf.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://is.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pf.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ei.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ub.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pe.haigaiapp.cn

================================================================================
来源：http://ut.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bx.szsharing.cn

================================================================================
来源：http://ln.shxzukj.cn

[Q01] 创建表
来源：http://jk.huixinmuqiang.cn

CREATE TABLE users (
来源：http://dg.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://te.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://fw.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://xn.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vj.yuntaijiaju.cn

);
来源：http://xx.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://hu.huanxung.cn

CREATE TABLE orders (
来源：http://xq.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eo.9csxet.cn

user_id INT NOT NULL,
来源：http://km.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://bj.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://es.huixinmuqiang.cn

);
来源：http://va.muxihuayi.cn

[Q03] 增加列
来源：http://fh.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://um.asd995.cn

[Q04] 修改列类型
来源：http://wy.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fs.gzmigu.cn

[Q05] 重命名列
来源：http://db.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ly.panjiajie.cn

[Q06] 删除列
来源：http://ny.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rr.gzmigu.cn

[Q07] 删除表
来源：http://kc.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://ie.asd995.cn

[Q08] 创建普通索引
来源：http://fb.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ns.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://wk.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ov.shtwfgs.cn

[Q10] 插入单行
来源：http://pv.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ti.huanxung.cn

[Q11] 一次插入多行
来源：http://ng.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oo.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://hh.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://go.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fn.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://ie.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rx.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://kg.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gn.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ap.yuntaijiaju.cn

[Q15] 查询全部
来源：http://wj.jianghongdianzi.cn

SELECT * FROM users;
来源：http://fv.hnjuh.cn

[Q16] 查询指定列
来源：http://lz.nszjky.cn

SELECT id, name FROM users;
来源：http://jg.huixiangedu.cn

[Q17] 条件查询
来源：http://sk.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hg.gzmigu.cn

[Q18] 模糊匹配
来源：http://lz.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sx.gzmigu.cn

[Q19] 范围查询
来源：http://jc.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hn.gzmigu.cn

[Q20] IN 列表
来源：http://ul.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ti.gzmigu.cn

[Q21] 空值判断
来源：http://lm.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kf.lnxyls.cn

[Q22] 排序
来源：http://cx.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wg.nicolike.cn

[Q23] 分页
来源：http://wu.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jy.panjiajie.cn

[Q24] 去重
来源：http://ep.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://fq.newstarts.cn

[Q25] 只取前 N 条
来源：http://fd.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hf.jctech888.com.cn

[Q26] 计数
来源：http://nj.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://uu.yuexingan06.cn

[Q27] 条件计数
来源：http://jk.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jm.hahajie.cn

[Q28] 求和与平均
来源：http://dw.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lu.521024.cn

[Q29] 最大最小值
来源：http://lz.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.bookmarksfly.cn

[Q30] 分组统计
来源：http://tf.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wn.asd995.cn

[Q31] 分组后过滤
来源：http://nn.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sj.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://fr.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yh.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jm.yuntaijiaju.cn

[Q33] 多列分组
来源：http://pj.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bv.nszjky.cn

[Q34] 每组取第一条
来源：http://ge.jianghongdianzi.cn

SELECT * FROM (
来源：http://eo.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pi.chemitech.net.cn

) t WHERE rn = 1;
来源：http://ct.wgjwhj.cn

[Q35] 内连接
来源：http://yk.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ym.hahajie.cn

[Q36] 左连接
来源：http://xz.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ue.gzmigu.cn

[Q37] 右连接
来源：http://rf.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dc.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jr.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vg.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://di.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dj.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fo.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oo.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ie.huixinmuqiang.cn

[Q41] 多表连接
来源：http://qg.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qp.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://rz.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://dt.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://al.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://ro.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qz.hahajie.cn

[Q43] 标量子查询
来源：http://kr.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qs.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://xb.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oc.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://mx.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ct.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sk.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yo.asd995.cn

[Q47] 与平均值比较
来源：http://ze.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gk.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://fr.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mm.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://in.wgjwhj.cn

[Q49] 更新单行
来源：http://wc.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vn.nicolike.cn

[Q50] 批量更新
来源：http://ao.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rl.szxytkj.cn

[Q51] 用子查询更新
来源：http://rp.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fi.muxihuayi.cn

[Q52] 删除指定行
来源：http://uz.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://bj.huixinmuqiang.cn

[Q53] 按条件删除
来源：http://yu.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jw.wgjwhj.cn

[Q54] 清空表
来源：http://iw.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://dm.huanxung.cn

[Q55] 排名（并列占位）
来源：http://ao.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jm.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://yg.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mz.521024.cn

[Q57] 行号
来源：http://qm.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xv.nicolike.cn

[Q58] 累计求和
来源：http://vv.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bn.shxzukj.cn

[Q59] 分组内累计
来源：http://qg.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qh.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://ht.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ox.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://of.szsharing.cn

[Q61] 移动平均
来源：http://qg.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ee.lnxyls.cn

[Q62] 分组占比
来源：http://ol.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oy.bjjhwx.cn

[Q63] 开启事务
来源：http://qi.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kn.bookmarksfly.cn

[Q64] 提交事务
来源：http://sw.shxzukj.cn

COMMIT;
来源：http://ep.nicolike.cn

[Q65] 回滚事务
来源：http://ha.shxzskj.cn

ROLLBACK;
来源：http://kk.asd995.cn

[Q66] 行锁查询
来源：http://du.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sf.newstarts.cn

[Q67] 设置隔离级别
来源：http://je.newstarts.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rz.szxytkj.cn

[Q68] 保存点
来源：http://ak.9csxet.cn

SAVEPOINT sp1;
来源：http://st.huixinmuqiang.cn

ROLLBACK TO sp1;
来源：http://te.nicolike.cn

[Q69] 查看执行计划
来源：http://gj.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tv.gzmigu.cn

[Q70] 更新统计信息
来源：http://hk.nszjky.cn

ANALYZE TABLE users;
来源：http://ru.chemitech.net.cn

[Q71] 查看建表语句
来源：http://ak.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fj.9csxet.cn

[Q72] 查看索引
来源：http://eb.shxzskj.cn

SHOW INDEX FROM users;
来源：http://az.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://av.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pc.lnxyls.cn

[Q74] 强制使用索引
来源：http://ld.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oq.hnjuh.cn

[Q75] 日期格式化
来源：http://rl.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yo.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bz.szsharing.cn

[Q76] 按天统计
来源：http://qp.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gk.521024.cn

[Q77] 时间加减
来源：http://hu.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ah.gzmigu.cn

[Q78] 当前时间
来源：http://vh.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ne.521024.cn

[Q79] 字符串拼接
来源：http://qg.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xm.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://tw.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vm.521024.cn

[Q81] 字符串替换
来源：http://vq.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cm.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://pg.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://im.bookmarksfly.cn

[Q83] 大小写转换
来源：http://ny.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xm.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://bt.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://bs.huanxung.cn

[Q85] 数值取整
来源：http://xl.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vq.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://pa.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zy.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://om.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vx.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://yb.lnxyls.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wl.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aw.szxytkj.cn

[Q89] 判断表是否存在
来源：http://kf.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zz.colortex.cn

[Q90] 生成序号列
来源：http://qg.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fd.muxihuayi.cn

================================================================================
来源：http://tl.bookmarksfly.cn

R. Bash 专题
来源：http://te.asd995.cn

================================================================================
来源：http://fr.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://sy.shtwfgs.cn

#!/usr/bin/env bash
来源：http://he.bookmarksfly.cn

set -euo pipefail
来源：http://re.panjiajie.cn

[R02] 变量赋值与使用
来源：http://ty.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://cw.bookmarksfly.cn

[R03] 只读变量
来源：http://vz.nicolike.cn

readonly PI=3.14
来源：http://ox.gzmigu.cn

[R04] 位置参数
来源：http://rg.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zn.bookmarksfly.cn

[R05] 参数默认值
来源：http://gk.huixiangedu.cn

name="${1:-default}"
来源：http://ea.hnjuh.cn

[R06] 判断命令是否存在
来源：http://op.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kv.yuexingan06.cn

[R07] if 判断文件
来源：http://ew.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zi.shxzukj.cn

[R08] 数值比较
来源：http://gh.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tk.chemitech.net.cn

[R09] 字符串比较
来源：http://dv.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ir.wgjwhj.cn

[R10] 正则匹配
来源：http://dw.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sj.huixinmuqiang.cn

[R11] case 多分支
来源：http://oc.gzmigu.cn

case "$1" in
来源：http://xb.shtwfgs.cn

start) echo "启动" ;;
来源：http://jg.colortex.cn

stop)  echo "停止" ;;
来源：http://cg.asd995.cn

*)     echo "未知命令" ;;
来源：http://vk.shxzskj.cn

esac
来源：http://ox.huixiangedu.cn

[R12] for 遍历文件
来源：http://cg.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://mb.wgjwhj.cn

[R13] for 计数循环
来源：http://lg.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://at.yuntaijiaju.cn

[R14] C 风格 for
来源：http://jx.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ti.colortex.cn

[R15] while 逐行读文件
来源：http://nq.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://us.jctech888.com.cn

[R16] until 等待条件
来源：http://is.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hb.nicolike.cn

[R17] 数组定义与取值
来源：http://tg.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wx.521024.cn

[R18] 遍历数组
来源：http://gj.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ug.wgjwhj.cn

[R19] 数组长度
来源：http://cm.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://uv.shxzukj.cn

[R20] 关联数组（字典）
来源：http://ab.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cs.hahajie.cn

[R21] 字符串长度
来源：http://nk.chemitech.net.cn

echo "${#s}"
来源：http://cw.521024.cn

[R22] 截取子串
来源：http://eg.jctech888.com.cn

echo "${s:0:5}"
来源：http://ba.muxihuayi.cn

[R23] 字符串替换
来源：http://xd.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oy.nszjky.cn

[R24] 大小写转换
来源：http://cy.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://eq.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://oh.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vh.hnjuh.cn

[R26] 命令替换
来源：http://pu.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://ax.colortex.cn

[R27] 算术展开
来源：http://ze.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://cu.szxytkj.cn

[R28] 浮点运算
来源：http://fi.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://af.nszjky.cn

[R29] 定义函数
来源：http://es.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xj.szxytkj.cn

[R30] 函数返回状态码
来源：http://zr.huixinmuqiang.cn

f() { return 0; }; f || echo "失败了"
来源：http://hj.nicolike.cn

[R31] 局部变量
来源：http://er.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://oh.wgjwhj.cn

[R32] 参数个数校验
来源：http://eg.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xg.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://mw.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fn.nszjky.cn

[R34] 退出时清理
来源：http://wn.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jx.szsharing.cn

[R35] 后台执行并等待
来源：http://xi.gzmigu.cn


<!-- 参考信息 -->