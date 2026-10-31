代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fs.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://an.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cg.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://mm.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rq.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qf.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://th.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dq.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lq.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://er.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nl.asd995.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ks.huanxung.cn

================================================================================
来源：http://nq.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://op.hnjuh.cn

================================================================================
来源：http://es.wgjwhj.cn

[Q01] 创建表
来源：http://bd.nszjky.cn

CREATE TABLE users (
来源：http://nc.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cq.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://fz.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://bk.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://be.muxihuayi.cn

);
来源：http://ws.huanxung.cn

[Q02] 创建带外键的表
来源：http://ts.muxihuayi.cn

CREATE TABLE orders (
来源：http://xl.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://av.nicolike.cn

user_id INT NOT NULL,
来源：http://yx.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://hh.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ma.hnjuh.cn

);
来源：http://jb.shtwfgs.cn

[Q03] 增加列
来源：http://xi.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xb.hnjuh.cn

[Q04] 修改列类型
来源：http://ue.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://me.szxytkj.cn

[Q05] 重命名列
来源：http://bs.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bs.jctech888.com.cn

[Q06] 删除列
来源：http://aq.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sc.colortex.cn

[Q07] 删除表
来源：http://fx.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://pw.asd995.cn

[Q08] 创建普通索引
来源：http://cd.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://co.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://yk.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yi.shxzukj.cn

[Q10] 插入单行
来源：http://zg.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rt.hahajie.cn

[Q11] 一次插入多行
来源：http://fh.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qp.asd995.cn

[Q12] 插入后取自增 ID
来源：http://sm.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wv.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lu.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://xd.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uq.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://cm.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ox.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nc.wgjwhj.cn

[Q15] 查询全部
来源：http://tw.huixinmuqiang.cn

SELECT * FROM users;
来源：http://av.9csxet.cn

[Q16] 查询指定列
来源：http://cz.shxzskj.cn

SELECT id, name FROM users;
来源：http://tt.colortex.cn

[Q17] 条件查询
来源：http://mx.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pu.colortex.cn

[Q18] 模糊匹配
来源：http://fc.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://by.521024.cn

[Q19] 范围查询
来源：http://am.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jv.muxihuayi.cn

[Q20] IN 列表
来源：http://li.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wn.yuntaijiaju.cn

[Q21] 空值判断
来源：http://zf.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jr.nicolike.cn

[Q22] 排序
来源：http://vc.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hl.bookmarksfly.cn

[Q23] 分页
来源：http://bm.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gj.hahajie.cn

[Q24] 去重
来源：http://bi.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://zv.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://cp.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ur.haigaiapp.cn

[Q26] 计数
来源：http://ls.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://kl.gzmigu.cn

[Q27] 条件计数
来源：http://bi.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yx.panjiajie.cn

[Q28] 求和与平均
来源：http://dx.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iq.9csxet.cn

[Q29] 最大最小值
来源：http://pk.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gp.bookmarksfly.cn

[Q30] 分组统计
来源：http://zc.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://is.huanxung.cn

[Q31] 分组后过滤
来源：http://bc.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mx.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://gt.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ny.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ra.shxzskj.cn

[Q33] 多列分组
来源：http://cl.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zm.panjiajie.cn

[Q34] 每组取第一条
来源：http://ay.chemitech.net.cn

SELECT * FROM (
来源：http://bm.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yw.haigaiapp.cn

) t WHERE rn = 1;
来源：http://jx.9csxet.cn

[Q35] 内连接
来源：http://pg.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jb.newstarts.cn

[Q36] 左连接
来源：http://ox.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ya.huanxung.cn

[Q37] 右连接
来源：http://lx.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fh.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bo.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qx.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://vm.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bs.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://au.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qa.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ef.huixinmuqiang.cn

[Q41] 多表连接
来源：http://dj.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hj.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://lg.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://zf.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://fy.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://zu.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yh.shxzskj.cn

[Q43] 标量子查询
来源：http://ja.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xg.nszjky.cn

[Q44] IN 子查询
来源：http://yh.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fk.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://av.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fd.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nq.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mr.chemitech.net.cn

[Q47] 与平均值比较
来源：http://yd.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dq.521024.cn

[Q48] CTE 公用表表达式
来源：http://ni.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qv.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://bh.gzmigu.cn

[Q49] 更新单行
来源：http://sk.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tw.shtwfgs.cn

[Q50] 批量更新
来源：http://bd.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vj.hahajie.cn

[Q51] 用子查询更新
来源：http://pz.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lj.shxzskj.cn

[Q52] 删除指定行
来源：http://oh.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://ft.shxzukj.cn

[Q53] 按条件删除
来源：http://am.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bk.yuexingan06.cn

[Q54] 清空表
来源：http://gz.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://fc.szsharing.cn

[Q55] 排名（并列占位）
来源：http://zi.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vi.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://qp.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rw.wgjwhj.cn

[Q57] 行号
来源：http://ey.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sj.shxzskj.cn

[Q58] 累计求和
来源：http://og.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lb.521024.cn

[Q59] 分组内累计
来源：http://gf.asd995.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dq.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://lj.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ms.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://df.hnjuh.cn

[Q61] 移动平均
来源：http://rn.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ky.jctech888.com.cn

[Q62] 分组占比
来源：http://ie.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jx.asd995.cn

[Q63] 开启事务
来源：http://ee.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vi.jctech888.com.cn

[Q64] 提交事务
来源：http://hl.szxytkj.cn

COMMIT;
来源：http://az.asd995.cn

[Q65] 回滚事务
来源：http://pi.huixiangedu.cn

ROLLBACK;
来源：http://ip.muxihuayi.cn

[Q66] 行锁查询
来源：http://gq.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ou.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://we.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://og.shtwfgs.cn

[Q68] 保存点
来源：http://uw.hnjuh.cn

SAVEPOINT sp1;
来源：http://ee.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://iy.newstarts.cn

[Q69] 查看执行计划
来源：http://hz.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bb.haigaiapp.cn

[Q70] 更新统计信息
来源：http://gq.lnxyls.cn

ANALYZE TABLE users;
来源：http://ob.huixiangedu.cn

[Q71] 查看建表语句
来源：http://vr.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tr.chemitech.net.cn

[Q72] 查看索引
来源：http://zp.shxzskj.cn

SHOW INDEX FROM users;
来源：http://fo.szsharing.cn

[Q73] 查看表状态
来源：http://qf.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bw.huanxung.cn

[Q74] 强制使用索引
来源：http://yn.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bl.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://ha.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dt.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tw.521024.cn

[Q76] 按天统计
来源：http://rr.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xs.szxytkj.cn

[Q77] 时间加减
来源：http://el.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dc.asd995.cn

[Q78] 当前时间
来源：http://yl.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kk.shtwfgs.cn

[Q79] 字符串拼接
来源：http://wn.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oh.chemitech.net.cn

[Q80] 字符串截取
来源：http://bx.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vz.bjjhwx.cn

[Q81] 字符串替换
来源：http://vv.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://um.colortex.cn

[Q82] 字符长度与字节长度
来源：http://me.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lr.szxytkj.cn

[Q83] 大小写转换
来源：http://pz.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tv.newstarts.cn

[Q84] 去除首尾空格
来源：http://pu.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://tn.shxzskj.cn

[Q85] 数值取整
来源：http://th.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://it.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://jj.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rm.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://wu.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qj.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://ah.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xk.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://za.nicolike.cn

[Q89] 判断表是否存在
来源：http://xr.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yw.gzmigu.cn

[Q90] 生成序号列
来源：http://ts.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://py.huixiangedu.cn

================================================================================
来源：http://ci.yuntaijiaju.cn

R. Bash 专题
来源：http://st.jianghongdianzi.cn

================================================================================
来源：http://nl.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://ho.panjiajie.cn

#!/usr/bin/env bash
来源：http://so.nicolike.cn

set -euo pipefail
来源：http://qd.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://eo.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://dy.wgjwhj.cn

[R03] 只读变量
来源：http://tx.szsharing.cn

readonly PI=3.14
来源：http://ff.newstarts.cn

[R04] 位置参数
来源：http://ls.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nn.shxzskj.cn

[R05] 参数默认值
来源：http://np.shxzskj.cn

name="${1:-default}"
来源：http://ld.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://cc.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ko.hahajie.cn

[R07] if 判断文件
来源：http://iq.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rt.521024.cn

[R08] 数值比较
来源：http://me.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ui.asd995.cn

[R09] 字符串比较
来源：http://nu.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rm.chemitech.net.cn

[R10] 正则匹配
来源：http://aj.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fn.szxytkj.cn

[R11] case 多分支
来源：http://dw.jianghongdianzi.cn

case "$1" in
来源：http://ne.asd995.cn

start) echo "启动" ;;
来源：http://fb.asd995.cn

stop)  echo "停止" ;;
来源：http://ix.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://sf.9csxet.cn

esac
来源：http://hz.bookmarksfly.cn

[R12] for 遍历文件
来源：http://aj.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://co.bookmarksfly.cn

[R13] for 计数循环
来源：http://bq.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://mj.shxzukj.cn

[R14] C 风格 for
来源：http://eq.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gl.haigaiapp.cn

[R15] while 逐行读文件
来源：http://ic.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vs.yuexingan06.cn

[R16] until 等待条件
来源：http://rw.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nb.jctech888.com.cn

[R17] 数组定义与取值
来源：http://hv.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rw.shxzukj.cn

[R18] 遍历数组
来源：http://ny.gzmigu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://we.lnxyls.cn

[R19] 数组长度
来源：http://oy.szsharing.cn

echo "${#arr[@]}"
来源：http://oo.lnxyls.cn

[R20] 关联数组（字典）
来源：http://be.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qo.nicolike.cn

[R21] 字符串长度
来源：http://ok.shtwfgs.cn

echo "${#s}"
来源：http://sf.521024.cn

[R22] 截取子串
来源：http://pn.521024.cn

echo "${s:0:5}"
来源：http://fc.shtwfgs.cn

[R23] 字符串替换
来源：http://vq.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jw.jianghongdianzi.cn

[R24] 大小写转换
来源：http://mz.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dq.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://wh.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hh.nszjky.cn

[R26] 命令替换
来源：http://wt.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://ec.hahajie.cn

[R27] 算术展开
来源：http://oi.nicolike.cn

echo $((1 + 2 * 3))
来源：http://rv.bjjhwx.cn

[R28] 浮点运算
来源：http://id.521024.cn

echo "scale=2; 10/3" | bc
来源：http://ir.hahajie.cn

[R29] 定义函数
来源：http://xo.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zh.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://hp.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://oz.hahajie.cn

[R31] 局部变量
来源：http://fe.hahajie.cn

f() { local x=1; echo "$x"; }
来源：http://or.nszjky.cn

[R32] 参数个数校验
来源：http://ok.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pq.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://qd.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bd.gzmigu.cn

[R34] 退出时清理
来源：http://qc.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wn.yuexingan06.cn

[R35] 后台执行并等待
来源：http://ot.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rf.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://jn.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vu.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://gf.muxihuayi.cn


<!-- 参考信息 -->