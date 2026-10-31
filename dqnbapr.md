代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uo.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kd.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ab.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://re.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yy.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vg.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pw.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vd.haigaiapp.cn

================================================================================
来源：http://yo.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mk.shxzukj.cn

================================================================================
来源：http://mi.haigaiapp.cn

[Q01] 创建表
来源：http://kp.huixiangedu.cn

CREATE TABLE users (
来源：http://rn.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wa.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://xv.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://jg.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yj.shxzskj.cn

);
来源：http://od.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://sd.chemitech.net.cn

CREATE TABLE orders (
来源：http://hu.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://do.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://bw.asd995.cn

amount DECIMAL(10, 2),
来源：http://ll.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ng.9csxet.cn

);
来源：http://tc.colortex.cn

[Q03] 增加列
来源：http://lg.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ev.lnxyls.cn

[Q04] 修改列类型
来源：http://fr.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iz.521024.cn

[Q05] 重命名列
来源：http://ea.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fi.nicolike.cn

[Q06] 删除列
来源：http://vn.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zk.hahajie.cn

[Q07] 删除表
来源：http://wp.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://oi.haigaiapp.cn

[Q08] 创建普通索引
来源：http://kj.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tv.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://bg.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yr.nicolike.cn

[Q10] 插入单行
来源：http://hi.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ah.muxihuayi.cn

[Q11] 一次插入多行
来源：http://mr.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vn.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://hk.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tk.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bs.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://om.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cs.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://iw.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kh.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lc.huanxung.cn

[Q15] 查询全部
来源：http://xe.gzmigu.cn

SELECT * FROM users;
来源：http://un.panjiajie.cn

[Q16] 查询指定列
来源：http://nr.9csxet.cn

SELECT id, name FROM users;
来源：http://xa.wgjwhj.cn

[Q17] 条件查询
来源：http://xf.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tl.jctech888.com.cn

[Q18] 模糊匹配
来源：http://xr.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://em.nszjky.cn

[Q19] 范围查询
来源：http://xz.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xq.haigaiapp.cn

[Q20] IN 列表
来源：http://gq.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cg.bjjhwx.cn

[Q21] 空值判断
来源：http://ef.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jy.muxihuayi.cn

[Q22] 排序
来源：http://gl.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ml.newstarts.cn

[Q23] 分页
来源：http://vf.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qs.hnjuh.cn

[Q24] 去重
来源：http://sm.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://yr.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://xm.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lu.panjiajie.cn

[Q26] 计数
来源：http://kn.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://am.huanxung.cn

[Q27] 条件计数
来源：http://wd.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ho.gzmigu.cn

[Q28] 求和与平均
来源：http://rn.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hr.muxihuayi.cn

[Q29] 最大最小值
来源：http://nx.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jm.bookmarksfly.cn

[Q30] 分组统计
来源：http://qt.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ag.hahajie.cn

[Q31] 分组后过滤
来源：http://fk.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nn.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://js.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yd.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ce.bookmarksfly.cn

[Q33] 多列分组
来源：http://sy.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tc.muxihuayi.cn

[Q34] 每组取第一条
来源：http://ak.panjiajie.cn

SELECT * FROM (
来源：http://ru.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uf.asd995.cn

) t WHERE rn = 1;
来源：http://ze.yuntaijiaju.cn

[Q35] 内连接
来源：http://bt.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ph.gzmigu.cn

[Q36] 左连接
来源：http://ot.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dr.9csxet.cn

[Q37] 右连接
来源：http://aq.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lw.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mp.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yy.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://im.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hs.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lj.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yg.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yh.nicolike.cn

[Q41] 多表连接
来源：http://wy.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uc.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://rd.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://qv.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://cr.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://ko.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oi.bjjhwx.cn

[Q43] 标量子查询
来源：http://ei.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ni.szxytkj.cn

[Q44] IN 子查询
来源：http://ro.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://em.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://oz.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eu.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jh.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fs.panjiajie.cn

[Q47] 与平均值比较
来源：http://hs.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gk.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://kf.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rl.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://mj.shxzukj.cn

[Q49] 更新单行
来源：http://bs.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xj.chemitech.net.cn

[Q50] 批量更新
来源：http://mv.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cy.shtwfgs.cn

[Q51] 用子查询更新
来源：http://td.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nv.panjiajie.cn

[Q52] 删除指定行
来源：http://ph.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://gp.gzmigu.cn

[Q53] 按条件删除
来源：http://mh.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ha.yuexingan06.cn

[Q54] 清空表
来源：http://to.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://rd.huanxung.cn

[Q55] 排名（并列占位）
来源：http://vg.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cm.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://ls.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zj.yuntaijiaju.cn

[Q57] 行号
来源：http://jw.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cu.chemitech.net.cn

[Q58] 累计求和
来源：http://hm.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kj.hahajie.cn

[Q59] 分组内累计
来源：http://dt.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://df.hahajie.cn

[Q60] 取上一行 / 下一行
来源：http://cg.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pv.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ug.bookmarksfly.cn

[Q61] 移动平均
来源：http://ec.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yr.jianghongdianzi.cn

[Q62] 分组占比
来源：http://sv.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vx.szxytkj.cn

[Q63] 开启事务
来源：http://it.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ay.bookmarksfly.cn

[Q64] 提交事务
来源：http://qz.shtwfgs.cn

COMMIT;
来源：http://jd.nicolike.cn

[Q65] 回滚事务
来源：http://yy.wgjwhj.cn

ROLLBACK;
来源：http://er.hnjuh.cn

[Q66] 行锁查询
来源：http://he.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://em.szxytkj.cn

[Q67] 设置隔离级别
来源：http://hb.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nb.hnjuh.cn

[Q68] 保存点
来源：http://yq.hnjuh.cn

SAVEPOINT sp1;
来源：http://di.huanxung.cn

ROLLBACK TO sp1;
来源：http://ui.shxzskj.cn

[Q69] 查看执行计划
来源：http://ov.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ro.bjjhwx.cn

[Q70] 更新统计信息
来源：http://ra.lnxyls.cn

ANALYZE TABLE users;
来源：http://gd.szxytkj.cn

[Q71] 查看建表语句
来源：http://hi.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tz.hnjuh.cn

[Q72] 查看索引
来源：http://st.szxytkj.cn

SHOW INDEX FROM users;
来源：http://ku.wgjwhj.cn

[Q73] 查看表状态
来源：http://kv.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pl.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://sd.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gw.asd995.cn

[Q75] 日期格式化
来源：http://rg.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pv.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oa.521024.cn

[Q76] 按天统计
来源：http://sc.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kk.newstarts.cn

[Q77] 时间加减
来源：http://mb.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sb.9csxet.cn

[Q78] 当前时间
来源：http://px.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://se.jctech888.com.cn

[Q79] 字符串拼接
来源：http://um.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yr.szxytkj.cn

[Q80] 字符串截取
来源：http://dx.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ym.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://zi.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://as.colortex.cn

[Q82] 字符长度与字节长度
来源：http://ay.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ln.lnxyls.cn

[Q83] 大小写转换
来源：http://uu.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sm.nszjky.cn

[Q84] 去除首尾空格
来源：http://po.shxzukj.cn

SELECT TRIM(name) FROM users;
来源：http://fe.szxytkj.cn

[Q85] 数值取整
来源：http://qe.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cg.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://sw.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wr.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://go.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gw.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://nx.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xb.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yw.colortex.cn

[Q89] 判断表是否存在
来源：http://qi.yuexingan06.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zz.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://hh.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zz.chemitech.net.cn

================================================================================
来源：http://nz.shxzskj.cn

R. Bash 专题
来源：http://hs.szsharing.cn

================================================================================
来源：http://hw.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://jr.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://ki.shxzskj.cn

set -euo pipefail
来源：http://mh.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://qm.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://hh.shxzskj.cn

[R03] 只读变量
来源：http://xd.jctech888.com.cn

readonly PI=3.14
来源：http://of.shxzukj.cn

[R04] 位置参数
来源：http://vf.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vt.bjjhwx.cn

[R05] 参数默认值
来源：http://dw.shxzukj.cn

name="${1:-default}"
来源：http://fd.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://cg.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lh.huixinmuqiang.cn

[R07] if 判断文件
来源：http://vz.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zr.haigaiapp.cn

[R08] 数值比较
来源：http://ia.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sx.bjjhwx.cn

[R09] 字符串比较
来源：http://sf.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vc.9csxet.cn

[R10] 正则匹配
来源：http://tp.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xu.521024.cn

[R11] case 多分支
来源：http://sj.bookmarksfly.cn

case "$1" in
来源：http://ew.jctech888.com.cn

start) echo "启动" ;;
来源：http://uo.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://lt.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://bl.yuexingan06.cn

esac
来源：http://cm.panjiajie.cn

[R12] for 遍历文件
来源：http://yg.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://jw.haigaiapp.cn

[R13] for 计数循环
来源：http://sc.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://gm.haigaiapp.cn

[R14] C 风格 for
来源：http://ze.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bi.hnjuh.cn

[R15] while 逐行读文件
来源：http://uc.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vs.huixinmuqiang.cn

[R16] until 等待条件
来源：http://oy.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fa.asd995.cn

[R17] 数组定义与取值
来源：http://my.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bj.muxihuayi.cn

[R18] 遍历数组
来源：http://ex.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xo.chemitech.net.cn

[R19] 数组长度
来源：http://lt.gzmigu.cn

echo "${#arr[@]}"
来源：http://qp.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://kx.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kj.panjiajie.cn

[R21] 字符串长度
来源：http://em.shxzskj.cn

echo "${#s}"
来源：http://ck.yuntaijiaju.cn

[R22] 截取子串
来源：http://cr.521024.cn

echo "${s:0:5}"
来源：http://vz.gzmigu.cn

[R23] 字符串替换
来源：http://vq.colortex.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gd.9csxet.cn

[R24] 大小写转换
来源：http://eb.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gl.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://pa.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://up.chemitech.net.cn

[R26] 命令替换
来源：http://hl.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://ue.newstarts.cn

[R27] 算术展开
来源：http://ec.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://ao.yuexingan06.cn

[R28] 浮点运算
来源：http://gz.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://cn.521024.cn

[R29] 定义函数
来源：http://ed.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yu.muxihuayi.cn

[R30] 函数返回状态码
来源：http://hn.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://fi.lnxyls.cn

[R31] 局部变量
来源：http://ys.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://vb.huanxung.cn

[R32] 参数个数校验
来源：http://ed.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://su.gzmigu.cn

[R33] 捕获错误并提示行号
来源：http://lc.yuntaijiaju.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sq.shtwfgs.cn

[R34] 退出时清理
来源：http://gl.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qj.bjjhwx.cn

[R35] 后台执行并等待
来源：http://fc.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://he.panjiajie.cn

[R36] 并发执行多个任务
来源：http://ow.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kk.bjjhwx.cn

[R37] 把输出赋给变量
来源：http://jf.gzmigu.cn

files=$(ls -1)
来源：http://ri.9csxet.cn

[R38] 管道串联
来源：http://zi.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ac.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://tr.newstarts.cn


<!-- 参考信息 -->