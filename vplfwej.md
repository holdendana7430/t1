代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zb.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kj.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uq.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fk.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bc.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qc.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dq.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ic.wgjwhj.cn

================================================================================
来源：http://cu.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cd.bookmarksfly.cn

================================================================================
来源：http://sd.nicolike.cn

[Q01] 创建表
来源：http://oa.wgjwhj.cn

CREATE TABLE users (
来源：http://xk.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://la.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://li.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://yv.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://je.wgjwhj.cn

);
来源：http://ey.hahajie.cn

[Q02] 创建带外键的表
来源：http://fo.szsharing.cn

CREATE TABLE orders (
来源：http://uo.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lm.521024.cn

user_id INT NOT NULL,
来源：http://cz.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://fl.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://db.asd995.cn

);
来源：http://ao.huanxung.cn

[Q03] 增加列
来源：http://ic.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wt.wgjwhj.cn

[Q04] 修改列类型
来源：http://ve.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uc.haigaiapp.cn

[Q05] 重命名列
来源：http://eu.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jb.panjiajie.cn

[Q06] 删除列
来源：http://dg.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wo.bjjhwx.cn

[Q07] 删除表
来源：http://yb.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://nd.huanxung.cn

[Q08] 创建普通索引
来源：http://xm.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ab.asd995.cn

[Q09] 创建唯一索引
来源：http://jh.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://og.jctech888.com.cn

[Q10] 插入单行
来源：http://wo.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wd.gzmigu.cn

[Q11] 一次插入多行
来源：http://jn.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ji.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://vm.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ya.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qe.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://kk.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lz.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://le.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kg.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fj.szsharing.cn

[Q15] 查询全部
来源：http://kj.hahajie.cn

SELECT * FROM users;
来源：http://jc.nicolike.cn

[Q16] 查询指定列
来源：http://ol.panjiajie.cn

SELECT id, name FROM users;
来源：http://iw.haigaiapp.cn

[Q17] 条件查询
来源：http://cy.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bm.wgjwhj.cn

[Q18] 模糊匹配
来源：http://qg.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xi.wgjwhj.cn

[Q19] 范围查询
来源：http://ig.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ia.colortex.cn

[Q20] IN 列表
来源：http://bt.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nu.9csxet.cn

[Q21] 空值判断
来源：http://kw.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cb.9csxet.cn

[Q22] 排序
来源：http://iq.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pm.bjjhwx.cn

[Q23] 分页
来源：http://eh.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jo.newstarts.cn

[Q24] 去重
来源：http://zg.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://eo.huanxung.cn

[Q25] 只取前 N 条
来源：http://dq.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rc.jianghongdianzi.cn

[Q26] 计数
来源：http://kg.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://ne.shxzskj.cn

[Q27] 条件计数
来源：http://wb.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ql.szxytkj.cn

[Q28] 求和与平均
来源：http://zf.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zg.bjjhwx.cn

[Q29] 最大最小值
来源：http://lh.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ji.bookmarksfly.cn

[Q30] 分组统计
来源：http://rf.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kf.asd995.cn

[Q31] 分组后过滤
来源：http://bq.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ud.asd995.cn

[Q32] 分组拼接字符串
来源：http://hg.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vk.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xz.bjjhwx.cn

[Q33] 多列分组
来源：http://ex.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sk.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://ta.9csxet.cn

SELECT * FROM (
来源：http://pl.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gm.huixiangedu.cn

) t WHERE rn = 1;
来源：http://ub.huixinmuqiang.cn

[Q35] 内连接
来源：http://ho.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sz.haigaiapp.cn

[Q36] 左连接
来源：http://yr.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dn.jianghongdianzi.cn

[Q37] 右连接
来源：http://tc.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://on.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ah.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sb.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://gu.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dz.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hv.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bi.colortex.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rr.yuexingan06.cn

[Q41] 多表连接
来源：http://sd.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://be.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://tc.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://jb.colortex.cn

[Q42] 连接条件附加过滤
来源：http://an.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://me.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kh.nicolike.cn

[Q43] 标量子查询
来源：http://nj.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ya.chemitech.net.cn

[Q44] IN 子查询
来源：http://gb.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ow.asd995.cn

[Q45] EXISTS 判断存在
来源：http://hh.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ez.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qi.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bo.521024.cn

[Q47] 与平均值比较
来源：http://kh.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ju.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://vc.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iw.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://lc.yuntaijiaju.cn

[Q49] 更新单行
来源：http://lr.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ny.huanxung.cn

[Q50] 批量更新
来源：http://ku.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.newstarts.cn

[Q51] 用子查询更新
来源：http://qa.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vy.lnxyls.cn

[Q52] 删除指定行
来源：http://up.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://gi.nicolike.cn

[Q53] 按条件删除
来源：http://yp.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rq.gzmigu.cn

[Q54] 清空表
来源：http://wt.bjjhwx.cn

TRUNCATE TABLE logs;
来源：http://hm.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://bl.shxzskj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vr.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://xv.huixinmuqiang.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gb.521024.cn

[Q57] 行号
来源：http://hw.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ey.shtwfgs.cn

[Q58] 累计求和
来源：http://te.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iv.wgjwhj.cn

[Q59] 分组内累计
来源：http://ym.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kb.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://hp.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kr.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tn.jianghongdianzi.cn

[Q61] 移动平均
来源：http://om.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gr.bjjhwx.cn

[Q62] 分组占比
来源：http://ee.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ut.jctech888.com.cn

[Q63] 开启事务
来源：http://xp.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://si.colortex.cn

[Q64] 提交事务
来源：http://ah.shtwfgs.cn

COMMIT;
来源：http://kt.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://fn.yuntaijiaju.cn

ROLLBACK;
来源：http://jb.bookmarksfly.cn

[Q66] 行锁查询
来源：http://os.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hw.huanxung.cn

[Q67] 设置隔离级别
来源：http://zs.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gl.gzmigu.cn

[Q68] 保存点
来源：http://yb.huanxung.cn

SAVEPOINT sp1;
来源：http://ge.hnjuh.cn

ROLLBACK TO sp1;
来源：http://yf.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://hb.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rf.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://ha.panjiajie.cn

ANALYZE TABLE users;
来源：http://sd.huixiangedu.cn

[Q71] 查看建表语句
来源：http://oe.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zc.szxytkj.cn

[Q72] 查看索引
来源：http://db.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://nm.huixiangedu.cn

[Q73] 查看表状态
来源：http://nv.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vu.panjiajie.cn

[Q74] 强制使用索引
来源：http://qx.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vt.bookmarksfly.cn

[Q75] 日期格式化
来源：http://we.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xl.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://up.shxzskj.cn

[Q76] 按天统计
来源：http://ut.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xu.wgjwhj.cn

[Q77] 时间加减
来源：http://zx.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oq.lnxyls.cn

[Q78] 当前时间
来源：http://oq.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ib.lnxyls.cn

[Q79] 字符串拼接
来源：http://qs.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wd.nicolike.cn

[Q80] 字符串截取
来源：http://xf.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vi.hahajie.cn

[Q81] 字符串替换
来源：http://tq.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cp.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://ol.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ue.huixiangedu.cn

[Q83] 大小写转换
来源：http://lz.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rs.9csxet.cn

[Q84] 去除首尾空格
来源：http://lc.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://ek.newstarts.cn

[Q85] 数值取整
来源：http://xh.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ry.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://cv.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wd.nszjky.cn

[Q87] JSON 字段做条件
来源：http://bn.huixiangedu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sp.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://yo.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bo.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cr.shxzskj.cn

[Q89] 判断表是否存在
来源：http://sw.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zf.9csxet.cn

[Q90] 生成序号列
来源：http://vi.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hm.yuexingan06.cn

================================================================================
来源：http://ka.shxzukj.cn

R. Bash 专题
来源：http://tw.jianghongdianzi.cn

================================================================================
来源：http://ph.hnjuh.cn

[R01] shebang 与严格模式
来源：http://qe.muxihuayi.cn

#!/usr/bin/env bash
来源：http://lu.nicolike.cn

set -euo pipefail
来源：http://ks.shxzskj.cn

[R02] 变量赋值与使用
来源：http://gz.asd995.cn

name="Tom"; echo "$name"
来源：http://xz.huanxung.cn

[R03] 只读变量
来源：http://mv.bjjhwx.cn

readonly PI=3.14
来源：http://uq.jianghongdianzi.cn

[R04] 位置参数
来源：http://fy.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eb.panjiajie.cn

[R05] 参数默认值
来源：http://nl.hahajie.cn

name="${1:-default}"
来源：http://ep.gzmigu.cn

[R06] 判断命令是否存在
来源：http://kd.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ht.lnxyls.cn

[R07] if 判断文件
来源：http://dy.colortex.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hx.bookmarksfly.cn

[R08] 数值比较
来源：http://ip.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gb.colortex.cn

[R09] 字符串比较
来源：http://wz.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fo.haigaiapp.cn

[R10] 正则匹配
来源：http://fm.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ws.jctech888.com.cn

[R11] case 多分支
来源：http://ip.szsharing.cn

case "$1" in
来源：http://ng.szsharing.cn

start) echo "启动" ;;
来源：http://jo.szsharing.cn

stop)  echo "停止" ;;
来源：http://ns.huanxung.cn

*)     echo "未知命令" ;;
来源：http://vd.haigaiapp.cn

esac
来源：http://wd.shxzskj.cn

[R12] for 遍历文件
来源：http://gh.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://qy.asd995.cn

[R13] for 计数循环
来源：http://wz.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://tj.wgjwhj.cn

[R14] C 风格 for
来源：http://ub.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pw.colortex.cn

[R15] while 逐行读文件
来源：http://yx.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cw.haigaiapp.cn

[R16] until 等待条件
来源：http://xk.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jc.yuexingan06.cn

[R17] 数组定义与取值
来源：http://as.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sv.huanxung.cn

[R18] 遍历数组
来源：http://uc.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ex.hahajie.cn

[R19] 数组长度
来源：http://do.szsharing.cn

echo "${#arr[@]}"
来源：http://ms.newstarts.cn

[R20] 关联数组（字典）
来源：http://ea.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mu.521024.cn

[R21] 字符串长度
来源：http://qb.yuexingan06.cn

echo "${#s}"
来源：http://sb.huixinmuqiang.cn

[R22] 截取子串
来源：http://mq.shxzskj.cn

echo "${s:0:5}"
来源：http://xa.yuntaijiaju.cn

[R23] 字符串替换
来源：http://zi.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jn.szxytkj.cn

[R24] 大小写转换
来源：http://jg.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ov.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://dr.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lc.gzmigu.cn

[R26] 命令替换
来源：http://mu.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://wg.szxytkj.cn

[R27] 算术展开
来源：http://pw.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://pq.521024.cn

[R28] 浮点运算
来源：http://wt.szsharing.cn

echo "scale=2; 10/3" | bc
来源：http://rw.lnxyls.cn

[R29] 定义函数
来源：http://cl.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pq.shxzskj.cn

[R30] 函数返回状态码
来源：http://vh.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://uf.wgjwhj.cn

[R31] 局部变量
来源：http://nr.521024.cn

f() { local x=1; echo "$x"; }
来源：http://gm.chemitech.net.cn

[R32] 参数个数校验
来源：http://bq.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rk.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://nf.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hj.shxzukj.cn

[R34] 退出时清理
来源：http://ve.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ju.jctech888.com.cn

[R35] 后台执行并等待
来源：http://vt.shxzskj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mg.9csxet.cn

[R36] 并发执行多个任务
来源：http://mr.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qm.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://et.jianghongdianzi.cn

files=$(ls -1)
来源：http://au.huixinmuqiang.cn

[R38] 管道串联
来源：http://dw.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://ir.yuntaijiaju.cn

[R39] 重定向标准输出与错误
来源：http://zm.muxihuayi.cn


<!-- 参考信息 -->