代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ha.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jj.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pa.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zj.huixiangedu.cn

================================================================================
来源：http://oj.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://af.yuexingan06.cn

================================================================================
来源：http://hj.shtwfgs.cn

[Q01] 创建表
来源：http://iq.huanxung.cn

CREATE TABLE users (
来源：http://pq.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nz.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://eg.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://jb.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iu.jianghongdianzi.cn

);
来源：http://zs.huixinmuqiang.cn

[Q02] 创建带外键的表
来源：http://ua.asd995.cn

CREATE TABLE orders (
来源：http://th.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wf.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://xg.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://at.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vp.bookmarksfly.cn

);
来源：http://tz.521024.cn

[Q03] 增加列
来源：http://dw.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dq.huixiangedu.cn

[Q04] 修改列类型
来源：http://gd.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rh.shxzukj.cn

[Q05] 重命名列
来源：http://ey.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xn.9csxet.cn

[Q06] 删除列
来源：http://qz.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ku.colortex.cn

[Q07] 删除表
来源：http://av.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://vv.huixiangedu.cn

[Q08] 创建普通索引
来源：http://ca.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ip.521024.cn

[Q09] 创建唯一索引
来源：http://cr.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ui.hnjuh.cn

[Q10] 插入单行
来源：http://ia.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vq.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://oe.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gn.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://eu.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jf.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mj.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://jn.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ra.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://nc.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qg.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jz.newstarts.cn

[Q15] 查询全部
来源：http://zm.gzmigu.cn

SELECT * FROM users;
来源：http://ex.shxzskj.cn

[Q16] 查询指定列
来源：http://pn.chemitech.net.cn

SELECT id, name FROM users;
来源：http://xd.bookmarksfly.cn

[Q17] 条件查询
来源：http://se.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fy.huanxung.cn

[Q18] 模糊匹配
来源：http://js.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hl.shxzukj.cn

[Q19] 范围查询
来源：http://pw.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ol.521024.cn

[Q20] IN 列表
来源：http://qa.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ei.yuexingan06.cn

[Q21] 空值判断
来源：http://rv.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sz.521024.cn

[Q22] 排序
来源：http://vb.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tg.chemitech.net.cn

[Q23] 分页
来源：http://pj.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zi.panjiajie.cn

[Q24] 去重
来源：http://ml.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://cs.panjiajie.cn

[Q25] 只取前 N 条
来源：http://va.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rk.muxihuayi.cn

[Q26] 计数
来源：http://bo.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://em.muxihuayi.cn

[Q27] 条件计数
来源：http://bz.shtwfgs.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vu.newstarts.cn

[Q28] 求和与平均
来源：http://pk.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://le.huanxung.cn

[Q29] 最大最小值
来源：http://hq.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://og.nicolike.cn

[Q30] 分组统计
来源：http://gp.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lj.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ol.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hc.shxzskj.cn

[Q32] 分组拼接字符串
来源：http://tw.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nl.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wl.521024.cn

[Q33] 多列分组
来源：http://aa.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xs.nszjky.cn

[Q34] 每组取第一条
来源：http://fi.lnxyls.cn

SELECT * FROM (
来源：http://pg.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ln.nicolike.cn

) t WHERE rn = 1;
来源：http://is.nszjky.cn

[Q35] 内连接
来源：http://iy.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ip.nszjky.cn

[Q36] 左连接
来源：http://nj.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qd.shxzskj.cn

[Q37] 右连接
来源：http://my.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hu.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://aa.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pf.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://pb.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cm.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://md.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jk.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rd.jctech888.com.cn

[Q41] 多表连接
来源：http://ec.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cj.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://jd.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://xl.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://ua.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://lu.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://el.jctech888.com.cn

[Q43] 标量子查询
来源：http://iv.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qm.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://te.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yn.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://ui.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oi.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uq.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://it.shtwfgs.cn

[Q47] 与平均值比较
来源：http://ff.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lt.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://mu.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hc.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://hp.shxzskj.cn

[Q49] 更新单行
来源：http://lb.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lv.huixiangedu.cn

[Q50] 批量更新
来源：http://ej.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ji.asd995.cn

[Q51] 用子查询更新
来源：http://lw.huixiangedu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mt.hahajie.cn

[Q52] 删除指定行
来源：http://qw.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://to.shxzskj.cn

[Q53] 按条件删除
来源：http://vj.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gk.yuntaijiaju.cn

[Q54] 清空表
来源：http://yz.hahajie.cn

TRUNCATE TABLE logs;
来源：http://jc.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://vq.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ah.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://yk.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jo.lnxyls.cn

[Q57] 行号
来源：http://cb.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yk.hahajie.cn

[Q58] 累计求和
来源：http://sp.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wf.bjjhwx.cn

[Q59] 分组内累计
来源：http://xx.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ve.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ni.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sx.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lc.hahajie.cn

[Q61] 移动平均
来源：http://qi.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mu.shtwfgs.cn

[Q62] 分组占比
来源：http://iq.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pw.shxzukj.cn

[Q63] 开启事务
来源：http://ri.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gw.panjiajie.cn

[Q64] 提交事务
来源：http://pr.shxzukj.cn

COMMIT;
来源：http://mc.huanxung.cn

[Q65] 回滚事务
来源：http://we.nicolike.cn

ROLLBACK;
来源：http://ph.jctech888.com.cn

[Q66] 行锁查询
来源：http://cb.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://te.shxzukj.cn

[Q67] 设置隔离级别
来源：http://rx.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://se.huanxung.cn

[Q68] 保存点
来源：http://ek.yuexingan06.cn

SAVEPOINT sp1;
来源：http://ba.nszjky.cn

ROLLBACK TO sp1;
来源：http://nb.lnxyls.cn

[Q69] 查看执行计划
来源：http://cq.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ln.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://dc.shxzukj.cn

ANALYZE TABLE users;
来源：http://ag.shxzukj.cn

[Q71] 查看建表语句
来源：http://uw.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vt.yuntaijiaju.cn

[Q72] 查看索引
来源：http://ga.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://xa.newstarts.cn

[Q73] 查看表状态
来源：http://jb.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yc.szsharing.cn

[Q74] 强制使用索引
来源：http://cx.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bo.huixiangedu.cn

[Q75] 日期格式化
来源：http://ym.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xs.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://av.huanxung.cn

[Q76] 按天统计
来源：http://mo.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nq.521024.cn

[Q77] 时间加减
来源：http://zi.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gp.huixiangedu.cn

[Q78] 当前时间
来源：http://et.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tx.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://xk.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nx.asd995.cn

[Q80] 字符串截取
来源：http://ev.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vr.nicolike.cn

[Q81] 字符串替换
来源：http://gd.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ui.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://lf.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gp.lnxyls.cn

[Q83] 大小写转换
来源：http://zm.yuexingan06.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dt.lnxyls.cn

[Q84] 去除首尾空格
来源：http://jm.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://eu.jianghongdianzi.cn

[Q85] 数值取整
来源：http://ko.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jd.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://hs.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://il.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://by.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bj.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://hf.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cd.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ez.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://rp.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ws.hnjuh.cn

[Q90] 生成序号列
来源：http://uq.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pn.gzmigu.cn

================================================================================
来源：http://hn.nszjky.cn

R. Bash 专题
来源：http://um.jianghongdianzi.cn

================================================================================
来源：http://yu.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://rt.shtwfgs.cn

#!/usr/bin/env bash
来源：http://bq.szsharing.cn

set -euo pipefail
来源：http://ki.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://ie.shxzukj.cn

name="Tom"; echo "$name"
来源：http://ga.huanxung.cn

[R03] 只读变量
来源：http://rm.huixiangedu.cn

readonly PI=3.14
来源：http://vr.hahajie.cn

[R04] 位置参数
来源：http://hz.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fa.szxytkj.cn

[R05] 参数默认值
来源：http://th.nszjky.cn

name="${1:-default}"
来源：http://hi.shxzukj.cn

[R06] 判断命令是否存在
来源：http://xl.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ku.huixiangedu.cn

[R07] if 判断文件
来源：http://hx.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qc.lnxyls.cn

[R08] 数值比较
来源：http://gl.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zc.521024.cn

[R09] 字符串比较
来源：http://wm.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vo.9csxet.cn

[R10] 正则匹配
来源：http://tg.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cq.jianghongdianzi.cn

[R11] case 多分支
来源：http://ym.9csxet.cn

case "$1" in
来源：http://nr.huanxung.cn

start) echo "启动" ;;
来源：http://xn.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://pj.9csxet.cn

*)     echo "未知命令" ;;
来源：http://mn.huixiangedu.cn

esac
来源：http://bj.hnjuh.cn

[R12] for 遍历文件
来源：http://qu.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://pj.huixinmuqiang.cn

[R13] for 计数循环
来源：http://jj.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://py.chemitech.net.cn

[R14] C 风格 for
来源：http://tp.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://io.huixiangedu.cn

[R15] while 逐行读文件
来源：http://hm.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xd.haigaiapp.cn

[R16] until 等待条件
来源：http://zm.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aq.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://fu.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://om.521024.cn

[R18] 遍历数组
来源：http://mx.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yn.haigaiapp.cn

[R19] 数组长度
来源：http://sh.szxytkj.cn

echo "${#arr[@]}"
来源：http://jh.shxzukj.cn

[R20] 关联数组（字典）
来源：http://gh.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bb.bjjhwx.cn

[R21] 字符串长度
来源：http://mz.gzmigu.cn

echo "${#s}"
来源：http://gr.wgjwhj.cn

[R22] 截取子串
来源：http://tv.shxzskj.cn

echo "${s:0:5}"
来源：http://dr.huanxung.cn

[R23] 字符串替换
来源：http://cw.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bp.panjiajie.cn

[R24] 大小写转换
来源：http://cm.newstarts.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pi.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://eu.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qs.newstarts.cn

[R26] 命令替换
来源：http://bx.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://cg.panjiajie.cn

[R27] 算术展开
来源：http://jv.asd995.cn

echo $((1 + 2 * 3))
来源：http://zq.9csxet.cn

[R28] 浮点运算
来源：http://zw.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://cl.bookmarksfly.cn

[R29] 定义函数
来源：http://jz.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iv.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://um.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://uh.newstarts.cn

[R31] 局部变量
来源：http://ep.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://kq.colortex.cn

[R32] 参数个数校验
来源：http://hg.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wp.521024.cn

[R33] 捕获错误并提示行号
来源：http://rs.hahajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://la.9csxet.cn

[R34] 退出时清理
来源：http://ne.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wc.lnxyls.cn

[R35] 后台执行并等待
来源：http://sf.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ql.colortex.cn

[R36] 并发执行多个任务
来源：http://gw.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ly.muxihuayi.cn

[R37] 把输出赋给变量
来源：http://le.shxzukj.cn

files=$(ls -1)
来源：http://dc.jianghongdianzi.cn

[R38] 管道串联
来源：http://yf.szsharing.cn

cat a.txt | grep -i error | wc -l
来源：http://zl.521024.cn

[R39] 重定向标准输出与错误
来源：http://mj.shxzskj.cn

cmd > out.log 2>&1
来源：http://ao.shtwfgs.cn

[R40] 追加写日志
来源：http://sh.chemitech.net.cn

echo "log" >> out.log
来源：http://zm.asd995.cn

[R41] 丢弃输出
来源：http://ma.newstarts.cn


<!-- 参考信息 -->