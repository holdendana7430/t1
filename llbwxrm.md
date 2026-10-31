代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zo.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jz.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mf.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hf.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ka.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cf.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nx.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bp.huixinmuqiang.cn

================================================================================
来源：http://ib.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jm.huanxung.cn

================================================================================
来源：http://ms.muxihuayi.cn

[Q01] 创建表
来源：http://ml.9csxet.cn

CREATE TABLE users (
来源：http://lg.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://do.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://ml.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://ug.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nw.nicolike.cn

);
来源：http://sn.hahajie.cn

[Q02] 创建带外键的表
来源：http://ja.muxihuayi.cn

CREATE TABLE orders (
来源：http://nb.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ii.wgjwhj.cn

user_id INT NOT NULL,
来源：http://nr.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://pf.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cz.chemitech.net.cn

);
来源：http://mq.9csxet.cn

[Q03] 增加列
来源：http://fr.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lu.haigaiapp.cn

[Q04] 修改列类型
来源：http://to.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wu.szsharing.cn

[Q05] 重命名列
来源：http://wi.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xf.bookmarksfly.cn

[Q06] 删除列
来源：http://rk.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nw.wgjwhj.cn

[Q07] 删除表
来源：http://yc.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://dp.jctech888.com.cn

[Q08] 创建普通索引
来源：http://az.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kk.hahajie.cn

[Q09] 创建唯一索引
来源：http://po.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gf.huanxung.cn

[Q10] 插入单行
来源：http://jr.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xd.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://rt.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hw.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://np.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nk.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zx.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://sb.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zk.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://pz.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fg.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zh.newstarts.cn

[Q15] 查询全部
来源：http://aw.newstarts.cn

SELECT * FROM users;
来源：http://ze.lnxyls.cn

[Q16] 查询指定列
来源：http://wv.panjiajie.cn

SELECT id, name FROM users;
来源：http://tu.521024.cn

[Q17] 条件查询
来源：http://xv.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qr.521024.cn

[Q18] 模糊匹配
来源：http://ns.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xa.newstarts.cn

[Q19] 范围查询
来源：http://ni.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://by.hnjuh.cn

[Q20] IN 列表
来源：http://ov.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://de.huanxung.cn

[Q21] 空值判断
来源：http://no.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vd.colortex.cn

[Q22] 排序
来源：http://te.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ng.chemitech.net.cn

[Q23] 分页
来源：http://ox.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fp.wgjwhj.cn

[Q24] 去重
来源：http://op.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://bk.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://no.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ov.nszjky.cn

[Q26] 计数
来源：http://yw.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://se.yuntaijiaju.cn

[Q27] 条件计数
来源：http://kc.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mu.521024.cn

[Q28] 求和与平均
来源：http://pg.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rs.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://im.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kq.9csxet.cn

[Q30] 分组统计
来源：http://ji.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://go.wgjwhj.cn

[Q31] 分组后过滤
来源：http://tf.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vh.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://ux.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ua.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://va.hnjuh.cn

[Q33] 多列分组
来源：http://rq.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jr.jctech888.com.cn

[Q34] 每组取第一条
来源：http://ei.yuntaijiaju.cn

SELECT * FROM (
来源：http://hk.huixinmuqiang.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pe.newstarts.cn

) t WHERE rn = 1;
来源：http://vd.jctech888.com.cn

[Q35] 内连接
来源：http://lm.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zl.nicolike.cn

[Q36] 左连接
来源：http://cx.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://po.yuntaijiaju.cn

[Q37] 右连接
来源：http://fy.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ge.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fi.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kf.muxihuayi.cn

[Q39] 自连接（查上下级）
来源：http://dq.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pd.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gh.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fy.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gy.muxihuayi.cn

[Q41] 多表连接
来源：http://kg.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jt.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://yi.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://yl.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://jl.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://ye.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://te.bookmarksfly.cn

[Q43] 标量子查询
来源：http://vm.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://of.huixiangedu.cn

[Q44] IN 子查询
来源：http://gs.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://al.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://zf.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zv.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bw.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://li.jctech888.com.cn

[Q47] 与平均值比较
来源：http://wq.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wz.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://ok.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ep.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ja.panjiajie.cn

[Q49] 更新单行
来源：http://hd.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nv.wgjwhj.cn

[Q50] 批量更新
来源：http://op.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yg.haigaiapp.cn

[Q51] 用子查询更新
来源：http://wm.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zt.panjiajie.cn

[Q52] 删除指定行
来源：http://kd.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://rv.shxzukj.cn

[Q53] 按条件删除
来源：http://ny.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gd.muxihuayi.cn

[Q54] 清空表
来源：http://ii.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://kv.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://eh.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ev.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://si.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vy.chemitech.net.cn

[Q57] 行号
来源：http://ge.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://no.huanxung.cn

[Q58] 累计求和
来源：http://gb.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aq.colortex.cn

[Q59] 分组内累计
来源：http://xp.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zx.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://bq.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vw.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pp.gzmigu.cn

[Q61] 移动平均
来源：http://hg.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lw.gzmigu.cn

[Q62] 分组占比
来源：http://dg.nszjky.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bo.muxihuayi.cn

[Q63] 开启事务
来源：http://dr.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fi.yuexingan06.cn

[Q64] 提交事务
来源：http://xf.haigaiapp.cn

COMMIT;
来源：http://vk.jctech888.com.cn

[Q65] 回滚事务
来源：http://ng.asd995.cn

ROLLBACK;
来源：http://le.nszjky.cn

[Q66] 行锁查询
来源：http://io.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qe.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://jv.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cx.yuntaijiaju.cn

[Q68] 保存点
来源：http://pf.haigaiapp.cn

SAVEPOINT sp1;
来源：http://ze.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://nw.nszjky.cn

[Q69] 查看执行计划
来源：http://kj.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mh.colortex.cn

[Q70] 更新统计信息
来源：http://ei.gzmigu.cn

ANALYZE TABLE users;
来源：http://wy.panjiajie.cn

[Q71] 查看建表语句
来源：http://jh.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qg.nicolike.cn

[Q72] 查看索引
来源：http://re.newstarts.cn

SHOW INDEX FROM users;
来源：http://gc.nicolike.cn

[Q73] 查看表状态
来源：http://bx.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bp.szsharing.cn

[Q74] 强制使用索引
来源：http://tt.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sd.gzmigu.cn

[Q75] 日期格式化
来源：http://gq.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yy.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dl.jianghongdianzi.cn

[Q76] 按天统计
来源：http://bb.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ws.muxihuayi.cn

[Q77] 时间加减
来源：http://lo.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sr.szxytkj.cn

[Q78] 当前时间
来源：http://qu.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sa.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://gr.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://be.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://hi.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://es.chemitech.net.cn

[Q81] 字符串替换
来源：http://kb.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pg.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://or.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://do.nszjky.cn

[Q83] 大小写转换
来源：http://dv.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tm.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://cg.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://og.haigaiapp.cn

[Q85] 数值取整
来源：http://jn.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jb.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://xl.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tg.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://po.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lk.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://nj.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qq.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cs.yuexingan06.cn

[Q89] 判断表是否存在
来源：http://mm.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yx.newstarts.cn

[Q90] 生成序号列
来源：http://nk.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qc.szxytkj.cn

================================================================================
来源：http://ep.colortex.cn

R. Bash 专题
来源：http://ll.szxytkj.cn

================================================================================
来源：http://wj.nicolike.cn

[R01] shebang 与严格模式
来源：http://lq.newstarts.cn

#!/usr/bin/env bash
来源：http://fn.9csxet.cn

set -euo pipefail
来源：http://re.colortex.cn

[R02] 变量赋值与使用
来源：http://lm.newstarts.cn

name="Tom"; echo "$name"
来源：http://io.asd995.cn

[R03] 只读变量
来源：http://ii.haigaiapp.cn

readonly PI=3.14
来源：http://jt.hahajie.cn

[R04] 位置参数
来源：http://yu.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ro.panjiajie.cn

[R05] 参数默认值
来源：http://hh.shxzukj.cn

name="${1:-default}"
来源：http://yb.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://uo.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://id.newstarts.cn

[R07] if 判断文件
来源：http://hx.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://et.colortex.cn

[R08] 数值比较
来源：http://xr.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sd.shxzskj.cn

[R09] 字符串比较
来源：http://ht.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vj.jianghongdianzi.cn

[R10] 正则匹配
来源：http://th.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fz.szsharing.cn

[R11] case 多分支
来源：http://kq.hnjuh.cn

case "$1" in
来源：http://ln.hahajie.cn

start) echo "启动" ;;
来源：http://uf.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://tc.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://ky.9csxet.cn

esac
来源：http://vq.gzmigu.cn

[R12] for 遍历文件
来源：http://qh.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://ph.chemitech.net.cn

[R13] for 计数循环
来源：http://ff.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://aa.bookmarksfly.cn

[R14] C 风格 for
来源：http://pc.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bf.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://aw.panjiajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ey.asd995.cn

[R16] until 等待条件
来源：http://sw.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dg.hahajie.cn

[R17] 数组定义与取值
来源：http://qo.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jj.521024.cn

[R18] 遍历数组
来源：http://qa.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wk.chemitech.net.cn

[R19] 数组长度
来源：http://bh.haigaiapp.cn

echo "${#arr[@]}"
来源：http://ji.szsharing.cn

[R20] 关联数组（字典）
来源：http://cj.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kx.shxzskj.cn

[R21] 字符串长度
来源：http://tx.jianghongdianzi.cn

echo "${#s}"
来源：http://pp.nicolike.cn

[R22] 截取子串
来源：http://rp.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://tu.muxihuayi.cn

[R23] 字符串替换
来源：http://se.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dg.chemitech.net.cn

[R24] 大小写转换
来源：http://og.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ff.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://hb.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nd.9csxet.cn

[R26] 命令替换
来源：http://mv.hnjuh.cn

now=$(date +%F); echo "$now"
来源：http://fc.huixinmuqiang.cn

[R27] 算术展开
来源：http://be.colortex.cn

echo $((1 + 2 * 3))
来源：http://eo.asd995.cn

[R28] 浮点运算
来源：http://us.hnjuh.cn

echo "scale=2; 10/3" | bc
来源：http://ea.szxytkj.cn

[R29] 定义函数
来源：http://tt.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dk.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://gs.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://rd.9csxet.cn

[R31] 局部变量
来源：http://dh.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://pg.haigaiapp.cn

[R32] 参数个数校验
来源：http://if.colortex.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xs.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://tw.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ya.lnxyls.cn

[R34] 退出时清理
来源：http://os.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bu.newstarts.cn

[R35] 后台执行并等待
来源：http://cf.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://th.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://pz.shxzukj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ah.huanxung.cn

[R37] 把输出赋给变量
来源：http://tv.panjiajie.cn

files=$(ls -1)
来源：http://ml.yuexingan06.cn

[R38] 管道串联
来源：http://wq.gzmigu.cn

cat a.txt | grep -i error | wc -l
来源：http://ry.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://pc.nicolike.cn


<!-- 参考信息 -->