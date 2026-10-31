代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tn.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sx.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vw.colortex.cn

[P08] 处理浮点精度问题
来源：http://zf.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rg.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eq.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nl.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wb.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gh.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hh.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qc.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nb.shxzskj.cn

================================================================================
来源：http://we.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ec.hnjuh.cn

================================================================================
来源：http://vp.asd995.cn

[Q01] 创建表
来源：http://dv.shxzskj.cn

CREATE TABLE users (
来源：http://mf.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kg.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://yl.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://ha.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dx.jianghongdianzi.cn

);
来源：http://ef.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://lm.muxihuayi.cn

CREATE TABLE orders (
来源：http://ro.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://li.521024.cn

user_id INT NOT NULL,
来源：http://oi.hahajie.cn

amount DECIMAL(10, 2),
来源：http://mq.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://an.shtwfgs.cn

);
来源：http://cv.huanxung.cn

[Q03] 增加列
来源：http://xr.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ih.panjiajie.cn

[Q04] 修改列类型
来源：http://tq.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://er.shtwfgs.cn

[Q05] 重命名列
来源：http://cd.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gl.shxzukj.cn

[Q06] 删除列
来源：http://fh.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://md.szxytkj.cn

[Q07] 删除表
来源：http://gs.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://bl.huixiangedu.cn

[Q08] 创建普通索引
来源：http://dc.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tu.panjiajie.cn

[Q09] 创建唯一索引
来源：http://tk.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ui.muxihuayi.cn

[Q10] 插入单行
来源：http://fx.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qf.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://ym.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xr.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://sn.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fu.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fh.521024.cn

[Q13] 忽略重复插入
来源：http://kr.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nt.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://wr.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iu.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nw.lnxyls.cn

[Q15] 查询全部
来源：http://uw.bookmarksfly.cn

SELECT * FROM users;
来源：http://fn.muxihuayi.cn

[Q16] 查询指定列
来源：http://dq.lnxyls.cn

SELECT id, name FROM users;
来源：http://ey.hnjuh.cn

[Q17] 条件查询
来源：http://ms.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ox.huixiangedu.cn

[Q18] 模糊匹配
来源：http://cj.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pt.yuntaijiaju.cn

[Q19] 范围查询
来源：http://of.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pz.bookmarksfly.cn

[Q20] IN 列表
来源：http://pg.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ot.yuntaijiaju.cn

[Q21] 空值判断
来源：http://uq.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pd.huixiangedu.cn

[Q22] 排序
来源：http://va.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://la.muxihuayi.cn

[Q23] 分页
来源：http://lb.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ib.hahajie.cn

[Q24] 去重
来源：http://ax.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://of.szsharing.cn

[Q25] 只取前 N 条
来源：http://wb.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ou.hahajie.cn

[Q26] 计数
来源：http://ea.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://pt.shxzukj.cn

[Q27] 条件计数
来源：http://ix.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nf.shtwfgs.cn

[Q28] 求和与平均
来源：http://ir.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ri.shxzskj.cn

[Q29] 最大最小值
来源：http://ie.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hr.szxytkj.cn

[Q30] 分组统计
来源：http://jb.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://py.panjiajie.cn

[Q31] 分组后过滤
来源：http://kq.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lp.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://tm.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nr.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ba.chemitech.net.cn

[Q33] 多列分组
来源：http://sv.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uy.colortex.cn

[Q34] 每组取第一条
来源：http://kr.shtwfgs.cn

SELECT * FROM (
来源：http://nf.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zh.chemitech.net.cn

) t WHERE rn = 1;
来源：http://sv.521024.cn

[Q35] 内连接
来源：http://ej.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kx.asd995.cn

[Q36] 左连接
来源：http://ck.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ay.gzmigu.cn

[Q37] 右连接
来源：http://sx.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cw.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tt.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://in.colortex.cn

[Q39] 自连接（查上下级）
来源：http://ye.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lb.yuexingan06.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rx.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zx.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rn.szxytkj.cn

[Q41] 多表连接
来源：http://de.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jc.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://hf.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://en.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://ul.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://wa.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fm.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://hc.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tw.lnxyls.cn

[Q44] IN 子查询
来源：http://lt.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yw.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://sp.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ai.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dp.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tv.nszjky.cn

[Q47] 与平均值比较
来源：http://fr.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oq.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://yd.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qz.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://ct.huanxung.cn

[Q49] 更新单行
来源：http://sg.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vd.muxihuayi.cn

[Q50] 批量更新
来源：http://ru.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kd.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://kq.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uu.huanxung.cn

[Q52] 删除指定行
来源：http://td.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://vi.yuexingan06.cn

[Q53] 按条件删除
来源：http://hg.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dj.bookmarksfly.cn

[Q54] 清空表
来源：http://xt.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://je.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://wb.colortex.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lf.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://ep.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kb.bjjhwx.cn

[Q57] 行号
来源：http://tu.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nc.szsharing.cn

[Q58] 累计求和
来源：http://sa.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yd.panjiajie.cn

[Q59] 分组内累计
来源：http://mf.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ju.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://gr.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vh.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cs.haigaiapp.cn

[Q61] 移动平均
来源：http://gd.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tn.colortex.cn

[Q62] 分组占比
来源：http://cs.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vr.nicolike.cn

[Q63] 开启事务
来源：http://di.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ip.szxytkj.cn

[Q64] 提交事务
来源：http://ga.hahajie.cn

COMMIT;
来源：http://jq.9csxet.cn

[Q65] 回滚事务
来源：http://mu.bookmarksfly.cn

ROLLBACK;
来源：http://mv.wgjwhj.cn

[Q66] 行锁查询
来源：http://kd.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yj.szxytkj.cn

[Q67] 设置隔离级别
来源：http://eg.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nj.gzmigu.cn

[Q68] 保存点
来源：http://dn.wgjwhj.cn

SAVEPOINT sp1;
来源：http://pj.hahajie.cn

ROLLBACK TO sp1;
来源：http://wf.shtwfgs.cn

[Q69] 查看执行计划
来源：http://gy.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dx.nicolike.cn

[Q70] 更新统计信息
来源：http://io.lnxyls.cn

ANALYZE TABLE users;
来源：http://eu.9csxet.cn

[Q71] 查看建表语句
来源：http://ln.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oq.jianghongdianzi.cn

[Q72] 查看索引
来源：http://bd.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://kk.nszjky.cn

[Q73] 查看表状态
来源：http://ln.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eg.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://xb.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zi.bjjhwx.cn

[Q75] 日期格式化
来源：http://nk.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xf.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aj.newstarts.cn

[Q76] 按天统计
来源：http://pn.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cc.bookmarksfly.cn

[Q77] 时间加减
来源：http://ry.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wn.hnjuh.cn

[Q78] 当前时间
来源：http://ec.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xu.gzmigu.cn

[Q79] 字符串拼接
来源：http://uu.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ot.huanxung.cn

[Q80] 字符串截取
来源：http://ni.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ga.haigaiapp.cn

[Q81] 字符串替换
来源：http://at.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xp.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://xg.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ct.yuexingan06.cn

[Q83] 大小写转换
来源：http://yt.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sz.newstarts.cn

[Q84] 去除首尾空格
来源：http://mo.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://ai.shtwfgs.cn

[Q85] 数值取整
来源：http://de.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mp.colortex.cn

[Q86] 读取 JSON 字段
来源：http://bh.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dx.newstarts.cn

[Q87] JSON 字段做条件
来源：http://oz.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ci.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://mh.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lw.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dc.lnxyls.cn

[Q89] 判断表是否存在
来源：http://es.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rj.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://uh.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kc.nicolike.cn

================================================================================
来源：http://bt.newstarts.cn

R. Bash 专题
来源：http://wq.szxytkj.cn

================================================================================
来源：http://ef.huanxung.cn

[R01] shebang 与严格模式
来源：http://tp.huanxung.cn

#!/usr/bin/env bash
来源：http://ar.lnxyls.cn

set -euo pipefail
来源：http://ac.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://ub.hnjuh.cn

name="Tom"; echo "$name"
来源：http://nc.chemitech.net.cn

[R03] 只读变量
来源：http://ok.muxihuayi.cn

readonly PI=3.14
来源：http://lx.szsharing.cn

[R04] 位置参数
来源：http://bv.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bh.hnjuh.cn

[R05] 参数默认值
来源：http://tn.muxihuayi.cn

name="${1:-default}"
来源：http://eb.hahajie.cn

[R06] 判断命令是否存在
来源：http://jv.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zx.9csxet.cn

[R07] if 判断文件
来源：http://zu.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zu.asd995.cn

[R08] 数值比较
来源：http://da.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ed.huixinmuqiang.cn

[R09] 字符串比较
来源：http://is.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nl.szsharing.cn

[R10] 正则匹配
来源：http://us.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://um.9csxet.cn

[R11] case 多分支
来源：http://cr.panjiajie.cn

case "$1" in
来源：http://sp.colortex.cn

start) echo "启动" ;;
来源：http://un.gzmigu.cn

stop)  echo "停止" ;;
来源：http://ks.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://yc.hahajie.cn

esac
来源：http://tr.huanxung.cn

[R12] for 遍历文件
来源：http://ot.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://kd.shtwfgs.cn

[R13] for 计数循环
来源：http://bj.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://rv.haigaiapp.cn

[R14] C 风格 for
来源：http://ly.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jg.lnxyls.cn

[R15] while 逐行读文件
来源：http://dv.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yk.lnxyls.cn

[R16] until 等待条件
来源：http://mj.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pw.shtwfgs.cn

[R17] 数组定义与取值
来源：http://qf.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nx.jctech888.com.cn

[R18] 遍历数组
来源：http://cz.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mr.szsharing.cn

[R19] 数组长度
来源：http://lv.lnxyls.cn

echo "${#arr[@]}"
来源：http://jf.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://wz.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wr.jianghongdianzi.cn

[R21] 字符串长度
来源：http://yz.huixinmuqiang.cn

echo "${#s}"
来源：http://yy.shxzukj.cn

[R22] 截取子串
来源：http://xv.panjiajie.cn

echo "${s:0:5}"
来源：http://oy.9csxet.cn

[R23] 字符串替换
来源：http://cu.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vr.colortex.cn

[R24] 大小写转换
来源：http://rn.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ji.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://vx.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mr.shtwfgs.cn

[R26] 命令替换
来源：http://ow.panjiajie.cn

now=$(date +%F); echo "$now"
来源：http://dm.jctech888.com.cn

[R27] 算术展开
来源：http://em.shtwfgs.cn

echo $((1 + 2 * 3))
来源：http://jd.521024.cn

[R28] 浮点运算
来源：http://xh.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://ev.muxihuayi.cn

[R29] 定义函数
来源：http://me.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ee.shxzukj.cn

[R30] 函数返回状态码
来源：http://zi.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://ga.wgjwhj.cn

[R31] 局部变量
来源：http://wi.jctech888.com.cn

f() { local x=1; echo "$x"; }
来源：http://rq.asd995.cn

[R32] 参数个数校验
来源：http://iu.yuexingan06.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://li.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://am.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ul.chemitech.net.cn

[R34] 退出时清理
来源：http://gw.bookmarksfly.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mu.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://lw.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uz.lnxyls.cn

[R36] 并发执行多个任务
来源：http://av.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fe.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://nj.panjiajie.cn


<!-- 参考信息 -->