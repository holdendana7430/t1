代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ap.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uw.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iz.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://bw.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qp.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kl.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ig.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ai.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yg.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eh.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://va.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tr.hnjuh.cn

================================================================================
来源：http://ov.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fc.huixiangedu.cn

================================================================================
来源：http://cg.chemitech.net.cn

[Q01] 创建表
来源：http://kj.yuntaijiaju.cn

CREATE TABLE users (
来源：http://yu.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zi.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://cr.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://bf.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gp.yuexingan06.cn

);
来源：http://tv.szsharing.cn

[Q02] 创建带外键的表
来源：http://hr.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://tq.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vp.jctech888.com.cn

user_id INT NOT NULL,
来源：http://rn.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://re.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ee.muxihuayi.cn

);
来源：http://qj.hahajie.cn

[Q03] 增加列
来源：http://ml.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ey.chemitech.net.cn

[Q04] 修改列类型
来源：http://pv.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xw.hahajie.cn

[Q05] 重命名列
来源：http://ay.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iy.lnxyls.cn

[Q06] 删除列
来源：http://rv.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fr.nszjky.cn

[Q07] 删除表
来源：http://gc.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://mo.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://oo.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://im.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://mg.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nv.bookmarksfly.cn

[Q10] 插入单行
来源：http://gt.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qh.szxytkj.cn

[Q11] 一次插入多行
来源：http://cm.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wn.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://xx.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eu.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hp.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://zm.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pz.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://sc.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jn.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hi.haigaiapp.cn

[Q15] 查询全部
来源：http://qo.gzmigu.cn

SELECT * FROM users;
来源：http://po.szxytkj.cn

[Q16] 查询指定列
来源：http://mu.521024.cn

SELECT id, name FROM users;
来源：http://qy.521024.cn

[Q17] 条件查询
来源：http://sf.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kt.521024.cn

[Q18] 模糊匹配
来源：http://ud.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://un.chemitech.net.cn

[Q19] 范围查询
来源：http://qv.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pp.chemitech.net.cn

[Q20] IN 列表
来源：http://vf.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://as.muxihuayi.cn

[Q21] 空值判断
来源：http://eb.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gw.lnxyls.cn

[Q22] 排序
来源：http://on.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://up.haigaiapp.cn

[Q23] 分页
来源：http://wn.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zw.wgjwhj.cn

[Q24] 去重
来源：http://xo.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://pn.shxzukj.cn

[Q25] 只取前 N 条
来源：http://wb.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xi.yuntaijiaju.cn

[Q26] 计数
来源：http://ay.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://bl.yuntaijiaju.cn

[Q27] 条件计数
来源：http://pf.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wa.hnjuh.cn

[Q28] 求和与平均
来源：http://wx.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pd.9csxet.cn

[Q29] 最大最小值
来源：http://nu.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aw.szsharing.cn

[Q30] 分组统计
来源：http://pk.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ll.szxytkj.cn

[Q31] 分组后过滤
来源：http://iy.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ex.9csxet.cn

[Q32] 分组拼接字符串
来源：http://gh.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wq.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yr.szsharing.cn

[Q33] 多列分组
来源：http://ka.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://as.wgjwhj.cn

[Q34] 每组取第一条
来源：http://dj.jctech888.com.cn

SELECT * FROM (
来源：http://ze.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yx.chemitech.net.cn

) t WHERE rn = 1;
来源：http://ec.jctech888.com.cn

[Q35] 内连接
来源：http://hv.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xu.shtwfgs.cn

[Q36] 左连接
来源：http://vd.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yc.yuntaijiaju.cn

[Q37] 右连接
来源：http://ll.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gf.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lw.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fz.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://rx.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lr.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://va.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pc.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://im.szxytkj.cn

[Q41] 多表连接
来源：http://kp.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cr.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://ev.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ih.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://qw.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://gq.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xn.panjiajie.cn

[Q43] 标量子查询
来源：http://zd.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://so.haigaiapp.cn

[Q44] IN 子查询
来源：http://oh.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ed.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://sh.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://my.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xf.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://th.asd995.cn

[Q47] 与平均值比较
来源：http://fs.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yd.huixiangedu.cn

[Q48] CTE 公用表表达式
来源：http://ao.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uv.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://tu.yuexingan06.cn

[Q49] 更新单行
来源：http://li.shxzskj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mf.521024.cn

[Q50] 批量更新
来源：http://qf.bookmarksfly.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ke.bjjhwx.cn

[Q51] 用子查询更新
来源：http://it.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cs.nicolike.cn

[Q52] 删除指定行
来源：http://ln.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://er.newstarts.cn

[Q53] 按条件删除
来源：http://as.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ro.chemitech.net.cn

[Q54] 清空表
来源：http://fd.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://zj.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://vf.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cw.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://yn.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://id.jianghongdianzi.cn

[Q57] 行号
来源：http://tm.shxzukj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uq.gzmigu.cn

[Q58] 累计求和
来源：http://sk.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zn.hnjuh.cn

[Q59] 分组内累计
来源：http://wm.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aw.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://fr.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ln.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rb.shxzukj.cn

[Q61] 移动平均
来源：http://dq.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gc.haigaiapp.cn

[Q62] 分组占比
来源：http://ab.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uj.hnjuh.cn

[Q63] 开启事务
来源：http://dz.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oq.9csxet.cn

[Q64] 提交事务
来源：http://ar.muxihuayi.cn

COMMIT;
来源：http://na.9csxet.cn

[Q65] 回滚事务
来源：http://qi.chemitech.net.cn

ROLLBACK;
来源：http://xv.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://hk.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://if.panjiajie.cn

[Q67] 设置隔离级别
来源：http://ry.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cj.9csxet.cn

[Q68] 保存点
来源：http://lf.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://oe.colortex.cn

ROLLBACK TO sp1;
来源：http://cl.hahajie.cn

[Q69] 查看执行计划
来源：http://pe.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://di.lnxyls.cn

[Q70] 更新统计信息
来源：http://tq.hahajie.cn

ANALYZE TABLE users;
来源：http://fj.jctech888.com.cn

[Q71] 查看建表语句
来源：http://qk.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iv.shxzukj.cn

[Q72] 查看索引
来源：http://mp.asd995.cn

SHOW INDEX FROM users;
来源：http://ae.bookmarksfly.cn

[Q73] 查看表状态
来源：http://xq.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kc.haigaiapp.cn

[Q74] 强制使用索引
来源：http://gd.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pd.shtwfgs.cn

[Q75] 日期格式化
来源：http://ux.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vs.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zq.huixinmuqiang.cn

[Q76] 按天统计
来源：http://dg.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://am.szsharing.cn

[Q77] 时间加减
来源：http://mu.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lu.shxzukj.cn

[Q78] 当前时间
来源：http://tc.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://st.bjjhwx.cn

[Q79] 字符串拼接
来源：http://uz.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tf.newstarts.cn

[Q80] 字符串截取
来源：http://ke.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uw.shxzukj.cn

[Q81] 字符串替换
来源：http://da.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yf.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://rt.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dp.shxzskj.cn

[Q83] 大小写转换
来源：http://rq.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uk.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://qg.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://dj.wgjwhj.cn

[Q85] 数值取整
来源：http://yn.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://va.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://em.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yg.521024.cn

[Q87] JSON 字段做条件
来源：http://cx.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bv.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://pu.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://js.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://my.nszjky.cn

[Q89] 判断表是否存在
来源：http://id.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uw.asd995.cn

[Q90] 生成序号列
来源：http://ti.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jb.lnxyls.cn

================================================================================
来源：http://oa.wgjwhj.cn

R. Bash 专题
来源：http://mi.muxihuayi.cn

================================================================================
来源：http://kj.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://wi.asd995.cn

#!/usr/bin/env bash
来源：http://mp.chemitech.net.cn

set -euo pipefail
来源：http://as.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://gc.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://pu.9csxet.cn

[R03] 只读变量
来源：http://vz.gzmigu.cn

readonly PI=3.14
来源：http://vv.jianghongdianzi.cn

[R04] 位置参数
来源：http://kc.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hw.nicolike.cn

[R05] 参数默认值
来源：http://ya.shxzskj.cn

name="${1:-default}"
来源：http://lz.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://eg.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ys.nicolike.cn

[R07] if 判断文件
来源：http://yh.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://at.shxzukj.cn

[R08] 数值比较
来源：http://bl.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jd.szsharing.cn

[R09] 字符串比较
来源：http://ls.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pf.huixiangedu.cn

[R10] 正则匹配
来源：http://rt.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yc.newstarts.cn

[R11] case 多分支
来源：http://af.panjiajie.cn

case "$1" in
来源：http://ra.haigaiapp.cn

start) echo "启动" ;;
来源：http://lu.szxytkj.cn

stop)  echo "停止" ;;
来源：http://jt.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://xg.jianghongdianzi.cn

esac
来源：http://mf.bookmarksfly.cn

[R12] for 遍历文件
来源：http://ai.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://gs.newstarts.cn

[R13] for 计数循环
来源：http://mi.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://hc.yuexingan06.cn

[R14] C 风格 for
来源：http://na.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vk.yuexingan06.cn

[R15] while 逐行读文件
来源：http://ht.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nh.yuexingan06.cn

[R16] until 等待条件
来源：http://ip.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gz.yuntaijiaju.cn

[R17] 数组定义与取值
来源：http://wg.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cu.nszjky.cn

[R18] 遍历数组
来源：http://tl.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qy.shxzukj.cn

[R19] 数组长度
来源：http://en.newstarts.cn

echo "${#arr[@]}"
来源：http://di.9csxet.cn

[R20] 关联数组（字典）
来源：http://vh.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://he.9csxet.cn

[R21] 字符串长度
来源：http://su.nicolike.cn

echo "${#s}"
来源：http://zv.gzmigu.cn

[R22] 截取子串
来源：http://hq.lnxyls.cn

echo "${s:0:5}"
来源：http://lv.panjiajie.cn

[R23] 字符串替换
来源：http://gc.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ih.huixinmuqiang.cn

[R24] 大小写转换
来源：http://cc.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ma.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://gi.jctech888.com.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dy.hnjuh.cn

[R26] 命令替换
来源：http://fr.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://lp.lnxyls.cn

[R27] 算术展开
来源：http://sw.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://nl.wgjwhj.cn

[R28] 浮点运算
来源：http://zd.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://xc.huanxung.cn

[R29] 定义函数
来源：http://mw.jianghongdianzi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mb.bjjhwx.cn

[R30] 函数返回状态码
来源：http://kn.bookmarksfly.cn

f() { return 0; }; f || echo "失败了"
来源：http://ma.yuntaijiaju.cn

[R31] 局部变量
来源：http://xv.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://du.newstarts.cn

[R32] 参数个数校验
来源：http://de.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lp.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://dn.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://if.wgjwhj.cn

[R34] 退出时清理
来源：http://mk.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ao.9csxet.cn

[R35] 后台执行并等待
来源：http://wr.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bj.panjiajie.cn

[R36] 并发执行多个任务
来源：http://rl.bjjhwx.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://up.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://iu.szxytkj.cn


<!-- 参考信息 -->