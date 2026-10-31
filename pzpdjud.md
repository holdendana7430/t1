代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rz.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gw.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vj.asd995.cn

[P08] 处理浮点精度问题
来源：http://pv.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cm.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zd.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rx.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uk.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ly.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rb.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://db.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://km.nicolike.cn

================================================================================
来源：http://xh.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xy.huixiangedu.cn

================================================================================
来源：http://yv.huixinmuqiang.cn

[Q01] 创建表
来源：http://nu.panjiajie.cn

CREATE TABLE users (
来源：http://iu.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qe.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://fi.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://bs.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zs.jctech888.com.cn

);
来源：http://ed.lnxyls.cn

[Q02] 创建带外键的表
来源：http://jq.hnjuh.cn

CREATE TABLE orders (
来源：http://no.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://he.jctech888.com.cn

user_id INT NOT NULL,
来源：http://rl.colortex.cn

amount DECIMAL(10, 2),
来源：http://gn.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yh.shxzukj.cn

);
来源：http://hg.hahajie.cn

[Q03] 增加列
来源：http://ke.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zl.chemitech.net.cn

[Q04] 修改列类型
来源：http://ip.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ht.shxzukj.cn

[Q05] 重命名列
来源：http://on.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ju.nicolike.cn

[Q06] 删除列
来源：http://fb.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zz.hahajie.cn

[Q07] 删除表
来源：http://od.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://km.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://sd.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xf.521024.cn

[Q09] 创建唯一索引
来源：http://rp.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lc.panjiajie.cn

[Q10] 插入单行
来源：http://lf.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ke.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://st.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://js.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://er.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uh.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pr.nicolike.cn

[Q13] 忽略重复插入
来源：http://df.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kp.521024.cn

[Q14] 存在则更新（upsert）
来源：http://es.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cg.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://um.jctech888.com.cn

[Q15] 查询全部
来源：http://vt.shxzskj.cn

SELECT * FROM users;
来源：http://ea.newstarts.cn

[Q16] 查询指定列
来源：http://vi.hahajie.cn

SELECT id, name FROM users;
来源：http://yw.lnxyls.cn

[Q17] 条件查询
来源：http://fm.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xm.asd995.cn

[Q18] 模糊匹配
来源：http://ry.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gf.lnxyls.cn

[Q19] 范围查询
来源：http://rs.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ab.bjjhwx.cn

[Q20] IN 列表
来源：http://jx.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ez.muxihuayi.cn

[Q21] 空值判断
来源：http://wl.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rn.jianghongdianzi.cn

[Q22] 排序
来源：http://ce.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dl.hahajie.cn

[Q23] 分页
来源：http://aw.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kr.huixinmuqiang.cn

[Q24] 去重
来源：http://yj.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://ej.szsharing.cn

[Q25] 只取前 N 条
来源：http://oh.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pa.hahajie.cn

[Q26] 计数
来源：http://wc.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://kl.9csxet.cn

[Q27] 条件计数
来源：http://xg.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pw.jctech888.com.cn

[Q28] 求和与平均
来源：http://um.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tv.newstarts.cn

[Q29] 最大最小值
来源：http://cw.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://og.szxytkj.cn

[Q30] 分组统计
来源：http://bv.chemitech.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://id.521024.cn

[Q31] 分组后过滤
来源：http://pi.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mp.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://jh.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://al.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://op.muxihuayi.cn

[Q33] 多列分组
来源：http://qd.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iz.haigaiapp.cn

[Q34] 每组取第一条
来源：http://zd.newstarts.cn

SELECT * FROM (
来源：http://mx.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pc.nszjky.cn

) t WHERE rn = 1;
来源：http://ln.lnxyls.cn

[Q35] 内连接
来源：http://ja.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lk.yuntaijiaju.cn

[Q36] 左连接
来源：http://yw.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xe.panjiajie.cn

[Q37] 右连接
来源：http://ww.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uz.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sd.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://au.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://fd.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kd.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ke.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mx.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ev.521024.cn

[Q41] 多表连接
来源：http://cl.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bp.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://jh.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://so.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://tu.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://ga.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jp.gzmigu.cn

[Q43] 标量子查询
来源：http://rv.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zr.hnjuh.cn

[Q44] IN 子查询
来源：http://ds.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hn.jianghongdianzi.cn

[Q45] EXISTS 判断存在
来源：http://wi.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gy.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ez.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kx.haigaiapp.cn

[Q47] 与平均值比较
来源：http://by.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lz.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://qr.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sk.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://kc.bookmarksfly.cn

[Q49] 更新单行
来源：http://nx.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jy.asd995.cn

[Q50] 批量更新
来源：http://fh.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ze.shxzukj.cn

[Q51] 用子查询更新
来源：http://le.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cs.521024.cn

[Q52] 删除指定行
来源：http://yj.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://wb.bookmarksfly.cn

[Q53] 按条件删除
来源：http://iy.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ku.colortex.cn

[Q54] 清空表
来源：http://nt.newstarts.cn

TRUNCATE TABLE logs;
来源：http://gp.newstarts.cn

[Q55] 排名（并列占位）
来源：http://la.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://th.lnxyls.cn

[Q56] 密集排名（并列不占位）
来源：http://yx.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cj.shxzskj.cn

[Q57] 行号
来源：http://zm.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lg.szxytkj.cn

[Q58] 累计求和
来源：http://hm.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://je.szsharing.cn

[Q59] 分组内累计
来源：http://hr.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bp.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://ia.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jg.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uq.chemitech.net.cn

[Q61] 移动平均
来源：http://jn.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qx.huixiangedu.cn

[Q62] 分组占比
来源：http://oo.bookmarksfly.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ho.huixinmuqiang.cn

[Q63] 开启事务
来源：http://wx.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rq.muxihuayi.cn

[Q64] 提交事务
来源：http://kt.wgjwhj.cn

COMMIT;
来源：http://rq.colortex.cn

[Q65] 回滚事务
来源：http://yk.jctech888.com.cn

ROLLBACK;
来源：http://pj.shtwfgs.cn

[Q66] 行锁查询
来源：http://vf.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mr.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://wz.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ba.shxzskj.cn

[Q68] 保存点
来源：http://iv.haigaiapp.cn

SAVEPOINT sp1;
来源：http://os.szsharing.cn

ROLLBACK TO sp1;
来源：http://nu.shxzukj.cn

[Q69] 查看执行计划
来源：http://xa.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yn.szsharing.cn

[Q70] 更新统计信息
来源：http://wk.gzmigu.cn

ANALYZE TABLE users;
来源：http://qg.gzmigu.cn

[Q71] 查看建表语句
来源：http://lr.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://au.yuexingan06.cn

[Q72] 查看索引
来源：http://do.shxzukj.cn

SHOW INDEX FROM users;
来源：http://yx.huanxung.cn

[Q73] 查看表状态
来源：http://rt.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jg.huixiangedu.cn

[Q74] 强制使用索引
来源：http://yv.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xh.huixiangedu.cn

[Q75] 日期格式化
来源：http://kd.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nv.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://al.nszjky.cn

[Q76] 按天统计
来源：http://mi.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ng.nszjky.cn

[Q77] 时间加减
来源：http://uw.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ze.huixinmuqiang.cn

[Q78] 当前时间
来源：http://ny.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pr.hahajie.cn

[Q79] 字符串拼接
来源：http://zj.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xx.hnjuh.cn

[Q80] 字符串截取
来源：http://sy.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eg.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://tf.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://al.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://yi.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hb.gzmigu.cn

[Q83] 大小写转换
来源：http://az.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ac.hahajie.cn

[Q84] 去除首尾空格
来源：http://is.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://rb.nszjky.cn

[Q85] 数值取整
来源：http://pb.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cz.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://di.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rm.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://dd.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hy.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://lh.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://re.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://js.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://sx.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tn.jctech888.com.cn

[Q90] 生成序号列
来源：http://dd.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fe.jianghongdianzi.cn

================================================================================
来源：http://jo.shxzukj.cn

R. Bash 专题
来源：http://hx.colortex.cn

================================================================================
来源：http://dh.lnxyls.cn

[R01] shebang 与严格模式
来源：http://qe.asd995.cn

#!/usr/bin/env bash
来源：http://sg.newstarts.cn

set -euo pipefail
来源：http://br.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://yr.521024.cn

name="Tom"; echo "$name"
来源：http://wl.nicolike.cn

[R03] 只读变量
来源：http://jx.yuntaijiaju.cn

readonly PI=3.14
来源：http://ig.wgjwhj.cn

[R04] 位置参数
来源：http://em.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xz.521024.cn

[R05] 参数默认值
来源：http://xb.shxzskj.cn

name="${1:-default}"
来源：http://ni.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://af.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sp.gzmigu.cn

[R07] if 判断文件
来源：http://ig.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sw.muxihuayi.cn

[R08] 数值比较
来源：http://bw.nszjky.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pe.521024.cn

[R09] 字符串比较
来源：http://ll.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lf.lnxyls.cn

[R10] 正则匹配
来源：http://vo.newstarts.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fb.shxzukj.cn

[R11] case 多分支
来源：http://mo.hnjuh.cn

case "$1" in
来源：http://kl.szsharing.cn

start) echo "启动" ;;
来源：http://nn.szxytkj.cn

stop)  echo "停止" ;;
来源：http://he.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://rz.szsharing.cn

esac
来源：http://rs.newstarts.cn

[R12] for 遍历文件
来源：http://tv.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://sa.chemitech.net.cn

[R13] for 计数循环
来源：http://ll.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://qc.jctech888.com.cn

[R14] C 风格 for
来源：http://if.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mm.colortex.cn

[R15] while 逐行读文件
来源：http://ic.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ct.wgjwhj.cn

[R16] until 等待条件
来源：http://ts.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://is.shtwfgs.cn

[R17] 数组定义与取值
来源：http://wh.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mk.gzmigu.cn

[R18] 遍历数组
来源：http://hq.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jb.muxihuayi.cn

[R19] 数组长度
来源：http://fi.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://yh.newstarts.cn

[R20] 关联数组（字典）
来源：http://uh.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cr.colortex.cn

[R21] 字符串长度
来源：http://pp.bookmarksfly.cn

echo "${#s}"
来源：http://sq.gzmigu.cn

[R22] 截取子串
来源：http://sa.newstarts.cn

echo "${s:0:5}"
来源：http://sh.colortex.cn

[R23] 字符串替换
来源：http://er.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qp.szxytkj.cn

[R24] 大小写转换
来源：http://de.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rx.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://xq.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wq.nszjky.cn

[R26] 命令替换
来源：http://hm.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://gn.muxihuayi.cn

[R27] 算术展开
来源：http://gp.szxytkj.cn

echo $((1 + 2 * 3))
来源：http://da.nicolike.cn

[R28] 浮点运算
来源：http://zy.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://lw.muxihuayi.cn

[R29] 定义函数
来源：http://qw.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://os.shtwfgs.cn

[R30] 函数返回状态码
来源：http://gp.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://du.shtwfgs.cn

[R31] 局部变量
来源：http://ek.nszjky.cn

f() { local x=1; echo "$x"; }
来源：http://mv.nszjky.cn

[R32] 参数个数校验
来源：http://mz.shxzukj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nb.asd995.cn

[R33] 捕获错误并提示行号
来源：http://cq.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jz.yuntaijiaju.cn

[R34] 退出时清理
来源：http://px.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ug.szxytkj.cn

[R35] 后台执行并等待
来源：http://wj.jctech888.com.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gu.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://vy.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tc.9csxet.cn

[R37] 把输出赋给变量
来源：http://ki.chemitech.net.cn


<!-- 参考信息 -->